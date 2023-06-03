# Comparing `tmp/triad-0.8.8.tar.gz` & `tmp/triad-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.8.tar", last modified: Tue May 23 06:36:43 2023, max compression
+gzip compressed data, was "triad-0.8.9.tar", last modified: Sat Jun  3 06:34:12 2023, max compression
```

## Comparing `triad-0.8.8.tar` & `triad-0.8.9.tar`

### file list

```diff
@@ -1,69 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 06:36:03.000000 triad-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-23 06:36:43.625054 triad-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-23 06:36:03.000000 triad-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 06:36:43.625054 triad-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-23 06:36:03.000000 triad-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:03.000000 triad-0.8.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/convert_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/utils/dispatcher_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pyarrow_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 06:36:03.000000 triad-0.8.8/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 06:36:03.000000 triad-0.8.8/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 06:36:03.000000 triad-0.8.8/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 06:36:03.000000 triad-0.8.8/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-03 06:33:22.000000 triad-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-03 06:34:12.801595 triad-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-03 06:33:22.000000 triad-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-03 06:34:12.801595 triad-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-03 06:33:22.000000 triad-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.789595 triad-0.8.9/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-03 06:33:22.000000 triad-0.8.9/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.793595 triad-0.8.9/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 06:33:22.000000 triad-0.8.9/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-03 06:33:22.000000 triad-0.8.9/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/batch_reslicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.793595 triad-0.8.9/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 06:33:22.000000 triad-0.8.9/triad_version/__init__.py
```

### Comparing `triad-0.8.8/LICENSE` & `triad-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/PKG-INFO` & `triad-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.8
+Version: 0.8.9
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,19 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.9
+        
+        * Add batch reslicers
+        * Fix package issue (exclude tests folder)
+        
         ### 0.8.8
         
         * Add type replacement utils for pyarrow
         
         ### 0.8.7
         
         * Fix pandas 2.0 warnings
```

### Comparing `triad-0.8.8/README.md` & `triad-0.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.8.9
+
+* Add batch reslicers
+* Fix package issue (exclude tests folder)
+
 ### 0.8.8
 
 * Add type replacement utils for pyarrow
 
 ### 0.8.7
 
 * Fix pandas 2.0 warnings
```

### Comparing `triad-0.8.8/setup.py` & `triad-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="triad",
     version=__version__,
-    packages=find_packages(),
+    packages=find_packages(include=["triad*"]),
     description="A collection of python utils for Fugue projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="fugue util utils utility utilities",
```

### Comparing `triad-0.8.8/triad/collections/dict.py` & `triad-0.8.9/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/collections/fs.py` & `triad-0.8.9/triad/collections/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             path=_path,
             namespaces=namespaces,
             case_sensitive=case_sensitive,
             exclude_dirs=exclude_dirs,
         )
 
 
-class _FSPath(object):
+class _FSPath:
     def __init__(self, path: str):
         if path is None:
             raise ValueError("path can't be None")
         path = _modify_path(path)
         self._is_windows = False
         if _is_windows(path):
             self._scheme = ""
```

### Comparing `triad-0.8.8/triad/collections/function_wrapper.py` & `triad-0.8.9/triad/collections/function_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..utils.assertion import assert_or_throw
 from ..utils.convert import get_full_type_path
 from ..utils.entry_points import load_entry_point
 from ..utils.hash import to_uuid
 from .dict import IndexedOrderedDict
 
 
-class FunctionWrapper(object):
+class FunctionWrapper:
     """Create a function wrapper that can recognize and validate all
     input types.
 
     :param func: the function to be wrapped
     :param params_re: paramter types regex expression
     :param return_re: return types regex expression
```

### Comparing `triad-0.8.8/triad/collections/schema.py` & `triad-0.8.9/triad/collections/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/assertion.py` & `triad-0.8.9/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/class_extension.py` & `triad-0.8.9/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/convert.py` & `triad-0.8.9/triad/utils/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     :raises ValueError: unable to find a matching object
 
     .. admonition:: Examples
 
         .. code-block:: python
 
-            class _Mock(object):
+            class _Mock:
                 def __init__(self, x=1):
                     self.x = x
 
             m = _Mock()
             assert 1 == str_to_object("m.x")
             assert 1 == str_to_object("m2.x", local_vars={"m2": m})
             assert RuntimeError == str_to_object("RuntimeError")
```

### Comparing `triad-0.8.8/triad/utils/dispatcher.py` & `triad-0.8.9/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/entry_points.py` & `triad-0.8.9/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/hash.py` & `triad-0.8.9/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/iter.py` & `triad-0.8.9/triad/utils/iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                 self._last = next(self._iter)
                 self._state = 1  # last filed not used
         except StopIteration:
             self._state = 3  # end
         return self._state
 
 
-class Slicer(object):
+class Slicer:
     """A better version of :func:`~triad.iter.slice_iterable`
 
     :param sizer: the function to get size of an item
     :param row_limit: max row for each slice, defaults to None
     :param size_limit: max byte size for each slice, defaults to None
     :param slicer: taking in current number, current value, last value,
         it decides if it's a new slice
```

### Comparing `triad-0.8.8/triad/utils/json.py` & `triad-0.8.9/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/pandas_like.py` & `triad-0.8.9/triad/utils/pandas_like.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/pyarrow.py` & `triad-0.8.9/triad/utils/pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
     if pa.types.is_date(data_type):
         return _date_eq
     if pa.types.is_timestamp(data_type):
         return _timestamp_eq
     return _general_eq
 
 
-class SchemaedDataPartitioner(object):
+class SchemaedDataPartitioner:
     """Partitioner for stream of array like data with given schema.
     It uses :func"`~triad.utils.iter.Slicer` to partition the stream
 
     :param schema: the schema of the data stream to process
     :param key_positions: positions of partition keys on `schema`
     :param sizer: the function to get size of an item
     :param row_limit: max row for each slice, defaults to None
@@ -807,15 +807,15 @@
     raise NotImplementedError(f"{obj} can't be converted to map")
 
 
 def _no_op_convert(obj: Any) -> Any:  # pragma: no cover
     return obj
 
 
-class _TypeConverter(object):
+class _TypeConverter:
     _CONVERTERS: Dict[pa.DataType, Any] = {
         pa.null(): _to_pynone,
         pa.string(): _to_pystr,
         pa.bool_(): _to_pybool,
         pa.int8(): _to_pyint,
         pa.int16(): _to_pyint,
         pa.int32(): _to_pyint,
```

### Comparing `triad-0.8.8/triad/utils/rename.py` & `triad-0.8.9/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/schema.py` & `triad-0.8.9/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/string.py` & `triad-0.8.9/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad/utils/threading.py` & `triad-0.8.9/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.8/triad.egg-info/PKG-INFO` & `triad-0.8.9/triad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.8
+Version: 0.8.9
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,19 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.9
+        
+        * Add batch reslicers
+        * Fix package issue (exclude tests folder)
+        
         ### 0.8.8
         
         * Add type replacement utils for pyarrow
         
         ### 0.8.7
         
         * Fix pandas 2.0 warnings
```

