# Comparing `tmp/pipen_annotate-0.7.2.tar.gz` & `tmp/pipen_annotate-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_annotate-0.7.2.tar", max compression
+gzip compressed data, was "pipen_annotate-0.7.3.tar", max compression
```

## Comparing `pipen_annotate-0.7.2.tar` & `pipen_annotate-0.7.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/LICENSE
--rw-r--r--   0        0        0     1592 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/README.md
--rw-r--r--   0        0        0      108 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/__init__.py
--rw-r--r--   0        0        0     5914 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/annotate.py
--rw-r--r--   0        0        0    11076 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/sections.py
--rw-r--r--   0        0        0      958 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.2/setup.py
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1592 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/README.md
+-rw-r--r--   0        0        0      108 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/__init__.py
+-rw-r--r--   0        0        0     7341 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/annotate.py
+-rw-r--r--   0        0        0    11354 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/sections.py
+-rw-r--r--   0        0        0      958 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.3/setup.py
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.3/PKG-INFO
```

### Comparing `pipen_annotate-0.7.2/LICENSE` & `pipen_annotate-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.2/README.md` & `pipen_annotate-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.2/pipen_annotate/annotate.py` & `pipen_annotate-0.7.3/pipen_annotate/annotate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import re
 import textwrap
 from typing import Any, Callable, Type, MutableMapping
 
 from diot import OrderedDiot
-from pipen import Proc
+from pipen import Proc, ProcGroup
+from pipen.utils import mark as proc_mark, get_marked as proc_get_marked
 
 from .sections import (
     Section,
     SectionSummary,
     SectionInput,
     SectionOutput,
     SectionEnvs,
     SectionItems,
+    SectionProcGroupArgs,
     SectionText,
 )
 
 SECTION_TYPES: MutableMapping[str, Type[Section]] = {
     "Summary": SectionSummary,
     "Input": SectionInput,
     "Output": SectionOutput,
@@ -34,15 +36,57 @@
     "Text": SectionText,
     "Items": SectionItems,
 }
 
 META_CONTAINER = "__meta__"
 
 
-def _annotate_uninherited(cls: Type[Proc]) -> OrderedDiot:
+def _mark(cls: type, **kwargs) -> type:
+    """Mark a class, not only a Proc
+
+    Args:
+        cls: The class to be marked
+        kwargs: The marks
+
+    Returns:
+        The marked class
+    """
+    if issubclass(cls, Proc):
+        return proc_mark(**kwargs)(cls)
+
+    if not getattr(cls, META_CONTAINER, None):
+        setattr(cls, META_CONTAINER, {})
+
+    meta = getattr(cls, META_CONTAINER)
+    meta.update(kwargs)
+    return cls
+
+
+def _get_marked(cls: type, mark_name: str, default: Any = None) -> Any:
+    """Get the marked value from a class, not only a Proc
+
+    Args:
+        cls: The class to get marked value from
+        mark_name: The mark name
+        default: The default value if not found
+
+    Returns:
+        The marked value
+    """
+    if issubclass(cls, Proc):
+        return proc_get_marked(cls, mark_name, default)
+
+    if not getattr(cls, META_CONTAINER, None):
+        setattr(cls, META_CONTAINER, {})
+
+    meta = getattr(cls, META_CONTAINER)
+    return meta.get(mark_name, default)
+
+
+def _annotate_uninherited(cls: type) -> OrderedDiot:
     """Annotate a Proc class with docstring, without inheriting from base.
 
     Args:
         cls: The class to be annotated.
 
     Returns:
         The annotated dict.
@@ -65,18 +109,21 @@
         section = SectionSummary(cls, section_name)
         for line in docstring.splitlines():
             line = line.rstrip()
             if line and line[-1] == ":":
                 if line[:-1] in SECTION_TYPES:
                     annotated[section_name] = section.parse()
                     section_name = line[:-1]
-                    section = SECTION_TYPES[section_name](
-                        cls,
-                        section_name,
-                    )
+                    if section_name == "Args" and issubclass(cls, ProcGroup):
+                        section = SectionProcGroupArgs(cls, section_name)
+                    else:
+                        section = SECTION_TYPES[section_name](
+                            cls,
+                            section_name,
+                        )
                 elif re.sub(r"(?!^) ", "", line[:-1]).isidentifier():
                     annotated[section_name] = section.parse()
                     section_name = line[:-1]
                     section = SectionText(cls, section_name)
                 else:
                     section.consume(line)
             else:
@@ -93,59 +140,71 @@
             annotated.Output = SectionOutput(cls, "Output").parse()
         if "Envs" not in annotated:
             annotated.Envs = SectionEnvs(cls, "Envs").parse()
 
     return annotated
 
 
-def _update_annotation(base: OrderedDiot, other: OrderedDiot) -> OrderedDiot:
+def _update_annotation(
+    base: OrderedDiot | None,
+    other: OrderedDiot,
+) -> OrderedDiot:
     """Update the annotation with another annotation."""
-    base = base.copy()
+    if base is None:
+        base = OrderedDiot()
+    else:
+        base = base.copy()
+
     for key, value in other.items():
         section_class = SECTION_TYPES.get(key)
         if key not in base or section_class is None:
             base[key] = value
         else:
             base[key] = section_class.update_parsed(base[key], value)
+
     return base
 
 
 def annotate(cls: Type[Any]) -> OrderedDiot:
     """Annotate a Proc class with docstring.
 
     Args:
         cls: The class to be annotated.
 
     Returns:
         The annotated dict.
     """
-    if not getattr(cls, META_CONTAINER, None):
-        setattr(cls, META_CONTAINER, {})
+    annotated = _get_marked(cls, "annotate_annotated")
+    inherit = _get_marked(cls, "annotate_inherit", True)
 
-    meta = getattr(cls, META_CONTAINER)
-
-    if not meta.get("annotate_annotated", False):
-        base = [
-            mro
-            for mro in cls.__mro__
-            if issubclass(mro, Proc) and mro is not Proc and mro is not cls
-        ]
+    if not annotated:
         annotated = _annotate_uninherited(cls)
-        if (
-            not meta.get("annotate_doc_inherit", True)
-            or not base
-        ):
-            meta["annotate_annotated"] = annotated
+        if issubclass(cls, Proc):
+            base = [
+                mro
+                for mro in cls.__mro__
+                if issubclass(mro, Proc)
+                and mro is not Proc
+                and mro is not cls
+                and mro is not object
+            ]
         else:
-            meta["annotate_annotated"] = _update_annotation(
-                annotate(base[0]),
-                annotated,
-            )
+            base = [
+                mro
+                for mro in cls.__mro__
+                if mro is not cls
+                and mro is not object
+            ]
+
+        base = base[0] if base else None
+        annotated_base = annotate(base) if inherit and base else None
+        annotated = _update_annotation(annotated_base, annotated)
+        _mark(cls, annotate_annotated=annotated)
 
-    return meta["annotate_annotated"]
+    return annotated
 
 
 def _register_section(
     section: str,
     section_class: Type[Section] | str | None = None,
 ) -> Callable[[Type[Section]], Type[Section]] | Type[Section]:
     """Register a section to be parsed.
@@ -183,19 +242,16 @@
 
     Args:
         section: The section name.
     """
     SECTION_TYPES.pop(section, None)
 
 
-def _no_doc_inherit(proc: Type[Proc]) -> Type[Proc]:
-    """A decorator to disable docstring inheritance for a Proc class"""
-    if not hasattr(proc, META_CONTAINER):
-        setattr(proc, META_CONTAINER, {})
-
-    getattr(proc, META_CONTAINER)["annotate_doc_inherit"] = False
+def _no_doc_inherit(proc: type) -> type:
+    """A decorator to disable docstring inheritance for a class"""
+    _mark(proc, annotate_inherit=False)
     return proc
 
 
 annotate.register_section = _register_section
 annotate.unregister_section = _unregister_section
-annotate.no_doc_inherit = _no_doc_inherit
+annotate.no_inherit = _no_doc_inherit
```

### Comparing `pipen_annotate-0.7.2/pipen_annotate/sections.py` & `pipen_annotate-0.7.3/pipen_annotate/sections.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,31 +149,34 @@
     return parts
 
 
 def _update_attrs_with_cls(
     parsed: Diot,
     envs: dict | None,
     prev_key: str | None = None,
-    cls_name: str | None = None,
 ) -> None:
     """Update the attrs of parsed terms with the class envs."""
     envs = envs or {}
     for key, value in envs.items():
         whole_key = f"{prev_key}.{key}" if prev_key else key
 
         if key not in parsed:
             parsed[key] = Diot(attrs={}, terms={}, help="")
 
-        if isinstance(value, dict):
-            # parsed[key].attrs.setdefault("action", "namespace")
+        if (
+            parsed[key].attrs.get("ns", False)
+            or parsed[key].attrs.get("namespace", False)
+            or parsed[key].attrs.get("action", "") in ("ns", "namespace")
+            or (isinstance(value, dict) and parsed[key].terms)
+        ):
+            parsed[key].attrs.setdefault("ns", True)
             _update_attrs_with_cls(
                 parsed[key].terms,
                 value,
                 prev_key=whole_key,
-                cls_name=cls_name,
             )
             # continue
 
         if "default" not in parsed[key].attrs:
             parsed[key].attrs["default"] = value
 
 
@@ -360,19 +363,23 @@
         return parsed
 
 
 class SectionEnvs(SectionItems):
 
     def parse(self) -> str | Diot | List[str]:
         parsed = super().parse()
-        _update_attrs_with_cls(
-            parsed,
-            self._cls.envs,
-            cls_name=self._cls.__name__,
-        )
+        _update_attrs_with_cls(parsed, self._cls.envs)
+        return parsed
+
+
+class SectionProcGroupArgs(SectionItems):
+
+    def parse(self) -> str | Diot | List[str]:
+        parsed = super().parse()
+        _update_attrs_with_cls(parsed, self._cls.DEFAULTS)
         return parsed
 
 
 class SectionText(Section):
 
     def parse(self) -> str | Diot | List[str]:
         return "\n".join(_dedent(self._lines))
```

### Comparing `pipen_annotate-0.7.2/pyproject.toml` & `pipen_annotate-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-annotate"
-version = "0.7.2"
+version = "0.7.3"
 description = "Use docstring to annotate pipen processes"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pipen_annotate-0.7.2/setup.py` & `pipen_annotate-0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pipen>=0.9,<0.10']
 
 setup_kwargs = {
     'name': 'pipen-annotate',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'Use docstring to annotate pipen processes',
     'long_description': '# pipen-annotate\n\nUse docstring to annotate [pipen](https://github.com/pwwang/pipen) processes\n\n## Installation\n\n```shell\npip install -U pipen-annotate\n```\n\n## Usage\n\n```python\nfrom pprint import pprint\nfrom pipen import Proc\nfrom pipen_annotate import annotate\n\n\nclass Process(Proc):\n    """Short description\n\n    Long description\n\n    Input:\n        infile: An input file\n        invar: An input variable\n\n    Output:\n        outfile: The output file\n\n    Envs:\n        ncores: Number of cores\n    """\n    input = "infile:file, invar"\n    output = "outfile:file:output.txt"\n    args = {\'ncores\': 1}\n\nannotated = annotate(Process)\n# prints:\n{\'Envs\': {\'ncores\': {\'attrs\': OrderedDiot([(\'default\', 1)]),\n                     \'help\': \'Number of cores\',\n                     \'terms\': OrderedDiot([])}},\n \'Input\': {\'infile\': {\'attrs\': {\'action\': \'extend\',\n                                \'itype\': \'file\',\n                                \'nargs\': \'+\'},\n                      \'help\': \'An input file\',\n                      \'terms\': OrderedDiot([])},\n           \'invar\': {\'attrs\': {\'action\': \'extend\',\n                               \'itype\': \'var\',\n                               \'nargs\': \'+\'},\n                     \'help\': \'An input variable\',\n                     \'terms\': OrderedDiot([])}},\n \'Output\': {\'outfile\': {\'attrs\': {\'default\': \'output.txt\',\n                                  \'otype\': \'file\'},\n                        \'help\': \'The output file\',\n                        \'terms\': OrderedDiot([])}},\n \'Summary\': {\'long\': \'Long description\\n\',\n             \'short\': \'Short description\'}}\n```\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_annotate-0.7.2/PKG-INFO` & `pipen_annotate-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-annotate
-Version: 0.7.2
+Version: 0.7.3
 Summary: Use docstring to annotate pipen processes
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

