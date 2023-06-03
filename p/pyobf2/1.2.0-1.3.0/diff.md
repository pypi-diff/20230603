# Comparing `tmp/pyobf2-1.2.0.tar.gz` & `tmp/pyobf2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobf2-1.2.0.tar", max compression
+gzip compressed data, was "pyobf2-1.3.0.tar", max compression
```

## Comparing `pyobf2-1.2.0.tar` & `pyobf2-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1493 2022-12-25 22:51:00.834716 pyobf2-1.2.0/LICENSE
--rw-r--r--   0        0        0     1626 2023-02-04 10:57:47.564798 pyobf2-1.2.0/README.md
--rw-r--r--   0        0        0    12727 2023-02-06 20:52:53.040407 pyobf2-1.2.0/pyobf2/__init__.py
--rw-r--r--   0        0        0       67 2023-02-12 09:33:16.084127 pyobf2-1.2.0/pyobf2/__main__.py
--rw-r--r--   0        0        0     5130 2023-02-12 10:03:25.578449 pyobf2-1.2.0/pyobf2/lib/__init__.py
--rw-r--r--   0        0        0     8438 2023-01-07 07:09:48.977055 pyobf2-1.2.0/pyobf2/lib/assembler.py
--rw-r--r--   0        0        0      318 2023-01-06 05:02:15.350303 pyobf2-1.2.0/pyobf2/lib/cfg.py
--rw-r--r--   0        0        0      543 2023-02-11 08:03:32.310946 pyobf2-1.2.0/pyobf2/lib/log.py
--rw-r--r--   0        0        0    15769 2023-02-10 16:31:42.072634 pyobf2-1.2.0/pyobf2/lib/renamer.py
--rw-r--r--   0        0        0     2769 2023-01-18 16:38:31.554663 pyobf2-1.2.0/pyobf2/lib/transformers/__init__.py
--rw-r--r--   0        0        0     5454 2023-01-07 07:09:48.981056 pyobf2-1.2.0/pyobf2/lib/transformers/collector.py
--rw-r--r--   0        0        0     2466 2023-01-18 16:35:55.899465 pyobf2-1.2.0/pyobf2/lib/transformers/compileFinalFiles.py
--rw-r--r--   0        0        0     7414 2023-02-11 08:03:32.294946 pyobf2-1.2.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py
--rw-r--r--   0        0        0     7919 2023-02-12 10:45:51.441055 pyobf2-1.2.0/pyobf2/lib/transformers/encodeStringsTransformer.py
--rw-r--r--   0        0        0     1395 2023-02-12 12:21:15.463667 pyobf2-1.2.0/pyobf2/lib/transformers/floatsToComplex.py
--rw-r--r--   0        0        0     1690 2023-01-07 07:09:48.993056 pyobf2-1.2.0/pyobf2/lib/transformers/fstrToFormatTransformer.py
--rw-r--r--   0        0        0     6416 2023-02-10 16:01:57.431356 pyobf2-1.2.0/pyobf2/lib/transformers/intObfuscatorTransformer.py
--rw-r--r--   0        0        0     1939 2023-02-12 10:02:46.417634 pyobf2-1.2.0/pyobf2/lib/transformers/logicTransformer.py
--rw-r--r--   0        0        0     2335 2023-02-10 18:30:28.528874 pyobf2-1.2.0/pyobf2/lib/transformers/memberRenamerTransformer.py
--rw-r--r--   0        0        0     4944 2023-01-24 05:53:53.382762 pyobf2-1.2.0/pyobf2/lib/transformers/packPyz.py
--rw-r--r--   0        0        0      872 2023-01-18 00:16:19.401707 pyobf2-1.2.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py
--rw-r--r--   0        0        0      876 2023-01-07 07:09:48.997056 pyobf2-1.2.0/pyobf2/lib/transformers/replaceAttribsTransformer.py
--rw-r--r--   0        0        0     1215 2023-02-06 20:36:10.818266 pyobf2-1.2.0/pyobf2/lib/transformers/unicodeNameTransformer.py
--rw-r--r--   0        0        0     8426 2023-01-11 16:23:11.226189 pyobf2-1.2.0/pyobf2/lib/util.py
--rw-r--r--   0        0        0      583 2023-02-12 12:22:51.241488 pyobf2-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 pyobf2-1.2.0/setup.py
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 pyobf2-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-05-29 20:30:26.316026 pyobf2-1.3.0/LICENSE
+-rw-r--r--   0        0        0    20749 2023-06-03 17:45:28.408096 pyobf2-1.3.0/README.md
+-rw-r--r--   0        0        0    12871 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/__main__.py
+-rw-r--r--   0        0        0     5344 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/__init__.py
+-rw-r--r--   0        0        0     8438 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/assembler.py
+-rw-r--r--   0        0        0      318 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/cfg.py
+-rw-r--r--   0        0        0      543 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/log.py
+-rw-r--r--   0        0        0    15769 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/renamer.py
+-rw-r--r--   0        0        0     2769 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/__init__.py
+-rw-r--r--   0        0        0     5454 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/collector.py
+-rw-r--r--   0        0        0     2466 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/compileFinalFiles.py
+-rw-r--r--   0        0        0     7414 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py
+-rw-r--r--   0        0        0     7919 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/encodeStringsTransformer.py
+-rw-r--r--   0        0        0     1732 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/floatsToComplex.py
+-rw-r--r--   0        0        0     1690 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/fstrToFormatTransformer.py
+-rw-r--r--   0        0        0     6416 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/intObfuscatorTransformer.py
+-rw-r--r--   0        0        0     1939 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/logicTransformer.py
+-rw-r--r--   0        0        0     2335 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/memberRenamerTransformer.py
+-rw-r--r--   0        0        0     4944 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/packPyz.py
+-rw-r--r--   0        0        0      872 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py
+-rw-r--r--   0        0        0      876 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/replaceAttribsTransformer.py
+-rw-r--r--   0        0        0     3303 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/stringCollectorTransformer.py
+-rw-r--r--   0        0        0     2674 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/typeAliasTransformer.py
+-rw-r--r--   0        0        0     1215 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/unicodeNameTransformer.py
+-rw-r--r--   0        0        0     8990 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/util.py
+-rw-r--r--   0        0        0      583 2023-06-03 18:52:45.803711 pyobf2-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    21443 1970-01-01 00:00:00.000000 pyobf2-1.3.0/PKG-INFO
```

### Comparing `pyobf2-1.2.0/LICENSE` & `pyobf2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/__init__.py` & `pyobf2-1.3.0/pyobf2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,25 +152,27 @@
     if not os.path.exists(output_file):
         os.makedirs(output_file)
     elif not os.path.isdir(output_file):
         console.log("Transitive obfuscation requires the output to be a directory", style="red")
         exit(1)
     console.log("Parsing inheritance tree...")
     deptree = get_dependency_tree(input_file)
-    if len(deptree) == 0:
+    if len(deptree) == 0 and len(general_settings["manual_include"].value) == 0:
         console.log(
             "Transitive run with no dependencies, aborting\nSet transitive to false in your config.toml if you have "
             "only one file",
             style="red",
         )
         exit(1)
-    common_prefix_l = len(os.path.commonpath(list(map(lambda x: os.path.dirname(x) + "/", deptree.keys())))) + 1
-    tree = rich.tree.Tree(os.path.abspath(input_file)[common_prefix_l:], style="green")
-    recurse_tree_inner(deptree, deptree[os.path.abspath(input_file)], common_prefix_l, tree)
-    console.log(tree)
+    if len(deptree) != 0:
+        common_prefix_l = len(os.path.commonpath(list(map(lambda x: os.path.dirname(x) + "/", deptree.keys())))) + 1
+        tree = rich.tree.Tree(os.path.abspath(input_file)[common_prefix_l:], style="green")
+        # console.log(deptree)
+        recurse_tree_inner(deptree, deptree[os.path.abspath(input_file)], common_prefix_l, tree)
+        console.log(tree)
     all_files = []
     for x in deptree.keys():
         if x not in all_files:
             all_files.append(x)
         for y in deptree[x]:
             if y not in all_files:
                 all_files.append(y)
@@ -226,14 +228,15 @@
             progress.update(
                 task, total=len(task_labels), completed=comp_i + 1, description=task_labels[math.floor(comp_i)]
             )
 
     console.log("Writing")
     for i in range(len(all_files)):
         file = all_files[i]
+        console.log("... " + file)
         out_ast = all_asts[i]
         full_path = os.path.join(output_file, file[common_prefix_l:])
         dname = os.path.dirname(full_path)
         if not os.path.exists(dname):
             os.makedirs(dname)
         try:
             src = NonEscapingUnparser().visit(out_ast)
@@ -242,15 +245,14 @@
             if str(e) == "Unable to avoid backslash in f-string expression part":
                 console.log(
                     "[red]An error occurred with re-parsing the python AST into source code.[/red] AST was not able to escape ASCII characters in an "
                     "F-String expression. Please check if you have any ASCII characters in F-Strings, and escape them manually. "
                 )
                 console.log("Current file:", full_path)
             exit(1)
-            return
 
         with open(full_path, "w", encoding="utf8") as f:
             f.write(src)
             f.flush()
     console.log("Doing post run")
     all_outs = [Path(os.path.join(output_file, x[common_prefix_l:])) for x in all_files]
     ofp = Path(output_file)
```

### Comparing `pyobf2-1.2.0/pyobf2/lib/__init__.py` & `pyobf2-1.3.0/pyobf2/lib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 from .transformers.fstrToFormatTransformer import FstringsToFormatSequence
 from .transformers.intObfuscatorTransformer import IntObfuscator
 from .transformers.logicTransformer import LogicTransformer
 from .transformers.memberRenamerTransformer import MemberRenamer
 from .transformers.packPyz import PackInPyz
 from .transformers.removeTypeHintsTransformer import RemoveTypeHints
 from .transformers.replaceAttribsTransformer import ReplaceAttribs
+from .transformers.typeAliasTransformer import TypeAliasTransformer
 from .transformers.unicodeNameTransformer import UnicodeNameTransformer
+from .transformers.stringCollectorTransformer import StringCollectorTransformer
 
 config_file = "config.toml"
 
 all_config_segments = []
 
 all_transformers = [
     x()
     for x in [
         LogicTransformer,
         RemoveTypeHints,
         FstringsToFormatSequence,
         EncodeStrings,
+        StringCollectorTransformer,
         FloatsToComplex,
         IntObfuscator,
         MemberRenamer,
+        TypeAliasTransformer,
         ReplaceAttribs,
         ConstructDynamicCodeObject,
         Collector,
         UnicodeNameTransformer,
         CompileFinalFiles,
         PackInPyz,
     ]
```

### Comparing `pyobf2-1.2.0/pyobf2/lib/assembler.py` & `pyobf2-1.3.0/pyobf2/lib/assembler.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/log.py` & `pyobf2-1.3.0/pyobf2/lib/log.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/renamer.py` & `pyobf2-1.3.0/pyobf2/lib/renamer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/__init__.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/collector.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/collector.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/compileFinalFiles.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/compileFinalFiles.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/encodeStringsTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/encodeStringsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/fstrToFormatTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/fstrToFormatTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/intObfuscatorTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/intObfuscatorTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/logicTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/logicTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/memberRenamerTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/memberRenamerTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/packPyz.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/packPyz.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/replaceAttribsTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/replaceAttribsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/transformers/unicodeNameTransformer.py` & `pyobf2-1.3.0/pyobf2/lib/transformers/unicodeNameTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.2.0/pyobf2/lib/util.py` & `pyobf2-1.3.0/pyobf2/lib/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import importlib.util
 import opcode
 import os.path
 import random
 from ast import *
 from types import CodeType
+import string
 
 _SINGLE_QUOTES = ("'", '"')
 _MULTI_QUOTES = ('"""', "'''")
 _ALL_QUOTES = (*_SINGLE_QUOTES, *_MULTI_QUOTES)
 
 
 class NonEscapingUnparser(getattr(ast, "_Unparser")):
@@ -108,21 +109,25 @@
     origin: str
     parent: str
 
 
 def get_file_from_import(name: str, parent: str, path: list[str]):
     try:
         resname = importlib.util.resolve_name(name, parent)
+        # print(name, parent, path, resname)
         searchfor = resname.split(".")
         for p in path:
             current_path = p
             visited_path = []
             for x in searchfor:
                 visited_path.append(x)
+                # print(visited_path)
                 current_path = os.path.join(current_path, x)
+                if not os.path.exists(current_path):
+                    return None
                 if os.path.isdir(current_path):  # this segment points to a folder, continue
                     continue
                 elif os.path.isfile(current_path + ".py"):  # we reached an end, the rest is speculation
                     return Imported(current_path + ".py", ".".join(visited_path[:-1]))
                 else:  # this doesn't exist as a file
                     prevpath = os.path.dirname(current_path)  # this is, based on previous checks, a directory
                     if os.path.isfile(
@@ -159,14 +164,16 @@
         if isinstance(node, Import):
             discorvered_specs = list(
                 filter(
                     lambda x: x is not None,
                     [get_file_from_import(x.name, current_package, search_path) for x in node.names],
                 )
             )
+
+            # print(discorvered_specs)
             if current_file not in lst:
                 lst[current_file] = []
 
             for x in discorvered_specs:
                 p = x.origin
                 if not p.startswith(namespace):
                     continue  # unwanted
@@ -212,7 +219,18 @@
 def strip_lnotab(c: CodeType) -> CodeType:
     consts = []
     for item in c.co_consts:
         if isinstance(item, CodeType):
             item = strip_lnotab(item)
         consts.append(item)
     return c.replace(co_linetable=b"", co_consts=tuple(consts))
+
+
+def random_identifier(length: int):
+    if length <= 0:
+        raise ValueError("length expected to be <= 1, got " + str(length))
+    valid_chars = string.ascii_letters + "_"
+    built = ""
+    built += random.choice(valid_chars)
+    for i in range(length - 1):
+        built += random.choice(valid_chars + string.digits)
+    return built
```

### Comparing `pyobf2-1.2.0/pyproject.toml` & `pyobf2-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pyobf2"
-version = "1.2.0"
+version = "1.3.0"
 description = "An in-place obfuscator for python 3.11"
 authors = ["0x150 <99053360+0x3C50@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/0x3C50/pyobf2"
 repository = "https://github.com/0x3C50/pyobf2"
 keywords = ["obfuscator", "obfuscator-api"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pycryptodome = "^3.16.0"
-rich = "^13.1.0"
-tomlkit = "^0.11.6"
+pycryptodome = "^3.18.0"
+rich = "^13.4.1"
+tomlkit = "^0.11.8"
 colorama = "^0.4.6"
 
 [tool.poetry.scripts]
 pyobf2 = "pyobf2:main"
 
 [build-system]
 requires = ["poetry-core"]
```

