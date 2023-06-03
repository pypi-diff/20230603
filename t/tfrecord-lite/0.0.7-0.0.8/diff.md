# Comparing `tmp/tfrecord_lite-0.0.7.tar.gz` & `tmp/tfrecord_lite-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfrecord_lite-0.0.7.tar", last modified: Fri Feb  7 09:11:36 2020, max compression
+gzip compressed data, was "tfrecord_lite-0.0.8.tar", last modified: Sat Jun  3 20:33:55 2023, max compression
```

## Comparing `tfrecord_lite-0.0.7.tar` & `tfrecord_lite-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     1057 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/LICENSE
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)       92 2020-02-07 08:51:55.000000 tfrecord_lite-0.0.7/MANIFEST.in
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)      767 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/PKG-INFO
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     1253 2020-02-07 08:58:00.000000 tfrecord_lite-0.0.7/README.md
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)       38 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/setup.cfg
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     1982 2020-02-07 09:09:32.000000 tfrecord_lite-0.0.7/setup.py
-drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/src/
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     2297 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/example.pb.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     2139 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/example.pb.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     4633 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/feature.pb.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     5888 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/feature.pb.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)    22670 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     2993 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_common.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     1421 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_common.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)    45657 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_decode.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     6503 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_decode.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)    25394 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_encode.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     6291 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/pb_encode.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     4207 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/tfrecord_lite.cpp
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)      694 2020-02-07 07:34:40.000000 tfrecord_lite-0.0.7/src/tfrecord_lite.h
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)   296278 2020-02-07 09:10:59.000000 tfrecord_lite-0.0.7/tfrecord_lite.cpp
-drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)      767 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/PKG-INFO
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)      483 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/SOURCES.txt
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)        1 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/dependency_links.txt
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)        6 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/requires.txt
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)       14 2020-02-07 09:11:36.000000 tfrecord_lite-0.0.7/tfrecord_lite.egg-info/top_level.txt
--rw-r--r--   0 jongwook  (1000) jongwook  (1000)     2897 2020-02-07 09:10:41.000000 tfrecord_lite-0.0.7/tfrecord_lite.pyx
+drwxr-xr-x   0 jongwook   (501) staff       (20)        0 2023-06-03 20:33:55.400682 tfrecord_lite-0.0.8/
+-rw-r--r--   0 jongwook   (501) staff       (20)     1057 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/LICENSE
+-rw-r--r--   0 jongwook   (501) staff       (20)      115 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/MANIFEST.in
+-rw-r--r--   0 jongwook   (501) staff       (20)      750 2023-06-03 20:33:55.400363 tfrecord_lite-0.0.8/PKG-INFO
+-rw-r--r--   0 jongwook   (501) staff       (20)     1253 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/README.md
+-rw-r--r--   0 jongwook   (501) staff       (20)      106 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/pyproject.toml
+-rw-r--r--   0 jongwook   (501) staff       (20)       38 2023-06-03 20:33:55.400740 tfrecord_lite-0.0.8/setup.cfg
+-rw-r--r--   0 jongwook   (501) staff       (20)     1982 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/setup.py
+drwxr-xr-x   0 jongwook   (501) staff       (20)        0 2023-06-03 20:33:55.391640 tfrecord_lite-0.0.8/src/
+-rw-r--r--   0 jongwook   (501) staff       (20)     2297 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/example.pb.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)     2139 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/example.pb.h
+-rw-r--r--   0 jongwook   (501) staff       (20)     4633 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/feature.pb.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)     5888 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/feature.pb.h
+-rw-r--r--   0 jongwook   (501) staff       (20)    22670 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb.h
+-rw-r--r--   0 jongwook   (501) staff       (20)     2993 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_common.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)     1421 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_common.h
+-rw-r--r--   0 jongwook   (501) staff       (20)    45657 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_decode.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)     6503 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_decode.h
+-rw-r--r--   0 jongwook   (501) staff       (20)    25394 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_encode.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)     6291 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/pb_encode.h
+-rw-r--r--   0 jongwook   (501) staff       (20)     4207 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/tfrecord_lite.cpp
+-rw-r--r--   0 jongwook   (501) staff       (20)      694 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/src/tfrecord_lite.h
+-rw-r--r--   0 jongwook   (501) staff       (20)   416673 2023-06-03 20:33:54.000000 tfrecord_lite-0.0.8/tfrecord_lite.cpp
+drwxr-xr-x   0 jongwook   (501) staff       (20)        0 2023-06-03 20:33:55.399828 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/
+-rw-r--r--   0 jongwook   (501) staff       (20)      750 2023-06-03 20:33:55.000000 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/PKG-INFO
+-rw-r--r--   0 jongwook   (501) staff       (20)      498 2023-06-03 20:33:55.000000 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 jongwook   (501) staff       (20)        1 2023-06-03 20:33:55.000000 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 jongwook   (501) staff       (20)        6 2023-06-03 20:33:55.000000 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/requires.txt
+-rw-r--r--   0 jongwook   (501) staff       (20)       14 2023-06-03 20:33:55.000000 tfrecord_lite-0.0.8/tfrecord_lite.egg-info/top_level.txt
+-rw-r--r--   0 jongwook   (501) staff       (20)     2906 2023-06-03 20:33:22.000000 tfrecord_lite-0.0.8/tfrecord_lite.pyx
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tfrecord_lite-0.0.7/LICENSE` & `tfrecord_lite-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/PKG-INFO` & `tfrecord_lite-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tfrecord_lite
-Version: 0.0.7
+Version: 0.0.8
 Summary: A lightweight tfrecord parser
 Home-page: https://github.com/jongwook/tfrecord_lite
 Author: Jong Wook Kim
 Author-email: jongwook@nyu.edu
 License: MIT
 Project-URL: Source, https://github.com/jongwook/tfrecord_lite
 Project-URL: Tracker, https://github.com/jongwook/tfrecord_lite/issues
-Description: UNKNOWN
 Keywords: tfrecord
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+License-File: LICENSE
```

### Comparing `tfrecord_lite-0.0.7/README.md` & `tfrecord_lite-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/setup.py` & `tfrecord_lite-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 if "darwin" in sys.platform:
     extra_compile_args += ["-mmacosx-version-min=10.9"]
     extra_link_args=["-stdlib=libc++", "-mmacosx-version-min=10.9"]
 
 setup(
     name="tfrecord_lite",
-    version="0.0.7",
+    version="0.0.8",
     description="A lightweight tfrecord parser",
     url="https://github.com/jongwook/tfrecord_lite",
     author="Jong Wook Kim",
     author_email="jongwook@nyu.edu",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `tfrecord_lite-0.0.7/src/example.pb.cpp` & `tfrecord_lite-0.0.8/src/example.pb.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/example.pb.h` & `tfrecord_lite-0.0.8/src/example.pb.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/feature.pb.cpp` & `tfrecord_lite-0.0.8/src/feature.pb.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/feature.pb.h` & `tfrecord_lite-0.0.8/src/feature.pb.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb.h` & `tfrecord_lite-0.0.8/src/pb.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_common.cpp` & `tfrecord_lite-0.0.8/src/pb_common.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_common.h` & `tfrecord_lite-0.0.8/src/pb_common.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_decode.cpp` & `tfrecord_lite-0.0.8/src/pb_decode.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_decode.h` & `tfrecord_lite-0.0.8/src/pb_decode.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_encode.cpp` & `tfrecord_lite-0.0.8/src/pb_encode.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/pb_encode.h` & `tfrecord_lite-0.0.8/src/pb_encode.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/tfrecord_lite.cpp` & `tfrecord_lite-0.0.8/src/tfrecord_lite.cpp`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/src/tfrecord_lite.h` & `tfrecord_lite-0.0.8/src/tfrecord_lite.h`

 * *Files identical despite different names*

### Comparing `tfrecord_lite-0.0.7/tfrecord_lite.cpp` & `tfrecord_lite-0.0.8/tfrecord_lite.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 3.0.0b2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/tfrecord_lite.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-Wall",
-            "-std=c++11"
+            "-std=c++11",
+            "-mmacosx-version-min=10.9"
+        ],
+        "extra_link_args": [
+            "-stdlib=libc++",
+            "-mmacosx-version-min=10.9"
         ],
         "include_dirs": [
             "src/"
         ],
         "language": "c++",
         "name": "tfrecord_lite",
         "sources": [
@@ -26,29 +31,43 @@
             "src/pb_encode.cpp"
         ]
     },
     "module_name": "tfrecord_lite"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_ABI "3_0_0b2"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000B2
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -59,30 +78,90 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -99,35 +178,107 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -142,54 +293,55 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -199,35 +351,68 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -245,78 +430,116 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
+        #else
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -332,99 +555,239 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -447,74 +810,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #else
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -524,68 +979,83 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
+#endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
-#endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -597,16 +1067,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -616,36 +1088,43 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE__tfrecord_lite
 #define __PYX_HAVE_API__tfrecord_lite
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <utility>
+
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
+    #include <type_traits>
+
+    namespace cython_std {
+    template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
+    template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
+    }
+
+    #endif
+    
 #include <set>
 #include <map>
 #include <string.h>
 #include <string>
 #include <vector>
 #include "tfrecord_lite.h"
 #ifdef _OPENMP
@@ -712,54 +1191,71 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -838,31 +1334,32 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "tfrecord_lite.pyx",
-  "stringsource",
+  "<stringsource>",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* #### Code section: numeric_typedefs ### */
+/* #### Code section: complex_type_declarations ### */
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator;
 
 /* "tfrecord_lite.pyx":51
  * 
  * 
@@ -883,89 +1380,161 @@
   PyObject *__pyx_v_names;
   PyObject *__pyx_t_0;
   PyObject *__pyx_t_1;
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3;
 };
 
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* MoveIfSupported.proto */
+#if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+  #include <utility>
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
+#else
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -986,158 +1555,217 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+#endif
+#endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* IterFinish.proto */
+static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
 
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
-/* IterFinish.proto */
-static CYTHON_INLINE int __Pyx_IterFinish(void);
+/* RaiseTooManyValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
+
+/* UnpackTupleError.proto */
+static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
+
+/* UnpackTuple2.proto */
+#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
+    (likely(is_tuple || PyTuple_Check(tuple)) ?\
+        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
+            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
+            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
+        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
+static int __Pyx_unpack_tuple2_generic(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
+
+/* dict_iter.proto */
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_is_dict);
+static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
+                                              PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
+
 /* PyObjectLookupSpecial.proto */
 #if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name) {
-    PyObject *res;
-    PyTypeObject *tp = Py_TYPE(obj);
-#if PY_MAJOR_VERSION < 3
-    if (unlikely(PyInstance_Check(obj)))
-        return __Pyx_PyObject_GetAttrStr(obj, attr_name);
-#endif
-    res = _PyType_Lookup(tp, attr_name);
-    if (likely(res)) {
-        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
-        if (!f) {
-            Py_INCREF(res);
-        } else {
-            res = f(res, obj, (PyObject *)tp);
-        }
-    } else {
-        PyErr_SetObject(PyExc_AttributeError, attr_name);
-    }
-    return res;
-}
+#define __Pyx_PyObject_LookupSpecialNoError(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 0)
+#define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
+static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
 #else
+#define __Pyx_PyObject_LookupSpecialNoError(o,n) __Pyx_PyObject_GetAttrStrNoError(o,n)
 #define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
 #endif
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
@@ -1160,25 +1788,14 @@
                                                      int is_list, int wraparound, int boundscheck);
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
@@ -1190,81 +1807,198 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
 /* SwapException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* IncludeStringH.proto */
-#include <string.h>
+/* pep479.proto */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen);
+
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
+
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
+#endif
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
+#endif
+
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+#else
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
+#endif
+
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* CppExceptionConversion.proto */
 #ifndef __Pyx_CppExn2PyErr
@@ -1304,74 +2038,92 @@
   catch (...)
   {
     PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
   }
 }
 #endif
 
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_Occurred(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
-/* FetchCommonType.proto */
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
-
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* CoroutineBase.proto */
-typedef PyObject *(*__pyx_coroutine_body_t)(PyObject *, PyThreadState *, PyObject *);
+struct __pyx_CoroutineObject;
+typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
 #if CYTHON_USE_EXC_INFO_STACK
 #define __Pyx_ExcInfoStruct  _PyErr_StackItem
 #else
 typedef struct {
     PyObject *exc_type;
     PyObject *exc_value;
     PyObject *exc_traceback;
 } __Pyx_ExcInfoStruct;
 #endif
-typedef struct {
+typedef struct __pyx_CoroutineObject {
     PyObject_HEAD
     __pyx_coroutine_body_t body;
     PyObject *closure;
     __Pyx_ExcInfoStruct gi_exc_state;
     PyObject *gi_weakreflist;
     PyObject *classobj;
     PyObject *yieldfrom;
     PyObject *gi_name;
     PyObject *gi_qualname;
     PyObject *gi_modulename;
     PyObject *gi_code;
+    PyObject *gi_frame;
     int resume_label;
     char is_running;
 } __pyx_CoroutineObject;
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
     PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
     PyObject *name, PyObject *qualname, PyObject *module_name);
 static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
@@ -1409,163 +2161,1133 @@
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
 
 /* PatchGeneratorABC.proto */
 static int __Pyx_patch_abc(void);
 
 /* Generator.proto */
 #define __Pyx_Generator_USED
-static PyTypeObject *__pyx_GeneratorType = 0;
-#define __Pyx_Generator_CheckExact(obj) (Py_TYPE(obj) == __pyx_GeneratorType)
+#define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
 #define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
     __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
 static PyObject *__Pyx_Generator_Next(PyObject *self);
-static int __pyx_Generator_init(void);
+static int __pyx_Generator_init(PyObject *module);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
 
-/* Module declarations from 'libcpp.utility' */
+/* Module declarations from "libcpp.utility" */
 
-/* Module declarations from 'libcpp.set' */
+/* Module declarations from "libcpp.set" */
 
-/* Module declarations from 'libcpp.map' */
+/* Module declarations from "libcpp.map" */
 
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libcpp.string' */
+/* Module declarations from "libcpp.string" */
 
-/* Module declarations from 'libcpp.vector' */
+/* Module declarations from "libcpp.vector" */
 
-/* Module declarations from 'tfrecord_lite' */
-static PyTypeObject *__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = 0;
+/* Module declarations from "tfrecord_lite" */
 static PyObject *__pyx_f_13tfrecord_lite_decode_example_internal(PyObject *, std::vector<std::string> ); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(const std::vector<std::string>  &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(std::vector<std::string>  const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static std::vector<std::string>  __pyx_convert_vector_from_py_std_3a__3a_string(PyObject *); /*proto*/
+/* #### Code section: typeinfo ### */
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "tfrecord_lite"
 extern int __pyx_module_is_main_tfrecord_lite;
 int __pyx_module_is_main_tfrecord_lite = 0;
 
-/* Implementation of 'tfrecord_lite' */
+/* Implementation of "tfrecord_lite" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_open;
+static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_range;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_Q[] = "Q";
+static const char __pyx_k__3[] = "*";
+static const char __pyx_k__9[] = "?";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_np[] = "_np";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_open[] = "open";
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_send[] = "send";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_names[] = "names";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_decode[] = "decode";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_header[] = "header";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "name";
 static const char __pyx_k_struct[] = "_struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_decoded[] = "decoded";
+static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float32[] = "float32";
 static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_struct_2[] = "struct";
+static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_frombuffer[] = "frombuffer";
 static const char __pyx_k_header_len[] = "header_len";
 static const char __pyx_k_header_str[] = "header_str";
+static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_event_bytes[] = "event_bytes";
 static const char __pyx_k_file_handle[] = "file_handle";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_tfrecord_lite[] = "tfrecord_lite";
 static const char __pyx_k_decode_example[] = "decode_example";
 static const char __pyx_k_crc_event_bytes[] = "crc_event_bytes";
 static const char __pyx_k_crc_header_bytes[] = "crc_header_bytes";
 static const char __pyx_k_tfrecord_lite_pyx[] = "tfrecord_lite.pyx";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_tf_record_iterator[] = "tf_record_iterator";
-static PyObject *__pyx_n_s_Q;
-static PyObject *__pyx_n_s_args;
-static PyObject *__pyx_n_s_buffer;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_close;
-static PyObject *__pyx_n_s_crc_event_bytes;
-static PyObject *__pyx_n_s_crc_header_bytes;
-static PyObject *__pyx_n_s_decode;
-static PyObject *__pyx_n_s_decode_example;
-static PyObject *__pyx_n_s_decoded;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_encode;
-static PyObject *__pyx_n_s_enter;
-static PyObject *__pyx_n_s_event_bytes;
-static PyObject *__pyx_n_s_exit;
-static PyObject *__pyx_n_s_file_handle;
-static PyObject *__pyx_n_s_filename;
-static PyObject *__pyx_n_s_float32;
-static PyObject *__pyx_n_s_frombuffer;
-static PyObject *__pyx_n_s_header;
-static PyObject *__pyx_n_s_header_len;
-static PyObject *__pyx_n_s_header_str;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_int64;
-static PyObject *__pyx_n_s_items;
-static PyObject *__pyx_n_s_key;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_n_s_names;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_n_s_open;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_s_rb;
-static PyObject *__pyx_n_s_read;
-static PyObject *__pyx_n_s_send;
-static PyObject *__pyx_n_s_struct;
-static PyObject *__pyx_n_s_struct_2;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_tf_record_iterator;
-static PyObject *__pyx_n_s_tfrecord_lite;
-static PyObject *__pyx_kp_s_tfrecord_lite_pyx;
-static PyObject *__pyx_n_s_throw;
-static PyObject *__pyx_n_s_unpack;
-static PyObject *__pyx_kp_s_utf_8;
-static PyObject *__pyx_n_s_value;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_13tfrecord_lite_decode_example(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_buffer, PyObject *__pyx_v_names); /* proto */
 static PyObject *__pyx_pf_13tfrecord_lite_2tf_record_iterator(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_names); /* proto */
 static PyObject *__pyx_tp_new_13tfrecord_lite___pyx_scope_struct__tf_record_iterator(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_4;
-static PyObject *__pyx_int_8;
-static PyObject *__pyx_codeobj_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_codeobj__4;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator;
+  #endif
+  PyTypeObject *__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator;
+  PyObject *__pyx_n_s_MemoryError;
+  PyObject *__pyx_n_s_Q;
+  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s__9;
+  PyObject *__pyx_n_s_args;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_buffer;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_close;
+  PyObject *__pyx_n_s_crc_event_bytes;
+  PyObject *__pyx_n_s_crc_header_bytes;
+  PyObject *__pyx_n_s_decode;
+  PyObject *__pyx_n_s_decode_example;
+  PyObject *__pyx_n_s_decoded;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_encode;
+  PyObject *__pyx_n_s_enter;
+  PyObject *__pyx_n_s_event_bytes;
+  PyObject *__pyx_n_s_exit;
+  PyObject *__pyx_n_s_file_handle;
+  PyObject *__pyx_n_s_filename;
+  PyObject *__pyx_n_s_float32;
+  PyObject *__pyx_n_s_frombuffer;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_header;
+  PyObject *__pyx_n_s_header_len;
+  PyObject *__pyx_n_s_header_str;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_int64;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_items;
+  PyObject *__pyx_n_s_key;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_name_2;
+  PyObject *__pyx_n_s_names;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_n_s_open;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_rb;
+  PyObject *__pyx_n_s_read;
+  PyObject *__pyx_n_s_send;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_struct;
+  PyObject *__pyx_n_s_struct_2;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_tf_record_iterator;
+  PyObject *__pyx_n_s_tfrecord_lite;
+  PyObject *__pyx_kp_s_tfrecord_lite_pyx;
+  PyObject *__pyx_n_s_throw;
+  PyObject *__pyx_n_s_unpack;
+  PyObject *__pyx_kp_s_utf_8;
+  PyObject *__pyx_n_s_value;
+  PyObject *__pyx_int_4;
+  PyObject *__pyx_int_8;
+  PyObject *__pyx_codeobj_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_codeobj__5;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator);
+  Py_CLEAR(clear_module_state->__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Q);
+  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s__9);
+  Py_CLEAR(clear_module_state->__pyx_n_s_args);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_buffer);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_crc_event_bytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_crc_header_bytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decode_example);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decoded);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_encode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_enter);
+  Py_CLEAR(clear_module_state->__pyx_n_s_event_bytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_exit);
+  Py_CLEAR(clear_module_state->__pyx_n_s_file_handle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_filename);
+  Py_CLEAR(clear_module_state->__pyx_n_s_float32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_frombuffer);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_header);
+  Py_CLEAR(clear_module_state->__pyx_n_s_header_len);
+  Py_CLEAR(clear_module_state->__pyx_n_s_header_str);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int64);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_items);
+  Py_CLEAR(clear_module_state->__pyx_n_s_key);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_names);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_n_s_open);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rb);
+  Py_CLEAR(clear_module_state->__pyx_n_s_read);
+  Py_CLEAR(clear_module_state->__pyx_n_s_send);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_struct);
+  Py_CLEAR(clear_module_state->__pyx_n_s_struct_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tf_record_iterator);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tfrecord_lite);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_tfrecord_lite_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_throw);
+  Py_CLEAR(clear_module_state->__pyx_n_s_unpack);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value);
+  Py_CLEAR(clear_module_state->__pyx_int_4);
+  Py_CLEAR(clear_module_state->__pyx_int_8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator);
+  Py_VISIT(traverse_module_state->__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Q);
+  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s__9);
+  Py_VISIT(traverse_module_state->__pyx_n_s_args);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_buffer);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_crc_event_bytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_crc_header_bytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decode_example);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decoded);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_encode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_enter);
+  Py_VISIT(traverse_module_state->__pyx_n_s_event_bytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_exit);
+  Py_VISIT(traverse_module_state->__pyx_n_s_file_handle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_filename);
+  Py_VISIT(traverse_module_state->__pyx_n_s_float32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_frombuffer);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_header);
+  Py_VISIT(traverse_module_state->__pyx_n_s_header_len);
+  Py_VISIT(traverse_module_state->__pyx_n_s_header_str);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int64);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_items);
+  Py_VISIT(traverse_module_state->__pyx_n_s_key);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_names);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_n_s_open);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rb);
+  Py_VISIT(traverse_module_state->__pyx_n_s_read);
+  Py_VISIT(traverse_module_state->__pyx_n_s_send);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_struct);
+  Py_VISIT(traverse_module_state->__pyx_n_s_struct_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tf_record_iterator);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tfrecord_lite);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_tfrecord_lite_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_throw);
+  Py_VISIT(traverse_module_state->__pyx_n_s_unpack);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value);
+  Py_VISIT(traverse_module_state->__pyx_int_4);
+  Py_VISIT(traverse_module_state->__pyx_int_8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator __pyx_mstate_global->__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator
+#endif
+#define __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator __pyx_mstate_global->__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator
+#define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
+#define __pyx_n_s_Q __pyx_mstate_global->__pyx_n_s_Q
+#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s__9 __pyx_mstate_global->__pyx_n_s__9
+#define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_buffer __pyx_mstate_global->__pyx_n_s_buffer
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
+#define __pyx_n_s_crc_event_bytes __pyx_mstate_global->__pyx_n_s_crc_event_bytes
+#define __pyx_n_s_crc_header_bytes __pyx_mstate_global->__pyx_n_s_crc_header_bytes
+#define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
+#define __pyx_n_s_decode_example __pyx_mstate_global->__pyx_n_s_decode_example
+#define __pyx_n_s_decoded __pyx_mstate_global->__pyx_n_s_decoded
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
+#define __pyx_n_s_enter __pyx_mstate_global->__pyx_n_s_enter
+#define __pyx_n_s_event_bytes __pyx_mstate_global->__pyx_n_s_event_bytes
+#define __pyx_n_s_exit __pyx_mstate_global->__pyx_n_s_exit
+#define __pyx_n_s_file_handle __pyx_mstate_global->__pyx_n_s_file_handle
+#define __pyx_n_s_filename __pyx_mstate_global->__pyx_n_s_filename
+#define __pyx_n_s_float32 __pyx_mstate_global->__pyx_n_s_float32
+#define __pyx_n_s_frombuffer __pyx_mstate_global->__pyx_n_s_frombuffer
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_header __pyx_mstate_global->__pyx_n_s_header
+#define __pyx_n_s_header_len __pyx_mstate_global->__pyx_n_s_header_len
+#define __pyx_n_s_header_str __pyx_mstate_global->__pyx_n_s_header_str
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_int64 __pyx_mstate_global->__pyx_n_s_int64
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
+#define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
+#define __pyx_n_s_names __pyx_mstate_global->__pyx_n_s_names
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_n_s_open __pyx_mstate_global->__pyx_n_s_open
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_rb __pyx_mstate_global->__pyx_n_s_rb
+#define __pyx_n_s_read __pyx_mstate_global->__pyx_n_s_read
+#define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_struct __pyx_mstate_global->__pyx_n_s_struct
+#define __pyx_n_s_struct_2 __pyx_mstate_global->__pyx_n_s_struct_2
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_tf_record_iterator __pyx_mstate_global->__pyx_n_s_tf_record_iterator
+#define __pyx_n_s_tfrecord_lite __pyx_mstate_global->__pyx_n_s_tfrecord_lite
+#define __pyx_kp_s_tfrecord_lite_pyx __pyx_mstate_global->__pyx_kp_s_tfrecord_lite_pyx
+#define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
+#define __pyx_n_s_unpack __pyx_mstate_global->__pyx_n_s_unpack
+#define __pyx_kp_s_utf_8 __pyx_mstate_global->__pyx_kp_s_utf_8
+#define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
+#define __pyx_int_4 __pyx_mstate_global->__pyx_int_4
+#define __pyx_int_8 __pyx_mstate_global->__pyx_int_8
+#define __pyx_codeobj_ __pyx_mstate_global->__pyx_codeobj_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
+/* #### Code section: module_code ### */
+
+/* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":32
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":38
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":44
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":50
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":56
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(std::vector<std::string>  const &__pyx_v_v) {
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  size_t __pyx_t_3;
+  size_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_string", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ * 
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(<Py_ssize_t> v.size())
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ * 
+ */
+  }
+
+  /* "vector.to_py":70
+ *         raise MemoryError()
+ * 
+ *     o = PyList_New(<Py_ssize_t> v.size())             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(((Py_ssize_t)__pyx_v_v.size())); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":75
+ *     cdef object item
+ * 
+ *     for i in range(v.size()):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v.size();
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":76
+ * 
+ *     for i in range(v.size()):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":77
+ *     for i in range(v.size()):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":78
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":80
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
+  Py_ssize_t __pyx_v_length;
+  char const *__pyx_v_data;
+  std::string __pyx_r;
+  __Pyx_RefNannyDeclarations
+  char const *__pyx_t_1;
+  std::string __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
+
+  /* "string.from_py":14
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)
+ */
+  __pyx_v_length = 0;
+
+  /* "string.from_py":15
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
+ *     return string(data, length)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_v_data = __pyx_t_1;
+
+  /* "string.from_py":16
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  try {
+    __pyx_t_2 = std::string(__pyx_v_data, __pyx_v_length);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 16, __pyx_L1_error)
+  }
+  __pyx_r = __pyx_t_2;
+  goto __pyx_L0;
+
+  /* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<std::string>  __pyx_convert_vector_from_py_std_3a__3a_string(PyObject *__pyx_v_o) {
+  std::vector<std::string>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<std::string>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  std::string __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_string", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_convert_string_from_py_std__in_string(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((std::string)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 
 /* "tfrecord_lite.pyx":23
  * 
  * 
  * cdef decode_example_internal(bytes buffer, vector[string] names):             # <<<<<<<<<<<<<<
  *     cdef decoder_options options
  *     options.names = set[string]()
@@ -1579,21 +3301,24 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   std::set<std::string>  __pyx_t_1;
   std::vector<std::string> ::iterator __pyx_t_2;
   std::string __pyx_t_3;
   unsigned char const *__pyx_t_4;
   Py_ssize_t __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  std::vector<std::string>  *__pyx_t_7;
+  struct decoder_output __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_example_internal", 0);
 
   /* "tfrecord_lite.pyx":25
  * cdef decode_example_internal(bytes buffer, vector[string] names):
  *     cdef decoder_options options
  *     options.names = set[string]()             # <<<<<<<<<<<<<<
  *     for name in names:
@@ -1601,29 +3326,29 @@
  */
   try {
     __pyx_t_1 = std::set<std::string> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 25, __pyx_L1_error)
   }
-  __pyx_v_options.names = __pyx_t_1;
+  __pyx_v_options.names = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1);
 
   /* "tfrecord_lite.pyx":26
  *     cdef decoder_options options
  *     options.names = set[string]()
  *     for name in names:             # <<<<<<<<<<<<<<
  *         options.names.insert(name)
  * 
  */
   __pyx_t_2 = __pyx_v_names.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_names.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
-    __pyx_v_name = __pyx_t_3;
+    __pyx_v_name = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
     /* "tfrecord_lite.pyx":27
  *     options.names = set[string]()
  *     for name in names:
  *         options.names.insert(name)             # <<<<<<<<<<<<<<
  * 
  *     cdef decoder_output decoded = decode_tfrecord_example(buffer, len(buffer), options)
@@ -1657,90 +3382,95 @@
   }
   __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_buffer); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
   if (unlikely(__pyx_v_buffer == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 29, __pyx_L1_error)
   }
   __pyx_t_5 = PyBytes_GET_SIZE(__pyx_v_buffer); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_v_decoded = decode_tfrecord_example(__pyx_t_4, __pyx_t_5, __pyx_v_options);
+  try {
+    __pyx_t_6 = decode_tfrecord_example(__pyx_t_4, __pyx_t_5, __pyx_v_options);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 29, __pyx_L1_error)
+  }
+  __pyx_v_decoded = __pyx_t_6;
 
   /* "tfrecord_lite.pyx":30
  * 
  *     cdef decoder_output decoded = decode_tfrecord_example(buffer, len(buffer), options)
  *     result = {}             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_v_result = ((PyObject*)__pyx_t_6);
-  __pyx_t_6 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_v_result = ((PyObject*)__pyx_t_7);
+  __pyx_t_7 = 0;
 
   /* "tfrecord_lite.pyx":33
  * 
  * 
  *     for name in decoded.names:             # <<<<<<<<<<<<<<
  *         if decoded.int64_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
  */
-  __pyx_t_7 = &__pyx_v_decoded.names;
-  __pyx_t_2 = __pyx_t_7->begin();
+  __pyx_t_2 = __pyx_v_decoded.names.begin();
   for (;;) {
-    if (!(__pyx_t_2 != __pyx_t_7->end())) break;
+    if (!(__pyx_t_2 != __pyx_v_decoded.names.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
-    __pyx_v_name = __pyx_t_3;
+    __pyx_v_name = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
     /* "tfrecord_lite.pyx":34
  * 
  *     for name in decoded.names:
  *         if decoded.int64_features.count(name) > 0:             # <<<<<<<<<<<<<<
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
  *         elif decoded.float_features.count(name) > 0:
  */
-    __pyx_t_8 = ((__pyx_v_decoded.int64_features.count(__pyx_v_name) > 0) != 0);
+    __pyx_t_8 = (__pyx_v_decoded.int64_features.count(__pyx_v_name) > 0);
     if (__pyx_t_8) {
 
       /* "tfrecord_lite.pyx":35
  *     for name in decoded.names:
  *         if decoded.int64_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)             # <<<<<<<<<<<<<<
  *         elif decoded.float_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_decoded.int64_features[__pyx_v_name])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_decoded.int64_features[__pyx_v_name])); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_GIVEREF(__pyx_t_6);
-      PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7);
+      __pyx_t_7 = 0;
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_int64); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 35, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_6, __pyx_t_12) < 0)) __PYX_ERR(0, 35, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_7, __pyx_t_12) < 0))) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
       /* "tfrecord_lite.pyx":34
  * 
  *     for name in decoded.names:
  *         if decoded.int64_features.count(name) > 0:             # <<<<<<<<<<<<<<
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
@@ -1752,28 +3482,28 @@
     /* "tfrecord_lite.pyx":36
  *         if decoded.int64_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
  *         elif decoded.float_features.count(name) > 0:             # <<<<<<<<<<<<<<
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)
  *         elif decoded.bytes_features.count(name) > 0:
  */
-    __pyx_t_8 = ((__pyx_v_decoded.float_features.count(__pyx_v_name) > 0) != 0);
+    __pyx_t_8 = (__pyx_v_decoded.float_features.count(__pyx_v_name) > 0);
     if (__pyx_t_8) {
 
       /* "tfrecord_lite.pyx":37
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
  *         elif decoded.float_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)             # <<<<<<<<<<<<<<
  *         elif decoded.bytes_features.count(name) > 0:
  *             result[name] = decoded.bytes_features[name]
  */
       __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_decoded.float_features[__pyx_v_name])); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_12);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_12);
@@ -1783,22 +3513,22 @@
       __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0))) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
       /* "tfrecord_lite.pyx":36
  *         if decoded.int64_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.int64_features[name], dtype=_np.int64)
  *         elif decoded.float_features.count(name) > 0:             # <<<<<<<<<<<<<<
@@ -1811,29 +3541,29 @@
     /* "tfrecord_lite.pyx":38
  *         elif decoded.float_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)
  *         elif decoded.bytes_features.count(name) > 0:             # <<<<<<<<<<<<<<
  *             result[name] = decoded.bytes_features[name]
  *         else:
  */
-    __pyx_t_8 = ((__pyx_v_decoded.bytes_features.count(__pyx_v_name) > 0) != 0);
+    __pyx_t_8 = (__pyx_v_decoded.bytes_features.count(__pyx_v_name) > 0);
     if (__pyx_t_8) {
 
       /* "tfrecord_lite.pyx":39
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)
  *         elif decoded.bytes_features.count(name) > 0:
  *             result[name] = decoded.bytes_features[name]             # <<<<<<<<<<<<<<
  *         else:
  *             result[name] = []
  */
       __pyx_t_11 = __pyx_convert_vector_to_py_std_3a__3a_string((__pyx_v_decoded.bytes_features[__pyx_v_name])); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 39, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_12 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 39, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
       /* "tfrecord_lite.pyx":38
  *         elif decoded.float_features.count(name) > 0:
  *             result[name] = _np.frombuffer(decoded.float_features[name], dtype=_np.float32)
  *         elif decoded.bytes_features.count(name) > 0:             # <<<<<<<<<<<<<<
@@ -1851,15 +3581,15 @@
  *     return result
  */
     /*else*/ {
       __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 41, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_12 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 41, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0)) __PYX_ERR(0, 41, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_12, __pyx_t_11) < 0))) __PYX_ERR(0, 41, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __pyx_L7:;
 
     /* "tfrecord_lite.pyx":33
  * 
@@ -1888,15 +3618,15 @@
  * cdef decode_example_internal(bytes buffer, vector[string] names):             # <<<<<<<<<<<<<<
  *     cdef decoder_options options
  *     options.names = set[string]()
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("tfrecord_lite.decode_example_internal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
@@ -1911,67 +3641,88 @@
  * 
  * def decode_example(bytes buffer, names=()):             # <<<<<<<<<<<<<<
  *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])
  *     return {key.decode('utf-8'): value for key, value in decoded.items()}
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13tfrecord_lite_1decode_example(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13tfrecord_lite_1decode_example = {"decode_example", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13tfrecord_lite_1decode_example, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13tfrecord_lite_1decode_example(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13tfrecord_lite_1decode_example(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_13tfrecord_lite_1decode_example = {"decode_example", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_13tfrecord_lite_1decode_example, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13tfrecord_lite_1decode_example(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_buffer = 0;
   PyObject *__pyx_v_names = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("decode_example (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_buffer,&__pyx_n_s_names,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_buffer,&__pyx_n_s_names,0};
     PyObject* values[2] = {0,0};
-    values[1] = ((PyObject *)__pyx_empty_tuple);
-    if (unlikely(__pyx_kwds)) {
+    values[1] = ((PyObject *)((PyObject*)__pyx_empty_tuple));
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_buffer)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_buffer)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_names);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_names);
           if (value) { values[1] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "decode_example") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_example") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_buffer = ((PyObject*)values[0]);
     __pyx_v_names = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_example", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decode_example", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tfrecord_lite.decode_example", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_buffer), (&PyBytes_Type), 1, "buffer", 1))) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_r = __pyx_pf_13tfrecord_lite_decode_example(__pyx_self, __pyx_v_buffer, __pyx_v_names);
@@ -1983,256 +3734,191 @@
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_13tfrecord_lite_decode_example(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_buffer, PyObject *__pyx_v_names) {
   PyObject *__pyx_v_decoded = NULL;
-  PyObject *__pyx_v_name = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_key = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_value = NULL;
+  PyObject *__pyx_7genexpr__pyx_v_name = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_key = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_value = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  std::vector<std::string>  __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *(*__pyx_t_10)(PyObject *);
+  int __pyx_t_8;
+  std::vector<std::string>  __pyx_t_9;
+  Py_ssize_t __pyx_t_10;
+  int __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_example", 0);
 
   /* "tfrecord_lite.pyx":47
  * 
  * def decode_example(bytes buffer, names=()):
  *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])             # <<<<<<<<<<<<<<
  *     return {key.decode('utf-8'): value for key, value in decoded.items()}
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (likely(PyList_CheckExact(__pyx_v_names)) || PyTuple_CheckExact(__pyx_v_names)) {
-    __pyx_t_2 = __pyx_v_names; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
-    __pyx_t_4 = NULL;
-  } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_names); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_4)) {
-      if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 47, __pyx_L1_error)
-        #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        #endif
-      } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 47, __pyx_L1_error)
-        #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        #endif
-      }
-    } else {
-      __pyx_t_5 = __pyx_t_4(__pyx_t_2);
-      if (unlikely(!__pyx_t_5)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_5);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_5);
-    __pyx_t_5 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_kp_s_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_s_utf_8);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 47, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_f_13tfrecord_lite_decode_example_internal(__pyx_v_buffer, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_decoded = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "tfrecord_lite.pyx":48
- * def decode_example(bytes buffer, names=()):
- *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])
- *     return {key.decode('utf-8'): value for key, value in decoded.items()}             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L7_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_decoded, __pyx_n_s_items); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L7_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L7_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-      __pyx_t_5 = __pyx_t_2; __Pyx_INCREF(__pyx_t_5); __pyx_t_3 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_names)) || PyTuple_CheckExact(__pyx_v_names)) {
+      __pyx_t_2 = __pyx_v_names; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L7_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L7_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_names); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L5_error)
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_5))) {
-          if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        if (likely(PyList_CheckExact(__pyx_t_2))) {
+          if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L7_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 47, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
-          if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+          if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L7_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 47, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
-        __pyx_t_2 = __pyx_t_4(__pyx_t_5);
-        if (unlikely(!__pyx_t_2)) {
+        __pyx_t_5 = __pyx_t_4(__pyx_t_2);
+        if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 48, __pyx_L7_error)
+            else __PYX_ERR(0, 47, __pyx_L5_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_5);
       }
-      if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-        PyObject* sequence = __pyx_t_2;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 48, __pyx_L7_error)
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
+      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_name, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      __pyx_t_8 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_8 = 1;
         }
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
-        #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 48, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        #endif
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      } else {
-        Py_ssize_t index = -1;
-        __pyx_t_9 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 48, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_10 = Py_TYPE(__pyx_t_9)->tp_iternext;
-        index = 0; __pyx_t_6 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_6)) goto __pyx_L10_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_6);
-        index = 1; __pyx_t_7 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_7)) goto __pyx_L10_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 48, __pyx_L7_error)
-        __pyx_t_10 = NULL;
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        goto __pyx_L11_unpacking_done;
-        __pyx_L10_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_10 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 48, __pyx_L7_error)
-        __pyx_L11_unpacking_done:;
       }
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_key, __pyx_t_6);
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_s_utf_8};
+        __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L5_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 47, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_name); __pyx_7genexpr__pyx_v_name = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_name); __pyx_7genexpr__pyx_v_name = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_t_9 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __pyx_f_13tfrecord_lite_decode_example_internal(__pyx_v_buffer, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_decoded = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "tfrecord_lite.pyx":48
+ * def decode_example(bytes buffer, names=()):
+ *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])
+ *     return {key.decode('utf-8'): value for key, value in decoded.items()}             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  { /* enter inner scope */
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L11_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = 0;
+    if (unlikely(__pyx_v_decoded == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+      __PYX_ERR(0, 48, __pyx_L11_error)
+    }
+    __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_decoded, 0, __pyx_n_s_items, (&__pyx_t_10), (&__pyx_t_8)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L11_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_5;
+    __pyx_t_5 = 0;
+    while (1) {
+      __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_10, &__pyx_t_3, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_8);
+      if (unlikely(__pyx_t_11 == 0)) break;
+      if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 48, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_key, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_value, __pyx_t_6);
       __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_value, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_key, __pyx_n_s_decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 48, __pyx_L7_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-        if (likely(__pyx_t_6)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-          __Pyx_INCREF(__pyx_t_6);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_key, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_7 = NULL;
+      __pyx_t_11 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_7, function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_11 = 1;
         }
       }
-      __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_kp_s_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_utf_8);
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L7_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_2, (PyObject*)__pyx_7genexpr__pyx_v_value))) __PYX_ERR(0, 48, __pyx_L7_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_s_utf_8};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L11_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_6, (PyObject*)__pyx_8genexpr1__pyx_v_value))) __PYX_ERR(0, 48, __pyx_L11_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key); __pyx_7genexpr__pyx_v_key = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_value); __pyx_7genexpr__pyx_v_value = 0;
-    goto __pyx_L12_exit_scope;
-    __pyx_L7_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key); __pyx_7genexpr__pyx_v_key = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_value); __pyx_7genexpr__pyx_v_value = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key); __pyx_8genexpr1__pyx_v_key = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_value); __pyx_8genexpr1__pyx_v_value = 0;
+    goto __pyx_L14_exit_scope;
+    __pyx_L11_error:;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key); __pyx_8genexpr1__pyx_v_key = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_value); __pyx_8genexpr1__pyx_v_value = 0;
     goto __pyx_L1_error;
-    __pyx_L12_exit_scope:;
+    __pyx_L14_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "tfrecord_lite.pyx":46
  * 
@@ -2245,22 +3931,21 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("tfrecord_lite.decode_example", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_decoded);
-  __Pyx_XDECREF(__pyx_v_name);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_value);
+  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_name);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_13tfrecord_lite_4generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "tfrecord_lite.pyx":51
@@ -2268,68 +3953,89 @@
  * 
  * def tf_record_iterator(filename, names=()):             # <<<<<<<<<<<<<<
  *     """
  *     Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13tfrecord_lite_3tf_record_iterator(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_13tfrecord_lite_2tf_record_iterator[] = "\n    Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.\n\n    :param filename: path to the file to read records from.\n    :param names: feature names of the record to include; reads all by default\n    :return: iterator over the decoded TFrecords\n    ";
-static PyMethodDef __pyx_mdef_13tfrecord_lite_3tf_record_iterator = {"tf_record_iterator", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13tfrecord_lite_3tf_record_iterator, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13tfrecord_lite_2tf_record_iterator};
-static PyObject *__pyx_pw_13tfrecord_lite_3tf_record_iterator(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13tfrecord_lite_3tf_record_iterator(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_13tfrecord_lite_2tf_record_iterator, "\n    Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.\n\n    :param filename: path to the file to read records from.\n    :param names: feature names of the record to include; reads all by default\n    :return: iterator over the decoded TFrecords\n    ");
+static PyMethodDef __pyx_mdef_13tfrecord_lite_3tf_record_iterator = {"tf_record_iterator", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_13tfrecord_lite_3tf_record_iterator, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_13tfrecord_lite_2tf_record_iterator};
+static PyObject *__pyx_pw_13tfrecord_lite_3tf_record_iterator(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_names = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("tf_record_iterator (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filename,&__pyx_n_s_names,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filename,&__pyx_n_s_names,0};
     PyObject* values[2] = {0,0};
-    values[1] = ((PyObject *)__pyx_empty_tuple);
-    if (unlikely(__pyx_kwds)) {
+    values[1] = ((PyObject *)((PyObject*)__pyx_empty_tuple));
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_names);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_names);
           if (value) { values[1] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "tf_record_iterator") < 0)) __PYX_ERR(0, 51, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "tf_record_iterator") < 0)) __PYX_ERR(0, 51, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_filename = values[0];
     __pyx_v_names = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("tf_record_iterator", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 51, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("tf_record_iterator", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 51, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tfrecord_lite.tf_record_iterator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13tfrecord_lite_2tf_record_iterator(__pyx_self, __pyx_v_filename, __pyx_v_names);
 
@@ -2338,22 +4044,25 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_13tfrecord_lite_2tf_record_iterator(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_names) {
   struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("tf_record_iterator", 0);
   __pyx_cur_scope = (struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *)__pyx_tp_new_13tfrecord_lite___pyx_scope_struct__tf_record_iterator(__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 51, __pyx_L1_error)
   } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_filename = __pyx_v_filename;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_filename);
   __pyx_cur_scope->__pyx_v_names = __pyx_v_names;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_names);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_names);
@@ -2364,42 +4073,44 @@
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("tfrecord_lite.tf_record_iterator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_gb_13tfrecord_lite_4generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *__pyx_cur_scope = ((struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  Py_ssize_t __pyx_t_9;
-  int __pyx_t_10;
+  PyObject *__pyx_t_9 = NULL;
+  Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
-  int __pyx_t_14;
+  int __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
-  PyObject *__pyx_t_18 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("tf_record_iterator", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L19_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
@@ -2428,37 +4139,42 @@
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 59, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L4_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    }
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
-        __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
-        __Pyx_XGOTREF(__pyx_t_6);
+        __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
+        __Pyx_XGOTREF(__pyx_t_9);
         /*try:*/ {
           __Pyx_GIVEREF(__pyx_t_4);
           __pyx_cur_scope->__pyx_v_file_handle = __pyx_t_4;
           __pyx_t_4 = 0;
 
           /* "tfrecord_lite.pyx":60
  *     """
@@ -2475,43 +4191,48 @@
  *             header_str = file_handle.read(8)             # <<<<<<<<<<<<<<
  *             if len(header_str) != 8:
  *                 # Hit EOF so exit
  */
             __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_file_handle, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_2);
             __pyx_t_1 = NULL;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
               __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
               if (likely(__pyx_t_1)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
                 __Pyx_INCREF(__pyx_t_1);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_2, function);
+                __pyx_t_6 = 1;
               }
             }
-            __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_int_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_int_8);
-            __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L8_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_int_8};
+              __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+              if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L8_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            }
             __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_header_str);
             __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_header_str, __pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_4);
             __pyx_t_4 = 0;
 
             /* "tfrecord_lite.pyx":63
  *             # Read the header
  *             header_str = file_handle.read(8)
  *             if len(header_str) != 8:             # <<<<<<<<<<<<<<
  *                 # Hit EOF so exit
  *                 return
  */
-            __pyx_t_9 = PyObject_Length(__pyx_cur_scope->__pyx_v_header_str); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L8_error)
-            __pyx_t_10 = ((__pyx_t_9 != 8) != 0);
-            if (__pyx_t_10) {
+            __pyx_t_10 = PyObject_Length(__pyx_cur_scope->__pyx_v_header_str); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L8_error)
+            __pyx_t_11 = (__pyx_t_10 != 8);
+            if (__pyx_t_11) {
 
               /* "tfrecord_lite.pyx":65
  *             if len(header_str) != 8:
  *                 # Hit EOF so exit
  *                 return             # <<<<<<<<<<<<<<
  *             header = _struct.unpack("Q", header_str)
  * 
@@ -2538,87 +4259,67 @@
  */
             __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_struct); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_2);
             __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_unpack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __pyx_t_2 = NULL;
-            __pyx_t_11 = 0;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
               __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
               if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
                 __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_1, function);
-                __pyx_t_11 = 1;
+                __pyx_t_6 = 1;
               }
             }
-            #if CYTHON_FAST_PYCALL
-            if (PyFunction_Check(__pyx_t_1)) {
-              PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_s_Q, __pyx_cur_scope->__pyx_v_header_str};
-              __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L8_error)
-              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __Pyx_GOTREF(__pyx_t_4);
-            } else
-            #endif
-            #if CYTHON_FAST_PYCCALL
-            if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-              PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_s_Q, __pyx_cur_scope->__pyx_v_header_str};
-              __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L8_error)
-              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __Pyx_GOTREF(__pyx_t_4);
-            } else
-            #endif
             {
-              __pyx_t_5 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L8_error)
-              __Pyx_GOTREF(__pyx_t_5);
-              if (__pyx_t_2) {
-                __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
-              }
-              __Pyx_INCREF(__pyx_n_s_Q);
-              __Pyx_GIVEREF(__pyx_n_s_Q);
-              PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_11, __pyx_n_s_Q);
-              __Pyx_INCREF(__pyx_cur_scope->__pyx_v_header_str);
-              __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_header_str);
-              PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_11, __pyx_cur_scope->__pyx_v_header_str);
-              __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L8_error)
+              PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_n_s_Q, __pyx_cur_scope->__pyx_v_header_str};
+              __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_4);
-              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+              __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             }
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_header);
             __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_header, __pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_4);
             __pyx_t_4 = 0;
 
             /* "tfrecord_lite.pyx":69
  * 
  *             # Read the crc32, which is 4 bytes, and disregard
  *             crc_header_bytes = file_handle.read(4)             # <<<<<<<<<<<<<<
  * 
  *             # The length of the header tells us how many bytes the Event
  */
             __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_file_handle, __pyx_n_s_read); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_5 = NULL;
+            __pyx_t_2 = NULL;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
-              if (likely(__pyx_t_5)) {
+              __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+              if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                __Pyx_INCREF(__pyx_t_5);
+                __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_1, function);
+                __pyx_t_6 = 1;
               }
             }
-            __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_int_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_int_4);
-            __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L8_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_int_4};
+              __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L8_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+            }
             __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_crc_header_bytes);
             __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_crc_header_bytes, __pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_4);
             __pyx_t_4 = 0;
 
             /* "tfrecord_lite.pyx":73
  *             # The length of the header tells us how many bytes the Event
@@ -2642,274 +4343,257 @@
  *             header_len = int(header[0])
  *             event_bytes = file_handle.read(header_len)             # <<<<<<<<<<<<<<
  * 
  *             # The next 4 bytes contain the crc32 of the Event string,
  */
             __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_file_handle, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 74, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_5 = NULL;
+            __pyx_t_2 = NULL;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-              if (likely(__pyx_t_5)) {
+              __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+              if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-                __Pyx_INCREF(__pyx_t_5);
+                __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_4, function);
+                __pyx_t_6 = 1;
               }
             }
-            __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_cur_scope->__pyx_v_header_len) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_cur_scope->__pyx_v_header_len);
-            __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L8_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_header_len};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L8_error)
+              __Pyx_GOTREF(__pyx_t_1);
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            }
             __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_event_bytes);
             __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_event_bytes, __pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_1);
             __pyx_t_1 = 0;
 
             /* "tfrecord_lite.pyx":79
  *             # which we check for integrity. Sometimes, the last Event
  *             # has no crc32, in which case we skip.
  *             crc_event_bytes = file_handle.read(4)             # <<<<<<<<<<<<<<
  * 
  *             # Set the current event to be read later by record() call
  */
             __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_file_handle, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_5 = NULL;
+            __pyx_t_2 = NULL;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-              if (likely(__pyx_t_5)) {
+              __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+              if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-                __Pyx_INCREF(__pyx_t_5);
+                __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_4, function);
+                __pyx_t_6 = 1;
               }
             }
-            __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_int_4) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_int_4);
-            __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L8_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_int_4};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L8_error)
+              __Pyx_GOTREF(__pyx_t_1);
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            }
             __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_crc_event_bytes);
             __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_crc_event_bytes, __pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_1);
             __pyx_t_1 = 0;
 
             /* "tfrecord_lite.pyx":82
  * 
  *             # Set the current event to be read later by record() call
  *             yield decode_example(event_bytes, names or [])             # <<<<<<<<<<<<<<
  */
             __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_example); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_names); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 82, __pyx_L8_error)
-            if (!__pyx_t_10) {
+            __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_names); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 82, __pyx_L8_error)
+            if (!__pyx_t_11) {
             } else {
               __Pyx_INCREF(__pyx_cur_scope->__pyx_v_names);
-              __pyx_t_5 = __pyx_cur_scope->__pyx_v_names;
+              __pyx_t_2 = __pyx_cur_scope->__pyx_v_names;
               goto __pyx_L17_bool_binop_done;
             }
-            __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L8_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_2);
-            __pyx_t_5 = __pyx_t_2;
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L8_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_5);
+            __pyx_t_2 = __pyx_t_5;
+            __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             __pyx_L17_bool_binop_done:;
-            __pyx_t_2 = NULL;
-            __pyx_t_11 = 0;
+            __pyx_t_5 = NULL;
+            __pyx_t_6 = 0;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-              __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-              if (likely(__pyx_t_2)) {
+              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+              if (likely(__pyx_t_5)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-                __Pyx_INCREF(__pyx_t_2);
+                __Pyx_INCREF(__pyx_t_5);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_4, function);
-                __pyx_t_11 = 1;
+                __pyx_t_6 = 1;
               }
             }
-            #if CYTHON_FAST_PYCALL
-            if (PyFunction_Check(__pyx_t_4)) {
-              PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_event_bytes, __pyx_t_5};
-              __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L8_error)
-              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-            } else
-            #endif
-            #if CYTHON_FAST_PYCCALL
-            if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-              PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_event_bytes, __pyx_t_5};
-              __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L8_error)
-              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-            } else
-            #endif
             {
-              __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 82, __pyx_L8_error)
-              __Pyx_GOTREF(__pyx_t_12);
-              if (__pyx_t_2) {
-                __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_2); __pyx_t_2 = NULL;
-              }
-              __Pyx_INCREF(__pyx_cur_scope->__pyx_v_event_bytes);
-              __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_event_bytes);
-              PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_cur_scope->__pyx_v_event_bytes);
-              __Pyx_GIVEREF(__pyx_t_5);
-              PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_5);
-              __pyx_t_5 = 0;
-              __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L8_error)
+              PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_event_bytes, __pyx_t_2};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
+              __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             }
-            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __pyx_r = __pyx_t_1;
             __pyx_t_1 = 0;
             __Pyx_XGIVEREF(__pyx_t_3);
             __pyx_cur_scope->__pyx_t_0 = __pyx_t_3;
-            __Pyx_XGIVEREF(__pyx_t_6);
-            __pyx_cur_scope->__pyx_t_1 = __pyx_t_6;
             __Pyx_XGIVEREF(__pyx_t_7);
-            __pyx_cur_scope->__pyx_t_2 = __pyx_t_7;
+            __pyx_cur_scope->__pyx_t_1 = __pyx_t_7;
             __Pyx_XGIVEREF(__pyx_t_8);
-            __pyx_cur_scope->__pyx_t_3 = __pyx_t_8;
+            __pyx_cur_scope->__pyx_t_2 = __pyx_t_8;
+            __Pyx_XGIVEREF(__pyx_t_9);
+            __pyx_cur_scope->__pyx_t_3 = __pyx_t_9;
             __Pyx_XGIVEREF(__pyx_r);
             __Pyx_RefNannyFinishContext();
             __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
             /* return from generator, yielding value */
             __pyx_generator->resume_label = 1;
             return __pyx_r;
             __pyx_L19_resume_from_yield:;
             __pyx_t_3 = __pyx_cur_scope->__pyx_t_0;
             __pyx_cur_scope->__pyx_t_0 = 0;
             __Pyx_XGOTREF(__pyx_t_3);
-            __pyx_t_6 = __pyx_cur_scope->__pyx_t_1;
+            __pyx_t_7 = __pyx_cur_scope->__pyx_t_1;
             __pyx_cur_scope->__pyx_t_1 = 0;
-            __Pyx_XGOTREF(__pyx_t_6);
-            __pyx_t_7 = __pyx_cur_scope->__pyx_t_2;
-            __pyx_cur_scope->__pyx_t_2 = 0;
             __Pyx_XGOTREF(__pyx_t_7);
-            __pyx_t_8 = __pyx_cur_scope->__pyx_t_3;
-            __pyx_cur_scope->__pyx_t_3 = 0;
+            __pyx_t_8 = __pyx_cur_scope->__pyx_t_2;
+            __pyx_cur_scope->__pyx_t_2 = 0;
             __Pyx_XGOTREF(__pyx_t_8);
+            __pyx_t_9 = __pyx_cur_scope->__pyx_t_3;
+            __pyx_cur_scope->__pyx_t_3 = 0;
+            __Pyx_XGOTREF(__pyx_t_9);
             if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 82, __pyx_L8_error)
           }
 
           /* "tfrecord_lite.pyx":59
  *     :return: iterator over the decoded TFrecords
  *     """
  *     with open(filename, "rb") as file_handle:             # <<<<<<<<<<<<<<
  *         while True:
  *             # Read the header
  */
         }
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L13_try_end;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tfrecord_lite.tf_record_iterator", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_12) < 0) __PYX_ERR(0, 59, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_2) < 0) __PYX_ERR(0, 59, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_4, __pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L10_except_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
+          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 59, __pyx_L10_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 59, __pyx_L10_except_error)
-          __pyx_t_14 = ((!(__pyx_t_10 != 0)) != 0);
-          if (__pyx_t_14) {
+          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 59, __pyx_L10_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          if (__pyx_t_11 < 0) __PYX_ERR(0, 59, __pyx_L10_except_error)
+          __pyx_t_13 = (!__pyx_t_11);
+          if (unlikely(__pyx_t_13)) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_4);
-            __Pyx_XGIVEREF(__pyx_t_12);
-            __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_4, __pyx_t_12);
-            __pyx_t_1 = 0; __pyx_t_4 = 0; __pyx_t_12 = 0; 
+            __Pyx_XGIVEREF(__pyx_t_2);
+            __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_4, __pyx_t_2);
+            __pyx_t_1 = 0; __pyx_t_4 = 0; __pyx_t_2 = 0; 
             __PYX_ERR(0, 59, __pyx_L10_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
-        __Pyx_XGIVEREF(__pyx_t_6);
         __Pyx_XGIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
-        __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
+        __Pyx_XGIVEREF(__pyx_t_9);
+        __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
         goto __pyx_L1_error;
         __pyx_L12_try_return:;
-        __Pyx_XGIVEREF(__pyx_t_6);
         __Pyx_XGIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
-        __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
+        __Pyx_XGIVEREF(__pyx_t_9);
+        __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
         goto __pyx_L5_return;
         __pyx_L9_exception_handled:;
-        __Pyx_XGIVEREF(__pyx_t_6);
         __Pyx_XGIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
-        __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
+        __Pyx_XGIVEREF(__pyx_t_9);
+        __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
         __pyx_L13_try_end:;
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL);
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 59, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         goto __pyx_L7;
       }
       __pyx_L5_return: {
         __Pyx_PyThreadState_assign
-        __pyx_t_8 = 0; __pyx_t_7 = 0; __pyx_t_6 = 0; __pyx_t_13 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
-        if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_13, &__pyx_t_15, &__pyx_t_16);
-        if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_8, &__pyx_t_7, &__pyx_t_6) < 0)) __Pyx_ErrFetch(&__pyx_t_8, &__pyx_t_7, &__pyx_t_6);
+        __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_7 = 0; __pyx_t_12 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
+        if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_12, &__pyx_t_14, &__pyx_t_15);
+        if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7) < 0)) __Pyx_ErrFetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
+        __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_7);
-        __Pyx_XGOTREF(__pyx_t_6);
-        __Pyx_XGOTREF(__pyx_t_13);
+        __Pyx_XGOTREF(__pyx_t_12);
+        __Pyx_XGOTREF(__pyx_t_14);
         __Pyx_XGOTREF(__pyx_t_15);
-        __Pyx_XGOTREF(__pyx_t_16);
-        __pyx_t_17 = __pyx_r;
+        __pyx_t_16 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
-          __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL);
+          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 59, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_18);
-          __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+          if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_17);
+          __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         }
-        __pyx_r = __pyx_t_17;
-        __pyx_t_17 = 0;
+        __pyx_r = __pyx_t_16;
+        __pyx_t_16 = 0;
         if (PY_MAJOR_VERSION >= 3) {
-          __Pyx_XGIVEREF(__pyx_t_13);
+          __Pyx_XGIVEREF(__pyx_t_12);
+          __Pyx_XGIVEREF(__pyx_t_14);
           __Pyx_XGIVEREF(__pyx_t_15);
-          __Pyx_XGIVEREF(__pyx_t_16);
-          __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_15, __pyx_t_16);
+          __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_14, __pyx_t_15);
         }
+        __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_8);
         __Pyx_XGIVEREF(__pyx_t_7);
-        __Pyx_XGIVEREF(__pyx_t_6);
-        __Pyx_ErrRestore(__pyx_t_8, __pyx_t_7, __pyx_t_6);
-        __pyx_t_8 = 0; __pyx_t_7 = 0; __pyx_t_6 = 0; __pyx_t_13 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
+        __Pyx_ErrRestore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
+        __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_7 = 0; __pyx_t_12 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
         goto __pyx_L0;
       }
       __pyx_L7:;
     }
     goto __pyx_L23;
     __pyx_L4_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -2926,542 +4610,77 @@
  *     Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("tf_record_iterator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":32
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":38
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":44
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":50
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":56
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(const std::vector<std::string>  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_string", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.from_py":13
- * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- */
-
-static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
-  Py_ssize_t __pyx_v_length;
-  char const *__pyx_v_data;
-  std::string __pyx_r;
-  __Pyx_RefNannyDeclarations
-  char const *__pyx_t_1;
-  __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
-
-  /* "string.from_py":14
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
- *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- *     return string(data, length)
- */
-  __pyx_v_length = 0;
-
-  /* "string.from_py":15
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
- *     return string(data, length)
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(1, 15, __pyx_L1_error)
-  __pyx_v_data = __pyx_t_1;
-
-  /* "string.from_py":16
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- *     return string(data, length)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = std::string(__pyx_v_data, __pyx_v_length);
-  goto __pyx_L0;
-
-  /* "string.from_py":13
- * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-static std::vector<std::string>  __pyx_convert_vector_from_py_std_3a__3a_string(PyObject *__pyx_v_o) {
-  std::vector<std::string>  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<std::string>  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  std::string __pyx_t_5;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_string", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __pyx_convert_string_from_py_std__in_string(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((std::string)__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *__pyx_freelist_13tfrecord_lite___pyx_scope_struct__tf_record_iterator[8];
 static int __pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = 0;
 
 static PyObject *__pyx_tp_new_13tfrecord_lite___pyx_scope_struct__tf_record_iterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator)))) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((int)(__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator)))) {
     o = (PyObject*)__pyx_freelist_13tfrecord_lite___pyx_scope_struct__tf_record_iterator[--__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator];
     memset(o, 0, sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
+  #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_13tfrecord_lite___pyx_scope_struct__tf_record_iterator(PyObject *o) {
   struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *p = (struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_13tfrecord_lite___pyx_scope_struct__tf_record_iterator) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_crc_event_bytes);
   Py_CLEAR(p->__pyx_v_crc_header_bytes);
   Py_CLEAR(p->__pyx_v_event_bytes);
   Py_CLEAR(p->__pyx_v_file_handle);
   Py_CLEAR(p->__pyx_v_filename);
   Py_CLEAR(p->__pyx_v_header);
   Py_CLEAR(p->__pyx_v_header_len);
   Py_CLEAR(p->__pyx_v_header_str);
   Py_CLEAR(p->__pyx_v_names);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
   Py_CLEAR(p->__pyx_t_3);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator)))) {
+  if (CYTHON_COMPILING_IN_CPYTHON && ((int)(__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator)))) {
     __pyx_freelist_13tfrecord_lite___pyx_scope_struct__tf_record_iterator[__pyx_freecount_13tfrecord_lite___pyx_scope_struct__tf_record_iterator++] = ((struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_13tfrecord_lite___pyx_scope_struct__tf_record_iterator(PyObject *o, visitproc v, void *a) {
@@ -3504,18 +4723,33 @@
     e = (*v)(p->__pyx_t_2, a); if (e) return e;
   }
   if (p->__pyx_t_3) {
     e = (*v)(p->__pyx_t_3, a); if (e) return e;
   }
   return 0;
 }
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_13tfrecord_lite___pyx_scope_struct__tf_record_iterator},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_13tfrecord_lite___pyx_scope_struct__tf_record_iterator},
+  {Py_tp_new, (void *)__pyx_tp_new_13tfrecord_lite___pyx_scope_struct__tf_record_iterator},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator_spec = {
+  "tfrecord_lite.__pyx_scope_struct__tf_record_iterator",
+  sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = {
   PyVarObject_HEAD_INIT(0, 0)
-  "tfrecord_lite.__pyx_scope_struct__tf_record_iterator", /*tp_name*/
+  "tfrecord_lite.""__pyx_scope_struct__tf_record_iterator", /*tp_name*/
   sizeof(struct __pyx_obj_13tfrecord_lite___pyx_scope_struct__tf_record_iterator), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_13tfrecord_lite___pyx_scope_struct__tf_record_iterator, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -3535,155 +4769,154 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_13tfrecord_lite___pyx_scope_struct__tf_record_iterator, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_13tfrecord_lite___pyx_scope_struct__tf_record_iterator, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_tfrecord_lite(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_tfrecord_lite},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "tfrecord_lite",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_Q, __pyx_k_Q, sizeof(__pyx_k_Q), 0, 0, 1, 1},
-  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {&__pyx_n_s_buffer, __pyx_k_buffer, sizeof(__pyx_k_buffer), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
-  {&__pyx_n_s_crc_event_bytes, __pyx_k_crc_event_bytes, sizeof(__pyx_k_crc_event_bytes), 0, 0, 1, 1},
-  {&__pyx_n_s_crc_header_bytes, __pyx_k_crc_header_bytes, sizeof(__pyx_k_crc_header_bytes), 0, 0, 1, 1},
-  {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
-  {&__pyx_n_s_decode_example, __pyx_k_decode_example, sizeof(__pyx_k_decode_example), 0, 0, 1, 1},
-  {&__pyx_n_s_decoded, __pyx_k_decoded, sizeof(__pyx_k_decoded), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
-  {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
-  {&__pyx_n_s_event_bytes, __pyx_k_event_bytes, sizeof(__pyx_k_event_bytes), 0, 0, 1, 1},
-  {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {&__pyx_n_s_file_handle, __pyx_k_file_handle, sizeof(__pyx_k_file_handle), 0, 0, 1, 1},
-  {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
-  {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
-  {&__pyx_n_s_frombuffer, __pyx_k_frombuffer, sizeof(__pyx_k_frombuffer), 0, 0, 1, 1},
-  {&__pyx_n_s_header, __pyx_k_header, sizeof(__pyx_k_header), 0, 0, 1, 1},
-  {&__pyx_n_s_header_len, __pyx_k_header_len, sizeof(__pyx_k_header_len), 0, 0, 1, 1},
-  {&__pyx_n_s_header_str, __pyx_k_header_str, sizeof(__pyx_k_header_str), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
-  {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
-  {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_n_s_names, __pyx_k_names, sizeof(__pyx_k_names), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_s_rb, __pyx_k_rb, sizeof(__pyx_k_rb), 0, 0, 1, 1},
-  {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
-  {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
-  {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
-  {&__pyx_n_s_struct_2, __pyx_k_struct_2, sizeof(__pyx_k_struct_2), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_tf_record_iterator, __pyx_k_tf_record_iterator, sizeof(__pyx_k_tf_record_iterator), 0, 0, 1, 1},
-  {&__pyx_n_s_tfrecord_lite, __pyx_k_tfrecord_lite, sizeof(__pyx_k_tfrecord_lite), 0, 0, 1, 1},
-  {&__pyx_kp_s_tfrecord_lite_pyx, __pyx_k_tfrecord_lite_pyx, sizeof(__pyx_k_tfrecord_lite_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
-  {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
-  {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
-  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_n_s_Q, __pyx_k_Q, sizeof(__pyx_k_Q), 0, 0, 1, 1},
+    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 1},
+    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_buffer, __pyx_k_buffer, sizeof(__pyx_k_buffer), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+    {&__pyx_n_s_crc_event_bytes, __pyx_k_crc_event_bytes, sizeof(__pyx_k_crc_event_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_crc_header_bytes, __pyx_k_crc_header_bytes, sizeof(__pyx_k_crc_header_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
+    {&__pyx_n_s_decode_example, __pyx_k_decode_example, sizeof(__pyx_k_decode_example), 0, 0, 1, 1},
+    {&__pyx_n_s_decoded, __pyx_k_decoded, sizeof(__pyx_k_decoded), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
+    {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
+    {&__pyx_n_s_event_bytes, __pyx_k_event_bytes, sizeof(__pyx_k_event_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+    {&__pyx_n_s_file_handle, __pyx_k_file_handle, sizeof(__pyx_k_file_handle), 0, 0, 1, 1},
+    {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
+    {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
+    {&__pyx_n_s_frombuffer, __pyx_k_frombuffer, sizeof(__pyx_k_frombuffer), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_header, __pyx_k_header, sizeof(__pyx_k_header), 0, 0, 1, 1},
+    {&__pyx_n_s_header_len, __pyx_k_header_len, sizeof(__pyx_k_header_len), 0, 0, 1, 1},
+    {&__pyx_n_s_header_str, __pyx_k_header_str, sizeof(__pyx_k_header_str), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
+    {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
+    {&__pyx_n_s_names, __pyx_k_names, sizeof(__pyx_k_names), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_rb, __pyx_k_rb, sizeof(__pyx_k_rb), 0, 0, 1, 1},
+    {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
+    {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
+    {&__pyx_n_s_struct_2, __pyx_k_struct_2, sizeof(__pyx_k_struct_2), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_tf_record_iterator, __pyx_k_tf_record_iterator, sizeof(__pyx_k_tf_record_iterator), 0, 0, 1, 1},
+    {&__pyx_n_s_tfrecord_lite, __pyx_k_tfrecord_lite, sizeof(__pyx_k_tfrecord_lite), 0, 0, 1, 1},
+    {&__pyx_kp_s_tfrecord_lite_pyx, __pyx_k_tfrecord_lite_pyx, sizeof(__pyx_k_tfrecord_lite_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
+    {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
+    {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 59, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 61, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 75, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "tfrecord_lite.pyx":59
  *     :return: iterator over the decoded TFrecords
@@ -3699,45 +4932,58 @@
   /* "tfrecord_lite.pyx":46
  * 
  * 
  * def decode_example(bytes buffer, names=()):             # <<<<<<<<<<<<<<
  *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])
  *     return {key.decode('utf-8'): value for key, value in decoded.items()}
  */
-  __pyx_tuple__3 = PyTuple_Pack(6, __pyx_n_s_buffer, __pyx_n_s_names, __pyx_n_s_decoded, __pyx_n_s_name_2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tfrecord_lite_pyx, __pyx_n_s_decode_example, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(6, __pyx_n_s_buffer, __pyx_n_s_names, __pyx_n_s_decoded, __pyx_n_s_name_2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tfrecord_lite_pyx, __pyx_n_s_decode_example, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, ((PyObject*)__pyx_empty_tuple)); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "tfrecord_lite.pyx":51
  * 
  * 
  * def tf_record_iterator(filename, names=()):             # <<<<<<<<<<<<<<
  *     """
  *     Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.
  */
-  __pyx_tuple__5 = PyTuple_Pack(9, __pyx_n_s_filename, __pyx_n_s_names, __pyx_n_s_file_handle, __pyx_n_s_header_str, __pyx_n_s_header, __pyx_n_s_crc_header_bytes, __pyx_n_s_header_len, __pyx_n_s_event_bytes, __pyx_n_s_crc_event_bytes); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(2, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tfrecord_lite_pyx, __pyx_n_s_tf_record_iterator, 51, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_filename, __pyx_n_s_names, __pyx_n_s_file_handle, __pyx_n_s_header_str, __pyx_n_s_header, __pyx_n_s_crc_header_bytes, __pyx_n_s_header_len, __pyx_n_s_event_bytes, __pyx_n_s_crc_event_bytes); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tfrecord_lite_pyx, __pyx_n_s_tf_record_iterator, 51, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, ((PyObject*)__pyx_empty_tuple)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  return 0;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -3765,24 +5011,38 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator.tp_print = 0;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator_spec, NULL); if (unlikely(!__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator)) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator_spec, __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  #else
+  __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = &__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator.tp_dictoffset && __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator->tp_dictoffset && __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_13tfrecord_lite___pyx_scope_struct__tf_record_iterator = &__pyx_type_13tfrecord_lite___pyx_scope_struct__tf_record_iterator;
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3807,25 +5067,76 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_tfrecord_lite(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_tfrecord_lite},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "tfrecord_lite",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC inittfrecord_lite(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC inittfrecord_lite(void)
@@ -3855,42 +5166,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -3898,25 +5223,62 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_tfrecord_lite(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'tfrecord_lite' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("tfrecord_lite", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to tfrecord_lite pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -3927,82 +5289,63 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("tfrecord_lite", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_tfrecord_lite) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "tfrecord_lite")) {
-      if (unlikely(PyDict_SetItemString(modules, "tfrecord_lite", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "tfrecord_lite", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -4010,96 +5353,116 @@
   /* "tfrecord_lite.pyx":6
  * from libcpp.vector cimport vector
  * 
  * import numpy as _np             # <<<<<<<<<<<<<<
  * import struct as _struct
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tfrecord_lite.pyx":7
  * 
  * import numpy as _np
  * import struct as _struct             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct_2, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_struct, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_struct_2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_struct, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tfrecord_lite.pyx":46
  * 
  * 
  * def decode_example(bytes buffer, names=()):             # <<<<<<<<<<<<<<
  *     decoded = decode_example_internal(buffer, [name.encode('utf-8') for name in names])
  *     return {key.decode('utf-8'): value for key, value in decoded.items()}
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13tfrecord_lite_1decode_example, NULL, __pyx_n_s_tfrecord_lite); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_example, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_13tfrecord_lite_1decode_example, 0, __pyx_n_s_decode_example, NULL, __pyx_n_s_tfrecord_lite, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__6);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_example, __pyx_t_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tfrecord_lite.pyx":51
  * 
  * 
  * def tf_record_iterator(filename, names=()):             # <<<<<<<<<<<<<<
  *     """
  *     Iterate over decoded tfrecord dictionaries; it does not perform CRC checks of the records.
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13tfrecord_lite_3tf_record_iterator, NULL, __pyx_n_s_tfrecord_lite); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_tf_record_iterator, __pyx_t_1) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_13tfrecord_lite_3tf_record_iterator, 0, __pyx_n_s_tf_record_iterator, NULL, __pyx_n_s_tfrecord_lite, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_tf_record_iterator, __pyx_t_2) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tfrecord_lite.pyx":1
  * from libcpp.set cimport set             # <<<<<<<<<<<<<<
  * from libcpp.map cimport map
  * from libcpp.string cimport string
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init tfrecord_lite", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init tfrecord_lite");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#if _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -4111,32 +5474,103 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
@@ -4182,14 +5616,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -4204,15 +5646,15 @@
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -4220,14 +5662,221 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -4237,34 +5886,46 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -4281,33 +5942,34 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -4324,19 +5986,20 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
@@ -4365,57 +6028,40 @@
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -4436,15 +6082,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -4452,15 +6097,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -4523,44 +6168,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
-
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -4574,87 +6189,89 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-#endif
-
-/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
 #else
-    if (likely(PyCFunction_Check(func)))
+        if (PyCFunction_Check(func))
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
 #endif
-
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
@@ -4684,30 +6301,375 @@
             return -1;
         }
     }
     return 0;
 #endif
 }
 
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
+    }
+    return __Pyx_IterFinish();
+}
+
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* UnpackTupleError */
+static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
+    if (t == Py_None) {
+      __Pyx_RaiseNoneNotIterableError();
+    } else if (PyTuple_GET_SIZE(t) < index) {
+      __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
     } else {
-        return __Pyx_IterFinish();
+      __Pyx_RaiseTooManyValuesError(index);
+    }
+}
+
+/* UnpackTuple2 */
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
+    PyObject *value1 = NULL, *value2 = NULL;
+#if CYTHON_COMPILING_IN_PYPY
+    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
+    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
+#else
+    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
+    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
+#endif
+    if (decref_tuple) {
+        Py_DECREF(tuple);
     }
+    *pvalue1 = value1;
+    *pvalue2 = value2;
     return 0;
+#if CYTHON_COMPILING_IN_PYPY
+bad:
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+#endif
+}
+static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
+                                       int has_known_size, int decref_tuple) {
+    Py_ssize_t index;
+    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
+    iternextfunc iternext;
+    iter = PyObject_GetIter(tuple);
+    if (unlikely(!iter)) goto bad;
+    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
+    iternext = __Pyx_PyObject_GetIterNextFunc(iter);
+    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
+    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
+    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
+    Py_DECREF(iter);
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
+unpacking_failed:
+    if (!has_known_size && __Pyx_IterFinish() == 0)
+        __Pyx_RaiseNeedMoreValuesError(index);
+bad:
+    Py_XDECREF(iter);
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+}
+
+/* dict_iter */
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_source_is_dict) {
+    is_dict = is_dict || likely(PyDict_CheckExact(iterable));
+    *p_source_is_dict = is_dict;
+    if (is_dict) {
+#if !CYTHON_COMPILING_IN_PYPY
+        *p_orig_length = PyDict_Size(iterable);
+        Py_INCREF(iterable);
+        return iterable;
+#elif PY_MAJOR_VERSION >= 3
+        static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
+        PyObject **pp = NULL;
+        if (method_name) {
+            const char *name = PyUnicode_AsUTF8(method_name);
+            if (strcmp(name, "iteritems") == 0) pp = &py_items;
+            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
+            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
+            if (pp) {
+                if (!*pp) {
+                    *pp = PyUnicode_FromString(name + 4);
+                    if (!*pp)
+                        return NULL;
+                }
+                method_name = *pp;
+            }
+        }
+#endif
+    }
+    *p_orig_length = 0;
+    if (method_name) {
+        PyObject* iter;
+        iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
+        if (!iterable)
+            return NULL;
+#if !CYTHON_COMPILING_IN_PYPY
+        if (PyTuple_CheckExact(iterable) || PyList_CheckExact(iterable))
+            return iterable;
+#endif
+        iter = PyObject_GetIter(iterable);
+        Py_DECREF(iterable);
+        return iter;
+    }
+    return PyObject_GetIter(iterable);
+}
+static CYTHON_INLINE int __Pyx_dict_iter_next(
+        PyObject* iter_obj, CYTHON_NCP_UNUSED Py_ssize_t orig_length, CYTHON_NCP_UNUSED Py_ssize_t* ppos,
+        PyObject** pkey, PyObject** pvalue, PyObject** pitem, int source_is_dict) {
+    PyObject* next_item;
+#if !CYTHON_COMPILING_IN_PYPY
+    if (source_is_dict) {
+        PyObject *key, *value;
+        if (unlikely(orig_length != PyDict_Size(iter_obj))) {
+            PyErr_SetString(PyExc_RuntimeError, "dictionary changed size during iteration");
+            return -1;
+        }
+        if (unlikely(!PyDict_Next(iter_obj, ppos, &key, &value))) {
+            return 0;
+        }
+        if (pitem) {
+            PyObject* tuple = PyTuple_New(2);
+            if (unlikely(!tuple)) {
+                return -1;
+            }
+            Py_INCREF(key);
+            Py_INCREF(value);
+            PyTuple_SET_ITEM(tuple, 0, key);
+            PyTuple_SET_ITEM(tuple, 1, value);
+            *pitem = tuple;
+        } else {
+            if (pkey) {
+                Py_INCREF(key);
+                *pkey = key;
+            }
+            if (pvalue) {
+                Py_INCREF(value);
+                *pvalue = value;
+            }
+        }
+        return 1;
+    } else if (PyTuple_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyTuple_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyTuple_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else if (PyList_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyList_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyList_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else
+#endif
+    {
+        next_item = PyIter_Next(iter_obj);
+        if (unlikely(!next_item)) {
+            return __Pyx_IterFinish();
+        }
+    }
+    if (pitem) {
+        *pitem = next_item;
+    } else if (pkey && pvalue) {
+        if (__Pyx_unpack_tuple2(next_item, pkey, pvalue, source_is_dict, source_is_dict, 1))
+            return -1;
+    } else if (pkey) {
+        *pkey = next_item;
+    } else {
+        *pvalue = next_item;
+    }
+    return 1;
+}
+
+/* PyObjectLookupSpecial */
+#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error) {
+    PyObject *res;
+    PyTypeObject *tp = Py_TYPE(obj);
+#if PY_MAJOR_VERSION < 3
+    if (unlikely(PyInstance_Check(obj)))
+        return with_error ? __Pyx_PyObject_GetAttrStr(obj, attr_name) : __Pyx_PyObject_GetAttrStrNoError(obj, attr_name);
+#endif
+    res = _PyType_Lookup(tp, attr_name);
+    if (likely(res)) {
+        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
+        if (!f) {
+            Py_INCREF(res);
+        } else {
+            res = f(res, obj, (PyObject *)tp);
+        }
+    } else if (with_error) {
+        PyErr_SetObject(PyExc_AttributeError, attr_name);
+    }
+    return res;
 }
+#endif
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (!j) return NULL;
+    if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -4760,27 +6722,35 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return m->sq_item(o, i);
+            return sm->sq_item(o, i);
         }
     }
 #else
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
@@ -4789,41 +6759,66 @@
 
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
         exc_info = exc_info->previous_item;
     }
     return exc_info;
 }
 #endif
 
 /* SaveResetException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
     *type = exc_info->exc_type;
     *value = exc_info->exc_value;
     *tb = exc_info->exc_traceback;
-    #else
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
     *type = tstate->exc_type;
     *value = tstate->exc_value;
     *tb = tstate->exc_traceback;
-    #endif
     Py_XINCREF(*type);
     Py_XINCREF(*value);
     Py_XINCREF(*tb);
+  #endif
 }
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = type;
@@ -4836,14 +6831,15 @@
     tstate->exc_type = type;
     tstate->exc_value = value;
     tstate->exc_traceback = tb;
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+  #endif
 }
 #endif
 
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
@@ -4881,20 +6877,29 @@
     *type = local_type;
     *value = local_value;
     *tb = local_tb;
 #if CYTHON_FAST_THREAD_STATE
     #if CYTHON_USE_EXC_INFO_STACK
     {
         _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
         tmp_type = exc_info->exc_type;
         tmp_value = exc_info->exc_value;
         tmp_tb = exc_info->exc_traceback;
         exc_info->exc_type = local_type;
         exc_info->exc_value = local_value;
         exc_info->exc_traceback = local_tb;
+      #endif
     }
     #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = local_type;
     tstate->exc_value = local_value;
@@ -4913,58 +6918,48 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        tmp_tb = PyException_GetTraceback(tmp_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
     exc_info->exc_value = *value;
     exc_info->exc_traceback = *tb;
-    #else
+  #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = *type;
     tstate->exc_value = *value;
     tstate->exc_traceback = *tb;
-    #endif
+  #endif
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -4972,25 +6967,254 @@
     PyErr_SetExcInfo(*type, *value, *tb);
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
+/* pep479 */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen) {
+    PyObject *exc, *val, *tb, *cur_exc;
+    __Pyx_PyThreadState_declare
+    #ifdef __Pyx_StopAsyncIteration_USED
+    int is_async_stopiteration = 0;
+    #endif
+    CYTHON_MAYBE_UNUSED_VAR(in_async_gen);
+    cur_exc = PyErr_Occurred();
+    if (likely(!__Pyx_PyErr_GivenExceptionMatches(cur_exc, PyExc_StopIteration))) {
+        #ifdef __Pyx_StopAsyncIteration_USED
+        if (in_async_gen && unlikely(__Pyx_PyErr_GivenExceptionMatches(cur_exc, __Pyx_PyExc_StopAsyncIteration))) {
+            is_async_stopiteration = 1;
+        } else
+        #endif
+            return;
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_GetException(&exc, &val, &tb);
+    Py_XDECREF(exc);
+    Py_XDECREF(val);
+    Py_XDECREF(tb);
+    PyErr_SetString(PyExc_RuntimeError,
+        #ifdef __Pyx_StopAsyncIteration_USED
+        is_async_stopiteration ? "async generator raised StopAsyncIteration" :
+        in_async_gen ? "async generator raised StopIteration" :
+        #endif
+        "generator raised StopIteration");
+}
+
+/* FixUpExtensionType */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    for (i = 1; i < n; i++)
+    {
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+    }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -5014,120 +7238,1302 @@
     }
     return descr;
 }
 #endif
 
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, empty_dict, empty_dict, from_list, level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FetchSharedCythonModule */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+#if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -5183,99 +8589,133 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5283,18 +8723,26 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -5315,14 +8763,29 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__9));
+    }
+    return name;
+}
+#endif
+
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -5338,249 +8801,67 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(size_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (size_t) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (size_t) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(size_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(size_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            size_t val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (size_t) -1;
-        }
-    } else {
-        size_t val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (size_t) -1;
-        val = __Pyx_PyInt_As_size_t(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to size_t");
-    return (size_t) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to size_t");
-    return (size_t) -1;
-}
-
-/* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (long) 0;
                 case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
                             return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
                             return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -5592,96 +8873,96 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (long) 0;
                 case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
                 case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
                             return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
 #else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
@@ -5717,59 +8998,66 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (int) 0;
                 case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
                             return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
                             return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -5781,96 +9069,96 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (int) 0;
                 case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
                 case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
                             return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
 #else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
@@ -5908,15 +9196,15 @@
     return (int) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -5929,14 +9217,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -5953,19 +9257,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -6004,58 +9308,19 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
-/* FetchCommonType */
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
-    PyObject* fake_module;
-    PyTypeObject* cached_type = NULL;
-    fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
-    if (!fake_module) return NULL;
-    Py_INCREF(fake_module);
-    cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
-    if (cached_type) {
-        if (!PyType_Check((PyObject*)cached_type)) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s is not a type object",
-                type->tp_name);
-            goto bad;
-        }
-        if (cached_type->tp_basicsize != type->tp_basicsize) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s has the wrong size, try recompiling",
-                type->tp_name);
-            goto bad;
-        }
-    } else {
-        if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-        PyErr_Clear();
-        if (PyType_Ready(type) < 0) goto bad;
-        if (PyObject_SetAttrString(fake_module, type->tp_name, (PyObject*) type) < 0)
-            goto bad;
-        Py_INCREF(type);
-        cached_type = type;
-    }
-done:
-    Py_DECREF(fake_module);
-    return cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -6180,130 +9445,40 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (descr != NULL) {
-        *method = descr;
-        return 0;
-    }
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
-#endif
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectCallMethod1 */
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
@@ -6317,35 +9492,41 @@
         return result;
     }
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
-#include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
-static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
+static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
+    CYTHON_UNUSED_VAR(__pyx_tstate);
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
         Py_XDECREF(ev);
         Py_INCREF(Py_None);
         *pvalue = Py_None;
         return 0;
     }
     if (likely(et == PyExc_StopIteration)) {
         if (!ev) {
             Py_INCREF(Py_None);
             value = Py_None;
         }
 #if PY_VERSION_HEX >= 0x030300A0
-        else if (Py_TYPE(ev) == (PyTypeObject*)PyExc_StopIteration) {
+        else if (likely(__Pyx_IS_TYPE(ev, (PyTypeObject*)PyExc_StopIteration))) {
             value = ((PyStopIterationObject *)ev)->value;
             Py_INCREF(value);
             Py_DECREF(ev);
         }
 #endif
         else if (unlikely(PyTuple_Check(ev))) {
             if (PyTuple_GET_SIZE(ev) >= 1) {
@@ -6401,28 +9582,33 @@
     }
 #endif
     *pvalue = value;
     return 0;
 }
 static CYTHON_INLINE
 void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_CLEAR(exc_state->exc_value);
+#else
     PyObject *t, *v, *tb;
     t = exc_state->exc_type;
     v = exc_state->exc_value;
     tb = exc_state->exc_traceback;
     exc_state->exc_type = NULL;
     exc_state->exc_value = NULL;
     exc_state->exc_traceback = NULL;
     Py_XDECREF(t);
     Py_XDECREF(v);
     Py_XDECREF(tb);
+#endif
 }
 #define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyRunningError(CYTHON_UNUSED __pyx_CoroutineObject *gen) {
+static void __Pyx__Coroutine_AlreadyRunningError(__pyx_CoroutineObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
         msg = "coroutine already executing";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
@@ -6430,16 +9616,17 @@
     #endif
     } else {
         msg = "generator already executing";
     }
     PyErr_SetString(PyExc_ValueError, msg);
 }
 #define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_NotStartedError(CYTHON_UNUSED PyObject *gen) {
+static void __Pyx__Coroutine_NotStartedError(PyObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check(gen)) {
         msg = "can't send non-None value to a just-started coroutine";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact(gen)) {
@@ -6447,15 +9634,17 @@
     #endif
     } else {
         msg = "can't send non-None value to a just-started generator";
     }
     PyErr_SetString(PyExc_TypeError, msg);
 }
 #define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyTerminatedError(CYTHON_UNUSED PyObject *gen, PyObject *value, CYTHON_UNUSED int closing) {
+static void __Pyx__Coroutine_AlreadyTerminatedError(PyObject *gen, PyObject *value, int closing) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    CYTHON_MAYBE_UNUSED_VAR(closing);
     #ifdef __Pyx_Coroutine_USED
     if (!closing && __Pyx_Coroutine_Check(gen)) {
         PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
     } else
     #endif
     if (value) {
         #ifdef __Pyx_AsyncGen_USED
@@ -6484,23 +9673,36 @@
 #if CYTHON_FAST_THREAD_STATE
     __Pyx_PyThreadState_assign
     tstate = __pyx_tstate;
 #else
     tstate = __Pyx_PyThreadState_Current;
 #endif
     exc_state = &self->gi_exc_state;
-    if (exc_state->exc_type) {
-        #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+    if (exc_state->exc_value) {
+        #if CYTHON_COMPILING_IN_PYPY
+        #else
+        PyObject *exc_tb;
+        #if PY_VERSION_HEX >= 0x030B00a4
+        exc_tb = PyException_GetTraceback(exc_state->exc_value);
         #else
-        if (exc_state->exc_traceback) {
-            PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
+        exc_tb = exc_state->exc_traceback;
+        #endif
+        if (exc_tb) {
+            PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
+            #if PY_VERSION_HEX >= 0x030B00a4
+            Py_DECREF(exc_tb);
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -6508,51 +9710,86 @@
         __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     } else {
         __Pyx_Coroutine_ExceptionClear(exc_state);
         __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     }
 #endif
     self->is_running = 1;
-    retval = self->body((PyObject *) self, tstate, value);
+    retval = self->body(self, tstate, value);
     self->is_running = 0;
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state = &self->gi_exc_state;
     tstate->exc_info = exc_state->previous_item;
     exc_state->previous_item = NULL;
     __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
 #endif
     return retval;
 }
 static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
-    PyObject *exc_tb = exc_state->exc_traceback;
-    if (likely(exc_tb)) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+#if CYTHON_COMPILING_IN_PYPY
+    CYTHON_UNUSED_VAR(exc_state);
 #else
+    PyObject *exc_tb;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    if (!exc_state->exc_value) return;
+    exc_tb = PyException_GetTraceback(exc_state->exc_value);
+    #else
+    exc_tb = exc_state->exc_traceback;
+    #endif
+    if (likely(exc_tb)) {
         PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
         PyFrameObject *f = tb->tb_frame;
         Py_CLEAR(f->f_back);
-#endif
+        #if PY_VERSION_HEX >= 0x030B00a4
+        Py_DECREF(exc_tb);
+        #endif
     }
+#endif
 }
 static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_MethodReturn(CYTHON_UNUSED PyObject* gen, PyObject *retval) {
+PyObject *__Pyx_Coroutine_MethodReturn(PyObject* gen, PyObject *retval) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if (unlikely(!retval)) {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         if (!__Pyx_PyErr_Occurred()) {
             PyObject *exc = PyExc_StopIteration;
             #ifdef __Pyx_AsyncGen_USED
             if (__Pyx_AsyncGen_CheckExact(gen))
                 exc = __Pyx_PyExc_StopAsyncIteration;
             #endif
             __Pyx_PyErr_SetNone(exc);
         }
     }
     return retval;
 }
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
+static CYTHON_INLINE
+PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
+#if PY_VERSION_HEX <= 0x030A00A1
+    return _PyGen_Send(gen, arg);
+#else
+    PyObject *result;
+    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
+        if (PyAsyncGen_CheckExact(gen)) {
+            assert(result == Py_None);
+            PyErr_SetNone(PyExc_StopAsyncIteration);
+        }
+        else if (result == Py_None) {
+            PyErr_SetNone(PyExc_StopIteration);
+        }
+        else {
+            _PyGen_SetStopIterationValue(result);
+        }
+        Py_CLEAR(result);
+    }
+    return result;
+#endif
+}
+#endif
 static CYTHON_INLINE
 PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
     PyObject *ret;
     PyObject *val = NULL;
     __Pyx_Coroutine_Undelegate(gen);
     __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
     ret = __Pyx_Coroutine_SendEx(gen, val, 0);
@@ -6581,25 +9818,25 @@
         #ifdef __Pyx_AsyncGen_USED
         if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
             ret = __Pyx_async_gen_asend_send(yf, value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyCoro_CheckExact(yf)) {
-            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         {
             if (value == Py_None)
-                ret = Py_TYPE(yf)->tp_iternext(yf);
+                ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
             else
                 ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
         }
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
@@ -6638,24 +9875,23 @@
     if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
         retval = __Pyx_async_gen_athrow_close(yf, NULL);
     } else
     #endif
     {
         PyObject *meth;
         gen->is_running = 1;
-        meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_close);
+        meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_close);
         if (unlikely(!meth)) {
-            if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+            if (unlikely(PyErr_Occurred())) {
                 PyErr_WriteUnraisable(yf);
             }
-            PyErr_Clear();
         } else {
-            retval = PyObject_CallFunction(meth, NULL);
+            retval = __Pyx_PyObject_CallNoArg(meth);
             Py_DECREF(meth);
-            if (!retval)
+            if (unlikely(!retval))
                 err = -1;
         }
         gen->is_running = 0;
     }
     Py_XDECREF(retval);
     return err;
 }
@@ -6670,32 +9906,33 @@
         #ifdef __Pyx_Generator_USED
         if (__Pyx_Generator_CheckExact(yf)) {
             ret = __Pyx_Generator_Next(yf);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = _PyGen_Send((PyGenObject*)yf, NULL);
+            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
         } else
         #endif
         #ifdef __Pyx_Coroutine_USED
         if (__Pyx_Coroutine_Check(yf)) {
             ret = __Pyx_Coroutine_Send(yf, Py_None);
         } else
         #endif
-            ret = Py_TYPE(yf)->tp_iternext(yf);
+            ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
         return __Pyx_Coroutine_FinishDelegation(gen);
     }
     return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
 }
-static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_Coroutine_Close(self);
 }
 static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject *retval, *raised_exception;
     PyObject *yf = gen->yieldfrom;
     int err = 0;
@@ -6768,30 +10005,30 @@
             ) {
             ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
         #ifdef __Pyx_Coroutine_USED
         } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
             ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
         #endif
         } else {
-            PyObject *meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_throw);
+            PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_throw);
             if (unlikely(!meth)) {
                 Py_DECREF(yf);
-                if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+                if (unlikely(PyErr_Occurred())) {
                     gen->is_running = 0;
                     return NULL;
                 }
-                PyErr_Clear();
                 __Pyx_Coroutine_Undelegate(gen);
                 gen->is_running = 0;
                 goto throw_here;
             }
             if (likely(args)) {
-                ret = PyObject_CallObject(meth, args);
+                ret = __Pyx_PyObject_Call(meth, args, NULL);
             } else {
-                ret = PyObject_CallFunctionObjArgs(meth, typ, val, tb, NULL);
+                PyObject *cargs[4] = {NULL, typ, val, tb};
+                ret = __Pyx_PyObject_FastCall(meth, cargs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
             }
             Py_DECREF(meth);
         }
         gen->is_running = 0;
         Py_DECREF(yf);
         if (!ret) {
             ret = __Pyx_Coroutine_FinishDelegation(gen);
@@ -6802,22 +10039,26 @@
     __Pyx_Raise(typ, val, tb, NULL);
     return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
 }
 static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
     PyObject *typ;
     PyObject *val = NULL;
     PyObject *tb = NULL;
-    if (!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb))
+    if (unlikely(!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb)))
         return NULL;
     return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
 }
 static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_VISIT(exc_state->exc_value);
+#else
     Py_VISIT(exc_state->exc_type);
     Py_VISIT(exc_state->exc_value);
     Py_VISIT(exc_state->exc_traceback);
+#endif
     return 0;
 }
 static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
     Py_VISIT(gen->closure);
     Py_VISIT(gen->classobj);
     Py_VISIT(gen->yieldfrom);
     return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
@@ -6830,31 +10071,32 @@
     __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
     }
 #endif
     Py_CLEAR(gen->gi_code);
+    Py_CLEAR(gen->gi_frame);
     Py_CLEAR(gen->gi_name);
     Py_CLEAR(gen->gi_qualname);
     Py_CLEAR(gen->gi_modulename);
     return 0;
 }
 static void __Pyx_Coroutine_dealloc(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject_GC_UnTrack(gen);
     if (gen->gi_weakreflist != NULL)
         PyObject_ClearWeakRefs(self);
     if (gen->resume_label >= 0) {
         PyObject_GC_Track(self);
 #if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
-        if (PyObject_CallFinalizerFromDealloc(self))
+        if (unlikely(PyObject_CallFinalizerFromDealloc(self)))
 #else
         Py_TYPE(gen)->tp_del(self);
-        if (self->ob_refcnt > 0)
+        if (unlikely(Py_REFCNT(self) > 0))
 #endif
         {
             return;
         }
         PyObject_GC_UnTrack(self);
     }
 #ifdef __Pyx_AsyncGen_USED
@@ -6862,26 +10104,26 @@
         /* We have to handle this case for asynchronous generators
            right here, because this code has to be between UNTRACK
            and GC_Del. */
         Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
     }
 #endif
     __Pyx_Coroutine_clear(self);
-    PyObject_GC_Del(gen);
+    __Pyx_PyHeapTypeObject_GC_Del(gen);
 }
 static void __Pyx_Coroutine_del(PyObject *self) {
     PyObject *error_type, *error_value, *error_traceback;
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     __Pyx_PyThreadState_declare
     if (gen->resume_label < 0) {
         return;
     }
 #if !CYTHON_USE_TP_FINALIZE
     assert(self->ob_refcnt == 0);
-    self->ob_refcnt = 1;
+    __Pyx_SET_REFCNT(self, 1);
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
         PyObject *finalizer = agen->ag_finalizer;
@@ -6940,90 +10182,110 @@
                 PyErr_WriteUnraisable(self);
         } else {
             Py_DECREF(res);
         }
     }
     __Pyx_ErrRestore(error_type, error_value, error_traceback);
 #if !CYTHON_USE_TP_FINALIZE
-    assert(self->ob_refcnt > 0);
-    if (--self->ob_refcnt == 0) {
+    assert(Py_REFCNT(self) > 0);
+    if (likely(--self->ob_refcnt == 0)) {
         return;
     }
     {
-        Py_ssize_t refcnt = self->ob_refcnt;
+        Py_ssize_t refcnt = Py_REFCNT(self);
         _Py_NewReference(self);
-        self->ob_refcnt = refcnt;
+        __Pyx_SET_REFCNT(self, refcnt);
     }
 #if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(self->ob_type) &&
+    assert(PyType_IS_GC(Py_TYPE(self)) &&
            _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
     _Py_DEC_REFTOTAL;
 #endif
 #ifdef COUNT_ALLOCS
     --Py_TYPE(self)->tp_frees;
     --Py_TYPE(self)->tp_allocs;
 #endif
 #endif
 }
 static PyObject *
-__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_name;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__name__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_name;
     Py_INCREF(value);
-    self->gi_name = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_name, value);
     return 0;
 }
 static PyObject *
-__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_qualname;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__qualname__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_qualname;
     Py_INCREF(value);
-    self->gi_qualname = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_qualname, value);
     return 0;
 }
+static PyObject *
+__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, void *context)
+{
+    PyObject *frame = self->gi_frame;
+    CYTHON_UNUSED_VAR(context);
+    if (!frame) {
+        if (unlikely(!self->gi_code)) {
+            Py_RETURN_NONE;
+        }
+        frame = (PyObject *) PyFrame_New(
+            PyThreadState_Get(),            /*PyThreadState *tstate,*/
+            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
+            __pyx_d,                 /*PyObject *globals,*/
+            0                               /*PyObject *locals*/
+        );
+        if (unlikely(!frame))
+            return NULL;
+        self->gi_frame = frame;
+    }
+    Py_INCREF(frame);
+    return frame;
+}
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
             PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
             PyObject *name, PyObject *qualname, PyObject *module_name) {
     __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
     if (unlikely(!gen))
         return NULL;
     return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
@@ -7034,29 +10296,34 @@
     gen->body = body;
     gen->closure = closure;
     Py_XINCREF(closure);
     gen->is_running = 0;
     gen->resume_label = 0;
     gen->classobj = NULL;
     gen->yieldfrom = NULL;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    gen->gi_exc_state.exc_value = NULL;
+    #else
     gen->gi_exc_state.exc_type = NULL;
     gen->gi_exc_state.exc_value = NULL;
     gen->gi_exc_state.exc_traceback = NULL;
+    #endif
 #if CYTHON_USE_EXC_INFO_STACK
     gen->gi_exc_state.previous_item = NULL;
 #endif
     gen->gi_weakreflist = NULL;
     Py_XINCREF(qualname);
     gen->gi_qualname = qualname;
     Py_XINCREF(name);
     gen->gi_name = name;
     Py_XINCREF(module_name);
     gen->gi_modulename = module_name;
     Py_XINCREF(code);
     gen->gi_code = code;
+    gen->gi_frame = NULL;
     PyObject_GC_Track(gen);
     return gen;
 }
 
 /* PatchModuleWithCoroutine */
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
@@ -7120,15 +10387,15 @@
 #endif
 static int __Pyx_patch_abc(void) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
     static int abc_patched = 0;
     if (CYTHON_REGISTER_ABCS && !abc_patched) {
         PyObject *module;
         module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
-        if (!module) {
+        if (unlikely(!module)) {
             PyErr_WriteUnraisable(NULL);
             if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
                     ((PY_MAJOR_VERSION >= 3) ?
                         "Cython module failed to register with collections.abc module" :
                         "Cython module failed to register with collections module"), 1) < 0)) {
                 return -1;
             }
@@ -7165,26 +10432,55 @@
     {0, 0, 0, 0}
 };
 static PyMemberDef __pyx_Generator_memberlist[] = {
     {(char *) "gi_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
     {(char*) "gi_yieldfrom", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
      (char*) PyDoc_STR("object being iterated by 'yield from', or None")},
     {(char*) "gi_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
+    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyGetSetDef __pyx_Generator_getsets[] = {
     {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the generator"), 0},
     {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the generator"), 0},
+    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
+     (char*) PyDoc_STR("Frame of the generator"), 0},
     {0, 0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_GeneratorType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
+    {Py_tp_traverse, (void *)__Pyx_Coroutine_traverse},
+    {Py_tp_iter, (void *)PyObject_SelfIter},
+    {Py_tp_iternext, (void *)__Pyx_Generator_Next},
+    {Py_tp_methods, (void *)__pyx_Generator_methods},
+    {Py_tp_members, (void *)__pyx_Generator_memberlist},
+    {Py_tp_getset, (void *)__pyx_Generator_getsets},
+    {Py_tp_getattro, (void *) __Pyx_PyObject_GenericGetAttrNoDict},
+#if CYTHON_USE_TP_FINALIZE
+    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
+#endif
+    {0, 0},
+};
+static PyType_Spec __pyx_GeneratorType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "generator",
+    sizeof(__pyx_CoroutineObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    __pyx_GeneratorType_slots
+};
+#else
 static PyTypeObject __pyx_GeneratorType_type = {
     PyVarObject_HEAD_INIT(0, 0)
-    "generator",
+    __PYX_TYPE_MODULE_PREFIX "generator",
     sizeof(__pyx_CoroutineObject),
     0,
     (destructor) __Pyx_Coroutine_dealloc,
     0,
     0,
     0,
     0,
@@ -7231,75 +10527,119 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
-static int __pyx_Generator_init(void) {
+#endif
+static int __pyx_Generator_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_GeneratorType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_GeneratorType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
+#endif
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
+#if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -7353,15 +10693,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -7382,30 +10722,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -7463,15 +10807,15 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
+    const digit* digits = __Pyx_PyLong_Digits(b);
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
         ival = likely(size) ? digits[0] : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
@@ -7512,16 +10856,41 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#if _MSV_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `tfrecord_lite-0.0.7/tfrecord_lite.egg-info/PKG-INFO` & `tfrecord_lite-0.0.8/tfrecord_lite.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tfrecord-lite
-Version: 0.0.7
+Version: 0.0.8
 Summary: A lightweight tfrecord parser
 Home-page: https://github.com/jongwook/tfrecord_lite
 Author: Jong Wook Kim
 Author-email: jongwook@nyu.edu
 License: MIT
 Project-URL: Source, https://github.com/jongwook/tfrecord_lite
 Project-URL: Tracker, https://github.com/jongwook/tfrecord_lite/issues
-Description: UNKNOWN
 Keywords: tfrecord
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+License-File: LICENSE
```

### Comparing `tfrecord_lite-0.0.7/tfrecord_lite.pyx` & `tfrecord_lite-0.0.8/tfrecord_lite.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     cdef struct decoder_output:
         vector[string] names
         map[string, vector[string]] bytes_features
         map[string, string] int64_features
         map[string, string] float_features
 
-    decoder_output decode_tfrecord_example(const unsigned char *bytes, size_t length, const decoder_options &options)
+    decoder_output decode_tfrecord_example(const unsigned char *bytes, size_t length, const decoder_options &options) except +
 
 
 cdef decode_example_internal(bytes buffer, vector[string] names):
     cdef decoder_options options
     options.names = set[string]()
     for name in names:
         options.names.insert(name)
```

