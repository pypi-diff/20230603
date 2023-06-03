# Comparing `tmp/asyncgnostic-0.1.0.tar.gz` & `tmp/asyncgnostic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncgnostic-0.1.0.tar", max compression
+gzip compressed data, was "asyncgnostic-0.1.1.tar", max compression
```

## Comparing `asyncgnostic-0.1.0.tar` & `asyncgnostic-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-06-03 04:10:44.943482 asyncgnostic-0.1.0/LICENSE
--rw-r--r--   0        0        0      982 2023-06-03 04:10:44.943482 asyncgnostic-0.1.0/README.md
--rw-r--r--   0        0        0      484 2023-06-03 04:10:44.943482 asyncgnostic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2858 2023-06-03 04:10:44.943482 asyncgnostic-0.1.0/src/asyncgnostic/__init__.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 asyncgnostic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1232 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/README.md
+-rw-r--r--   0        0        0      484 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3074 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/src/asyncgnostic/__init__.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 asyncgnostic-0.1.1/PKG-INFO
```

### Comparing `asyncgnostic-0.1.0/LICENSE` & `asyncgnostic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgnostic-0.1.0/README.md` & `asyncgnostic-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,41 +8,55 @@
 ## Example:
 
 ```python
 import asyncio
 from asyncgnostic import awaitable
 
 
-def handler() -> str:
+# Define a sync function
+def handler() -> str:  # type: ignore
     return "Running Sync"
 
 
+# Pair the sync function with an async function
 @awaitable(handler)
 async def handler() -> str:
     return "Running Async"
 
 
+# Call the function from sync context
 def sync_main():
     print("sync context", handler())
 
 
+# Call the function from async context
 async def async_main():
     print("async context:", await handler())
 
 
+# Run the sync and async functions
 sync_main()
 asyncio.run(async_main())
 ```
 
 Output:
 
 ```console
 sync context Running Sync
 async context: Running Async
 ```
+
+
+## Install
+
+```
+pip install asyncgnostic
+```
+
+
 ## Credits:
 
 Gratefully borrowed improvements from [curio](https://github.com/dabeaz/curio/).
 
 Reference:
   - https://mastodon.sharma.io/@harshad/110476942596328864
   - https://mastodon.social/@dabeaz/110477080111974062
```

### Comparing `asyncgnostic-0.1.0/src/asyncgnostic/__init__.py` & `asyncgnostic-0.1.1/src/asyncgnostic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Borrows heavily from Curio's meta.py module:
+
+https://github.com/dabeaz/curio/blob/master/curio/meta.py
+
+Curio is licensed under the BSD 3-Clause License.
+
+https://github.com/dabeaz/curio/blob/master/LICENSE
+"""
 from sys import _getframe
 from functools import wraps as _wraps
 import inspect as _inspect
 
 
 def awaited(depth=2, _cache={}) -> bool:
     """
```

### Comparing `asyncgnostic-0.1.0/PKG-INFO` & `asyncgnostic-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncgnostic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python functions agnostic towards being called with await or otherwise.
 License: MIT
 Author: Harshad Sharma
 Author-email: harshad@sharma.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,41 +23,55 @@
 ## Example:
 
 ```python
 import asyncio
 from asyncgnostic import awaitable
 
 
-def handler() -> str:
+# Define a sync function
+def handler() -> str:  # type: ignore
     return "Running Sync"
 
 
+# Pair the sync function with an async function
 @awaitable(handler)
 async def handler() -> str:
     return "Running Async"
 
 
+# Call the function from sync context
 def sync_main():
     print("sync context", handler())
 
 
+# Call the function from async context
 async def async_main():
     print("async context:", await handler())
 
 
+# Run the sync and async functions
 sync_main()
 asyncio.run(async_main())
 ```
 
 Output:
 
 ```console
 sync context Running Sync
 async context: Running Async
 ```
+
+
+## Install
+
+```
+pip install asyncgnostic
+```
+
+
 ## Credits:
 
 Gratefully borrowed improvements from [curio](https://github.com/dabeaz/curio/).
 
 Reference:
   - https://mastodon.sharma.io/@harshad/110476942596328864
   - https://mastodon.social/@dabeaz/110477080111974062
```

