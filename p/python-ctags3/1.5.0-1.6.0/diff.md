# Comparing `tmp/python-ctags3-1.5.0.tar.gz` & `tmp/python-ctags3-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-ctags3-1.5.0.tar", last modified: Sat Sep  5 20:07:25 2020, max compression
+gzip compressed data, was "python-ctags3-1.6.0.tar", last modified: Sat Jun  3 15:00:57 2023, max compression
```

## Comparing `python-ctags3-1.5.0.tar` & `python-ctags3-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.699202 python-ctags3-1.5.0/
--rw-r--r--   0 j          (501) staff       (20)      148 2017-04-27 16:36:28.000000 python-ctags3-1.5.0/MANIFEST.in
--rw-r--r--   0 j          (501) staff       (20)     1577 2020-09-05 20:07:25.698520 python-ctags3-1.5.0/PKG-INFO
--rw-r--r--   0 j          (501) staff       (20)     3521 2020-09-05 12:08:18.000000 python-ctags3-1.5.0/README.md
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.690442 python-ctags3-1.5.0/python_ctags3.egg-info/
--rw-r--r--   0 j          (501) staff       (20)     1577 2020-09-05 20:07:25.000000 python-ctags3-1.5.0/python_ctags3.egg-info/PKG-INFO
--rw-r--r--   0 j          (501) staff       (20)      355 2020-09-05 20:07:25.000000 python-ctags3-1.5.0/python_ctags3.egg-info/SOURCES.txt
--rw-r--r--   0 j          (501) staff       (20)        1 2020-09-05 20:07:25.000000 python-ctags3-1.5.0/python_ctags3.egg-info/dependency_links.txt
--rw-r--r--   0 j          (501) staff       (20)       16 2020-09-05 20:07:25.000000 python-ctags3-1.5.0/python_ctags3.egg-info/top_level.txt
--rw-r--r--   0 j          (501) staff       (20)       38 2020-09-05 20:07:25.699433 python-ctags3-1.5.0/setup.cfg
--rw-r--r--   0 j          (501) staff       (20)     1925 2020-09-05 20:06:43.000000 python-ctags3-1.5.0/setup.py
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.692579 python-ctags3-1.5.0/src/
--rw-r--r--   0 j          (501) staff       (20)   295652 2020-09-05 20:07:19.000000 python-ctags3-1.5.0/src/_readtags.c
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.693319 python-ctags3-1.5.0/src/ctags/
--rw-r--r--   0 j          (501) staff       (20)      985 2017-04-27 16:36:28.000000 python-ctags3-1.5.0/src/ctags/__init__.py
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.694657 python-ctags3-1.5.0/src/examples/
--rw-r--r--   0 j          (501) staff       (20)      812 2020-09-05 20:01:59.000000 python-ctags3-1.5.0/src/examples/example.py
--rw-r--r--   0 j          (501) staff       (20)    49524 2017-04-27 16:36:28.000000 python-ctags3-1.5.0/src/examples/tags
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.695511 python-ctags3-1.5.0/src/include/
--rw-r--r--   0 j          (501) staff       (20)     8300 2020-09-05 20:07:16.000000 python-ctags3-1.5.0/src/include/readtags.h
--rw-r--r--   0 j          (501) staff       (20)    18274 2020-09-05 20:07:16.000000 python-ctags3-1.5.0/src/readtags.c
-drwxr-xr-x   0 j          (501) staff       (20)        0 2020-09-05 20:07:25.697510 python-ctags3-1.5.0/tests/
--rw-r--r--   0 j          (501) staff       (20)        0 2017-04-27 16:36:28.000000 python-ctags3-1.5.0/tests/__init__.py
--rw-r--r--   0 j          (501) staff       (20)     1556 2020-09-05 19:52:21.000000 python-ctags3-1.5.0/tests/test_ctags.py
--rw-r--r--   0 j          (501) staff       (20)      109 2020-09-05 19:52:14.000000 python-ctags3-1.5.0/tests/test_import.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.144115 python-ctags3-1.6.0/
+-rw-r--r--   0 j          (501) wheel        (0)      148 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/MANIFEST.in
+-rw-r--r--   0 j          (501) wheel        (0)     1576 2023-06-03 15:00:57.143995 python-ctags3-1.6.0/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     3521 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/README.md
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.141758 python-ctags3-1.6.0/python_ctags3.egg-info/
+-rw-r--r--   0 j          (501) wheel        (0)     1576 2023-06-03 15:00:57.000000 python-ctags3-1.6.0/python_ctags3.egg-info/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)      355 2023-06-03 15:00:57.000000 python-ctags3-1.6.0/python_ctags3.egg-info/SOURCES.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2023-06-03 15:00:57.000000 python-ctags3-1.6.0/python_ctags3.egg-info/dependency_links.txt
+-rw-r--r--   0 j          (501) wheel        (0)       16 2023-06-03 15:00:57.000000 python-ctags3-1.6.0/python_ctags3.egg-info/top_level.txt
+-rw-r--r--   0 j          (501) wheel        (0)       38 2023-06-03 15:00:57.144145 python-ctags3-1.6.0/setup.cfg
+-rw-r--r--   0 j          (501) wheel        (0)     2025 2023-06-03 15:00:14.000000 python-ctags3-1.6.0/setup.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.142603 python-ctags3-1.6.0/src/
+-rw-r--r--   0 j          (501) wheel        (0)   318403 2023-06-03 13:39:22.000000 python-ctags3-1.6.0/src/_readtags.c
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.142918 python-ctags3-1.6.0/src/ctags/
+-rw-r--r--   0 j          (501) wheel        (0)      985 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/src/ctags/__init__.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.143274 python-ctags3-1.6.0/src/examples/
+-rw-r--r--   0 j          (501) wheel        (0)      812 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/src/examples/example.py
+-rw-r--r--   0 j          (501) wheel        (0)    49524 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/src/examples/tags
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.143449 python-ctags3-1.6.0/src/include/
+-rw-r--r--   0 j          (501) wheel        (0)    10722 2023-06-03 13:38:47.000000 python-ctags3-1.6.0/src/include/readtags.h
+-rw-r--r--   0 j          (501) wheel        (0)    30458 2023-06-03 13:38:46.000000 python-ctags3-1.6.0/src/readtags.c
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:00:57.143834 python-ctags3-1.6.0/tests/
+-rw-r--r--   0 j          (501) wheel        (0)        0 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/tests/__init__.py
+-rw-r--r--   0 j          (501) wheel        (0)     2678 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/tests/test_ctags.py
+-rw-r--r--   0 j          (501) wheel        (0)      109 2023-06-03 13:37:26.000000 python-ctags3-1.6.0/tests/test_import.py
```

### Comparing `python-ctags3-1.5.0/PKG-INFO` & `python-ctags3-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-ctags3
-Version: 1.5.0
+Version: 1.6.0
 Summary: Ctags indexing python bindings
 Home-page: https://github.com/jonashaag/python-ctags
 Author: Aaron H. K. Diep
 Author-email: ahkdiep@gmail.com
 License: LGPL
-Description: Ctags supports indexing of many modern programming languages. Python
-        is a powerful scriptable dynamic language. Using Python to access Ctags index
-        file is a natural fit in extending an application's capability to examine source
-        code.
-        
-        This project wrote a wrapper for readtags.c distributed from Universal-ctags project
-        (https://ctags.io). I have been using the package in
-        a couple of projects and it has been shown that it could easily handle hundreds
-        source files.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+
+Ctags supports indexing of many modern programming languages. Python
+is a powerful scriptable dynamic language. Using Python to access Ctags index
+file is a natural fit in extending an application's capability to examine source
+code.
+
+This project wrote a wrapper for readtags.c distributed from Universal-ctags project
+(https://ctags.io). I have been using the package in
+a couple of projects and it has been shown that it could easily handle hundreds
+source files.
```

### Comparing `python-ctags3-1.5.0/README.md` & `python-ctags3-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python-ctags3-1.5.0/python_ctags3.egg-info/PKG-INFO` & `python-ctags3-1.6.0/python_ctags3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-ctags3
-Version: 1.5.0
+Version: 1.6.0
 Summary: Ctags indexing python bindings
 Home-page: https://github.com/jonashaag/python-ctags
 Author: Aaron H. K. Diep
 Author-email: ahkdiep@gmail.com
 License: LGPL
-Description: Ctags supports indexing of many modern programming languages. Python
-        is a powerful scriptable dynamic language. Using Python to access Ctags index
-        file is a natural fit in extending an application's capability to examine source
-        code.
-        
-        This project wrote a wrapper for readtags.c distributed from Universal-ctags project
-        (https://ctags.io). I have been using the package in
-        a couple of projects and it has been shown that it could easily handle hundreds
-        source files.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+
+Ctags supports indexing of many modern programming languages. Python
+is a powerful scriptable dynamic language. Using Python to access Ctags index
+file is a natural fit in extending an application's capability to examine source
+code.
+
+This project wrote a wrapper for readtags.c distributed from Universal-ctags project
+(https://ctags.io). I have been using the package in
+a couple of projects and it has been shown that it could easily handle hundreds
+source files.
```

### Comparing `python-ctags3-1.5.0/setup.py` & `python-ctags3-1.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 from setuptools import setup, Extension
 
 doclines = __doc__.split("\n")
 
 setup(
     name='python-ctags3',
-    version='1.5.0' ,
+    version='1.6.0' ,
     description=doclines[0],
     long_description="\n".join(doclines[2:]),
     author='Aaron H. K. Diep',
     author_email='ahkdiep@gmail.com',
     license = 'LGPL',
     url='https://github.com/jonashaag/python-ctags',
     packages = ['ctags'],
@@ -37,14 +37,16 @@
         'Programming Language :: C',
         'License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Topic :: Software Development :: Libraries :: Python Modules',
         "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `python-ctags3-1.5.0/src/_readtags.c` & `python-ctags3-1.6.0/src/_readtags.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-/* Generated by Cython 0.29.21 */
+/* Generated by Cython 0.29.35 */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_21"
-#define CYTHON_HEX_VERSION 0x001D15F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -43,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -71,26 +74,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -120,18 +131,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -143,61 +203,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
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
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
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
@@ -306,17 +377,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
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
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
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
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -422,27 +552,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
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
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -538,18 +676,18 @@
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
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -566,16 +704,18 @@
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
@@ -699,14 +839,15 @@
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
@@ -969,21 +1110,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1124,26 +1273,26 @@
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
 
@@ -1206,14 +1355,31 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE sortType __Pyx_PyInt_As_sortType(PyObject *);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE short __Pyx_PyInt_As_short(PyObject *);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value);
 
 /* CIntToPy.proto */
@@ -1221,26 +1387,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_sortType(sortType value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_tagResult(tagResult value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE sortType __Pyx_PyInt_As_sortType(PyObject *);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE short __Pyx_PyInt_As_short(PyObject *);
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -1361,16 +1515,19 @@
 static PyObject *__pyx_pf_9_readtags_5CTags_4__getitem__(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_6open(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, PyObject *__pyx_v_filepath); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_8setSortType(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, sortType __pyx_v_type); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_10first(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_12find(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry, char *__pyx_v_name, int __pyx_v_options); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_14findNext(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry); /* proto */
 static PyObject *__pyx_pf_9_readtags_5CTags_16next(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry); /* proto */
-static PyObject *__pyx_pf_9_readtags_5CTags_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9_readtags_5CTags_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9_readtags_5CTags_18firstPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry); /* proto */
+static PyObject *__pyx_pf_9_readtags_5CTags_20findPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry, char *__pyx_v_name, int __pyx_v_options); /* proto */
+static PyObject *__pyx_pf_9_readtags_5CTags_22nextPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry); /* proto */
+static PyObject *__pyx_pf_9_readtags_5CTags_24__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9_readtags_5CTags_26__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_9_readtags_TagEntry(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_9_readtags_CTags(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
@@ -3458,14 +3615,15 @@
 }
 
 /* "_readtags.pyx":145
  *         return ctagsFindNext(self.file, &entry.c_entry)
  * 
  *     def next(self, TagEntry entry):             # <<<<<<<<<<<<<<
  *         return ctagsNext(self.file, &entry.c_entry)
+ * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9_readtags_5CTags_17next(PyObject *__pyx_v_self, PyObject *__pyx_v_entry); /*proto*/
 static PyObject *__pyx_pw_9_readtags_5CTags_17next(PyObject *__pyx_v_self, PyObject *__pyx_v_entry) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -3494,60 +3652,331 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next", 0);
 
   /* "_readtags.pyx":146
  * 
  *     def next(self, TagEntry entry):
  *         return ctagsNext(self.file, &entry.c_entry)             # <<<<<<<<<<<<<<
+ * 
+ *     def firstPseudoTag(self, TagEntry entry):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_tagResult(tagsNext(__pyx_v_self->file, (&__pyx_v_entry->c_entry))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "_readtags.pyx":145
  *         return ctagsFindNext(self.file, &entry.c_entry)
  * 
  *     def next(self, TagEntry entry):             # <<<<<<<<<<<<<<
  *         return ctagsNext(self.file, &entry.c_entry)
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("_readtags.CTags.next", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "_readtags.pyx":148
+ *         return ctagsNext(self.file, &entry.c_entry)
+ * 
+ *     def firstPseudoTag(self, TagEntry entry):             # <<<<<<<<<<<<<<
+ *         return ctagsFirstPseudoTag(self.file, &entry.c_entry)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9_readtags_5CTags_19firstPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_v_entry); /*proto*/
+static PyObject *__pyx_pw_9_readtags_5CTags_19firstPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_v_entry) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("firstPseudoTag (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_entry), __pyx_ptype_9_readtags_TagEntry, 1, "entry", 0))) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9_readtags_5CTags_18firstPseudoTag(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self), ((struct __pyx_obj_9_readtags_TagEntry *)__pyx_v_entry));
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9_readtags_5CTags_18firstPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("firstPseudoTag", 0);
+
+  /* "_readtags.pyx":149
+ * 
+ *     def firstPseudoTag(self, TagEntry entry):
+ *         return ctagsFirstPseudoTag(self.file, &entry.c_entry)             # <<<<<<<<<<<<<<
+ * 
+ *     def findPseudoTag(self, TagEntry entry, char* name, int options):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_tagResult(tagsFirstPseudoTag(__pyx_v_self->file, (&__pyx_v_entry->c_entry))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "_readtags.pyx":148
+ *         return ctagsNext(self.file, &entry.c_entry)
+ * 
+ *     def firstPseudoTag(self, TagEntry entry):             # <<<<<<<<<<<<<<
+ *         return ctagsFirstPseudoTag(self.file, &entry.c_entry)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("_readtags.CTags.firstPseudoTag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "_readtags.pyx":151
+ *         return ctagsFirstPseudoTag(self.file, &entry.c_entry)
+ * 
+ *     def findPseudoTag(self, TagEntry entry, char* name, int options):             # <<<<<<<<<<<<<<
+ *         return ctagsFindPseudoTag(self.file, &entry.c_entry, name, options)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9_readtags_5CTags_21findPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9_readtags_5CTags_21findPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry = 0;
+  char *__pyx_v_name;
+  int __pyx_v_options;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("findPseudoTag (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_entry,&__pyx_n_s_name,&__pyx_n_s_options,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_entry)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("findPseudoTag", 1, 3, 3, 1); __PYX_ERR(1, 151, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("findPseudoTag", 1, 3, 3, 2); __PYX_ERR(1, 151, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "findPseudoTag") < 0)) __PYX_ERR(1, 151, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v_entry = ((struct __pyx_obj_9_readtags_TagEntry *)values[0]);
+    __pyx_v_name = __Pyx_PyObject_AsWritableString(values[1]); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(1, 151, __pyx_L3_error)
+    __pyx_v_options = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_options == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 151, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("findPseudoTag", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 151, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("_readtags.CTags.findPseudoTag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_entry), __pyx_ptype_9_readtags_TagEntry, 1, "entry", 0))) __PYX_ERR(1, 151, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9_readtags_5CTags_20findPseudoTag(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self), __pyx_v_entry, __pyx_v_name, __pyx_v_options);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9_readtags_5CTags_20findPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry, char *__pyx_v_name, int __pyx_v_options) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("findPseudoTag", 0);
+
+  /* "_readtags.pyx":152
+ * 
+ *     def findPseudoTag(self, TagEntry entry, char* name, int options):
+ *         return ctagsFindPseudoTag(self.file, &entry.c_entry, name, options)             # <<<<<<<<<<<<<<
+ * 
+ *     def nextPseudoTag(self, TagEntry entry):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_tagResult(tagsFindPseudoTag(__pyx_v_self->file, (&__pyx_v_entry->c_entry), __pyx_v_name, __pyx_v_options)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "_readtags.pyx":151
+ *         return ctagsFirstPseudoTag(self.file, &entry.c_entry)
+ * 
+ *     def findPseudoTag(self, TagEntry entry, char* name, int options):             # <<<<<<<<<<<<<<
+ *         return ctagsFindPseudoTag(self.file, &entry.c_entry, name, options)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("_readtags.CTags.findPseudoTag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "_readtags.pyx":154
+ *         return ctagsFindPseudoTag(self.file, &entry.c_entry, name, options)
+ * 
+ *     def nextPseudoTag(self, TagEntry entry):             # <<<<<<<<<<<<<<
+ *         return ctagsNextPseudoTag(self.file, &entry.c_entry)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9_readtags_5CTags_23nextPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_v_entry); /*proto*/
+static PyObject *__pyx_pw_9_readtags_5CTags_23nextPseudoTag(PyObject *__pyx_v_self, PyObject *__pyx_v_entry) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("nextPseudoTag (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_entry), __pyx_ptype_9_readtags_TagEntry, 1, "entry", 0))) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9_readtags_5CTags_22nextPseudoTag(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self), ((struct __pyx_obj_9_readtags_TagEntry *)__pyx_v_entry));
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9_readtags_5CTags_22nextPseudoTag(struct __pyx_obj_9_readtags_CTags *__pyx_v_self, struct __pyx_obj_9_readtags_TagEntry *__pyx_v_entry) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("nextPseudoTag", 0);
+
+  /* "_readtags.pyx":155
+ * 
+ *     def nextPseudoTag(self, TagEntry entry):
+ *         return ctagsNextPseudoTag(self.file, &entry.c_entry)             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_tagResult(tagsNextPseudoTag(__pyx_v_self->file, (&__pyx_v_entry->c_entry))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "_readtags.pyx":154
+ *         return ctagsFindPseudoTag(self.file, &entry.c_entry, name, options)
+ * 
+ *     def nextPseudoTag(self, TagEntry entry):             # <<<<<<<<<<<<<<
+ *         return ctagsNextPseudoTag(self.file, &entry.c_entry)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("_readtags.CTags.nextPseudoTag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9_readtags_5CTags_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9_readtags_5CTags_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9_readtags_5CTags_25__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9_readtags_5CTags_25__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9_readtags_5CTags_18__reduce_cython__(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9_readtags_5CTags_24__reduce_cython__(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9_readtags_5CTags_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self) {
+static PyObject *__pyx_pf_9_readtags_5CTags_24__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -3584,27 +4013,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9_readtags_5CTags_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9_readtags_5CTags_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9_readtags_5CTags_27__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9_readtags_5CTags_27__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9_readtags_5CTags_20__setstate_cython__(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9_readtags_5CTags_26__setstate_cython__(((struct __pyx_obj_9_readtags_CTags *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9_readtags_5CTags_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9_readtags_5CTags_26__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9_readtags_CTags *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -3761,20 +4190,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyObject *__pyx_tp_new_9_readtags_CTags(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
@@ -3815,16 +4247,19 @@
 static PyMethodDef __pyx_methods_9_readtags_CTags[] = {
   {"open", (PyCFunction)__pyx_pw_9_readtags_5CTags_7open, METH_O, 0},
   {"setSortType", (PyCFunction)__pyx_pw_9_readtags_5CTags_9setSortType, METH_O, 0},
   {"first", (PyCFunction)__pyx_pw_9_readtags_5CTags_11first, METH_O, 0},
   {"find", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9_readtags_5CTags_13find, METH_VARARGS|METH_KEYWORDS, 0},
   {"findNext", (PyCFunction)__pyx_pw_9_readtags_5CTags_15findNext, METH_O, 0},
   {"next", (PyCFunction)__pyx_pw_9_readtags_5CTags_17next, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9_readtags_5CTags_19__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9_readtags_5CTags_21__setstate_cython__, METH_O, 0},
+  {"firstPseudoTag", (PyCFunction)__pyx_pw_9_readtags_5CTags_19firstPseudoTag, METH_O, 0},
+  {"findPseudoTag", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9_readtags_5CTags_21findPseudoTag, METH_VARARGS|METH_KEYWORDS, 0},
+  {"nextPseudoTag", (PyCFunction)__pyx_pw_9_readtags_5CTags_23nextPseudoTag, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9_readtags_5CTags_25__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9_readtags_5CTags_27__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PySequenceMethods __pyx_tp_as_sequence_CTags = {
   0, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
@@ -3900,20 +4335,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -4062,15 +4500,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -4303,19 +4741,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_readtags", __pyx_methods, __pyx_k_Id_This_file_is_part_of_Python, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -4326,15 +4762,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main__readtags) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -4538,15 +4974,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -4825,15 +5261,15 @@
 #endif
 #endif
 
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
@@ -4869,15 +5305,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -4928,15 +5364,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -5077,18 +5513,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
@@ -5425,28 +5859,28 @@
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
@@ -5791,25 +6225,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -5846,14 +6298,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -5922,15 +6376,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -5952,15 +6406,15 @@
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
@@ -6046,41 +6500,48 @@
     Py_INCREF(code_object);
 }
 
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
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -6091,34 +6552,49 @@
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
@@ -6149,172 +6625,24 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
-    const unsigned long neg_one = (unsigned long) ((unsigned long) 0 - (unsigned long) 1), const_zero = (unsigned long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned long),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
-    const short neg_one = (short) ((short) 0 - (short) 1), const_zero = (short) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(short) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(short) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(short) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(short) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(short) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(short),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_sortType(sortType value) {
-    const sortType neg_one = (sortType) ((sortType) 0 - (sortType) 1), const_zero = (sortType) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(sortType) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(sortType) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(sortType) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(sortType) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(sortType) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(sortType),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_tagResult(tagResult value) {
-    const tagResult neg_one = (tagResult) ((tagResult) 0 - (tagResult) 1), const_zero = (tagResult) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(tagResult) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(tagResult) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(tagResult) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(tagResult) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(tagResult) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(tagResult),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE sortType __Pyx_PyInt_As_sortType(PyObject *x) {
-    const sortType neg_one = (sortType) ((sortType) 0 - (sortType) 1), const_zero = (sortType) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const sortType neg_one = (sortType) -1, const_zero = (sortType) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(sortType) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(sortType, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -6357,15 +6685,15 @@
                         } else if (8 * sizeof(sortType) >= 4 * PyLong_SHIFT) {
                             return (sortType) (((((((((sortType)digits[3]) << PyLong_SHIFT) | (sortType)digits[2]) << PyLong_SHIFT) | (sortType)digits[1]) << PyLong_SHIFT) | (sortType)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6495,15 +6823,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to sortType");
     return (sortType) -1;
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
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -6546,15 +6881,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6684,15 +7019,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *x) {
-    const unsigned long neg_one = (unsigned long) ((unsigned long) 0 - (unsigned long) 1), const_zero = (unsigned long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const unsigned long neg_one = (unsigned long) -1, const_zero = (unsigned long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(unsigned long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(unsigned long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -6735,15 +7077,15 @@
                         } else if (8 * sizeof(unsigned long) >= 4 * PyLong_SHIFT) {
                             return (unsigned long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6873,15 +7215,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned long");
     return (unsigned long) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE short __Pyx_PyInt_As_short(PyObject *x) {
-    const short neg_one = (short) ((short) 0 - (short) 1), const_zero = (short) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const short neg_one = (short) -1, const_zero = (short) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(short) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(short, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -6924,15 +7273,15 @@
                         } else if (8 * sizeof(short) >= 4 * PyLong_SHIFT) {
                             return (short) (((((((((short)digits[3]) << PyLong_SHIFT) | (short)digits[2]) << PyLong_SHIFT) | (short)digits[1]) << PyLong_SHIFT) | (short)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7061,16 +7410,213 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to short");
     return (short) -1;
 }
 
 /* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const unsigned long neg_one = (unsigned long) -1, const_zero = (unsigned long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(unsigned long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(unsigned long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(unsigned long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(unsigned long),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const short neg_one = (short) -1, const_zero = (short) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(short) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(short) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(short) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(short) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(short) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(short),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_sortType(sortType value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const sortType neg_one = (sortType) -1, const_zero = (sortType) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(sortType) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(sortType) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(sortType) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(sortType) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(sortType) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(sortType),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_tagResult(tagResult value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const tagResult neg_one = (tagResult) -1, const_zero = (tagResult) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(tagResult) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(tagResult) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(tagResult) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(tagResult) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(tagResult) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(tagResult),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
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
@@ -7093,15 +7639,22 @@
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
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
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -7144,15 +7697,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7382,19 +7935,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
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
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -7644,14 +8219,31 @@
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
```

### Comparing `python-ctags3-1.5.0/src/ctags/__init__.py` & `python-ctags3-1.6.0/src/ctags/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ctags3-1.5.0/src/examples/example.py` & `python-ctags3-1.6.0/src/examples/example.py`

 * *Files identical despite different names*

### Comparing `python-ctags3-1.5.0/src/examples/tags` & `python-ctags3-1.6.0/src/examples/tags`

 * *Files identical despite different names*

### Comparing `python-ctags3-1.5.0/src/include/readtags.h` & `python-ctags3-1.6.0/src/include/readtags.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 /*
-*   $Id$
-*
 *   Copyright (c) 1996-2003, Darren Hiebert
 *
 *   This source code is released for the public domain.
 *
 *   This file defines the public interface for looking up tag entries in tag
 *   files.
 *
 *   The functions defined in this interface are intended to provide tag file
 *   support to a software tool. The tag lookups provided are sufficiently fast
 *   enough to permit opening a sorted tag file, searching for a matching tag,
 *   then closing the tag file each time a tag is looked up (search times are
-*   on the order of hundreths of a second, even for huge tag files). This is
+*   on the order of hundredths of a second, even for huge tag files). This is
 *   the recommended use of this library for most tool applications. Adhering
 *   to this approach permits a user to regenerate a tag file at will without
 *   the tool needing to detect and resynchronize with changes to the tag file.
 *   Even for an unsorted 24MB tag file, tag searches take about one second.
 */
 #ifndef READTAGS_H
 #define READTAGS_H
@@ -28,51 +26,69 @@
 /*
 *  MACROS
 */
 
 /* Options for tagsSetSortType() */
 typedef enum {
 	TAG_UNSORTED, TAG_SORTED, TAG_FOLDSORTED
-} sortType ;
+} tagSortType ;
+
+/* For source code level compatibility, sortType is defined here.
+*  Define TAG_NO_COMPAT_SORT_TYPE if you want to avoid namespace pollution.
+*/
+#ifndef TAG_NO_COMPAT_SORT_TYPE
+#define sortType tagSortType
+#endif
 
-/* Options for tagsFind() */
+/* Options for tagsFind() and tagsFindPseudoTag() */
 #define TAG_FULLMATCH     0x0
 #define TAG_PARTIALMATCH  0x1
 
 #define TAG_OBSERVECASE   0x0
 #define TAG_IGNORECASE    0x2
 
 /*
 *  DATA DECLARATIONS
 */
 
 typedef enum { TagFailure = 0, TagSuccess = 1 } tagResult;
 
+typedef enum {
+	TagErrnoUnexpectedSortedMethod = -1, /* Unexpected sorted method */
+	TagErrnoUnexpectedFormat       = -2, /* Unexpected format number */
+	TagErrnoUnexpectedLineno       = -3, /* Unexpected value for line: field
+										  * (Zero or a positive integer is expected.) */
+	TagErrnoInvalidArgument        = -4, /* Unexpected argument passed to the API
+										  * function */
+	TagErrnoFileMaybeTooBig        = -5, /* Maybe the tags file is too big */
+} tagErrno;
+
 struct sTagFile;
 
 typedef struct sTagFile tagFile;
 
 /* This structure contains information about the tag file. */
 typedef struct {
 
 	struct {
 			/* was the tag file successfully opened? */
 		int opened;
 
-			/* errno value when 'opened' is false */
+			/* errno value or tagErrno typed value
+			   when 'opened' is false */
 		int error_number;
 	} status;
 
 		/* information about the structure of the tag file */
 	struct {
 				/* format of tag file (1 = original, 2 = extended) */
 			short format;
 
 				/* how is the tag file sorted? */
-			sortType sort;
+			tagSortType sort;
 	} file;
 
 
 		/* information about the program which created this tag file */
 	struct {
 			/* name of author of generating program (may be null) */
 		const char *author;
@@ -104,15 +120,16 @@
 
 /* This structure contains information about a specific tag. */
 typedef struct {
 
 		/* name of tag */
 	const char *name;
 
-		/* path of source file containing definition of tag */
+		/* path of source file containing definition of tag.
+		   For a broken tags file, this can be NULL. */
 	const char *file;
 
 		/* address for locating tag in source file */
 	struct {
 			/* pattern for locating source line
 			 * (may be NULL if not present) */
 		const char *pattern;
@@ -146,18 +163,22 @@
 
 /*
 *  This function must be called before calling other functions in this
 *  library. It is passed the path to the tag file to read and a (possibly
 *  null) pointer to a structure which, if not null, will be populated with
 *  information about the tag file. If successful, the function will return a
 *  handle which must be supplied to other calls to read information from the
-*  tag file, and info.status.opened will be set to true. If unsuccessful,
-*  info.status.opened will be set to false and info.status.error_number will
-*  be set to the errno value representing the system error preventing the tag
-*  file from being successfully opened.
+*  tag file, and info.status.opened will be set to true.
+*  If unsuccessful, the function will return NULL, and
+*  info.status.opened will be set to false and
+*  info.status.error_number will be set to either the errno value
+*  representing the system error preventing the tag file from being
+*  successfully opened, or the tagErrno typed value representing the
+*  library level error. The error_number will be ENOMEM if the memory
+*  allocation for the handle is failed.
 */
 extern tagFile *tagsOpen (const char *const filePath, tagFileInfo *const info);
 
 /*
 *  This function allows the client to override the normal automatic detection
 *  of how a tag file is sorted. Permissible values for `type' are
 *  TAG_UNSORTED, TAG_SORTED, TAG_FOLDSORTED. Tag files in the new extended
@@ -166,15 +187,15 @@
 *  sorted, preventing this library from taking advantage of fast binary
 *  lookups. If the client knows that such an unmarked tag file is indeed
 *  sorted (or not), it can override the automatic detection. Note that
 *  incorrect lookup results will result if a tag file is marked as sorted when
 *  it actually is not. The function will return TagSuccess if called on an
 *  open tag file or TagFailure if not.
 */
-extern tagResult tagsSetSortType (tagFile *const file, const sortType type);
+extern tagResult tagsSetSortType (tagFile *const file, const tagSortType type);
 
 /*
 *  Reads the first tag in the file, if any. It is passed the handle to an
 *  opened tag file and a (possibly null) pointer to a structure which, if not
 *  null, will be populated with information about the first tag file entry.
 *  The function will return TagSuccess another tag entry is found, or
 *  TagFailure if not (i.e. it reached end of file).
@@ -211,19 +232,19 @@
 *    TAG_PARTIALMATCH
 *        Tags whose leading characters match `name' will qualify.
 *
 *    TAG_FULLMATCH
 *        Only tags whose full lengths match `name' will qualify.
 *
 *    TAG_IGNORECASE
-*        Matching will be performed in a case-insenstive manner. Note that
+*        Matching will be performed in a case-insensitive manner. Note that
 *        this disables binary searches of the tag file.
 *
 *    TAG_OBSERVECASE
-*        Matching will be performed in a case-senstive manner. Note that
+*        Matching will be performed in a case-sensitive manner. Note that
 *        this enables binary searches of the tag file.
 *
 *  The function will return TagSuccess if a tag matching the name is found, or
 *  TagFailure if not.
 */
 extern tagResult tagsFind (tagFile *const file, tagEntry *const entry, const char *const name, const int options);
 
@@ -233,20 +254,58 @@
 *  `entry' will be populated with information about the tag file entry. The
 *  function will return TagSuccess if another tag matching the name is found,
 *  or TagFailure if not.
 */
 extern tagResult tagsFindNext (tagFile *const file, tagEntry *const entry);
 
 /*
-*  Call tagsTerminate() at completion of reading the tag file, which will
+*  Does the same as tagsFirst(), but is specialized to pseudo tags.
+*  If tagFileInfo doesn't contain pseudo tags you are interested in, read
+*  them sequentially with this function and tagsNextPseudoTag().
+*/
+extern tagResult tagsFirstPseudoTag (tagFile *const file, tagEntry *const entry);
+
+/*
+*  Does the same as tagsNext(), but is specialized to pseudo tags. Use with
+*  tagsFirstPseudoTag().
+*/
+extern tagResult tagsNextPseudoTag (tagFile *const file, tagEntry *const entry);
+
+/*
+* Does the same as tagsFind(), but is specialized to pseudo tags.
+* The available values for `match' are:
+*
+*    TAG_PARTIALMATCH
+*        Tags whose leading characters match `name' will qualify.
+*
+*    TAG_FULLMATCH
+*        Only tags whose full lengths match `name' will qualify.
+*
+* NOTE: unlike tagsFind(), this function uses liner-searching even if
+* the tags file is sorted.
+*/
+extern tagResult tagsFindPseudoTag (tagFile *const file, tagEntry *const entry, const char *const name, const int match);
+
+/*
+*  Call tagsClose() at completion of reading the tag file, which will
 *  close the file and free any internal memory allocated. The function will
-*  return TagFailure is no file is currently open, TagSuccess otherwise.
+*  return TagFailure if no file is currently open, TagSuccess otherwise.
 */
 extern tagResult tagsClose (tagFile *const file);
 
+/*
+*  Get the error status set in the last API call.
+*  Much of the API functions return TagFailure because (1) no tag is
+*  found, or (2) an error occurs. tagsGetErrno() is for distinguishing
+*  (1) or (2). This function will return 0 for (1). The errno value
+*  representing the system error or tagErrno value for (2).
+*
+*  This function does not deal with the results of tagsOpen(),
+*  tagsClose(), and tagsField().
+*/
+extern int tagsGetErrno (tagFile *const file);
+
 #ifdef __cplusplus
 };
 #endif
 
 #endif
-
-/* vi:set tabstop=4 shiftwidth=4: */
```

### Comparing `python-ctags3-1.5.0/tests/test_ctags.py` & `python-ctags3-1.6.0/tests/test_ctags.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,12 +41,52 @@
                 b"/^static tagResult find (tagFile "
                 b"*const file, tagEntry *const entry,$/",
                 b"function",
                 b"C",
             ],
         )
 
+    def test_ptag_find(self):
+        entry = ctags.TagEntry()
+        self.ctags.findPseudoTag(entry, b"!_TAG_PROGRAM_URL", ctags.TAG_FULLMATCH)
+        entry_info = [
+            entry[_] for _ in ("file", "name", "pattern")
+        ]
+        self.assertEqual(
+            entry_info,
+            [
+                b"http://ctags.sourceforge.net",
+                b"!_TAG_PROGRAM_URL",
+                b"/official site/",
+            ],
+        )
+
+        self.ctags.nextPseudoTag(entry)
+        entry_info = [
+            entry[_] for _ in ("file", "name", "pattern")
+        ]
+        self.assertEqual(
+            entry_info,
+            [
+                b"5.6b1",
+                b"!_TAG_PROGRAM_VERSION",
+                b"//",
+            ],
+        )
+
+        self.ctags.firstPseudoTag(entry)
+        entry_info = [
+            entry[_] for _ in ("file", "name", "pattern")
+        ]
+        self.assertEqual(
+            entry_info,
+            [
+                b"2",
+                b"!_TAG_FILE_FORMAT",
+                b"/extended format; --format=1 will not append ;\" to lines/",
+            ],
+        )
 
 class TestCTagsParseBytes(TestCTagsParse):
     def setUp(self):
         file_path = os.path.join(src_dir, "examples", "tags")
         self.ctags = ctags.CTags(file_path.encode(sys.getfilesystemencoding()))
```

