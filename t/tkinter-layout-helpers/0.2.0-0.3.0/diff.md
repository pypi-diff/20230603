# Comparing `tmp/tkinter_layout_helpers-0.2.0.tar.gz` & `tmp/tkinter_layout_helpers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_layout_helpers-0.2.0.tar", max compression
+gzip compressed data, was "tkinter_layout_helpers-0.3.0.tar", max compression
```

## Comparing `tkinter_layout_helpers-0.2.0.tar` & `tkinter_layout_helpers-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/LICENSE
--rw-r--r--   0        0        0     1934 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/README.md
--rw-r--r--   0        0        0      923 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      130 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/grid_helper.py
--rw-r--r--   0        0        0     1703 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/pack_helper.py
--rw-r--r--   0        0        0      687 2023-05-26 17:17:40.480941 tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/parent_manager.py
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 tkinter_layout_helpers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2141 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/README.md
+-rw-r--r--   0        0        0      923 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/__init__.py
+-rw-r--r--   0        0        0     3235 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/grid_helper.py
+-rw-r--r--   0        0        0     1733 2023-06-03 11:02:28.108512 tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/pack_helper.py
+-rw-r--r--   0        0        0      771 2023-06-03 11:02:28.112513 tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/parent_manager.py
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 tkinter_layout_helpers-0.3.0/PKG-INFO
```

### Comparing `tkinter_layout_helpers-0.2.0/LICENSE` & `tkinter_layout_helpers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_layout_helpers-0.2.0/README.md` & `tkinter_layout_helpers-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Tkinter Layout Helpers
 
 [![Python package](https://github.com/insolor/tkinter_layout_helpers/actions/workflows/python-tests.yml/badge.svg)](https://github.com/insolor/tkinter_layout_helpers/actions/workflows/python-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/insolor/tkinter_layout_helpers/badge.svg?branch=master)](https://coveralls.io/github/insolor/tkinter_layout_helpers?branch=master)
+[![PyPI](https://img.shields.io/pypi/v/tkinter_layout_helpers)](https://pypi.org/project/tkinter_layout_helpers/)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/tkinter_layout_helpers)
+
 
 A library which is intended to simplify a placement of widgets with `.grid()` and `.pack()` methods:
 
 - avoid manual calculation of indices of columns and rows when you add a widget;
 - avoid typing-in some common parameters (like `sticky=tk.EW`) each time you add a widget;
 - and more...
```

### Comparing `tkinter_layout_helpers-0.2.0/pyproject.toml` & `tkinter_layout_helpers-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkinter_layout_helpers"
-version = "0.2.0"
+version = "0.3.0"
 description = "A library which is intended to simplify a placement of widgets with .grid() and .pack() methods"
 authors = ["insolor <insolor@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/insolor/tkinter_layout_helpers"
 repository = "https://github.com/insolor/tkinter_layout_helpers"
 keywords = ["tkinter", "grid", "pack"]
@@ -18,13 +18,13 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
-pytest-cov = "^4.0.0"
-flake8 = "^4.0.1"
+pytest-cov = "^4.1.0"
+flake8 = "^5.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/grid_helper.py` & `tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/grid_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import contextlib
 import tkinter as tk
 from dataclasses import dataclass, field
-from typing import Any, ContextManager, Dict, List, Union
+from typing import Any, ContextManager, Dict, Generic, List
 
-from tkinter_layout_helpers.parent_manager import set_parent
+from tkinter_layout_helpers.parent_manager import TParent, set_parent
 
 
 @dataclass
 class Cell:
     widget: tk.Widget
     column_index: int
     row_index: int
@@ -60,21 +60,21 @@
         self.__grid.parent.grid_rowconfigure(self.__row_index, *args, **kwargs)
 
     @property
     def cells(self) -> List[Cell]:
         return self.__cells
 
 
-class Grid:
-    parent: tk.Widget
+class Grid(Generic[TParent]):
+    parent: TParent
     rows: List[Row]
     __row_index: int
     __kwargs: Dict[str, Any]
 
-    def __init__(self, parent: tk.Widget, **kwargs):
+    def __init__(self, parent: TParent, **kwargs):
         self.parent = parent
         self.rows = []
         self.__row_index = 0
         self.__kwargs = kwargs
 
     def new_row(self) -> Row:
         row = Row(self, self.__row_index)
@@ -104,12 +104,12 @@
                 )
                 # Parameters of add() override all the previous parameters
                 kwargs.update(cell.options)
                 cell.widget.grid(**kwargs)
 
 
 @contextlib.contextmanager
-def grid_manager(parent: Union[tk.Tk, tk.Widget], **kwargs) -> ContextManager[Grid]:
+def grid_manager(parent: TParent, **kwargs) -> ContextManager[Grid]:
     with set_parent(parent):
         grid = Grid(parent, **kwargs)
         yield grid
         grid.build()
```

### Comparing `tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/pack_helper.py` & `tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/pack_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import contextlib
 import tkinter as tk
-from typing import Any, ContextManager, Mapping
+from typing import Any, ContextManager, Generic, Mapping
 
-from tkinter_layout_helpers.parent_manager import set_parent
+from tkinter_layout_helpers.parent_manager import TParent, set_parent
 
 
 def pack_expanded(widget: tk.Widget, **kwargs):
     kwargs.update(dict(fill=tk.BOTH, expand=True))
     widget.pack(**kwargs)
 
 
-class Packer:
-    parent: tk.Widget
+class Packer(Generic[TParent]):
+    parent: TParent
     __kwargs: Mapping[str, Any]
 
-    def __init__(self, parent: tk.Widget, **kwargs):
+    def __init__(self, parent: TParent, **kwargs):
         self.parent = parent
         self.__kwargs = kwargs
 
     def pack_all(self, *args: tk.Widget, **kwargs):
         kwargs.update(self.__kwargs)
         for item in args:
             item.pack(**kwargs)
@@ -50,11 +50,11 @@
 
     def pack_expanded(self, widget: tk.Widget, **kwargs):
         pack_expanded(widget, **self.__kwargs, **kwargs)
         return self
 
 
 @contextlib.contextmanager
-def pack_manager(parent: tk.Widget, **kwargs) -> ContextManager[Packer]:
+def pack_manager(parent: TParent, **kwargs) -> ContextManager[Packer]:
     with set_parent(parent):
         packer = Packer(parent, **kwargs)
         yield packer
```

### Comparing `tkinter_layout_helpers-0.2.0/tkinter_layout_helpers/parent_manager.py` & `tkinter_layout_helpers-0.3.0/tkinter_layout_helpers/parent_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import contextlib
 import tkinter as tk
-from typing import ContextManager
+from typing import ContextManager, TypeVar, Union
+
+TParent = TypeVar("TParent", bound=Union[tk.Tk, tk.Toplevel, tk.Widget])
 
 
 class DefaultRootWrapper:  # pragma: no cover
     @property
     def default_root(self) -> tk.Widget:
         return tk._default_root  # type: ignore # noqa
 
     @default_root.setter
-    def default_root(self, value: tk.Widget):
+    def default_root(self, value: TParent):
         tk._default_root = value  # type: ignore
 
 
 _default_root_wrapper = DefaultRootWrapper()
 
 
 @contextlib.contextmanager
-def set_parent(parent: tk.Widget) -> ContextManager[tk.Widget]:
+def set_parent(parent: TParent) -> ContextManager[TParent]:
     old_root = _default_root_wrapper.default_root
     _default_root_wrapper.default_root = parent
     try:
         yield parent
     finally:
         _default_root_wrapper.default_root = old_root
```

### Comparing `tkinter_layout_helpers-0.2.0/PKG-INFO` & `tkinter_layout_helpers-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinter-layout-helpers
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library which is intended to simplify a placement of widgets with .grid() and .pack() methods
 Home-page: https://github.com/insolor/tkinter_layout_helpers
 License: MIT
 Keywords: tkinter,grid,pack
 Author: insolor
 Author-email: insolor@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -22,14 +22,17 @@
 Project-URL: Repository, https://github.com/insolor/tkinter_layout_helpers
 Description-Content-Type: text/markdown
 
 # Tkinter Layout Helpers
 
 [![Python package](https://github.com/insolor/tkinter_layout_helpers/actions/workflows/python-tests.yml/badge.svg)](https://github.com/insolor/tkinter_layout_helpers/actions/workflows/python-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/insolor/tkinter_layout_helpers/badge.svg?branch=master)](https://coveralls.io/github/insolor/tkinter_layout_helpers?branch=master)
+[![PyPI](https://img.shields.io/pypi/v/tkinter_layout_helpers)](https://pypi.org/project/tkinter_layout_helpers/)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/tkinter_layout_helpers)
+
 
 A library which is intended to simplify a placement of widgets with `.grid()` and `.pack()` methods:
 
 - avoid manual calculation of indices of columns and rows when you add a widget;
 - avoid typing-in some common parameters (like `sticky=tk.EW`) each time you add a widget;
 - and more...
```

