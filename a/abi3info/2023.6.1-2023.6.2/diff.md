# Comparing `tmp/abi3info-2023.6.1.tar.gz` & `tmp/abi3info-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2023.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3info-2023.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `abi3info-2023.6.1.tar` & `abi3info-2023.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-06-01 05:02:17.806133 abi3info-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1915 2023-06-01 05:02:17.806133 abi3info-2023.6.1/README.md
--rw-r--r--   0        0        0     1038 2023-06-01 05:02:17.806133 abi3info-2023.6.1/abi3info/__init__.py
--rw-r--r--   0        0        0   190490 2023-06-01 05:02:17.806133 abi3info-2023.6.1/abi3info/_internal.py
--rw-r--r--   0        0        0     7791 2023-06-01 05:02:17.806133 abi3info-2023.6.1/abi3info/models.py
--rw-r--r--   0        0        0     1885 2023-06-01 05:02:17.806133 abi3info-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 abi3info-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-02 22:35:00.674314 abi3info-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     1915 2023-06-02 22:35:00.674314 abi3info-2023.6.2/README.md
+-rw-r--r--   0        0        0     1038 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/__init__.py
+-rw-r--r--   0        0        0   190471 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/_internal.py
+-rw-r--r--   0        0        0     7791 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/models.py
+-rw-r--r--   0        0        0     1885 2023-06-02 22:35:00.674314 abi3info-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 abi3info-2023.6.2/PKG-INFO
```

### Comparing `abi3info-2023.6.1/LICENSE` & `abi3info-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.1/README.md` & `abi3info-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.1/abi3info/__init__.py` & `abi3info-2023.6.2/abi3info/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2023.06.01"
+__version__ = "2023.06.02"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2023.6.1/abi3info/_internal.py` & `abi3info-2023.6.2/abi3info/_internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PyCFunction_Call"): Function(
         symbol=Symbol(name="PyCFunction_Call"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyCFunction_GetFlags"): Function(
         symbol=Symbol(name="PyCFunction_GetFlags"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -790,15 +790,15 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PyEval_AcquireLock"): Function(
         symbol=Symbol(name="PyEval_AcquireLock"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyEval_AcquireThread"): Function(
         symbol=Symbol(name="PyEval_AcquireThread"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -880,21 +880,21 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PyEval_InitThreads"): Function(
         symbol=Symbol(name="PyEval_InitThreads"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyEval_ReleaseLock"): Function(
         symbol=Symbol(name="PyEval_ReleaseLock"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyEval_ReleaseThread"): Function(
         symbol=Symbol(name="PyEval_ReleaseThread"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -910,15 +910,15 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PyEval_ThreadsInitialized"): Function(
         symbol=Symbol(name="PyEval_ThreadsInitialized"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyException_GetCause"): Function(
         symbol=Symbol(name="PyException_GetCause"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -2290,21 +2290,21 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PySys_AddWarnOption"): Function(
         symbol=Symbol(name="PySys_AddWarnOption"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_AddWarnOptionUnicode"): Function(
         symbol=Symbol(name="PySys_AddWarnOptionUnicode"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_FormatStderr"): Function(
         symbol=Symbol(name="PySys_FormatStderr"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -2320,45 +2320,45 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PySys_HasWarnOptions"): Function(
         symbol=Symbol(name="PySys_HasWarnOptions"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_ResetWarnOptions"): Function(
         symbol=Symbol(name="PySys_ResetWarnOptions"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PySys_SetArgv"): Function(
         symbol=Symbol(name="PySys_SetArgv"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_SetArgvEx"): Function(
         symbol=Symbol(name="PySys_SetArgvEx"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_SetObject"): Function(
         symbol=Symbol(name="PySys_SetObject"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PySys_SetPath"): Function(
         symbol=Symbol(name="PySys_SetPath"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_WriteStderr"): Function(
         symbol=Symbol(name="PySys_WriteStderr"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -3256,21 +3256,21 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="Py_SetProgramName"): Function(
         symbol=Symbol(name="Py_SetProgramName"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="Py_SetPythonHome"): Function(
         symbol=Symbol(name="Py_SetPythonHome"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="Py_SetRecursionLimit"): Function(
         symbol=Symbol(name="Py_SetRecursionLimit"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=False,
     ),
@@ -3370,33 +3370,33 @@
         ifdef=None,
         abi_only=True,
     ),
     Symbol(name="PyObject_AsCharBuffer"): Function(
         symbol=Symbol(name="PyObject_AsCharBuffer"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyObject_AsReadBuffer"): Function(
         symbol=Symbol(name="PyObject_AsReadBuffer"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyObject_AsWriteBuffer"): Function(
         symbol=Symbol(name="PyObject_AsWriteBuffer"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyObject_CheckReadBuffer"): Function(
         symbol=Symbol(name="PyObject_CheckReadBuffer"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyMarshal_ReadObjectFromString"): Function(
         symbol=Symbol(name="PyMarshal_ReadObjectFromString"),
         added=PyVersion(major=3, minor=2),
         ifdef=None,
         abi_only=True,
     ),
@@ -3762,15 +3762,15 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="PySys_AddXOption"): Function(
         symbol=Symbol(name="PySys_AddXOption"),
         added=PyVersion(major=3, minor=7),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PySys_GetXOptions"): Function(
         symbol=Symbol(name="PySys_GetXOptions"),
         added=PyVersion(major=3, minor=7),
         ifdef=None,
         abi_only=False,
     ),
@@ -3852,15 +3852,15 @@
         ifdef=None,
         abi_only=False,
     ),
     Symbol(name="Py_SetPath"): Function(
         symbol=Symbol(name="Py_SetPath"),
         added=PyVersion(major=3, minor=7),
         ifdef=None,
-        abi_only=False,
+        abi_only=True,
     ),
     Symbol(name="PyErr_SetExcFromWindowsErr"): Function(
         symbol=Symbol(name="PyErr_SetExcFromWindowsErr"),
         added=PyVersion(major=3, minor=7),
         ifdef=FeatureMacro(name="MS_WINDOWS", doc="on Windows", windows=True),
         abi_only=False,
     ),
```

### Comparing `abi3info-2023.6.1/abi3info/models.py` & `abi3info-2023.6.2/abi3info/models.py`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.1/pyproject.toml` & `abi3info-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.1/PKG-INFO` & `abi3info-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

