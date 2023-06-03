# Comparing `tmp/parasect-1.1.2.tar.gz` & `tmp/parasect-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parasect-1.1.2.tar", max compression
+gzip compressed data, was "parasect-1.2.0.tar", max compression
```

## Comparing `parasect-1.1.2.tar` & `parasect-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2023-04-26 11:56:51.177681 parasect-1.1.2/LICENSE.rst
--rw-r--r--   0        0        0     4351 2023-04-26 11:56:51.177681 parasect-1.1.2/README.rst
--rw-r--r--   0        0        0     2233 2023-04-26 11:57:09.569968 parasect-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      193 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/__init__.py
--rw-r--r--   0        0        0     3502 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/__main__.py
--rw-r--r--   0        0        0    27635 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/_helpers.py
--rwxr-xr-x   0        0        0    28340 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/build_lib.py
--rwxr-xr-x   0        0        0    15184 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/compare_lib.py
--rw-r--r--   0        0        0        0 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/py.typed
--rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 parasect-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-03 19:53:41.023769 parasect-1.2.0/LICENSE.rst
+-rw-r--r--   0        0        0     4808 2023-06-03 19:53:41.023769 parasect-1.2.0/README.rst
+-rw-r--r--   0        0        0     2233 2023-06-03 19:53:54.087894 parasect-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/__init__.py
+-rw-r--r--   0        0        0     3502 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/__main__.py
+-rw-r--r--   0        0        0    32181 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/_helpers.py
+-rwxr-xr-x   0        0        0    31426 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/build_lib.py
+-rwxr-xr-x   0        0        0    15444 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/compare_lib.py
+-rw-r--r--   0        0        0        0 2023-06-03 19:53:41.031769 parasect-1.2.0/src/parasect/py.typed
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 parasect-1.2.0/PKG-INFO
```

### Comparing `parasect-1.1.2/LICENSE.rst` & `parasect-1.2.0/LICENSE.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 ===========
 
-Copyright © 2022 Avy B.V.
+Copyright © 2022-2023 Avy B.V.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `parasect-1.1.2/README.rst` & `parasect-1.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 *Parasect* has two-fold capabilities:
 
 1. Compare two parameter sets and highlighting their differences.
 2. Parsing from user-defined content and generating new parameter sets, ready for loading into an autopilot.
 
 List of currently supported autopilots:
 
+* Ardupilot_
 * PX4_
 
 Requirements
 ------------
 
 *Parasect* is a pure-Python project. Its requirements are managed by the Poetry_ dependency manager.
 When you install *Parasect* via pip_ its requirements will also be installed automatically.
@@ -78,14 +79,22 @@
 
 You can install *Parasect* via pip_ from PyPI_:
 
 .. code:: console
 
    $ pip install parasect
 
+If you don't care about using *Parasect* as a library and are only interested in
+command-line use, you can also use `pipx`_, that provides better isolation from
+the rest of the system:
+
+.. code:: console
+
+   $ pipx install parasect
+
 
 Usage
 -----
 
 *Parasect* is primarily used as a command-line program.
 In its simplest form, two parameter files can be compared via:
 
@@ -126,22 +135,27 @@
 Credits
 -------
 
 This project was sponsored by `Avy B.V. <Avy_>`_, a UAV company in Amsterdam.
 
 This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
 
+The project logo was created by `Cynthia de Vries <Cynthia_>`_.
+
 .. _@cjolowicz: https://github.com/cjolowicz
+.. _Cynthia: https://www.linkedin.com/in/cynthia-de-vries-497991231/
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _PyPI: https://pypi.org/
 .. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 .. _file an issue: https://github.com/AvyFly/parasect/issues
 .. _pip: https://pip.pypa.io/
+.. _pipx: https://github.com/pypa/pipx
 .. _CLI usage: https://parasect.readthedocs.io/en/latest/reference.html#cli-reference
 .. _API usage: https://parasect.readthedocs.io/en/latest/reference.html#api-reference
 .. _Concepts: https://parasect.readthedocs.io/en/latest/concepts.html
 .. _PX4: https://px4.io/
+.. _Ardupilot: https://ardupilot.org/
 .. _Poetry: https://python-poetry.org/
 .. _Avy: https://avy.eu
 .. github-only
 .. _Contributor Guide: CONTRIBUTING.rst
```

### Comparing `parasect-1.1.2/pyproject.toml` & `parasect-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parasect"
-version = "1.1.2"
+version = "1.2.0"
 description = "Utility for manipulating parameter sets for autopilots."
 authors = ["George Zogopoulos <geo.zogop.papal@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/AvyFly/parasect"
 repository = "https://github.com/AvyFly/parasect"
 documentation = "https://parasect.readthedocs.io"
@@ -21,16 +21,16 @@
 PyYAML = "^6.0"
 defusedxml = "^0.7.1"
 pydantic = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 coverage = {extras = ["toml"], version = "^7.2"}
-safety = "^2.2.0"
-mypy = "^1.0.1"
+safety = "^2.3.0"
+mypy = "^1.3.0"
 typeguard = "^2.13.3"
 xdoctest = {extras = ["colors"], version = "^1.0.0"}
 sphinx = "^6.2.1"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^3.2.2"
 flake8 = "^4.0.1"
 black = ">=21.10b0"
@@ -40,15 +40,15 @@
 flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.0"
 darglint = "^1.8.1"
 reorder-python-imports = "^3.1.0"
 pre-commit-hooks = "^4.3.0"
 sphinx-click = "^4.4.0"
 Pygments = "^2.10.0"
-pyupgrade = "^3.3.2"
+pyupgrade = "^3.4.0"
 furo = ">=2022.12.7"
 
 [tool.poetry.scripts]
 parasect = "parasect.__main__:cli"
 
 [tool.poetry.group.dev.dependencies]
 directory-tree = "^0.0.3.1"
```

### Comparing `parasect-1.1.2/src/parasect/__main__.py` & `parasect-1.2.0/src/parasect/__main__.py`

 * *Files identical despite different names*

### Comparing `parasect-1.1.2/src/parasect/_helpers.py` & `parasect-1.2.0/src/parasect/_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # noqa: D101, D102, D103
 """Module with helper functions for the whole package."""
 import csv
 import logging
 import math
 import os
+import re
 import typing
 from abc import ABC
 from abc import abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Any
+from typing import Callable
 from typing import Dict
 from typing import Generator
 from typing import KeysView
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Sequence
@@ -190,17 +192,22 @@
     """Simple parameter name, value .csv file."""
     px4 = "px4"
     """QGroundControl-style parameter file."""
     px4afv1 = "px4afv1"
     """Legacy PX4 airframe file, prior to version 1.11."""
     px4afv2 = "px4afv2"
     """New PX4 airframe file, version 1.11 and later."""
+    apm = "apm"
+    """Ardupilot-compatible file."""
+    apj = "apj"
+    """File compatible with Ardupilot's apj tool."""
 
 
 ReservedOptions = Literal[
+    "defaults",
     "frame_id",
     "sitl",
     "hitl",
     "parent",
     "remove_calibration",
     "remove_operator",
     "add_new",
@@ -345,14 +352,16 @@
                 "remove_calibration",
                 "remove_operator",
                 "add_new",
             ]:
                 check_type(key, value, bool)
             elif key in ["frame_id"]:
                 check_type(key, value, int)
+            elif key in ["defaults"]:
+                check_type(key, value, (str, type(None)))
             else:  # This is a custom dish
                 check_type(key, value, (str, type(None)))
 
     def __getitem__(self, item):
         """Access the model in a dict-like manner."""
         return self.__root__[item]
 
@@ -456,32 +465,34 @@
     default_value: Union[int, float]
     min_value = float("-inf")
     max_value = float("inf")
     increment = None  # Instruction for increments for UIs
     unit = None
     decimal = None  # Suggested increment by the parameter documentation
     reboot_required = False
+    readonly: bool
     group: Optional[str] = None
     vid: int  # Vehicle ID, default 1
     cid: int  # Component ID, default 1
 
     def __init__(
         self,
         name: str,
         value: Union[int, float],
         param_type: Optional[str] = None,
         vid: int = 1,
         cid: int = 1,
     ) -> None:
         """Class constructor."""
-        self.name = name.upper()
+        self.name = name
         self.value = value
         self.param_type = param_type
         self.vid = vid
         self.cid = cid
+        self.readonly = False
 
     @property
     def value(self) -> Union[int, float]:
         """Getter for parameter value."""
         if self.param_type == "INT32":
             return int(self._value)
         else:
@@ -619,14 +630,62 @@
     def keys(self) -> KeysView:
         """__keys__ dunder method.
 
         It returns the names of the parameters it contains.
         """
         return self.params.keys()
 
+    def update_param(self, param: Parameter) -> None:
+        """Update a parameter with the values of another.
+
+        All relevant values must be copied.
+        """
+        param_hash = self.build_param_hash_from_param(param)
+
+        # Try to deduce parameter type
+        if param.param_type is not None:
+            # If we know the new parameter type, use that.
+            new_value = param.value
+        elif self.params[param_hash].param_type is None:
+            # If we don't know the existing parameter type either, just paste it.
+            new_value = param.value
+        else:
+            # We know the target type, cast the new parameter value.
+            param_type = self.params[param_hash].param_type
+            new_value = cast_param_value(param.value, param_type)
+        self.params[param_hash].value = new_value
+
+        # Copy the rest of the attributes. This list must be kept up to date.
+        attr_list = [
+            "reasoning",
+            "short_desc",
+            "long_desc",
+            "default_value",
+            "min_value",
+            "max_value",
+            "increment",
+            "unit",
+            "decimal",
+            "reboot_required",
+            "readonly",
+            "group",
+            "vid",
+            "cid",
+        ]
+        for attr in attr_list:
+            try:
+                new_attr_value = getattr(param, attr)
+            except AttributeError:
+                continue
+            if new_attr_value and (
+                not isinstance(new_attr_value, str) or len(new_attr_value) > 1
+            ):
+                # The new value is not None and if it's a string, it's not empty.
+                setattr(self.params[param_hash], attr, new_attr_value)
+
     def add_param(
         self, param: Parameter, safe: bool = False, overwrite: bool = True
     ) -> None:
         """Add a Parameter to the list."""
         # param: The parameter object
         # safe: allow adding new parameters
         # overwrite: allow overwriting existing parameters
@@ -636,41 +695,39 @@
             raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
         if not overwrite and param_hash in self.params.keys():
             raise KeyError(f"Tried to overwrite key {param.name} with cid={param.cid}")
         # If parameter doesn't exist, create it
         if param_hash not in self.params:
             get_logger().debug(f"Creating new {param.name}")
             self.params[param_hash] = param
-        # otherwise copy only the value
+        # otherwise copy only the values
         else:
             get_logger().debug(f"Overwriting {param.name}")
-            # Try to deduce parameter type
-            if param.param_type is not None:
-                # If we know the new parameter type
-                new_value = param.value
-            elif self.params[param_hash].param_type is None:
-                # If we don't know the existing parameter type
-                new_value = param.value
-            else:
-                # We know the target type, cast the new parameter value
-                param_type = self.params[param_hash].param_type
-                new_value = cast_param_value(param.value, param_type)
-            self.params[param_hash].value = new_value
+            self.update_param(param)
 
     def remove_param(self, param: Parameter, safe: bool = True) -> None:
         """Remove a Parameter from the list."""
         # param: The parameter object
         # safe: don't try to remove not existing parameters
         param_hash = self.build_param_hash_from_param(param)
         if safe and param_hash not in self.params:
             raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
         get_logger().debug(f"Removing {param.name}.")
         self.params.pop(param_hash, None)
 
 
+def filter_regex(regex_list: List[str], param_list: ParameterList) -> None:
+    """Remove from param_list all parameters that match any of the regex_list."""
+    regex_obj_list = [re.compile(s) for s in regex_list]
+    for param in param_list:
+        if any(r.fullmatch(param.name) for r in regex_obj_list):
+            get_logger().debug(f"Matched {param.name} to a regex.")
+            param_list.remove_param(param)
+
+
 # Construct parameters from structured input
 ############################################
 
 
 def build_param_from_xml(parameter: XmlElement) -> Parameter:
     """Build a Parameter from an PX4-type xml entry."""
     name = str(parameter.get("name"))
@@ -722,14 +779,34 @@
         param_value = float(row[1])
 
     param = Parameter(param_name, param_value)
 
     return param
 
 
+def build_param_from_mavproxy(item: Sequence) -> Parameter:
+    """Convert a mavproxy parameter line to a parameter.
+
+    item should be a 3-length sequence of strings.
+    """
+    name = item[0]
+    value: Union[int, float]
+    value = item[1]
+    try:
+        value = int(item[1])
+    except ValueError:
+        value = float(item[1])
+    reasoning = item[2]
+
+    param = Parameter(name, value)
+    param.reasoning = reasoning
+
+    return param
+
+
 def build_param_from_iter(item: Sequence) -> Parameter:
     """Convert a param list item to a parameter.
 
     Item should be of the form [name, value, reasoning string]
     """
     name = item[0]
     value = item[1]
@@ -737,132 +814,193 @@
 
     if value is None:
         # This is typically the case of Allergens, where no value is needed
         value = 0
     param = Parameter(name, value)
     param.reasoning = reasoning
 
+    # Mark the parameter as readonly (supported in Ardupilot)
+    if reasoning and reasoning.find("@READONLY") > 1:
+        get_logger().debug(f"Marking {name} as READONLY.")
+        param.readonly = True
+
     return param
 
 
 # Read parameter text files
 ###########################
 
+parsers: List[Callable[[Path], ParameterList]] = []
+
+
+def parser(parser_func: Callable) -> Callable:
+    """Decorator to mark and collect parser functions."""
+    parsers.append(parser_func)
+    return parser_func
+
 
 def get_group_params_xml(group: XmlElement) -> Generator[XmlElement, None, None]:
     """Read parameter elements from an PX4-style XML group element.
 
     Receives an XmlElement
     Returns an XmlElement
     """
     yield from group.findall("parameter")
 
 
+@parser
 def read_params_xml(filepath: Path) -> ParameterList:
     """Read and parse an PX4-style XML parameter list."""
-    tree = eTree.parse(filepath)
-    root = tree.getroot()
+    try:
+        tree = eTree.parse(filepath)
+        root = tree.getroot()
 
-    param_list = ParameterList()
+        param_list = ParameterList()
+
+        # Parse all parameter groups
+        for group in root.findall("group"):
+            group_name = group.get("name")
+            for param_xml in get_group_params_xml(group):
+                param = build_param_from_xml(param_xml)
+                param.group = group_name
+                get_logger().debug(f"Created new parameter from XML: {param}")
+                param_list.add_param(param)
 
-    # Parse all parameter groups
-    for group in root.findall("group"):
-        group_name = group.get("name")
-        for param_xml in get_group_params_xml(group):
+        # Parse all loose parameters
+        for param_xml in root.findall("parameter"):
             param = build_param_from_xml(param_xml)
-            param.group = group_name.upper()
-            get_logger().debug(f"Created new parameter from XML: {param}")
             param_list.add_param(param)
 
-    # Parse all loose parameters
-    for param_xml in root.findall("parameter"):
-        param = build_param_from_xml(param_xml)
-        param_list.add_param(param)
-
-    return param_list
+        return param_list
+    except eTree.ParseError as e:
+        raise SyntaxError("File is not of XML format.") from e
 
 
+@parser
 def read_params_qgc(filepath: Path) -> ParameterList:
     """Read and parse a QGC/AMC/Auterion Suite parameters file."""
     param_list = ParameterList()
 
-    with open(filepath) as csvfile:
-        param_reader = csv.reader(csvfile, delimiter="\t")
-        for param_row in param_reader:  # pragma: no branch
-            get_logger().debug(f"Examining line: {param_row}")
-            if len(param_row) == 0:  # Skip empty lines
-                continue
-            if param_row[0][0] == "#":  # Skip comment lines
-                continue
-            # Test for wrong number of elements
-            if len(param_row) != 5:
-                raise SyntaxError("Wrong number of line elements")
-            param = build_param_from_qgc(param_row)
-            param_list.add_param(param)
+    try:
+        with open(filepath) as csvfile:
+            param_reader = csv.reader(csvfile, delimiter="\t")
+            for param_row in param_reader:  # pragma: no branch
+                get_logger().debug(f"Examining line: {param_row}")
+                if len(param_row) == 0:  # Skip empty lines
+                    continue
+                if param_row[0][0] == "#":  # Skip comment lines
+                    continue
+                # Test for wrong number of elements
+                if len(param_row) != 5:
+                    raise SyntaxError("Wrong number of line elements")
+                param = build_param_from_qgc(param_row)
+                param_list.add_param(param)
 
-    if len(param_list.params) == 0:
-        raise (SyntaxError("Could not extract any parameter from file."))
+        if len(param_list.params) == 0:
+            raise (SyntaxError("Could not extract any parameter from file."))
 
-    return param_list
+        return param_list
+    except SyntaxError as e:
+        raise SyntaxError(f"File is not of QGC format:\n{e}") from e
 
 
+@parser
 def read_params_ulog_param(filepath: Path) -> ParameterList:
     """Read and parse the outputs of the ulog_params program."""
     param_list = ParameterList()
 
-    with open(filepath) as csvfile:
-        param_reader = csv.reader(csvfile, delimiter=",")
-        for param_row in param_reader:  # pragma: no branch
-            # Check if line has exactly two elements
-            if len(param_row) != 2:
-                raise SyntaxError(
-                    f"Invalid number of elements for ulog param decoder: {len(param_row)}"
-                )
-            # Check if first element is a string
-            try:
-                float(param_row[0])
-                raise SyntaxError("First row element must be a parameter name string")
-            except ValueError:
-                pass
-            param = build_param_from_ulog_params(param_row)
-            param_list.add_param(param)
-
-    if len(param_list.params) == 0:
-        raise (SyntaxError("Could not extract any parameter from file."))
+    try:
+        with open(filepath) as csvfile:
+            param_reader = csv.reader(csvfile, delimiter=",")
+            for param_row in param_reader:  # pragma: no branch
+                if param_row[0][0] == "#":  # Skip comment lines
+                    continue
+                # Check if line has exactly two elements
+                if len(param_row) != 2:
+                    raise SyntaxError(
+                        f"Invalid number of elements for ulog param decoder: {len(param_row)}"
+                    )
+                # Check if first element is a string
+                try:
+                    float(param_row[0])
+                    raise SyntaxError(
+                        "First row element must be a parameter name string"
+                    )
+                except ValueError:
+                    pass
+                param = build_param_from_ulog_params(param_row)
+                param_list.add_param(param)
 
-    return param_list
+        if len(param_list.params) == 0:
+            raise (SyntaxError("Could not extract any parameter from file."))
 
+        return param_list
+    except SyntaxError as e:
+        raise SyntaxError(f"File is not of ulog format:\n{e}") from e
 
-def read_params(filepath: Path) -> ParameterList:
-    """Universal parameter reader."""
-    get_logger().debug(f"Attempting to read file {filepath}")
-    protocols_recognized = 0
 
+def split_mavproxy_row(row: str) -> Sequence:
+    """Split a line, assuming it is mavproxy syntax."""
+    params = row.split()
+    # Check if line has exactly two elements
+    if len(params) not in (2, 3):
+        raise SyntaxError(
+            f"Invalid number of elements for mavproxy param decoder: {len(params)}"
+        )
+    # Check if first element is a string
     try:
-        param_list = read_params_xml(filepath)
-        protocols_recognized += 1
-    except eTree.ParseError:
-        get_logger().debug("File is not of XML format.")
+        float(params[0])
+        raise SyntaxError("First row element must be a parameter name string.")
+    except ValueError:
         pass
+    try:
+        float(params[1])
+    except ValueError as e:
+        raise SyntaxError("First row element must be a parameter name string.") from e
+    # Insert empty reasoning if item 3 doesn't exist.
+    if len(params) == 2:
+        params.append("")
+
+    return params
+
+
+@parser
+def read_params_mavproxy(filepath: Path) -> ParameterList:
+    """Read and parse the outputs of mavproxy."""
+    param_list = ParameterList()
 
     try:
-        param_list = read_params_ulog_param(filepath)
-        protocols_recognized += 1
+        with open(filepath) as f:
+            for line in f:  # pragma: no branch
+                if line[0] == "#":  # Skip comment lines
+                    continue
+                params = split_mavproxy_row(line)
+                param = build_param_from_mavproxy(params)
+                param_list.add_param(param)
+
+        if len(param_list.params) == 0:
+            raise (SyntaxError("Could not extract any parameter from file."))
+
+        return param_list
     except SyntaxError as e:
-        get_logger().debug(f"File is not of ulog format:\n{e}")
-        pass
+        raise SyntaxError(f"File is not of mavproxy format:\n{e}") from e
 
-    try:
-        param_list = read_params_qgc(filepath)
-        protocols_recognized += 1
-    except SyntaxError:
-        get_logger().debug("File is not of QGC format.")
-        pass
-    # except ValueError:
-    #     pass
+
+def read_params(filepath: Path) -> ParameterList:
+    """Universal parameter reader."""
+    get_logger().debug(f"Attempting to read file {filepath}")
+    protocols_recognized = 0
+
+    for parser in parsers:
+        try:
+            param_list = parser(filepath)
+            protocols_recognized += 1
+        except SyntaxError as e:
+            get_logger().debug(e)
+            pass
 
     if protocols_recognized == 0:
         raise SyntaxError("Could not recognize log protocol.")
     if protocols_recognized > 1:
         raise SyntaxError("Protocol ambiguous, fits more than one parser.")
 
     # Add filename to list
```

### Comparing `parasect-1.1.2/src/parasect/build_lib.py` & `parasect-1.2.0/src/parasect/build_lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Union
 
 from ._helpers import Allergens
 from ._helpers import BoilerplateText
 from ._helpers import build_param_from_iter
 from ._helpers import ConfigPaths
 from ._helpers import DishModel
+from ._helpers import filter_regex
 from ._helpers import Formats
 from ._helpers import get_boilerplate
 from ._helpers import get_dish
 from ._helpers import get_logger
 from ._helpers import get_meals_menu
 from ._helpers import MealMenuModel
 from ._helpers import MealType
@@ -203,15 +204,17 @@
 class Meal:
     """An order able to build the full parameter list of a vehicle."""
 
     name = ""
     frame_id: int
     is_sitl = False
     is_hitl = False
+    add_header = False
     header: Optional[str] = None
+    add_footer = False
     footer: Optional[str] = None
     parent: Optional["Meal"] = None
     add_new = False
     remove_calibration_flag = False
     remove_operator_flag = False
     param_list: ParameterList
     default_param_list: ParameterList
@@ -234,15 +237,15 @@
         # Parse frame_id
         if "frame_id" in meal_dict.keys():
             self.frame_id = meal_dict["frame_id"]
         else:
             self.frame_id = 0
 
         # Parse the default parameters
-        self.parse_default_parameters(default_params_filepath)
+        self.parse_default_parameters(meal_dict, configs_path, default_params_filepath)
 
         self.parse_parent(
             meal_dict,
             meals_menu,
             default_params_filepath,
             configs_path,
         )
@@ -289,19 +292,14 @@
         # Remove blacklist parameters
         self.remove_blacklist(black_param_list, black_group_list)
 
         self.remove_calibration()
 
         self.remove_operator()
 
-        # Add the AUTOSTART value for each configuration
-        autostart = Parameter("SYS_AUTOSTART", self.frame_id)
-        autostart.param_type = "INT32"
-        self.param_list.add_param(autostart, safe=(not self.add_new))
-
     def parse_parent(
         self,
         meal_dict: MealType,
         all_meals: MealMenuModel,
         default_params_filepath: Optional[Path],
         configs_path: Path,
     ) -> None:
@@ -312,29 +310,63 @@
             self.parent = Meal(
                 all_meals, default_params_filepath, configs_path, parent_name  # type: ignore # Pydantic guarantees this is a string
             )
 
     def parse_header_footer(self, meal_dict: MealType) -> None:
         """Store the desired header and footer files."""
         # Bring in the parent's options first
-        if self.parent:
+        if self.parent and self.parent.add_header:
+            self.add_header = True
             self.header = self.parent.header
+
+        if self.parent and self.parent.add_footer:
+            self.add_footer = True
             self.footer = self.parent.footer
 
         # Overwrite with newly specified ones
         if "header" in meal_dict.keys():
+            self.add_header = True
             self.header = meal_dict["header"]  # type: ignore # Pydantic guarantees this is a string
         if "footer" in meal_dict.keys():
+            self.add_footer = True
             self.footer = meal_dict["footer"]  # type: ignore # Pydantic guarantees this is a string
 
-    def parse_default_parameters(self, default_params_filepath: Optional[Path]) -> None:
-        """Generate the default parameters list."""
-        if default_params_filepath:
+    def parse_default_parameters(
+        self,
+        meal_dict: MealType,
+        configs_path: Path,
+        default_params_filepath: Optional[Path],
+    ) -> None:
+        """Generate the default parameters list.
+
+        If a defaults path is passed in the meal, then it is used.
+        If its value is None, then explicitly don't set up any defaults.
+        If no defaults are passed in the meal, then the externally passed path is used.
+        """
+        if "defaults" in meal_dict.keys():
+            defaults_value = meal_dict["defaults"]
+            get_logger().debug(f"Using defaults from meal: {defaults_value}.")
+            if defaults_value:
+                defaults_path = Path(defaults_value)  # type: ignore
+                # 'defaults' is guaranteed to be a string or None. Pathing errors will surface on access.
+                # If a non-None defaults is passed,
+                # if the path passed is not absolute, assume is relative to the menu folder
+                if not defaults_path.is_absolute():
+                    defaults_path = configs_path / defaults_path
+                self.default_param_list = read_params(defaults_path)
+            else:
+                # If defaults is None, force an empty set.
+                self.default_param_list = ParameterList()
+        elif default_params_filepath:
+            get_logger().debug(
+                f"Using defaults externally passed: {default_params_filepath}."
+            )
             self.default_param_list = read_params(default_params_filepath)
         else:
+            get_logger().debug("Using empty defaults.")
             self.default_param_list = ParameterList()
 
     def load_base_parameters(self) -> None:
         """Load base parameter list."""
         if self.parent:
             # If a parent is specified, load their parameters
             self.param_list = self.parent.param_list
@@ -397,26 +429,22 @@
                 self.param_list.remove_param(param)
 
     def remove_calibration(self) -> None:
         """Remove calibration parameter from the blacklist."""
         if self.remove_calibration_flag:
             get_logger().debug(f"Removing calibration for {self.name}")
             # Remove calibration values (need to keep their list up-to-date)
-            calibration_params = Calibration()
-            for param in calibration_params:
-                self.param_list.remove_param(param)
+            filter_regex([s.name for s in Calibration()], self.param_list)
 
     def remove_operator(self) -> None:
         """Remove user data from the recipe."""
         if self.remove_operator_flag:
             get_logger().debug(f"Removing user data for {self.name}")
             # Remove user-defined values
-            user_params = Operator()
-            for param in user_params:
-                self.param_list.remove_param(param)
+            filter_regex([s.name for s in Operator()], self.param_list)
 
     def apply_edits(
         self,
         edited_param_list: ParameterList,
         default_params_filepath: Optional[Path],
     ) -> None:
         """Edit custom parameters."""
@@ -472,54 +500,74 @@
 
         return dishes_dict
 
     def build_header_footer(
         self,
         boilerplate_model: BoilerplateText,
         variant_name: Optional[str],
-        text_type: str,
+        format_type: Formats,
     ) -> Generator[str, None, None]:
         """Grab the header and footer sections from the corresponding dish."""
         # Load common list
-        get_logger().debug("Parsing common parameters")
+        get_logger().debug("Parsing common header/footer parameters")
 
         # Read text common across text_types
         common_text = boilerplate_model.common
         if common_text is not None:
             for row in common_text:
                 yield row + "\n"
 
         # Read text specific to the text_type
-        format_text = boilerplate_model.formats[text_type].common
+        format_text = boilerplate_model.formats[format_type.value].common
         if format_text is not None:
             for row in format_text:
                 yield row + "\n"
 
         # Read text specific to the meal
         if variant_name is not None:
-            variants = boilerplate_model.formats[text_type].variants
+            variants = boilerplate_model.formats[format_type.value].variants
             if variants is not None:
                 meal_text = variants[variant_name].common
                 for row in meal_text:  # type: ignore # Pydantic guarantees this is a List[str]
                     yield row + "\n"
 
     def __str__(self):
         """__str__ dunder method."""
         return self.param_list.__str__()
 
     def __contains__(self, item: Union[str, Parameter]) -> bool:
         """Answer if the Meal contains a parameter."""
         return self.param_list.__contains__(item)
 
+    def retrieve_header_footer(
+        self, option: str, fmt: Formats
+    ) -> Generator[str, None, None]:
+        """Retrieve a header or footer for a format export.
+
+        INPUTS:
+            option: "header" or "footer".
+            fmt: String representation of one of export Formats.
+        """
+        # Return empty if the meal needs no header or footer.
+        if option == "header" and not self.add_header:
+            return
+        if option == "footer" and not self.add_footer:
+            return
+
+        variant = getattr(self, option)
+        get_logger().debug(
+            f"Loading header/footer parameter {option}/{variant} for {fmt}."
+        )
+        model = get_boilerplate(ConfigPaths().staple_dishes, option)
+        yield from self.build_header_footer(model, variant, fmt)  # noqa
+
     def export_to_px4(self) -> Generator[str, None, None]:
         """Export as PX4 parameter file."""
         # Read header
-        get_logger().debug("Loading parameter header")
-        header_model = get_boilerplate(ConfigPaths().staple_dishes, "header")
-        yield from self.build_header_footer(header_model, self.header, "px4")
+        yield from self.retrieve_header_footer("header", Formats.px4)
 
         param_hashes = sorted(self.param_list.keys())
         for param_hash in param_hashes:
             param_name = self.param_list[param_hash].name
             param_value = self.param_list[param_hash].get_pretty_value()
             internal_type = self.param_list[param_hash].param_type
             if internal_type == "FLOAT":
@@ -536,42 +584,38 @@
             yield f"{vid}\t{cid}\t{param_name}\t{param_value}\t{param_type}\n"
 
     def export_to_px4af(self, version: int) -> Generator[str, None, None]:
         """PX4 airframe file build helper."""
         # Diversivy versions
         if version == 1:
             directive = "set"
-            dish = "px4afv1"
+            dish = Formats.px4afv1
         elif version == 2:
             directive = "set-default"
-            dish = "px4afv2"
+            dish = Formats.px4afv2
         else:
             raise ValueError(f"PX4 aiframe version {version} not supported.")
 
         # Read header
-        get_logger().debug("Loading parameter header.")
-        header_dish = get_boilerplate(ConfigPaths().staple_dishes, "header")
-        yield from self.build_header_footer(header_dish, self.header, dish)
+        yield from self.retrieve_header_footer("header", dish)
 
         if not self.is_sitl:
             indentation = "\t"
         else:
             indentation = ""
 
         param_hashes = sorted(self.param_list.keys())
         for param_hash in param_hashes:
             param_name = self.param_list[param_hash].name
             param_value = self.param_list[param_hash].get_pretty_value()
 
             yield f"{indentation}param {directive} {param_name} {param_value}\n"
 
         # Read footer
-        get_logger().debug("Loading parameter footer.")
-        footer_dict = get_boilerplate(ConfigPaths().staple_dishes, "footer")
-        yield from self.build_header_footer(footer_dict, self.footer, dish)
+        yield from self.retrieve_header_footer("footer", dish)
 
     def export_to_px4afv1(self) -> Generator[str, None, None]:
         """Export as legacy PX4 airframe file.
 
         Utilizes the 'param set' directive.
         """
         yield from self.export_to_px4af(1)
@@ -582,42 +626,81 @@
         Utilizes the 'param set-default' directive.
         """
         yield from self.export_to_px4af(2)
 
     def export_to_csv(self) -> Generator[str, None, None]:
         """Export as csv file."""
         # Read header
-        get_logger().debug("Loading parameter header.")
-        header_dish = get_boilerplate(ConfigPaths().staple_dishes, "header")
-        yield from self.build_header_footer(header_dish, self.header, "csv")
+        yield from self.retrieve_header_footer("header", Formats.csv)
 
         indentation = ""
 
         param_hashes = sorted(self.param_list.keys())
         for param_name in param_hashes:
             param_name = self.param_list[param_name].name
             param_value = self.param_list[param_name].get_pretty_value()
 
             yield f"{indentation}{param_name},{param_value}\n"
 
         # Read footer
-        get_logger().debug("Loading parameter footer.")
-        footer_dict = get_boilerplate(ConfigPaths().staple_dishes, "footer")
-        yield from self.build_header_footer(footer_dict, self.footer, "csv")
+        yield from self.retrieve_header_footer("footer", Formats.csv)
+
+    def export_to_apm(
+        self, include_readonly: bool = False
+    ) -> Generator[str, None, None]:
+        """Export as apm parameter file.
+
+        INPUTS:
+            include_readonly: flag to enable including @READONLY on a parameter.
+                Necessary for apj tools, unsuitable for loading via a GCS.
+        """
+        # Read header
+        yield from self.retrieve_header_footer("header", Formats.apm)
+
+        indentation = ""
+
+        param_hashes = sorted(self.param_list.keys())
+        for param_name in param_hashes:
+            param_name = self.param_list[param_name].name
+            param_value = self.param_list[param_name].get_pretty_value()
+            is_readonly = self.param_list[param_name].readonly
+            if include_readonly and is_readonly:
+                readonly_string = "\t@READONLY"
+            else:
+                readonly_string = ""
+
+            yield f"{indentation}{param_name}\t{param_value}{readonly_string}\n"
+
+        # Read footer
+        yield from self.retrieve_header_footer("footer", Formats.apm)
+
+    def apply_additions_px4(self) -> None:
+        # Add the AUTOSTART value for each configuration
+        autostart = Parameter("SYS_AUTOSTART", self.frame_id)
+        autostart.param_type = "INT32"
+        self.param_list.add_param(autostart, safe=(not self.add_new))
 
     def export(self, format: Formats) -> Iterable[str]:
         """Export general method."""
+        # Perform format-related additions.
         if format == Formats.csv:
             return self.export_to_csv()
         elif format == Formats.px4:
+            self.apply_additions_px4()
             return self.export_to_px4()
         elif format == Formats.px4afv1:
+            self.apply_additions_px4()
             return self.export_to_px4afv1()
         elif format == Formats.px4afv2:
+            self.apply_additions_px4()
             return self.export_to_px4afv2()
+        elif format == Formats.apm:
+            return self.export_to_apm(include_readonly=False)
+        elif format == Formats.apj:
+            return self.export_to_apm(include_readonly=True)
         else:
             raise ValueError(f"Output format {format} not supported.")
 
 
 def build_meals(names: Optional[List[str]] = None) -> Dict[str, Meal]:
     """Build the meal of the provided aircraft."""
     meals_menu = get_meals_menu(ConfigPaths().meals)
@@ -642,28 +725,30 @@
     return meals_dict
 
 
 def build_filename(format: Formats, meal: Meal) -> str:
     """Generate the output filename."""
     if format == Formats.csv:
         return f"{meal.name}.csv"
-    elif format == Formats.px4:
+    elif format in (Formats.px4,):
         return f"{meal.name}.params"
     elif format == Formats.px4afv1 or format == Formats.px4afv2:
         filename = f"{meal.frame_id}_{meal.name}"
         if meal.is_hitl:
             filename += ".hil"
         return filename
+    elif format in (Formats.apm, Formats.apj):
+        return f"{meal.name}.param"
     else:
         raise ValueError(f"Unsupported format {format}")
 
 
 def build_helper(
     meal_ordered: Optional[str],
-    format: Union[Formats, str],
+    format: Formats,
     input_folder: Optional[str],
     default_params: Optional[str],
     output_folder: Optional[str] = None,
     sitl: bool = False,
 ) -> None:
     """Build parameter sets.
 
@@ -693,22 +778,15 @@
 
     if default_params:
         ConfigPaths().DEFAULT_PARAMS_PATH = Path(default_params)
         get_logger().debug(
             f"Setting DEFAULT_PARAMS override to {ConfigPaths().default_parameters}"
         )
 
-    if isinstance(format, str):
-        output_format = Formats(format)
-    else:
-        output_format = format
-
-    get_logger().debug(
-        f"Building configuration {meal_ordered} for format {output_format}"
-    )
+    get_logger().debug(f"Building configuration {meal_ordered} for format {format}")
 
     # Generate the meals
     meals_dict = build_meals(meal_list)
 
     # Write output files in selected output
     output_folder_path = convert_str_to_path(output_folder)
 
@@ -721,19 +799,19 @@
         for _, meal in meals_dict.items():
             # Skip config if sitl/non-sitl is requested
             if (sitl) and (not meal.is_sitl):
                 continue
             if (not sitl) and meal.is_sitl:
                 continue
 
-            export_meal(meal, output_format, output_folder_path)
+            export_meal(meal, format, output_folder_path)
     else:
         # Export only a single config
         meal = meals_dict[meal_list[0]]
-        export_meal(meal, output_format, output_folder_path)
+        export_meal(meal, format, output_folder_path)
 
 
 def convert_str_to_path(path: Optional[str]) -> Optional[Path]:
     """Convert a str path representation to Optional[Path]."""
     if path:
         return Path(path)
     else:
```

### Comparing `parasect-1.1.2/src/parasect/compare_lib.py` & `parasect-1.2.0/src/parasect/compare_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Union
 
 from ._helpers import ConfigPaths
+from ._helpers import filter_regex
 from ._helpers import get_logger
 from ._helpers import read_params
 from .build_lib import Calibration
 from .build_lib import Operator
 from .build_lib import Parameter
 from .build_lib import ParameterList
 
@@ -35,21 +36,23 @@
     Each list item refers to a unique (vehicle-id, component-id) tuple
     """
     # Collect vehicle IDs and component IDs
     id_dict = collect_vid_cid(param_list_1, param_list_2)
 
     # Remove calibration parameters from both lists
     if nocal:
-        param_list_1 -= Calibration().param_list
-        param_list_2 -= Calibration().param_list
+        get_logger().debug("Removing calibration from comparison sets")
+        filter_regex([s.name for s in Calibration()], param_list_1)
+        filter_regex([s.name for s in Calibration()], param_list_2)
 
     # Remove user parameters from both lists
     if noop:
-        param_list_1 -= Operator().param_list
-        param_list_2 -= Operator().param_list
+        get_logger().debug("Removing operator params from comparison sets")
+        filter_regex([s.name for s in Operator()], param_list_1)
+        filter_regex([s.name for s in Operator()], param_list_2)
 
     # Generate comparison results
     comparison_results = list()
 
     # Iterate over all VIDs
     for vid, cids in id_dict.items():
         # Iterate over all CIDs:
@@ -95,15 +98,15 @@
     param_list_2: ParameterList,
     vid: Optional[int],
     cid: Optional[int],
 ) -> List[Tuple[Optional[Parameter], Optional[Parameter]]]:
     """Compare two parameter lists, potentially filtering with vid and cid.
 
     Returns a list of tuples. Each tuple contains the old parameter and the new parameter.
-    None is inserted if parameter does not exist
+    None is inserted if parameter does not exist.
     """
     param_names_1 = param_list_1.keys()
     param_names_2 = param_list_2.keys()
     all_param_names = sorted(set(param_names_1) | set(param_names_2))
 
     comparison_list = list()
```

### Comparing `parasect-1.1.2/PKG-INFO` & `parasect-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parasect
-Version: 1.1.2
+Version: 1.2.0
 Summary: Utility for manipulating parameter sets for autopilots.
 Home-page: https://github.com/AvyFly/parasect
 License: MIT
 Author: George Zogopoulos
 Author-email: geo.zogop.papal@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -80,14 +80,15 @@
 *Parasect* has two-fold capabilities:
 
 1. Compare two parameter sets and highlighting their differences.
 2. Parsing from user-defined content and generating new parameter sets, ready for loading into an autopilot.
 
 List of currently supported autopilots:
 
+* Ardupilot_
 * PX4_
 
 Requirements
 ------------
 
 *Parasect* is a pure-Python project. Its requirements are managed by the Poetry_ dependency manager.
 When you install *Parasect* via pip_ its requirements will also be installed automatically.
@@ -103,14 +104,22 @@
 
 You can install *Parasect* via pip_ from PyPI_:
 
 .. code:: console
 
    $ pip install parasect
 
+If you don't care about using *Parasect* as a library and are only interested in
+command-line use, you can also use `pipx`_, that provides better isolation from
+the rest of the system:
+
+.. code:: console
+
+   $ pipx install parasect
+
 
 Usage
 -----
 
 *Parasect* is primarily used as a command-line program.
 In its simplest form, two parameter files can be compared via:
 
@@ -151,23 +160,28 @@
 Credits
 -------
 
 This project was sponsored by `Avy B.V. <Avy_>`_, a UAV company in Amsterdam.
 
 This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
 
+The project logo was created by `Cynthia de Vries <Cynthia_>`_.
+
 .. _@cjolowicz: https://github.com/cjolowicz
+.. _Cynthia: https://www.linkedin.com/in/cynthia-de-vries-497991231/
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _PyPI: https://pypi.org/
 .. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 .. _file an issue: https://github.com/AvyFly/parasect/issues
 .. _pip: https://pip.pypa.io/
+.. _pipx: https://github.com/pypa/pipx
 .. _CLI usage: https://parasect.readthedocs.io/en/latest/reference.html#cli-reference
 .. _API usage: https://parasect.readthedocs.io/en/latest/reference.html#api-reference
 .. _Concepts: https://parasect.readthedocs.io/en/latest/concepts.html
 .. _PX4: https://px4.io/
+.. _Ardupilot: https://ardupilot.org/
 .. _Poetry: https://python-poetry.org/
 .. _Avy: https://avy.eu
 .. github-only
 .. _Contributor Guide: CONTRIBUTING.rst
```

