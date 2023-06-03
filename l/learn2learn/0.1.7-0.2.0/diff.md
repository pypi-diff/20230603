# Comparing `tmp/learn2learn-0.1.7.tar.gz` & `tmp/learn2learn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/learn2learn-0.1.7.tar", last modified: Thu Feb 10 03:33:40 2022, max compression
+gzip compressed data, was "learn2learn-0.2.0.tar", last modified: Sat Jun  3 21:18:23 2023, max compression
```

## Comparing `learn2learn-0.1.7.tar` & `learn2learn-0.2.0.tar`

### file list

```diff
@@ -1,548 +1,684 @@
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3321 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Code.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2918 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/FlowControl.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2468 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/ParseTreeTransforms.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8903 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Parsing.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2113 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Scanning.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1792 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Visitor.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/Tests/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       71 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/Tests/cfuncs.c
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       61 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       66 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_bool.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_buffer.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       67 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_bytes.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_cobject.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_complex.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       66 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_dict.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_exc.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       67 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_float.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       70 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_function.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_getargs.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       70 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_instance.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_int.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       70 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_iterator.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       66 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_list.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       66 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_long.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_mapping.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_mem.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_method.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_module.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_number.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_object.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       71 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_oldbuffer.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       71 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_pycapsule.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_ref.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       70 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_sequence.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_set.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       68 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_string.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       67 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_tuple.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       66 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_type.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_unicode.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_version.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       69 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_weakref.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       64 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stdio.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stdlib.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2187 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stl.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8254 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/__init__.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6034 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/array.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1359 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bool.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4831 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/buffer.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1443 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytearray.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     9906 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytes.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      236 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ceval.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1524 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/cobject.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1777 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/complex.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6779 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/datetime.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6877 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/dict.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    13606 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/exc.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1424 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/float.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2671 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/function.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      775 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/getargs.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      985 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/instance.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4131 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/int.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1319 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/iterator.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4084 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/list.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     7051 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/long.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      445 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/longintrepr.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2693 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mapping.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5386 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mem.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2504 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/memoryview.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2196 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/method.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     9226 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/module.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    11315 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/number.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    18366 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/object.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2916 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/oldbuffer.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5721 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pycapsule.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1985 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pylifecycle.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3683 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pystate.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1946 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pythread.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2557 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ref.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6008 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/sequence.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5383 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/set.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2113 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/slice.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     9944 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/string.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3206 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/tuple.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1831 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/type.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    25841 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/unicode.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      847 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/version.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1984 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/weakref.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       13 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/__init__.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2050 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/errno.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      966 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/float.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      621 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/limits.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1140 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/locale.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2796 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/math.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      297 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/setjmp.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1170 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/signal.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      164 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stddef.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3449 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdint.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2476 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdio.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2444 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdlib.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2038 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/string.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1317 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/time.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       94 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/__init__.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1770 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/algorithm.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      501 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/cast.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3012 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/complex.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3106 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/deque.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2392 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/forward_list.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      381 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/functional.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1432 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/iterator.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1661 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/limits.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2658 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/list.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2551 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/map.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3600 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/memory.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       27 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/pair.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      649 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/queue.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2170 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/set.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      292 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/stack.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5071 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/string.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      524 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeindex.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      304 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeinfo.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2838 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_map.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2622 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_set.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      485 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/utility.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3350 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/vector.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    38092 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/__init__.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5807 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/math.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1713 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/openmp.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       13 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/__init__.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      355 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/dlfcn.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1175 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/fcntl.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       99 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/ioctl.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3362 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/mman.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1254 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/resource.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      546 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/select.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1876 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/signal.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1734 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stat.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1054 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdio.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      934 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdlib.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      374 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/strings.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1980 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/time.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1162 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/types.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8061 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/unistd.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1244 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/wait.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      585 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Actions.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1481 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Scanners.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6279 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/refnanny.pyx
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    40051 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/AsyncGen.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    29541 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Buffer.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    16589 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Builtins.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4338 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CConvert.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2566 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CMath.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      505 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Capsule.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2558 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CommonStructures.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    10043 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Complex.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    86539 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Coroutine.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1893 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CpdefEnums.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6098 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CppConvert.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    43920 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CythonFunction.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6675 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Embed.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    26361 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Exceptions.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8591 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ExtensionTypes.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    12026 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/FunctionArguments.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    22105 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ImportExport.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    49610 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    28907 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView_C.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    50383 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ModuleSetupCode.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    87240 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ObjectHandling.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    45132 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Optimize.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    12358 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Overflow.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5103 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Printing.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    16749 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Profile.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    41010 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/StringTools.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      152 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCyUtilityLoader.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1595 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCythonScope.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      279 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestUtilityLoader.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    35453 2020-03-02 00:59:17.000000 learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TypeConversion.c
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3321 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Code.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2918 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/FlowControl.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2468 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     8984 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Parsing.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2113 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Scanning.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1792 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Visitor.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/Tests/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       71 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/Tests/cfuncs.c
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       61 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       66 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_bool.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_buffer.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       67 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_bytes.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_cobject.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_complex.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       66 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_dict.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_exc.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       67 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_float.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       70 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_function.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_getargs.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       70 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_instance.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_int.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       70 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_iterator.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       66 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_list.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       66 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_long.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_mapping.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_mem.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_method.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_module.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_number.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_object.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       71 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_oldbuffer.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       71 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_pycapsule.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_ref.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       70 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_sequence.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_set.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       68 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_string.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       67 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_tuple.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       66 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_type.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_unicode.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_version.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       69 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_weakref.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       64 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stdio.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       65 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stdlib.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2187 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stl.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     8254 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/__init__.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6056 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/array.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1359 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bool.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4870 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/buffer.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1443 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytearray.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     9906 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytes.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1390 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cellobject.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      236 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ceval.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1524 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cobject.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5084 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/codecs.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1777 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/complex.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1696 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/conversion.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6776 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/datetime.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6877 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/dict.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    13606 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/exc.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1424 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/float.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2671 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/function.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1052 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/genobject.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      775 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/getargs.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      985 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/instance.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4131 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/int.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1319 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterator.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1036 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterobject.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4084 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/list.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     7051 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/long.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      445 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/longintrepr.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2693 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mapping.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5386 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mem.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2504 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/memoryview.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2196 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/method.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     9226 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/module.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    11922 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/number.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    18366 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/object.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2916 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5692 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2000 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3683 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pystate.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1946 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pythread.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2557 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ref.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6008 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/sequence.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5383 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/set.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3111 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/slice.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     9944 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/string.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3206 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/tuple.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1831 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/type.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    26247 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/unicode.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      847 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/version.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1984 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/weakref.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       13 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/__init__.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2050 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/errno.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      966 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/float.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      621 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/limits.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1140 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/locale.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2948 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/math.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      297 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/setjmp.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1170 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/signal.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      164 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stddef.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3449 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdint.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2476 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdio.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2444 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdlib.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2038 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/string.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1317 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/time.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       94 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/__init__.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1770 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      501 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/cast.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3012 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/complex.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3106 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/deque.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2392 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      381 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/functional.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1432 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/iterator.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1661 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/limits.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2658 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/list.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2551 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/map.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3600 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/memory.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       27 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/pair.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      649 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/queue.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2170 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/set.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      292 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/stack.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     8731 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/string.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      524 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      304 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeinfo.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2867 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2622 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      903 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/utility.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3350 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/vector.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    38138 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/__init__.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5807 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/math.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1713 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/openmp.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       13 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/__init__.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      355 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/dlfcn.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1194 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/fcntl.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       99 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/ioctl.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3362 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/mman.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1254 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/resource.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      546 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/select.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1876 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/signal.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1734 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stat.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1054 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdio.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      934 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdlib.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      374 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/strings.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1980 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/time.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1162 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/types.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     8061 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/unistd.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1244 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/wait.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      585 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Actions.pxd
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1481 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Scanners.pxd
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6279 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/refnanny.pyx
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    40051 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/AsyncGen.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    29654 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Buffer.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    16783 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Builtins.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4338 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CConvert.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2566 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CMath.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      505 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Capsule.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2558 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CommonStructures.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    10043 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Complex.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    88160 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Coroutine.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1893 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CpdefEnums.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6098 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CppConvert.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    45595 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CythonFunction.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6854 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Embed.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    26379 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Exceptions.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    10831 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ExtensionTypes.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    12040 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/FunctionArguments.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    22279 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ImportExport.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    49621 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    29243 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView_C.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    51626 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ModuleSetupCode.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    88574 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ObjectHandling.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    45184 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Optimize.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    12358 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Overflow.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5103 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Printing.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    17169 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Profile.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    42181 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/StringTools.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      152 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCyUtilityLoader.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1595 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCythonScope.pyx
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      279 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestUtilityLoader.c
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    36001 2021-11-07 00:52:51.000000 learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TypeConversion.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1120 2019-11-07 17:27:04.000000 learn2learn-0.1.7/LICENSE
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       86 2020-05-19 02:44:30.000000 learn2learn-0.1.7/MANIFEST.in
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    10558 2022-02-10 03:33:40.000000 learn2learn-0.1.7/PKG-INFO
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8586 2021-11-06 23:35:40.000000 learn2learn-0.1.7/README.md
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      218 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       22 2022-02-10 03:26:47.000000 learn2learn-0.1.7/learn2learn/_version.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/algorithms/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      363 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/algorithms/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      483 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/algorithms/base_learner.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     7345 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/algorithms/gbml.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      394 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6176 2021-08-22 19:36:05.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_anil.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4219 2021-11-07 05:30:39.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_episodic_module.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5885 2021-08-22 19:36:05.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_maml.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5088 2021-08-22 19:36:05.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_metaoptnet.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5931 2021-08-22 19:36:05.000000 learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_protonet.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     7479 2022-01-14 00:35:09.000000 learn2learn-0.1.7/learn2learn/algorithms/maml.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4918 2022-02-10 03:24:17.000000 learn2learn-0.1.7/learn2learn/algorithms/meta_sgd.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/data/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      334 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/data/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)   420260 2021-11-07 00:53:40.000000 learn2learn-0.1.7/learn2learn/data/meta_dataset.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8697 2020-10-21 22:02:56.000000 learn2learn-0.1.7/learn2learn/data/meta_dataset.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)   424769 2021-10-30 07:08:58.000000 learn2learn-0.1.7/learn2learn/data/task_dataset.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      121 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/data/task_dataset.pxd
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5851 2020-06-14 23:34:44.000000 learn2learn-0.1.7/learn2learn/data/task_dataset.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)  1423642 2022-01-21 21:52:56.000000 learn2learn-0.1.7/learn2learn/data/transforms.c
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    13195 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/data/transforms.pyx
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6870 2021-11-06 23:38:27.000000 learn2learn-0.1.7/learn2learn/data/utils.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/gym/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2748 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/README.md
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      221 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/gym/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1526 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/async_vec_env.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/gym/envs/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1174 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/envs/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2117 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/envs/meta_env.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/gym/envs/metaworld/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       90 2020-06-20 17:57:33.000000 learn2learn-0.1.7/learn2learn/gym/envs/metaworld/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6351 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/gym/envs/metaworld/metaworld.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      354 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4641 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/ant_direction.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4578 2021-11-06 23:35:40.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/ant_forward_backward.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1083 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/dummy_mujoco_env.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4290 2022-02-08 22:05:03.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/halfcheetah_forward_backward.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5042 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/humanoid_direction.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4858 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/gym/envs/mujoco/humanoid_forward_backward.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/gym/envs/particles/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       65 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/envs/particles/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3070 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/envs/particles/particles_2d.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3788 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/gym/envs/subproc_vec_env.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/nn/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      227 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/nn/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6493 2021-02-19 01:16:38.000000 learn2learn-0.1.7/learn2learn/nn/kroneckers.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6290 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/nn/metaoptnet.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2061 2021-11-07 05:30:44.000000 learn2learn-0.1.7/learn2learn/nn/misc.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5337 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/nn/protonet.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/optim/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      253 2020-08-30 16:45:28.000000 learn2learn-0.1.7/learn2learn/optim/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3956 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/learnable_optimizer.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4849 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/parameter_update.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/optim/transforms/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      512 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/transforms/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2574 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/transforms/kronecker_transform.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3176 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/transforms/metacurvature_transform.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2145 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/transforms/module_transform.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      880 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/transforms/transform_dictionary.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/optim/update_rules/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       74 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/update_rules/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1640 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/optim/update_rules/differentiable_sgd.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/text/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       47 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/text/__init__.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/text/datasets/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       76 2019-11-07 17:27:04.000000 learn2learn-0.1.7/learn2learn/text/datasets/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2754 2021-02-19 05:01:32.000000 learn2learn-0.1.7/learn2learn/text/datasets/news_classification.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/utils/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    12339 2022-02-10 03:24:17.000000 learn2learn-0.1.7/learn2learn/utils/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2105 2021-01-04 19:14:00.000000 learn2learn-0.1.7/learn2learn/utils/lightning.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/vision/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      194 2020-07-26 18:29:23.000000 learn2learn-0.1.7/learn2learn/vision/__init__.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4493 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2597 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/cifarfs_benchmark.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2568 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/fc100_benchmark.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     3567 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/mini_imagenet_benchmark.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     2587 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/omniglot_benchmark.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     4010 2021-09-03 05:52:09.000000 learn2learn-0.1.7/learn2learn/vision/benchmarks/tiered_imagenet_benchmark.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/vision/datasets/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      523 2020-09-15 02:53:55.000000 learn2learn-0.1.7/learn2learn/vision/datasets/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4501 2020-06-20 17:57:33.000000 learn2learn-0.1.7/learn2learn/vision/datasets/cifarfs.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    15746 2021-11-06 23:35:40.000000 learn2learn-0.1.7/learn2learn/vision/datasets/cu_birds200.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5313 2020-09-02 22:10:21.000000 learn2learn-0.1.7/learn2learn/vision/datasets/describable_textures.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4520 2020-10-21 16:24:44.000000 learn2learn-0.1.7/learn2learn/vision/datasets/fc100.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    10191 2021-11-06 23:35:40.000000 learn2learn-0.1.7/learn2learn/vision/datasets/fgvc_aircraft.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    58192 2020-09-15 02:53:55.000000 learn2learn-0.1.7/learn2learn/vision/datasets/fgvc_fungi.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3162 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/vision/datasets/full_omniglot.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5052 2021-11-09 19:52:43.000000 learn2learn-0.1.7/learn2learn/vision/datasets/mini_imagenet.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    13024 2020-09-14 22:04:49.000000 learn2learn-0.1.7/learn2learn/vision/datasets/quickdraw.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4680 2020-05-19 02:44:30.000000 learn2learn-0.1.7/learn2learn/vision/datasets/tiered_imagenet.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5299 2020-09-02 22:10:21.000000 learn2learn-0.1.7/learn2learn/vision/datasets/vgg_flowers.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn/vision/models/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4010 2021-11-07 05:30:44.000000 learn2learn-0.1.7/learn2learn/vision/models/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     9420 2021-11-07 05:30:39.000000 learn2learn-0.1.7/learn2learn/vision/models/cnn4.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    11364 2021-11-06 23:35:40.000000 learn2learn-0.1.7/learn2learn/vision/models/resnet12.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4950 2021-08-22 19:36:05.000000 learn2learn-0.1.7/learn2learn/vision/models/wrn28.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1556 2022-02-09 01:28:15.000000 learn2learn-0.1.7/learn2learn/vision/transforms.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn.egg-info/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    10558 2022-02-10 03:33:37.000000 learn2learn-0.1.7/learn2learn.egg-info/PKG-INFO
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    31989 2022-02-10 03:33:40.000000 learn2learn-0.1.7/learn2learn.egg-info/SOURCES.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        1 2022-02-10 03:33:37.000000 learn2learn-0.1.7/learn2learn.egg-info/dependency_links.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        1 2020-03-02 01:55:53.000000 learn2learn-0.1.7/learn2learn.egg-info/not-zip-safe
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)       98 2022-02-10 03:33:37.000000 learn2learn-0.1.7/learn2learn.egg-info/requires.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       18 2022-02-10 03:33:37.000000 learn2learn-0.1.7/learn2learn.egg-info/top_level.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       38 2022-02-10 03:33:40.000000 learn2learn-0.1.7/setup.cfg
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2615 2021-11-06 23:35:40.000000 learn2learn-0.1.7/setup.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       23 2019-11-07 17:27:04.000000 learn2learn-0.1.7/tests/__init__.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/integration/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        0 2019-11-07 17:27:04.000000 learn2learn-0.1.7/tests/integration/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     7831 2020-08-25 22:18:33.000000 learn2learn-0.1.7/tests/integration/maml_miniimagenet_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8588 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/integration/maml_omniglot_test.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     8135 2020-07-26 18:29:23.000000 learn2learn-0.1.7/tests/integration/protonets_miniimagenet_test_notravis.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/unit/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        0 2019-11-07 17:27:04.000000 learn2learn-0.1.7/tests/unit/__init__.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/unit/algorithms/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        0 2019-11-07 17:27:04.000000 learn2learn-0.1.7/tests/unit/algorithms/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     5600 2020-07-26 18:29:23.000000 learn2learn-0.1.7/tests/unit/algorithms/gbml_test.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1992 2021-09-03 05:52:09.000000 learn2learn-0.1.7/tests/unit/algorithms/lightning_anil_test_notravis.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1653 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/algorithms/lightning_maml_test_notravis.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1631 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/algorithms/lightning_metaoptnet_test_notravis.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1645 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/algorithms/lightning_protonet_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     7703 2022-02-10 03:24:17.000000 learn2learn-0.1.7/tests/unit/algorithms/maml_test.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3902 2022-02-10 03:24:17.000000 learn2learn-0.1.7/tests/unit/algorithms/metasgd_test.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/unit/data/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        0 2020-01-07 16:31:05.000000 learn2learn-0.1.7/tests/unit/data/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5000 2022-02-10 03:24:17.000000 learn2learn-0.1.7/tests/unit/data/metadataset_test.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3839 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/unit/data/task_dataset_test.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3739 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/unit/data/transforms_test.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1686 2020-07-26 18:29:23.000000 learn2learn-0.1.7/tests/unit/data/util_datasets.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1518 2021-11-07 05:30:44.000000 learn2learn-0.1.7/tests/unit/data/utils_test.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/unit/nn/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)        0 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/nn/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2656 2021-02-19 01:16:38.000000 learn2learn-0.1.7/tests/unit/nn/kroneckers_test.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1381 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/nn/metaoptnet_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      845 2021-11-06 23:35:40.000000 learn2learn-0.1.7/tests/unit/nn/misc.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1734 2021-01-04 19:14:00.000000 learn2learn-0.1.7/tests/unit/nn/protonet_test.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)    12049 2022-02-10 01:56:47.000000 learn2learn-0.1.7/tests/unit/utils_test.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2022-02-10 03:33:40.000000 learn2learn-0.1.7/tests/unit/vision/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        0 2019-11-07 17:27:04.000000 learn2learn-0.1.7/tests/unit/vision/__init__.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     1008 2020-07-26 18:29:23.000000 learn2learn-0.1.7/tests/unit/vision/benchmarks_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      453 2020-06-20 17:57:33.000000 learn2learn-0.1.7/tests/unit/vision/cifarfs_test_notravis.py
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)      849 2020-08-30 17:02:15.000000 learn2learn-0.1.7/tests/unit/vision/cu_birds200_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      922 2020-09-02 22:10:21.000000 learn2learn-0.1.7/tests/unit/vision/describable_textures_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1217 2020-06-20 17:57:33.000000 learn2learn-0.1.7/tests/unit/vision/fc100_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      965 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/unit/vision/fgvc_aircraft_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1078 2021-11-07 05:30:44.000000 learn2learn-0.1.7/tests/unit/vision/pretrained_backbones_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      847 2020-09-02 22:10:21.000000 learn2learn-0.1.7/tests/unit/vision/quickdraw_test_no.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1070 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/unit/vision/tiered_imagenet_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1988 2022-02-09 01:28:15.000000 learn2learn-0.1.7/tests/unit/vision/transform_test_notravis.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      783 2020-05-19 02:44:30.000000 learn2learn-0.1.7/tests/unit/vision/vgg_flowers_test_notravis.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.812631 learn2learn-0.2.0/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.599057 learn2learn-0.2.0/.eggs/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.598170 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.598983 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.607427 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3321 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Code.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2918 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/FlowControl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2468 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/ParseTreeTransforms.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8903 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Parsing.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2113 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Scanning.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1792 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Visitor.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.598328 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.607672 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/Tests/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Debugger/Tests/cfuncs.c
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.607931 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.614301 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       61 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_bool.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_buffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_bytes.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_cobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_dict.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_exc.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_function.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_getargs.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_instance.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_int.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_long.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_mapping.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_mem.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_method.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_module.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_number.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_object.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_oldbuffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_pycapsule.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_ref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_sequence.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_tuple.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_type.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_unicode.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_version.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/python_weakref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       64 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2187 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stl.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.625993 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8254 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6034 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/array.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1359 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bool.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4831 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/buffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1443 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytearray.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9906 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytes.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      236 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ceval.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1524 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/cobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1777 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6779 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/datetime.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6877 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/dict.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13606 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/exc.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1424 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2671 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/function.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      775 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/getargs.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      985 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/instance.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4131 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/int.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1319 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4084 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7051 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/long.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      445 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/longintrepr.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2693 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mapping.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5386 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mem.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2504 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/memoryview.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2196 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/method.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9226 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/module.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11315 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/number.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    18366 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/object.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2916 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/oldbuffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5721 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pycapsule.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1985 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pylifecycle.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3683 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pystate.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1946 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pythread.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2557 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6008 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/sequence.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5383 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2113 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/slice.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9944 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3206 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/tuple.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1831 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/type.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    25841 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/unicode.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      847 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/version.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1984 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/weakref.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.629822 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       13 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2050 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/errno.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      966 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      621 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/limits.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1140 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/locale.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2796 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/math.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      297 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/setjmp.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1170 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/signal.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      164 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stddef.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3449 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdint.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2476 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2444 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2038 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1317 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/time.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.639438 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       94 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1770 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/algorithm.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      501 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/cast.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3012 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3106 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/deque.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2392 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/forward_list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      381 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/functional.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1432 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1661 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/limits.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2658 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2551 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/map.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3600 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/memory.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       27 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/pair.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      649 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/queue.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2170 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      292 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/stack.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5071 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      524 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeindex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      304 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeinfo.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2838 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_map.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2622 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      485 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/utility.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3350 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/vector.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.640393 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    38092 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5807 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/math.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1713 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/openmp.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.644327 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       13 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      355 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/dlfcn.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1175 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/fcntl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       99 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/ioctl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3362 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/mman.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1254 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/resource.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      546 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/select.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1876 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/signal.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1734 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stat.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1054 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      934 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      374 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/strings.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1980 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/time.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1162 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/types.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8061 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/unistd.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1244 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/wait.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.644827 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      585 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Actions.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1481 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Scanners.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.645066 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6279 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/refnanny.pyx
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.662931 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    40051 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/AsyncGen.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    29541 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Buffer.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16589 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Builtins.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4338 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CConvert.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2566 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CMath.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)      505 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Capsule.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2558 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CommonStructures.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10043 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Complex.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    86539 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Coroutine.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1893 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CpdefEnums.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6098 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CppConvert.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)    43920 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CythonFunction.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6675 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Embed.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    26361 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Exceptions.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8591 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ExtensionTypes.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12026 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/FunctionArguments.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    22105 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ImportExport.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    49610 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)    28907 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView_C.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    50383 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ModuleSetupCode.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    87240 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ObjectHandling.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    45132 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Optimize.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12358 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Overflow.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5103 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Printing.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16749 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Profile.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    41010 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/StringTools.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)      152 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCyUtilityLoader.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1595 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCythonScope.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)      279 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestUtilityLoader.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    35453 2020-03-02 00:59:17.000000 learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TypeConversion.c
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.599099 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.600011 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.665297 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3321 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Code.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2918 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/FlowControl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2468 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8984 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Parsing.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2113 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Scanning.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1792 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Visitor.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.599248 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.665569 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/Tests/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Debugger/Tests/cfuncs.c
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.665851 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.673099 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       61 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_bool.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_buffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_bytes.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_cobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_dict.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_exc.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_function.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_getargs.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_instance.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_int.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_long.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_mapping.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_mem.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_method.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_module.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_number.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_object.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_oldbuffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       71 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_pycapsule.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_ref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       70 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_sequence.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       68 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       67 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_tuple.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       66 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_type.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_unicode.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_version.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       69 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/python_weakref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       64 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2187 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stl.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.690430 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8254 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6056 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/array.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1359 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bool.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4870 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/buffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1443 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytearray.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9906 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytes.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1390 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cellobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      236 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ceval.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1524 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5084 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/codecs.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1777 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1696 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/conversion.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6776 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/datetime.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6877 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/dict.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13606 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/exc.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1424 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2671 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/function.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1052 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/genobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      775 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/getargs.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      985 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/instance.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4131 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/int.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1319 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1036 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterobject.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4084 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7051 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/long.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      445 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/longintrepr.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2693 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mapping.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5386 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mem.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2504 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/memoryview.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2196 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/method.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9226 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/module.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11922 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/number.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    18366 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/object.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2916 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5692 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2000 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3683 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pystate.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1946 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pythread.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2557 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ref.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6008 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/sequence.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5383 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3111 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/slice.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9944 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3206 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/tuple.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1831 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/type.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)    26247 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/unicode.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      847 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/version.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1984 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/weakref.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.693053 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       13 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2050 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/errno.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      966 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/float.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      621 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/limits.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1140 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/locale.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2948 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/math.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      297 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/setjmp.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1170 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/signal.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      164 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stddef.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3449 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdint.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2476 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2444 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2038 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1317 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/time.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.697317 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       94 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1770 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      501 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/cast.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3012 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/complex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3106 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/deque.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2392 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      381 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/functional.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1432 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/iterator.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1661 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/limits.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2658 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/list.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2551 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/map.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3600 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/memory.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       27 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/pair.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      649 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/queue.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2170 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      292 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/stack.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8731 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/string.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      524 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      304 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeinfo.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2867 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2622 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      903 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/utility.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3350 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/vector.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.697730 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    38138 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5807 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/math.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1713 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/openmp.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.700549 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       13 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/__init__.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      355 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/dlfcn.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1194 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/fcntl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)       99 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/ioctl.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3362 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/mman.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1254 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/resource.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      546 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/select.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1876 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/signal.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1734 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stat.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1054 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdio.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      934 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdlib.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)      374 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/strings.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1980 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/time.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1162 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/types.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8061 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/unistd.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1244 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/wait.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.700916 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      585 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Actions.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1481 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Scanners.pxd
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.701100 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6279 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/refnanny.pyx
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.708519 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    40051 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/AsyncGen.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    29654 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Buffer.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16783 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Builtins.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4338 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CConvert.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2566 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CMath.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)      505 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Capsule.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2558 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CommonStructures.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10043 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Complex.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    88160 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Coroutine.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1893 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CpdefEnums.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6098 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CppConvert.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)    45595 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CythonFunction.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6854 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Embed.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    26379 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Exceptions.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10831 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ExtensionTypes.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12040 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/FunctionArguments.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    22279 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ImportExport.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    49621 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)    29243 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView_C.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    51626 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ModuleSetupCode.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    88574 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ObjectHandling.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    45184 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Optimize.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12358 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Overflow.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5103 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Printing.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    17169 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Profile.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    42181 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/StringTools.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)      152 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCyUtilityLoader.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1595 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCythonScope.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)      279 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestUtilityLoader.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    36001 2021-11-07 00:52:51.000000 learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TypeConversion.c
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.708760 learn2learn-0.2.0/.github/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      691 2021-02-19 05:01:32.000000 learn2learn-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.710832 learn2learn-0.2.0/.github/workflows/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2320 2023-05-29 10:46:05.000000 learn2learn-0.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2487 2023-06-03 21:13:45.000000 learn2learn-0.2.0/.github/workflows/python_unittest.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1402 2021-01-04 19:14:00.000000 learn2learn-0.2.0/.gitignore
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5538 2023-06-03 21:14:49.000000 learn2learn-0.2.0/CHANGELOG.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      509 2023-05-29 10:46:05.000000 learn2learn-0.2.0/CITATION.cff
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1120 2019-11-07 17:27:04.000000 learn2learn-0.2.0/LICENSE
+-rw-r--r--   0 seba-1511   (501) staff       (20)       86 2020-05-19 02:44:30.000000 learn2learn-0.2.0/MANIFEST.in
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1855 2023-05-29 10:46:05.000000 learn2learn-0.2.0/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9009 2023-06-03 21:18:23.812751 learn2learn-0.2.0/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8578 2023-06-03 21:13:45.000000 learn2learn-0.2.0/README.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.712202 learn2learn-0.2.0/docs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       16 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/CNAME
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.600366 learn2learn-0.2.0/docs/assets/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.712610 learn2learn-0.2.0/docs/assets/css/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1393 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/css/l2l_material.css
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.723898 learn2learn-0.2.0/docs/assets/img/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.725993 learn2learn-0.2.0/docs/assets/img/community/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    36629 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/community/amazon_science.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3363 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/community/pytorch_lightning.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16959 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/community/uiuc.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    58030 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/community/usc.png
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.727018 learn2learn-0.2.0/docs/assets/img/examples/
+-rw-r--r--   0 seba-1511   (501) staff       (20)   244355 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/examples/ant_fwdbwd_rewards.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   450198 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/examples/cheetah_fwdbwd_rewards.png
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.733254 learn2learn-0.2.0/docs/assets/img/favicons/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4822 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-144x144.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5448 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-192x192.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1816 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-36x36.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2102 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-48x48.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2670 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-72x72.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3101 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/android-icon-96x96.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3562 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-114x114.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3638 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-120x120.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4822 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-144x144.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5161 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-152x152.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6352 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-180x180.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2310 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-57x57.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2456 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-60x60.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2670 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-72x72.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2669 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-76x76.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6024 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon-precomposed.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6024 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/apple-icon.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1208 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/favicon-16x16.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1640 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/favicon-32x32.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3101 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/favicon-96x96.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1150 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/favicon.ico
+-rw-r--r--   0 seba-1511   (501) staff       (20)      819 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/manifest.json
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4822 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/ms-icon-144x144.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5117 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/ms-icon-150x150.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13971 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/ms-icon-310x310.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2562 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/favicons/ms-icon-70x70.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)  4291753 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/halfcheetah.gif
+-rw-r--r--   0 seba-1511   (501) staff       (20)   139923 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/l2l-full.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   636573 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/learn2learn.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1528 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/learn2learn.svg
+-rw-r--r--   0 seba-1511   (501) staff       (20)    18105 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/assets/img/learn2learn_white.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5062 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/changelog.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1985 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/community.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.738374 learn2learn-0.2.0/docs/docs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      740 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.algorithms.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1200 2023-06-03 21:13:45.000000 learn2learn-0.2.0/docs/docs/learn2learn.data.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1523 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.gym.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      207 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      925 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.nn.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      615 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.optim.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1882 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/docs/learn2learn.vision.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.739065 learn2learn-0.2.0/docs/examples/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/examples/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      834 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/examples/optim.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      997 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/examples/rl.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5533 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/examples/vision.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8586 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/index.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)    54709 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/paper_list.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.739240 learn2learn-0.2.0/docs/tutorials/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.740611 learn2learn-0.2.0/docs/tutorials/anil_tutorial/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13749 2023-06-03 21:13:45.000000 learn2learn-0.2.0/docs/tutorials/anil_tutorial/ANIL_tutorial.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)   243034 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/tutorials/anil_tutorial/MAML_vs_ANIL.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   126403 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/tutorials/anil_tutorial/rapid_learning_or_feature_reuse.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1613 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/tutorials/getting_started.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.745998 learn2learn-0.2.0/docs/tutorials/task_transform_tutorial/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    29319 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/tutorials/task_transform_tutorial/few-shot.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   182742 2023-05-29 10:46:05.000000 learn2learn-0.2.0/docs/tutorials/task_transform_tutorial/l2l-task-transform.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    35390 2023-06-03 21:13:45.000000 learn2learn-0.2.0/docs/tutorials/task_transform_tutorial/transform_tutorial.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.747509 learn2learn-0.2.0/examples/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2621 2021-01-04 19:14:00.000000 learn2learn-0.2.0/examples/maml_sine.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1974 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/maml_toy.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1190 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/metamodule_toy.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.747972 learn2learn-0.2.0/examples/optimization/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      834 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/optimization/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4462 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/optimization/hypergrad_mnist.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.751981 learn2learn-0.2.0/examples/rl/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      997 2020-05-19 02:44:30.000000 learn2learn-0.2.0/examples/rl/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       23 2019-11-07 17:27:04.000000 learn2learn-0.2.0/examples/rl/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8685 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/rl/cavia_trpo.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9139 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/rl/dist_promp.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4144 2021-02-19 01:16:38.000000 learn2learn-0.2.0/examples/rl/maml_dice.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8363 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/rl/maml_trpo.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10678 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/rl/maml_trpo_metaworld.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3825 2020-08-25 21:19:19.000000 learn2learn-0.2.0/examples/rl/metasgd_a2c.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4554 2020-07-26 18:29:23.000000 learn2learn-0.2.0/examples/rl/policies.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8576 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/rl/promp.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.752607 learn2learn-0.2.0/examples/text/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3647 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/text/gpt2_adapters.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1620 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/text/nanogpt_lora.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    17309 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/text/nanogpt_model.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.755550 learn2learn-0.2.0/examples/vision/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1335 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5533 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7760 2023-06-03 21:13:45.000000 learn2learn-0.2.0/examples/vision/anil_fc100.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9038 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/anilkfo_cifarfs.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5464 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/distributed_maml.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.756586 learn2learn-0.2.0/examples/vision/lightning/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2849 2021-01-04 19:14:00.000000 learn2learn-0.2.0/examples/vision/lightning/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3253 2021-01-04 19:14:00.000000 learn2learn-0.2.0/examples/vision/lightning/main.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6436 2022-01-14 00:58:29.000000 learn2learn-0.2.0/examples/vision/maml_miniimagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6044 2020-12-05 21:37:00.000000 learn2learn-0.2.0/examples/vision/maml_omniglot.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.757834 learn2learn-0.2.0/examples/vision/mamlpp/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11093 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/mamlpp/MAMLpp.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9845 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/mamlpp/cnn4_bnrs.py
+-rwxr-xr-x   0 seba-1511   (501) staff       (20)    11268 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/mamlpp/maml++_miniimagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6149 2023-06-03 21:13:45.000000 learn2learn-0.2.0/examples/vision/meta_mnist.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6849 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/metacurvature_fc100.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7086 2023-06-03 21:13:45.000000 learn2learn-0.2.0/examples/vision/protonet_miniimagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8575 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/reptile_miniimagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9273 2023-05-29 10:46:05.000000 learn2learn-0.2.0/examples/vision/supervised_pretraining.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.758524 learn2learn-0.2.0/learn2learn/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      218 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)       22 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/_version.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.761619 learn2learn-0.2.0/learn2learn/algorithms/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      363 2021-01-04 19:14:00.000000 learn2learn-0.2.0/learn2learn/algorithms/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      483 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/algorithms/base_learner.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7345 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/algorithms/gbml.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.763131 learn2learn-0.2.0/learn2learn/algorithms/lightning/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      394 2021-01-04 19:14:00.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6176 2021-08-22 19:36:05.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_anil.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4260 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_episodic_module.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5885 2021-08-22 19:36:05.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_maml.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5088 2021-08-22 19:36:05.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_metaoptnet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5931 2021-08-22 19:36:05.000000 learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_protonet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7479 2022-01-14 00:35:09.000000 learn2learn-0.2.0/learn2learn/algorithms/maml.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4918 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/algorithms/meta_sgd.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.771660 learn2learn-0.2.0/learn2learn/data/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      343 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/data/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)   421092 2023-06-03 21:17:40.000000 learn2learn-0.2.0/learn2learn/data/meta_dataset.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8723 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/data/meta_dataset.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2036 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/data/samplers.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)   443333 2023-06-03 21:17:40.000000 learn2learn-0.2.0/learn2learn/data/task_dataset.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)      121 2020-05-19 02:44:30.000000 learn2learn-0.2.0/learn2learn/data/task_dataset.pxd
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6120 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/data/task_dataset.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)  1423642 2022-01-21 21:52:56.000000 learn2learn-0.2.0/learn2learn/data/transforms.c
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13195 2020-05-19 02:44:30.000000 learn2learn-0.2.0/learn2learn/data/transforms.pyx
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6870 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/data/utils.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.775632 learn2learn-0.2.0/learn2learn/gym/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2748 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      221 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/gym/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1526 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/async_vec_env.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.776543 learn2learn-0.2.0/learn2learn/gym/envs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1174 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/envs/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2130 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/gym/envs/meta_env.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.777070 learn2learn-0.2.0/learn2learn/gym/envs/metaworld/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       90 2020-06-20 17:57:33.000000 learn2learn-0.2.0/learn2learn/gym/envs/metaworld/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6351 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/gym/envs/metaworld/metaworld.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.779079 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      354 2020-05-19 02:44:30.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4641 2020-04-21 20:40:54.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/ant_direction.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4578 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/ant_forward_backward.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1083 2020-04-21 20:40:54.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/dummy_mujoco_env.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4290 2020-04-21 20:40:54.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/halfcheetah_forward_backward.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5042 2020-04-21 20:40:54.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/humanoid_direction.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4858 2020-04-21 20:40:54.000000 learn2learn-0.2.0/learn2learn/gym/envs/mujoco/humanoid_forward_backward.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.779655 learn2learn-0.2.0/learn2learn/gym/envs/particles/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       65 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/envs/particles/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3070 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/envs/particles/particles_2d.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3788 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/gym/envs/subproc_vec_env.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.781129 learn2learn-0.2.0/learn2learn/nn/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      282 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6543 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/kroneckers.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.781805 learn2learn-0.2.0/learn2learn/nn/metalayers/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       88 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/metalayers/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3900 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/metalayers/metamodule.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3100 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/metalayers/parameter_transform.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6290 2021-01-04 19:14:00.000000 learn2learn-0.2.0/learn2learn/nn/metaoptnet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3226 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/nn/misc.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5337 2021-01-04 19:14:00.000000 learn2learn-0.2.0/learn2learn/nn/protonet.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.782569 learn2learn-0.2.0/learn2learn/optim/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      253 2020-08-30 16:45:28.000000 learn2learn-0.2.0/learn2learn/optim/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3956 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/learnable_optimizer.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4849 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/parameter_update.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.784063 learn2learn-0.2.0/learn2learn/optim/transforms/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      512 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/transforms/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2574 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/transforms/kronecker_transform.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3176 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/transforms/metacurvature_transform.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2145 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/transforms/module_transform.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      880 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/transforms/transform_dictionary.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.784623 learn2learn-0.2.0/learn2learn/optim/update_rules/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       74 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/update_rules/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1640 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/optim/update_rules/differentiable_sgd.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.784899 learn2learn-0.2.0/learn2learn/text/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       47 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/text/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.785466 learn2learn-0.2.0/learn2learn/text/datasets/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       76 2019-11-07 17:27:04.000000 learn2learn-0.2.0/learn2learn/text/datasets/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2754 2021-02-19 05:01:32.000000 learn2learn-0.2.0/learn2learn/text/datasets/news_classification.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.786484 learn2learn-0.2.0/learn2learn/utils/
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13187 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/utils/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2109 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/utils/lightning.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.786963 learn2learn-0.2.0/learn2learn/vision/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      194 2020-07-26 18:29:23.000000 learn2learn-0.2.0/learn2learn/vision/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.791620 learn2learn-0.2.0/learn2learn/vision/benchmarks/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4465 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2597 2021-09-03 05:52:09.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/cifarfs_benchmark.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2568 2021-09-03 05:52:09.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/fc100_benchmark.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3578 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/mini_imagenet_benchmark.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2587 2021-09-03 05:52:09.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/omniglot_benchmark.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4021 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/benchmarks/tiered_imagenet_benchmark.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.795839 learn2learn-0.2.0/learn2learn/vision/datasets/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      523 2020-09-15 02:53:55.000000 learn2learn-0.2.0/learn2learn/vision/datasets/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4884 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/datasets/cifarfs.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16099 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/cu_birds200.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5309 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/describable_textures.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4934 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/fc100.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11302 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/fgvc_aircraft.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    58188 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/fgvc_fungi.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3162 2020-02-26 17:58:27.000000 learn2learn-0.2.0/learn2learn/vision/datasets/full_omniglot.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5732 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/datasets/mini_imagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13020 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/quickdraw.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6018 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/tiered_imagenet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5295 2023-06-03 21:13:45.000000 learn2learn-0.2.0/learn2learn/vision/datasets/vgg_flowers.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.796773 learn2learn-0.2.0/learn2learn/vision/models/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4011 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/models/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9420 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/models/cnn4.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11364 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/models/resnet12.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4950 2021-08-22 19:36:05.000000 learn2learn-0.2.0/learn2learn/vision/models/wrn28.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1556 2023-05-29 10:46:05.000000 learn2learn-0.2.0/learn2learn/vision/transforms.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.760133 learn2learn-0.2.0/learn2learn.egg-info/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9009 2023-06-03 21:18:07.000000 learn2learn-0.2.0/learn2learn.egg-info/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)    35910 2023-06-03 21:18:23.000000 learn2learn-0.2.0/learn2learn.egg-info/SOURCES.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        1 2023-06-03 21:18:07.000000 learn2learn-0.2.0/learn2learn.egg-info/dependency_links.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        1 2020-03-02 01:55:53.000000 learn2learn-0.2.0/learn2learn.egg-info/not-zip-safe
+-rw-r--r--   0 seba-1511   (501) staff       (20)       98 2023-06-03 21:18:07.000000 learn2learn-0.2.0/learn2learn.egg-info/requires.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       18 2023-06-03 21:18:07.000000 learn2learn-0.2.0/learn2learn.egg-info/top_level.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2623 2023-05-30 09:46:39.000000 learn2learn-0.2.0/mkdocs.yml
+-rw-r--r--   0 seba-1511   (501) staff       (20)      301 2023-05-29 10:46:05.000000 learn2learn-0.2.0/requirements-dev.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        2 2020-02-24 03:00:45.000000 learn2learn-0.2.0/requirements.txt
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.800991 learn2learn-0.2.0/scripts/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3357 2020-09-02 22:10:21.000000 learn2learn-0.2.0/scripts/bibtex_to_gsheets.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3719 2020-09-02 22:10:21.000000 learn2learn-0.2.0/scripts/compile_paper_list.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      437 2020-09-02 22:10:21.000000 learn2learn-0.2.0/scripts/credentials.json
+-rw-r--r--   0 seba-1511   (501) staff       (20)       38 2023-06-03 21:18:23.813574 learn2learn-0.2.0/setup.cfg
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2615 2023-05-29 10:46:05.000000 learn2learn-0.2.0/setup.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.801399 learn2learn-0.2.0/tests/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       23 2019-11-07 17:27:04.000000 learn2learn-0.2.0/tests/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.803109 learn2learn-0.2.0/tests/integration/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-11-07 17:27:04.000000 learn2learn-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7680 2023-06-03 21:13:45.000000 learn2learn-0.2.0/tests/integration/maml_miniimagenet_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8437 2023-06-03 21:13:45.000000 learn2learn-0.2.0/tests/integration/maml_omniglot_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8031 2023-06-03 21:13:45.000000 learn2learn-0.2.0/tests/integration/protonets_miniimagenet_test_notravis.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.803749 learn2learn-0.2.0/tests/unit/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-11-07 17:27:04.000000 learn2learn-0.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.806811 learn2learn-0.2.0/tests/unit/algorithms/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-11-07 17:27:04.000000 learn2learn-0.2.0/tests/unit/algorithms/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5600 2020-07-26 18:29:23.000000 learn2learn-0.2.0/tests/unit/algorithms/gbml_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1992 2021-09-03 05:52:09.000000 learn2learn-0.2.0/tests/unit/algorithms/lightning_anil_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1653 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/algorithms/lightning_maml_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1631 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/algorithms/lightning_metaoptnet_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1645 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/algorithms/lightning_protonet_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7703 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/algorithms/maml_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3902 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/algorithms/metasgd_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.808289 learn2learn-0.2.0/tests/unit/data/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2020-01-07 16:31:05.000000 learn2learn-0.2.0/tests/unit/data/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5000 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/data/metadataset_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3770 2023-06-03 21:13:45.000000 learn2learn-0.2.0/tests/unit/data/task_dataset_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3493 2023-06-03 21:13:45.000000 learn2learn-0.2.0/tests/unit/data/transforms_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1686 2020-07-26 18:29:23.000000 learn2learn-0.2.0/tests/unit/data/util_datasets.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1518 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/data/utils_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.809256 learn2learn-0.2.0/tests/unit/nn/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/nn/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2656 2021-02-19 01:16:38.000000 learn2learn-0.2.0/tests/unit/nn/kroneckers_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1381 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/nn/metaoptnet_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      845 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/nn/misc.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1734 2021-01-04 19:14:00.000000 learn2learn-0.2.0/tests/unit/nn/protonet_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12049 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/utils_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-03 21:18:23.812281 learn2learn-0.2.0/tests/unit/vision/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-11-07 17:27:04.000000 learn2learn-0.2.0/tests/unit/vision/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1008 2020-07-26 18:29:23.000000 learn2learn-0.2.0/tests/unit/vision/benchmarks_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      453 2020-06-20 17:57:33.000000 learn2learn-0.2.0/tests/unit/vision/cifarfs_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      849 2020-08-30 17:02:15.000000 learn2learn-0.2.0/tests/unit/vision/cu_birds200_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      922 2020-09-01 19:27:39.000000 learn2learn-0.2.0/tests/unit/vision/describable_textures_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1217 2020-06-20 17:57:33.000000 learn2learn-0.2.0/tests/unit/vision/fc100_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1192 2023-05-30 09:44:06.000000 learn2learn-0.2.0/tests/unit/vision/fgvc_aircraft_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1078 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/vision/pretrained_backbones_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      847 2020-09-02 22:10:21.000000 learn2learn-0.2.0/tests/unit/vision/quickdraw_test_no.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1070 2020-02-22 20:39:10.000000 learn2learn-0.2.0/tests/unit/vision/tiered_imagenet_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1988 2023-05-29 10:46:05.000000 learn2learn-0.2.0/tests/unit/vision/transform_test_notravis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      783 2020-02-22 20:39:10.000000 learn2learn-0.2.0/tests/unit/vision/vgg_flowers_test_notravis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Code.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Code.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/FlowControl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/FlowControl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/ParseTreeTransforms.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/ParseTreeTransforms.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Parsing.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Parsing.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Scanning.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Scanning.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Visitor.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Visitor.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/Deprecated/stl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/__init__.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/__init__.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/array.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/array.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bool.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bool.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/buffer.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/buffer.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytearray.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytearray.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytes.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/bytes.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/cobject.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/cobject.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/complex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/complex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/datetime.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/datetime.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/dict.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/dict.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/exc.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/exc.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/float.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/float.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/function.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/function.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/getargs.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/getargs.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/instance.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/instance.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/int.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/int.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/iterator.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/iterator.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/long.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/long.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mapping.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mapping.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mem.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/mem.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/memoryview.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/memoryview.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/method.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/method.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/module.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/module.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/number.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/number.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/object.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/object.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/oldbuffer.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/oldbuffer.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pycapsule.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pycapsule.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pylifecycle.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pylifecycle.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pystate.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pystate.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pythread.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/pythread.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ref.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/ref.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/sequence.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/sequence.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/slice.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/slice.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/tuple.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/tuple.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/type.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/type.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/unicode.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/unicode.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/version.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/version.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/weakref.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/cpython/weakref.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/errno.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/errno.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/float.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/float.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/limits.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/limits.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/locale.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/locale.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/math.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/math.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/signal.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/signal.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdint.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdint.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdio.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdio.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdlib.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/stdlib.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/time.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libc/time.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/algorithm.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/algorithm.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/complex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/complex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/deque.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/deque.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/forward_list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/forward_list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/iterator.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/iterator.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/limits.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/limits.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/map.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/map.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/memory.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/memory.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/queue.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/queue.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeindex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/typeindex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_map.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_map.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/unordered_set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/vector.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/libcpp/vector.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/__init__.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/__init__.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/math.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/numpy/math.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/openmp.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/openmp.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/fcntl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/fcntl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/mman.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/mman.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/resource.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/resource.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/select.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/select.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/signal.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/signal.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stat.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stat.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdio.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdio.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdlib.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/stdlib.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/time.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/time.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/types.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/types.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/unistd.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/unistd.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/wait.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Includes/posix/wait.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Actions.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Actions.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Scanners.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Plex/Scanners.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/refnanny.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Runtime/refnanny.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/AsyncGen.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/AsyncGen.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Buffer.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Buffer.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Builtins.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Builtins.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CConvert.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CConvert.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CMath.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CMath.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CommonStructures.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CommonStructures.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Complex.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Complex.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Coroutine.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Coroutine.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CpdefEnums.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CpdefEnums.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CppConvert.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CppConvert.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CythonFunction.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/CythonFunction.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Embed.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Embed.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Exceptions.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Exceptions.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ExtensionTypes.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ExtensionTypes.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/FunctionArguments.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/FunctionArguments.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ImportExport.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ImportExport.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView_C.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/MemoryView_C.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ModuleSetupCode.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ModuleSetupCode.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ObjectHandling.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/ObjectHandling.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Optimize.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Optimize.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Overflow.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Overflow.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Printing.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Printing.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Profile.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/Profile.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/StringTools.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/StringTools.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCythonScope.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TestCythonScope.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TypeConversion.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.15-py3.7.egg/Cython/Utility/TypeConversion.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Code.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Code.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/FlowControl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/FlowControl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Parsing.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Parsing.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Scanning.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Scanning.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Visitor.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Compiler/Visitor.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/Deprecated/stl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/__init__.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/__init__.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/array.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/array.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bool.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bool.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/buffer.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/buffer.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytearray.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytearray.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytes.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/bytes.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cellobject.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cellobject.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cobject.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/cobject.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/codecs.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/codecs.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/complex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/complex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/conversion.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/conversion.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/datetime.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/datetime.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/dict.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/dict.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/exc.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/exc.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/float.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/float.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/function.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/function.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/genobject.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/genobject.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/getargs.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/getargs.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/instance.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/instance.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/int.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/int.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterator.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterator.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterobject.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/iterobject.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/long.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/long.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mapping.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mapping.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mem.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/mem.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/memoryview.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/memoryview.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/method.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/method.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/module.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/module.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/number.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/number.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/object.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/object.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pystate.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pystate.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pythread.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/pythread.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ref.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/ref.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/sequence.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/sequence.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/slice.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/slice.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/tuple.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/tuple.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/type.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/type.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/unicode.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/unicode.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/version.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/version.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/weakref.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/cpython/weakref.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/errno.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/errno.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/float.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/float.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/limits.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/limits.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/locale.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/locale.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/math.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/math.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/signal.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/signal.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdint.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdint.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdio.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdio.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdlib.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/stdlib.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/time.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libc/time.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/complex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/complex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/deque.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/deque.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/iterator.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/iterator.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/limits.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/limits.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/list.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/list.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/map.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/map.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/memory.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/memory.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/queue.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/queue.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/string.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/string.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/utility.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/utility.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/vector.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/libcpp/vector.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/__init__.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/__init__.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/math.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/numpy/math.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/openmp.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/openmp.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/fcntl.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/fcntl.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/mman.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/mman.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/resource.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/resource.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/select.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/select.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/signal.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/signal.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stat.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stat.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdio.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdio.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdlib.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/stdlib.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/time.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/time.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/types.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/types.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/unistd.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/unistd.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/wait.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Includes/posix/wait.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Actions.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Actions.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Scanners.pxd` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Plex/Scanners.pxd`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/refnanny.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Runtime/refnanny.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/AsyncGen.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/AsyncGen.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Buffer.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Buffer.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Builtins.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Builtins.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CConvert.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CConvert.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CMath.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CMath.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CommonStructures.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CommonStructures.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Complex.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Complex.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Coroutine.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Coroutine.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CpdefEnums.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CpdefEnums.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CppConvert.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CppConvert.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CythonFunction.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/CythonFunction.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Embed.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Embed.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Exceptions.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Exceptions.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ExtensionTypes.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ExtensionTypes.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/FunctionArguments.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/FunctionArguments.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ImportExport.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ImportExport.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView_C.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/MemoryView_C.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ModuleSetupCode.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ModuleSetupCode.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ObjectHandling.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/ObjectHandling.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Optimize.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Optimize.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Overflow.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Overflow.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Printing.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Printing.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Profile.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Profile.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/StringTools.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/StringTools.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCythonScope.pyx` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCythonScope.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TypeConversion.c` & `learn2learn-0.2.0/.eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TypeConversion.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/LICENSE` & `learn2learn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/PKG-INFO` & `learn2learn-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,206 +1,194 @@
-Metadata-Version: 2.1
-Name: learn2learn
-Version: 0.1.7
-Summary: PyTorch Library for Meta-Learning Research
-Home-page: https://github.com/learnables/learn2learn
-Author: Debajyoti Datta, Ian bunner, Seb Arnold, Praateek Mahajan
-Author-email: smr.arnold@gmail.com
-License: MIT
-Download-URL: https://github.com/learnables/learn2learn/archive/0.1.7.zip
-Description: <p align="center"><img src="https://raw.githubusercontent.com/learnables/learn2learn/gh-pages/assets/img/l2l-full.png" height="120px" /></p>
-        
-        --------------------------------------------------------------------------------
-        
-        ![Test Status](https://github.com/learnables/learn2learn/workflows/Testing/badge.svg?branch=master)
-        [![arXiv](https://img.shields.io/badge/arXiv-2008.12284-b31b1b.svg)](https://arxiv.org/abs/2008.12284)
-        
-        learn2learn is a software library for meta-learning research.
-        
-        learn2learn builds on top of PyTorch to accelerate two aspects of the meta-learning research cycle:
-        
-        * *fast prototyping*, essential in letting researchers quickly try new ideas, and
-        * *correct reproducibility*, ensuring that these ideas are evaluated fairly.
-        
-        learn2learn provides low-level utilities and unified interface to create new algorithms and domains, together with high-quality implementations of existing algorithms and standardized benchmarks.
-        It retains compatibility with [torchvision](https://pytorch.org/vision/), [torchaudio](https://pytorch.org/audio/), [torchtext](https://pytorch.org/text/), [cherry](http://cherry-rl.net/), and any other PyTorch-based library you might be using.
-        
-        To learn more, see our whitepaper: [arXiv:2008.12284](https://arxiv.org/abs/2008.12284)
-        
-        **Overview**
-        
-        * [`learn2learn.data`](http://learn2learn.net/docs/learn2learn.data/): `TaskDataset` and transforms to create few-shot tasks from any PyTorch dataset.
-        * [`learn2learn.vision`](http://learn2learn.net/docs/learn2learn.vision/): Models, datasets, and benchmarks for computer vision and few-shot learning.
-        * [`learn2learn.gym`](http://learn2learn.net/docs/learn2learn.gym/): Environment and utilities for meta-reinforcement learning.
-        * [`learn2learn.algorithms`](http://learn2learn.net/docs/learn2learn.algorithms/): High-level wrappers for existing meta-learning algorithms.
-        * [`learn2learn.optim`](http://learn2learn.net/docs/learn2learn.optim/): Utilities and algorithms for differentiable optimization and meta-descent.
-        
-        **Resources**
-        
-        * Website: [http://learn2learn.net/](http://learn2learn.net/)
-        * Documentation: [http://learn2learn.net/docs/learn2learn](http://learn2learn.net/docs/learn2learn)
-        * Tutorials: [http://learn2learn.net/tutorials/getting_started/](http://learn2learn.net/tutorials/getting_started/)
-        * Examples: [https://github.com/learnables/learn2learn/tree/master/examples](https://github.com/learnables/learn2learn/tree/master/examples)
-        * GitHub: [https://github.com/learnables/learn2learn/](https://github.com/learnables/learn2learn/)
-        * Slack: [http://slack.learn2learn.net/](http://slack.learn2learn.net/)
-        
-        ## Installation
-        
-        ~~~bash
-        pip install learn2learn
-        ~~~
-        
-        ## Snippets & Examples
-        
-        The following snippets provide a sneak peek at the functionalities of learn2learn.
-        
-        ### High-level Wrappers
-        
-        <details>
-        <summary><b>Few-Shot Learning with MAML</b></summary>
-        
-        For more algorithms (ProtoNets, ANIL, Meta-SGD, Reptile, Meta-Curvature, KFO) refer to the <a href="https://github.com/learnables/learn2learn/tree/master/examples/vision">examples</a> folder.
-        Most of them can be implemented with with the `GBML` wrapper. (<a href="http://learn2learn.net/docs/learn2learn.algorithms/#gbml">documentation</a>).
-            
-        ~~~python
-        maml = l2l.algorithms.MAML(model, lr=0.1)
-        opt = torch.optim.SGD(maml.parameters(), lr=0.001)
-        for iteration in range(10):
-            opt.zero_grad()
-            task_model = maml.clone()  # torch.clone() for nn.Modules
-            adaptation_loss = compute_loss(task_model)
-            task_model.adapt(adaptation_loss)  # computes gradient, update task_model in-place
-            evaluation_loss = compute_loss(task_model)
-            evaluation_loss.backward()  # gradients w.r.t. maml.parameters()
-            opt.step()
-        ~~~
-        </details>
-        
-        <details>
-        <summary><b>Meta-Descent with Hypergradient</b></summary>
-            
-        Learn any kind of optimization algorithm with the `LearnableOptimizer`. (<a href="https://github.com/learnables/learn2learn/tree/master/examples/optimization">example</a> and <a href="http://learn2learn.net/docs/learn2learn.optim/#learnableoptimizer">documentation</a>)
-        
-        ~~~python
-        linear = nn.Linear(784, 10)
-        transform = l2l.optim.ModuleTransform(l2l.nn.Scale)
-        metaopt = l2l.optim.LearnableOptimizer(linear, transform, lr=0.01)  # metaopt has .step()
-        opt = torch.optim.SGD(metaopt.parameters(), lr=0.001)  # metaopt also has .parameters()
-        
-        metaopt.zero_grad()
-        opt.zero_grad()
-        error = loss(linear(X), y)
-        error.backward()
-        opt.step()  # update metaopt
-        metaopt.step()  # update linear
-        ~~~
-        </details>
-        
-        ### Learning Domains
-        
-        <details>
-        <summary><b>Custom Few-Shot Dataset</b></summary>
-        
-        Many standardized datasets (Omniglot, mini-/tiered-ImageNet, FC100, CIFAR-FS) are readily available in `learn2learn.vision.datasets`.
-        (<a href="http://learn2learn.net/docs/learn2learn.vision/#learn2learnvisiondatasets">documentation</a>)
-        
-        ~~~python
-        dataset = l2l.data.MetaDataset(MyDataset())  # any PyTorch dataset
-        transforms = [  # Easy to define your own transform
-            l2l.data.transforms.NWays(dataset, n=5),
-            l2l.data.transforms.KShots(dataset, k=1),
-            l2l.data.transforms.LoadData(dataset),
-        ]
-        taskset = TaskDataset(dataset, transforms, num_tasks=20000)
-        for task in taskset:
-            X, y = task
-            # Meta-train on the task
-        ~~~
-        </details>
-        
-        
-        <details>
-        <summary><b>Environments and Utilities for Meta-RL</b></summary>
-        
-        Parallelize your own meta-environments with `AsyncVectorEnv`, or use the standardized ones.
-        (<a href="http://learn2learn.net/docs/learn2learn.gym/#metaenv">documentation</a>)
-        
-        ~~~python
-        def make_env():
-            env = l2l.gym.HalfCheetahForwardBackwardEnv()
-            env = cherry.envs.ActionSpaceScaler(env)
-            return env
-        
-        env = l2l.gym.AsyncVectorEnv([make_env for _ in range(16)])  # uses 16 threads
-        for task_config in env.sample_tasks(20):
-            env.set_task(task)  # all threads receive the same task
-            state = env.reset()  # use standard Gym API
-            action = my_policy(env)
-            env.step(action)
-        ~~~
-        </details>
-        
-        ### Low-Level Utilities
-        
-        <details>
-        <summary><b>Differentiable Optimization</b></summary>
-        
-        Learn and differentiate through updates of PyTorch Modules.
-        (<a href="http://learn2learn.net/docs/learn2learn.optim/#parameterupdate">documentation</a>)
-            
-        ~~~python
-        
-        model = MyModel()
-        transform = l2l.optim.KroneckerTransform(l2l.nn.KroneckerLinear)
-        learned_update = l2l.optim.ParameterUpdate(  # learnable update function
-                model.parameters(), transform)
-        clone = l2l.clone_module(model)  # torch.clone() for nn.Modules
-        error = loss(clone(X), y)
-        updates = learned_update(  # similar API as torch.autograd.grad
-            error,
-            clone.parameters(),
-            create_graph=True,
-        )
-        l2l.update_module(clone, updates=updates)
-        loss(clone(X), y).backward()  # Gradients w.r.t model.parameters() and learned_update.parameters()
-        ~~~
-        </details>
-        
-        ## Changelog
-        
-        A human-readable changelog is available in the [CHANGELOG.md](CHANGELOG.md) file.
-        
-        ## Citation
-        
-        To cite the `learn2learn` repository in your academic publications, please use the following reference.
-        
-        > Arnold, Sebastien M. R., Praateek Mahajan, Debajyoti Datta, Ian Bunner, and Konstantinos Saitas Zarkias. 2020. “learn2learn: A Library for Meta-Learning Research.” arXiv [cs.LG]. http://arxiv.org/abs/2008.12284.
-        
-        You can also use the following Bibtex entry.
-        
-        ~~~bib
-        @article{Arnold2020-ss,
-          title         = "learn2learn: A Library for {Meta-Learning} Research",
-          author        = "Arnold, S{\'e}bastien M R and Mahajan, Praateek and Datta,
-                           Debajyoti and Bunner, Ian and Zarkias, Konstantinos Saitas",
-          month         =  aug,
-          year          =  2020,
-          url           = "http://arxiv.org/abs/2008.12284",
-          archivePrefix = "arXiv",
-          primaryClass  = "cs.LG",
-          eprint        = "2008.12284"
-        }
-        
-        ~~~
-        
-        ### Acknowledgements & Friends
-        
-        1. [TorchMeta](https://github.com/tristandeleu/pytorch-meta) is similar library, with a focus on datasets for supervised meta-learning. 
-        2. [higher](https://github.com/facebookresearch/higher) is a PyTorch library that enables differentiating through optimization inner-loops. While they monkey-patch `nn.Module` to be stateless, learn2learn retains the stateful PyTorch look-and-feel. For more information, refer to [their ArXiv paper](https://arxiv.org/abs/1910.01727).
-        3. We are thankful to the following open-source implementations which helped guide the design of learn2learn:
-            * Tristan Deleu's [pytorch-maml-rl](https://github.com/tristandeleu/pytorch-maml-rl)
-            * Jonas Rothfuss' [ProMP](https://github.com/jonasrothfuss/ProMP/)
-            * Kwonjoon Lee's [MetaOptNet](https://github.com/kjunelee/MetaOptNet)
-            * Han-Jia Ye's and Hexiang Hu's [FEAT](https://github.com/Sha-Lab/FEAT)
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<p align="center"><img src="https://raw.githubusercontent.com/learnables/learn2learn/gh-pages/assets/img/l2l-full.png" height="120px" /></p>
+
+--------------------------------------------------------------------------------
+
+![Test Status](https://github.com/learnables/learn2learn/workflows/Testing/badge.svg?branch=master)
+[![arXiv](https://img.shields.io/badge/arXiv-2008.12284-b31b1b.svg)](https://arxiv.org/abs/2008.12284)
+
+learn2learn is a software library for meta-learning research.
+
+learn2learn builds on top of PyTorch to accelerate two aspects of the meta-learning research cycle:
+
+* *fast prototyping*, essential in letting researchers quickly try new ideas, and
+* *correct reproducibility*, ensuring that these ideas are evaluated fairly.
+
+learn2learn provides low-level utilities and unified interface to create new algorithms and domains, together with high-quality implementations of existing algorithms and standardized benchmarks.
+It retains compatibility with [torchvision](https://pytorch.org/vision/), [torchaudio](https://pytorch.org/audio/), [torchtext](https://pytorch.org/text/), [cherry](http://cherry-rl.net/), and any other PyTorch-based library you might be using.
+
+To learn more, see our whitepaper: [arXiv:2008.12284](https://arxiv.org/abs/2008.12284)
+
+**Overview**
+
+* [`learn2learn.data`](http://learn2learn.net/docs/learn2learn.data/): `Taskset` and transforms to create few-shot tasks from any PyTorch dataset.
+* [`learn2learn.vision`](http://learn2learn.net/docs/learn2learn.vision/): Models, datasets, and benchmarks for computer vision and few-shot learning.
+* [`learn2learn.gym`](http://learn2learn.net/docs/learn2learn.gym/): Environment and utilities for meta-reinforcement learning.
+* [`learn2learn.algorithms`](http://learn2learn.net/docs/learn2learn.algorithms/): High-level wrappers for existing meta-learning algorithms.
+* [`learn2learn.optim`](http://learn2learn.net/docs/learn2learn.optim/): Utilities and algorithms for differentiable optimization and meta-descent.
+
+**Resources**
+
+* Website: [http://learn2learn.net/](http://learn2learn.net/)
+* Documentation: [http://learn2learn.net/docs/learn2learn](http://learn2learn.net/docs/learn2learn)
+* Tutorials: [http://learn2learn.net/tutorials/getting_started/](http://learn2learn.net/tutorials/getting_started/)
+* Examples: [https://github.com/learnables/learn2learn/tree/master/examples](https://github.com/learnables/learn2learn/tree/master/examples)
+* GitHub: [https://github.com/learnables/learn2learn/](https://github.com/learnables/learn2learn/)
+* Slack: [http://slack.learn2learn.net/](http://slack.learn2learn.net/)
+
+## Installation
+
+~~~bash
+pip install learn2learn
+~~~
+
+## Snippets & Examples
+
+The following snippets provide a sneak peek at the functionalities of learn2learn.
+
+### High-level Wrappers
+
+<details>
+<summary><b>Few-Shot Learning with MAML</b></summary>
+
+For more algorithms (ProtoNets, ANIL, Meta-SGD, Reptile, Meta-Curvature, KFO) refer to the <a href="https://github.com/learnables/learn2learn/tree/master/examples/vision">examples</a> folder.
+Most of them can be implemented with with the `GBML` wrapper. (<a href="http://learn2learn.net/docs/learn2learn.algorithms/#gbml">documentation</a>).
+    
+~~~python
+maml = l2l.algorithms.MAML(model, lr=0.1)
+opt = torch.optim.SGD(maml.parameters(), lr=0.001)
+for iteration in range(10):
+    opt.zero_grad()
+    task_model = maml.clone()  # torch.clone() for nn.Modules
+    adaptation_loss = compute_loss(task_model)
+    task_model.adapt(adaptation_loss)  # computes gradient, update task_model in-place
+    evaluation_loss = compute_loss(task_model)
+    evaluation_loss.backward()  # gradients w.r.t. maml.parameters()
+    opt.step()
+~~~
+</details>
+
+<details>
+<summary><b>Meta-Descent with Hypergradient</b></summary>
+    
+Learn any kind of optimization algorithm with the `LearnableOptimizer`. (<a href="https://github.com/learnables/learn2learn/tree/master/examples/optimization">example</a> and <a href="http://learn2learn.net/docs/learn2learn.optim/#learnableoptimizer">documentation</a>)
+
+~~~python
+linear = nn.Linear(784, 10)
+transform = l2l.optim.ModuleTransform(l2l.nn.Scale)
+metaopt = l2l.optim.LearnableOptimizer(linear, transform, lr=0.01)  # metaopt has .step()
+opt = torch.optim.SGD(metaopt.parameters(), lr=0.001)  # metaopt also has .parameters()
+
+metaopt.zero_grad()
+opt.zero_grad()
+error = loss(linear(X), y)
+error.backward()
+opt.step()  # update metaopt
+metaopt.step()  # update linear
+~~~
+</details>
+
+### Learning Domains
+
+<details>
+<summary><b>Custom Few-Shot Dataset</b></summary>
+
+Many standardized datasets (Omniglot, mini-/tiered-ImageNet, FC100, CIFAR-FS) are readily available in `learn2learn.vision.datasets`.
+(<a href="http://learn2learn.net/docs/learn2learn.vision/#learn2learnvisiondatasets">documentation</a>)
+
+~~~python
+dataset = l2l.data.MetaDataset(MyDataset())  # any PyTorch dataset
+transforms = [  # Easy to define your own transform
+    l2l.data.transforms.NWays(dataset, n=5),
+    l2l.data.transforms.KShots(dataset, k=1),
+    l2l.data.transforms.LoadData(dataset),
+]
+taskset = Taskset(dataset, transforms, num_tasks=20000)
+for task in taskset:
+    X, y = task
+    # Meta-train on the task
+~~~
+</details>
+
+
+<details>
+<summary><b>Environments and Utilities for Meta-RL</b></summary>
+
+Parallelize your own meta-environments with `AsyncVectorEnv`, or use the standardized ones.
+(<a href="http://learn2learn.net/docs/learn2learn.gym/#metaenv">documentation</a>)
+
+~~~python
+def make_env():
+    env = l2l.gym.HalfCheetahForwardBackwardEnv()
+    env = cherry.envs.ActionSpaceScaler(env)
+    return env
+
+env = l2l.gym.AsyncVectorEnv([make_env for _ in range(16)])  # uses 16 threads
+for task_config in env.sample_tasks(20):
+    env.set_task(task)  # all threads receive the same task
+    state = env.reset()  # use standard Gym API
+    action = my_policy(env)
+    env.step(action)
+~~~
+</details>
+
+### Low-Level Utilities
+
+<details>
+<summary><b>Differentiable Optimization</b></summary>
+
+Learn and differentiate through updates of PyTorch Modules.
+(<a href="http://learn2learn.net/docs/learn2learn.optim/#parameterupdate">documentation</a>)
+    
+~~~python
+
+model = MyModel()
+transform = l2l.optim.KroneckerTransform(l2l.nn.KroneckerLinear)
+learned_update = l2l.optim.ParameterUpdate(  # learnable update function
+        model.parameters(), transform)
+clone = l2l.clone_module(model)  # torch.clone() for nn.Modules
+error = loss(clone(X), y)
+updates = learned_update(  # similar API as torch.autograd.grad
+    error,
+    clone.parameters(),
+    create_graph=True,
+)
+l2l.update_module(clone, updates=updates)
+loss(clone(X), y).backward()  # Gradients w.r.t model.parameters() and learned_update.parameters()
+~~~
+</details>
+
+## Changelog
+
+A human-readable changelog is available in the [CHANGELOG.md](CHANGELOG.md) file.
+
+## Citation
+
+To cite the `learn2learn` repository in your academic publications, please use the following reference.
+
+> Arnold, Sebastien M. R., Praateek Mahajan, Debajyoti Datta, Ian Bunner, and Konstantinos Saitas Zarkias. 2020. “learn2learn: A Library for Meta-Learning Research.” arXiv [cs.LG]. http://arxiv.org/abs/2008.12284.
+
+You can also use the following Bibtex entry.
+
+~~~bib
+@article{Arnold2020-ss,
+  title         = "learn2learn: A Library for {Meta-Learning} Research",
+  author        = "Arnold, S{\'e}bastien M R and Mahajan, Praateek and Datta,
+                   Debajyoti and Bunner, Ian and Zarkias, Konstantinos Saitas",
+  month         =  aug,
+  year          =  2020,
+  url           = "http://arxiv.org/abs/2008.12284",
+  archivePrefix = "arXiv",
+  primaryClass  = "cs.LG",
+  eprint        = "2008.12284"
+}
+
+~~~
+
+### Acknowledgements & Friends
+
+1. [TorchMeta](https://github.com/tristandeleu/pytorch-meta) is similar library, with a focus on datasets for supervised meta-learning. 
+2. [higher](https://github.com/facebookresearch/higher) is a PyTorch library that enables differentiating through optimization inner-loops. While they monkey-patch `nn.Module` to be stateless, learn2learn retains the stateful PyTorch look-and-feel. For more information, refer to [their ArXiv paper](https://arxiv.org/abs/1910.01727).
+3. We are thankful to the following open-source implementations which helped guide the design of learn2learn:
+    * Tristan Deleu's [pytorch-maml-rl](https://github.com/tristandeleu/pytorch-maml-rl)
+    * Jonas Rothfuss' [ProMP](https://github.com/jonasrothfuss/ProMP/)
+    * Kwonjoon Lee's [MetaOptNet](https://github.com/kjunelee/MetaOptNet)
+    * Han-Jia Ye's and Hexiang Hu's [FEAT](https://github.com/Sha-Lab/FEAT)
```

### Comparing `learn2learn-0.1.7/README.md` & `learn2learn-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/gbml.py` & `learn2learn-0.2.0/learn2learn/algorithms/gbml.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_anil.py` & `learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_anil.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_episodic_module.py` & `learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_episodic_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 try:
     from pytorch_lightning import LightningModule
 except ImportError:
     from learn2learn.utils import _ImportRaiser
 
     class LightningRaiser(_ImportRaiser):
 
-        def __init__(self, *args, **kwargs):
-            self.name = 'pytorch_lightning'
-            self.command = 'pip install pytorch_lightning==1.0.2'
+        def __init__(self, **kwargs):
+            name = 'pytorch_lightning'
+            command = 'pip install pytorch_lightning'
+            super(LightningRaiser, self).__init__(name, command)
 
     LightningModule = LightningRaiser
 
 from torch import optim
 from argparse import ArgumentParser
```

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_maml.py` & `learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_maml.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_metaoptnet.py` & `learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_metaoptnet.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/lightning/lightning_protonet.py` & `learn2learn-0.2.0/learn2learn/algorithms/lightning/lightning_protonet.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/maml.py` & `learn2learn-0.2.0/learn2learn/algorithms/maml.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/algorithms/meta_sgd.py` & `learn2learn-0.2.0/learn2learn/algorithms/meta_sgd.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/data/meta_dataset.c` & `learn2learn-0.2.0/learn2learn/data/meta_dataset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1456,14 +1456,15 @@
 static const char __pyx_k_ds[] = "ds";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_wb[] = "wb";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_idx[] = "idx";
+static const char __pyx_k_l2l[] = "l2l";
 static const char __pyx_k_len[] = "__len__";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dump[] = "dump";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_item[] = "item";
 static const char __pyx_k_keys[] = "keys";
@@ -1502,14 +1503,15 @@
 static const char __pyx_k_idx_count[] = "idx_count";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_MetaDataset[] = "MetaDataset";
 static const char __pyx_k_bookkeeping[] = "_bookkeeping";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_defaultdict[] = "defaultdict";
+static const char __pyx_k_learn2learn[] = "learn2learn";
 static const char __pyx_k_labels_count[] = "labels_count";
 static const char __pyx_k_indices_count[] = "indices_count";
 static const char __pyx_k_labels_nooffset[] = "labels_nooffset";
 static const char __pyx_k_to_true_indices[] = "to_true_indices";
 static const char __pyx_k_UnionMetaDataset[] = "UnionMetaDataset";
 static const char __pyx_k_bookkeeping_path[] = "_bookkeeping_path";
 static const char __pyx_k_load_bookkeeping[] = "load_bookkeeping";
@@ -1596,21 +1598,23 @@
 static PyObject *__pyx_n_s_indices_to_labels;
 static PyObject *__pyx_n_u_indices_to_labels;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_item;
 static PyObject *__pyx_n_u_item;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_keys;
+static PyObject *__pyx_n_s_l2l;
 static PyObject *__pyx_n_s_label;
 static PyObject *__pyx_n_s_labels;
 static PyObject *__pyx_n_u_labels;
 static PyObject *__pyx_n_s_labels_count;
 static PyObject *__pyx_n_s_labels_nooffset;
 static PyObject *__pyx_n_s_labels_to_indices;
 static PyObject *__pyx_n_u_labels_to_indices;
+static PyObject *__pyx_n_s_learn2learn;
 static PyObject *__pyx_n_s_learn2learn_data_meta_dataset;
 static PyObject *__pyx_kp_s_learn2learn_data_meta_dataset_py;
 static PyObject *__pyx_n_s_len;
 static PyObject *__pyx_n_s_load;
 static PyObject *__pyx_n_s_load_bookkeeping;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_metaclass;
@@ -1677,15 +1681,15 @@
 static PyObject *__pyx_codeobj__20;
 static PyObject *__pyx_codeobj__22;
 static PyObject *__pyx_codeobj__24;
 static PyObject *__pyx_codeobj__26;
 static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
-/* "learn2learn/data/meta_dataset.pyx":48
+/* "learn2learn/data/meta_dataset.pyx":49
  *     """
  * 
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(dataset, Dataset):
  */
 
@@ -1729,15 +1733,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dataset)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 48, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 49, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_labels_to_indices);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -1745,15 +1749,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices_to_labels);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 49, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -1766,15 +1770,15 @@
     __pyx_v_self = values[0];
     __pyx_v_dataset = values[1];
     __pyx_v_labels_to_indices = values[2];
     __pyx_v_indices_to_labels = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 48, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 49, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_11MetaDataset___init__(__pyx_self, __pyx_v_self, __pyx_v_dataset, __pyx_v_labels_to_indices, __pyx_v_indices_to_labels);
 
@@ -1793,156 +1797,156 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":50
+  /* "learn2learn/data/meta_dataset.pyx":51
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):
  * 
  *         if not isinstance(dataset, Dataset):             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 "MetaDataset only accepts a torch dataset as input")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "learn2learn/data/meta_dataset.pyx":51
+    /* "learn2learn/data/meta_dataset.pyx":52
  * 
  *         if not isinstance(dataset, Dataset):
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 "MetaDataset only accepts a torch dataset as input")
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 51, __pyx_L1_error)
+    __PYX_ERR(0, 52, __pyx_L1_error)
 
-    /* "learn2learn/data/meta_dataset.pyx":50
+    /* "learn2learn/data/meta_dataset.pyx":51
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):
  * 
  *         if not isinstance(dataset, Dataset):             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 "MetaDataset only accepts a torch dataset as input")
  */
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":54
+  /* "learn2learn/data/meta_dataset.pyx":55
  *                 "MetaDataset only accepts a torch dataset as input")
  * 
  *         self.dataset = dataset             # <<<<<<<<<<<<<<
  * 
  *         if hasattr(dataset, '_bookkeeping_path'):
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dataset, __pyx_v_dataset) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dataset, __pyx_v_dataset) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":56
+  /* "learn2learn/data/meta_dataset.pyx":57
  *         self.dataset = dataset
  * 
  *         if hasattr(dataset, '_bookkeeping_path'):             # <<<<<<<<<<<<<<
  *             self.load_bookkeeping(dataset._bookkeeping_path)
  *         else:
  */
-  __pyx_t_3 = __Pyx_HasAttr(__pyx_v_dataset, __pyx_n_u_bookkeeping_path); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_HasAttr(__pyx_v_dataset, __pyx_n_u_bookkeeping_path); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "learn2learn/data/meta_dataset.pyx":57
+    /* "learn2learn/data/meta_dataset.pyx":58
  * 
  *         if hasattr(dataset, '_bookkeeping_path'):
  *             self.load_bookkeeping(dataset._bookkeeping_path)             # <<<<<<<<<<<<<<
  *         else:
  *             self.create_bookkeeping(
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_load_bookkeeping); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_load_bookkeeping); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_bookkeeping_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_bookkeeping_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":56
+    /* "learn2learn/data/meta_dataset.pyx":57
  *         self.dataset = dataset
  * 
  *         if hasattr(dataset, '_bookkeeping_path'):             # <<<<<<<<<<<<<<
  *             self.load_bookkeeping(dataset._bookkeeping_path)
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":59
+  /* "learn2learn/data/meta_dataset.pyx":60
  *             self.load_bookkeeping(dataset._bookkeeping_path)
  *         else:
  *             self.create_bookkeeping(             # <<<<<<<<<<<<<<
  *                 labels_to_indices=labels_to_indices,
  *                 indices_to_labels=indices_to_labels,
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_bookkeeping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_bookkeeping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "learn2learn/data/meta_dataset.pyx":60
+    /* "learn2learn/data/meta_dataset.pyx":61
  *         else:
  *             self.create_bookkeeping(
  *                 labels_to_indices=labels_to_indices,             # <<<<<<<<<<<<<<
  *                 indices_to_labels=indices_to_labels,
  *             )
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
 
-    /* "learn2learn/data/meta_dataset.pyx":61
+    /* "learn2learn/data/meta_dataset.pyx":62
  *             self.create_bookkeeping(
  *                 labels_to_indices=labels_to_indices,
  *                 indices_to_labels=indices_to_labels,             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
 
-    /* "learn2learn/data/meta_dataset.pyx":59
+    /* "learn2learn/data/meta_dataset.pyx":60
  *             self.load_bookkeeping(dataset._bookkeeping_path)
  *         else:
  *             self.create_bookkeeping(             # <<<<<<<<<<<<<<
  *                 labels_to_indices=labels_to_indices,
  *                 indices_to_labels=indices_to_labels,
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_L4:;
 
-  /* "learn2learn/data/meta_dataset.pyx":48
+  /* "learn2learn/data/meta_dataset.pyx":49
  *     """
  * 
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(dataset, Dataset):
  */
 
@@ -1958,15 +1962,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":64
+/* "learn2learn/data/meta_dataset.pyx":65
  *             )
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.dataset[item]
  * 
  */
 
@@ -2002,32 +2006,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_item)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 64, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 65, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 64, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_item = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 64, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 65, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_11MetaDataset_2__getitem__(__pyx_self, __pyx_v_self, __pyx_v_item);
 
@@ -2042,32 +2046,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":65
+  /* "learn2learn/data/meta_dataset.pyx":66
  * 
  *     def __getitem__(self, item):
  *         return self.dataset[item]             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/meta_dataset.pyx":64
+  /* "learn2learn/data/meta_dataset.pyx":65
  *             )
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.dataset[item]
  * 
  */
 
@@ -2079,15 +2083,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":67
+/* "learn2learn/data/meta_dataset.pyx":68
  *         return self.dataset[item]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.dataset)
  * 
  */
 
@@ -2112,33 +2116,33 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":68
+  /* "learn2learn/data/meta_dataset.pyx":69
  * 
  *     def __len__(self):
  *         return len(self.dataset)             # <<<<<<<<<<<<<<
  * 
  *     def create_bookkeeping(self, labels_to_indices=None, indices_to_labels=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/meta_dataset.pyx":67
+  /* "learn2learn/data/meta_dataset.pyx":68
  *         return self.dataset[item]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.dataset)
  * 
  */
 
@@ -2149,15 +2153,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":70
+/* "learn2learn/data/meta_dataset.pyx":71
  *         return len(self.dataset)
  * 
  *     def create_bookkeeping(self, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  *         """
  *         Iterates over the entire dataset and creates a map of target to indices.
  */
 
@@ -2208,15 +2212,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices_to_labels);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "create_bookkeeping") < 0)) __PYX_ERR(0, 70, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "create_bookkeeping") < 0)) __PYX_ERR(0, 71, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2227,15 +2231,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_labels_to_indices = values[1];
     __pyx_v_indices_to_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("create_bookkeeping", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 70, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("create_bookkeeping", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.create_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_11MetaDataset_6create_bookkeeping(__pyx_self, __pyx_v_self, __pyx_v_labels_to_indices, __pyx_v_indices_to_labels);
 
@@ -2281,143 +2285,143 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_bookkeeping", 0);
   __Pyx_INCREF(__pyx_v_labels_to_indices);
   __Pyx_INCREF(__pyx_v_indices_to_labels);
 
-  /* "learn2learn/data/meta_dataset.pyx":77
+  /* "learn2learn/data/meta_dataset.pyx":78
  *         """
  * 
  *         assert hasattr(self.dataset, '__getitem__'), \             # <<<<<<<<<<<<<<
  *             'Requires iterable-style dataset.'
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_HasAttr(__pyx_t_1, __pyx_n_u_getitem); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_HasAttr(__pyx_t_1, __pyx_n_u_getitem); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!(__pyx_t_2 != 0))) {
       PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_Requires_iterable_style_dataset);
-      __PYX_ERR(0, 77, __pyx_L1_error)
+      __PYX_ERR(0, 78, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "learn2learn/data/meta_dataset.pyx":81
+  /* "learn2learn/data/meta_dataset.pyx":82
  * 
  *         # Bootstrap from arguments
  *         if labels_to_indices is not None:             # <<<<<<<<<<<<<<
  *             indices_to_labels = {
  *                 idx: label
  */
   __pyx_t_2 = (__pyx_v_labels_to_indices != Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "learn2learn/data/meta_dataset.pyx":82
+    /* "learn2learn/data/meta_dataset.pyx":83
  *         # Bootstrap from arguments
  *         if labels_to_indices is not None:
  *             indices_to_labels = {             # <<<<<<<<<<<<<<
  *                 idx: label
  *                 for label, indices in labels_to_indices.items()
  */
     { /* enter inner scope */
-      __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L6_error)
+      __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "learn2learn/data/meta_dataset.pyx":84
+      /* "learn2learn/data/meta_dataset.pyx":85
  *             indices_to_labels = {
  *                 idx: label
  *                 for label, indices in labels_to_indices.items()             # <<<<<<<<<<<<<<
  *                 for idx in indices
  *             }
  */
       __pyx_t_5 = 0;
       if (unlikely(__pyx_v_labels_to_indices == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-        __PYX_ERR(0, 84, __pyx_L6_error)
+        __PYX_ERR(0, 85, __pyx_L6_error)
       }
-      __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_labels_to_indices, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L6_error)
+      __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_labels_to_indices, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_4);
       __pyx_t_4 = __pyx_t_8;
       __pyx_t_8 = 0;
       while (1) {
         __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_6, &__pyx_t_5, &__pyx_t_8, &__pyx_t_9, NULL, __pyx_t_7);
         if (unlikely(__pyx_t_10 == 0)) break;
-        if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 84, __pyx_L6_error)
+        if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 85, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_label, __pyx_t_8);
         __pyx_t_8 = 0;
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_indices, __pyx_t_9);
         __pyx_t_9 = 0;
 
-        /* "learn2learn/data/meta_dataset.pyx":85
+        /* "learn2learn/data/meta_dataset.pyx":86
  *                 idx: label
  *                 for label, indices in labels_to_indices.items()
  *                 for idx in indices             # <<<<<<<<<<<<<<
  *             }
  *         elif indices_to_labels is not None:
  */
         if (likely(PyList_CheckExact(__pyx_7genexpr__pyx_v_indices)) || PyTuple_CheckExact(__pyx_7genexpr__pyx_v_indices)) {
           __pyx_t_9 = __pyx_7genexpr__pyx_v_indices; __Pyx_INCREF(__pyx_t_9); __pyx_t_11 = 0;
           __pyx_t_12 = NULL;
         } else {
-          __pyx_t_11 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_7genexpr__pyx_v_indices); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 85, __pyx_L6_error)
+          __pyx_t_11 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_7genexpr__pyx_v_indices); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_12 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 85, __pyx_L6_error)
+          __pyx_t_12 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 86, __pyx_L6_error)
         }
         for (;;) {
           if (likely(!__pyx_t_12)) {
             if (likely(PyList_CheckExact(__pyx_t_9))) {
               if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_9)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_8 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_11); __Pyx_INCREF(__pyx_t_8); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 85, __pyx_L6_error)
+              __pyx_t_8 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_11); __Pyx_INCREF(__pyx_t_8); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 86, __pyx_L6_error)
               #else
-              __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L6_error)
+              __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L6_error)
               __Pyx_GOTREF(__pyx_t_8);
               #endif
             } else {
               if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_11); __Pyx_INCREF(__pyx_t_8); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 85, __pyx_L6_error)
+              __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_11); __Pyx_INCREF(__pyx_t_8); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 86, __pyx_L6_error)
               #else
-              __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 85, __pyx_L6_error)
+              __pyx_t_8 = PySequence_ITEM(__pyx_t_9, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L6_error)
               __Pyx_GOTREF(__pyx_t_8);
               #endif
             }
           } else {
             __pyx_t_8 = __pyx_t_12(__pyx_t_9);
             if (unlikely(!__pyx_t_8)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 85, __pyx_L6_error)
+                else __PYX_ERR(0, 86, __pyx_L6_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_8);
           }
           __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_idx, __pyx_t_8);
           __pyx_t_8 = 0;
 
-          /* "learn2learn/data/meta_dataset.pyx":83
+          /* "learn2learn/data/meta_dataset.pyx":84
  *         if labels_to_indices is not None:
  *             indices_to_labels = {
  *                 idx: label             # <<<<<<<<<<<<<<
  *                 for label, indices in labels_to_indices.items()
  *                 for idx in indices
  */
-          if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_idx, (PyObject*)__pyx_7genexpr__pyx_v_label))) __PYX_ERR(0, 83, __pyx_L6_error)
+          if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_idx, (PyObject*)__pyx_7genexpr__pyx_v_label))) __PYX_ERR(0, 84, __pyx_L6_error)
 
-          /* "learn2learn/data/meta_dataset.pyx":85
+          /* "learn2learn/data/meta_dataset.pyx":86
  *                 idx: label
  *                 for label, indices in labels_to_indices.items()
  *                 for idx in indices             # <<<<<<<<<<<<<<
  *             }
  *         elif indices_to_labels is not None:
  */
         }
@@ -2434,185 +2438,185 @@
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_label); __pyx_7genexpr__pyx_v_label = 0;
       goto __pyx_L1_error;
       __pyx_L11_exit_scope:;
     } /* exit inner scope */
     __Pyx_DECREF_SET(__pyx_v_indices_to_labels, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":81
+    /* "learn2learn/data/meta_dataset.pyx":82
  * 
  *         # Bootstrap from arguments
  *         if labels_to_indices is not None:             # <<<<<<<<<<<<<<
  *             indices_to_labels = {
  *                 idx: label
  */
     goto __pyx_L3;
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":87
+  /* "learn2learn/data/meta_dataset.pyx":88
  *                 for idx in indices
  *             }
  *         elif indices_to_labels is not None:             # <<<<<<<<<<<<<<
  *             labels_to_indices = defaultdict(list)
  *             for idx, label in indices_to_labels.items():
  */
   __pyx_t_3 = (__pyx_v_indices_to_labels != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "learn2learn/data/meta_dataset.pyx":88
+    /* "learn2learn/data/meta_dataset.pyx":89
  *             }
  *         elif indices_to_labels is not None:
  *             labels_to_indices = defaultdict(list)             # <<<<<<<<<<<<<<
  *             for idx, label in indices_to_labels.items():
  *                 labels_to_indices[label].append(idx)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_9, ((PyObject *)(&PyList_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyList_Type)));
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_labels_to_indices, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":89
+    /* "learn2learn/data/meta_dataset.pyx":90
  *         elif indices_to_labels is not None:
  *             labels_to_indices = defaultdict(list)
  *             for idx, label in indices_to_labels.items():             # <<<<<<<<<<<<<<
  *                 labels_to_indices[label].append(idx)
  *         else:  # Create from scratch
  */
     __pyx_t_6 = 0;
     if (unlikely(__pyx_v_indices_to_labels == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 89, __pyx_L1_error)
+      __PYX_ERR(0, 90, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_indices_to_labels, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_indices_to_labels, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1);
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
     while (1) {
       __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_5, &__pyx_t_6, &__pyx_t_4, &__pyx_t_9, NULL, __pyx_t_7);
       if (unlikely(__pyx_t_10 == 0)) break;
-      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 89, __pyx_L1_error)
+      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 90, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_XDECREF_SET(__pyx_v_label, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":90
+      /* "learn2learn/data/meta_dataset.pyx":91
  *             labels_to_indices = defaultdict(list)
  *             for idx, label in indices_to_labels.items():
  *                 labels_to_indices[label].append(idx)             # <<<<<<<<<<<<<<
  *         else:  # Create from scratch
  *             labels_to_indices = defaultdict(list)
  */
-      __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_13 = __Pyx_PyObject_Append(__pyx_t_9, __pyx_v_idx); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_Append(__pyx_t_9, __pyx_v_idx); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":87
+    /* "learn2learn/data/meta_dataset.pyx":88
  *                 for idx in indices
  *             }
  *         elif indices_to_labels is not None:             # <<<<<<<<<<<<<<
  *             labels_to_indices = defaultdict(list)
  *             for idx, label in indices_to_labels.items():
  */
     goto __pyx_L3;
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":92
+  /* "learn2learn/data/meta_dataset.pyx":93
  *                 labels_to_indices[label].append(idx)
  *         else:  # Create from scratch
  *             labels_to_indices = defaultdict(list)             # <<<<<<<<<<<<<<
  *             indices_to_labels = defaultdict(int)
  *             for i in range(len(self.dataset)):
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, ((PyObject *)(&PyList_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_9, ((PyObject *)(&PyList_Type)));
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF_SET(__pyx_v_labels_to_indices, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":93
+    /* "learn2learn/data/meta_dataset.pyx":94
  *         else:  # Create from scratch
  *             labels_to_indices = defaultdict(list)
  *             indices_to_labels = defaultdict(int)             # <<<<<<<<<<<<<<
  *             for i in range(len(self.dataset)):
  *                 try:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_9, ((PyObject *)(&PyInt_Type)));
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF_SET(__pyx_v_indices_to_labels, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":94
+    /* "learn2learn/data/meta_dataset.pyx":95
  *             labels_to_indices = defaultdict(list)
  *             indices_to_labels = defaultdict(int)
  *             for i in range(len(self.dataset)):             # <<<<<<<<<<<<<<
  *                 try:
  *                     label = self.dataset[i][1]
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_6; __pyx_t_11+=1) {
       __pyx_v_i = __pyx_t_11;
 
-      /* "learn2learn/data/meta_dataset.pyx":95
+      /* "learn2learn/data/meta_dataset.pyx":96
  *             indices_to_labels = defaultdict(int)
  *             for i in range(len(self.dataset)):
  *                 try:             # <<<<<<<<<<<<<<
  *                     label = self.dataset[i][1]
  *                     # if label is a Tensor, then take get the scalar value
  */
       {
@@ -2620,89 +2624,89 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
         __Pyx_XGOTREF(__pyx_t_14);
         __Pyx_XGOTREF(__pyx_t_15);
         __Pyx_XGOTREF(__pyx_t_16);
         /*try:*/ {
 
-          /* "learn2learn/data/meta_dataset.pyx":96
+          /* "learn2learn/data/meta_dataset.pyx":97
  *             for i in range(len(self.dataset)):
  *                 try:
  *                     label = self.dataset[i][1]             # <<<<<<<<<<<<<<
  *                     # if label is a Tensor, then take get the scalar value
  *                     if hasattr(label, 'item'):
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L16_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_1, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 96, __pyx_L16_error)
+          __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_1, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 97, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_9, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L16_error)
+          __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_9, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_XDECREF_SET(__pyx_v_label, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          /* "learn2learn/data/meta_dataset.pyx":98
+          /* "learn2learn/data/meta_dataset.pyx":99
  *                     label = self.dataset[i][1]
  *                     # if label is a Tensor, then take get the scalar value
  *                     if hasattr(label, 'item'):             # <<<<<<<<<<<<<<
  *                         label = self.dataset[i][1].item()
  *                 except ValueError as e:
  */
-          __pyx_t_2 = __Pyx_HasAttr(__pyx_v_label, __pyx_n_u_item); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 98, __pyx_L16_error)
+          __pyx_t_2 = __Pyx_HasAttr(__pyx_v_label, __pyx_n_u_item); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 99, __pyx_L16_error)
           __pyx_t_3 = (__pyx_t_2 != 0);
           if (__pyx_t_3) {
 
-            /* "learn2learn/data/meta_dataset.pyx":99
+            /* "learn2learn/data/meta_dataset.pyx":100
  *                     # if label is a Tensor, then take get the scalar value
  *                     if hasattr(label, 'item'):
  *                         label = self.dataset[i][1].item()             # <<<<<<<<<<<<<<
  *                 except ValueError as e:
  *                     raise ValueError(
  */
-            __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 99, __pyx_L16_error)
+            __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L16_error)
             __Pyx_GOTREF(__pyx_t_9);
-            __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_9, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L16_error)
+            __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_9, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L16_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-            __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 99, __pyx_L16_error)
+            __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L16_error)
             __Pyx_GOTREF(__pyx_t_9);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_item); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L16_error)
+            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_item); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L16_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
             __pyx_t_9 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
               __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
               if (likely(__pyx_t_9)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
                 __Pyx_INCREF(__pyx_t_9);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_4, function);
               }
             }
             __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L16_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L16_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_DECREF_SET(__pyx_v_label, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "learn2learn/data/meta_dataset.pyx":98
+            /* "learn2learn/data/meta_dataset.pyx":99
  *                     label = self.dataset[i][1]
  *                     # if label is a Tensor, then take get the scalar value
  *                     if hasattr(label, 'item'):             # <<<<<<<<<<<<<<
  *                         label = self.dataset[i][1].item()
  *                 except ValueError as e:
  */
           }
 
-          /* "learn2learn/data/meta_dataset.pyx":95
+          /* "learn2learn/data/meta_dataset.pyx":96
  *             indices_to_labels = defaultdict(int)
  *             for i in range(len(self.dataset)):
  *                 try:             # <<<<<<<<<<<<<<
  *                     label = self.dataset[i][1]
  *                     # if label is a Tensor, then take get the scalar value
  */
         }
@@ -2712,61 +2716,61 @@
         goto __pyx_L23_try_end;
         __pyx_L16_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "learn2learn/data/meta_dataset.pyx":100
+        /* "learn2learn/data/meta_dataset.pyx":101
  *                     if hasattr(label, 'item'):
  *                         label = self.dataset[i][1].item()
  *                 except ValueError as e:             # <<<<<<<<<<<<<<
  *                     raise ValueError(
  *                         'Requires scalar labels. \n' + str(e))
  */
         __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
         if (__pyx_t_7) {
           __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.create_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_9) < 0) __PYX_ERR(0, 100, __pyx_L18_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_9) < 0) __PYX_ERR(0, 101, __pyx_L18_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_4);
           __pyx_v_e = __pyx_t_4;
           /*try:*/ {
 
-            /* "learn2learn/data/meta_dataset.pyx":102
+            /* "learn2learn/data/meta_dataset.pyx":103
  *                 except ValueError as e:
  *                     raise ValueError(
  *                         'Requires scalar labels. \n' + str(e))             # <<<<<<<<<<<<<<
  * 
  *                 labels_to_indices[label].append(i)
  */
-            __pyx_t_8 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_e); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 102, __pyx_L30_error)
+            __pyx_t_8 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_e); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 103, __pyx_L30_error)
             __Pyx_GOTREF(__pyx_t_8);
-            __pyx_t_17 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Requires_scalar_labels, __pyx_t_8); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 102, __pyx_L30_error)
+            __pyx_t_17 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Requires_scalar_labels, __pyx_t_8); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 103, __pyx_L30_error)
             __Pyx_GOTREF(__pyx_t_17);
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-            /* "learn2learn/data/meta_dataset.pyx":101
+            /* "learn2learn/data/meta_dataset.pyx":102
  *                         label = self.dataset[i][1].item()
  *                 except ValueError as e:
  *                     raise ValueError(             # <<<<<<<<<<<<<<
  *                         'Requires scalar labels. \n' + str(e))
  * 
  */
-            __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_17); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 101, __pyx_L30_error)
+            __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_17); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 102, __pyx_L30_error)
             __Pyx_GOTREF(__pyx_t_8);
             __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
             __Pyx_Raise(__pyx_t_8, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-            __PYX_ERR(0, 101, __pyx_L30_error)
+            __PYX_ERR(0, 102, __pyx_L30_error)
           }
 
-          /* "learn2learn/data/meta_dataset.pyx":100
+          /* "learn2learn/data/meta_dataset.pyx":101
  *                     if hasattr(label, 'item'):
  *                         label = self.dataset[i][1].item()
  *                 except ValueError as e:             # <<<<<<<<<<<<<<
  *                     raise ValueError(
  *                         'Requires scalar labels. \n' + str(e))
  */
           /*finally:*/ {
@@ -2805,156 +2809,156 @@
               goto __pyx_L18_except_error;
             }
           }
         }
         goto __pyx_L18_except_error;
         __pyx_L18_except_error:;
 
-        /* "learn2learn/data/meta_dataset.pyx":95
+        /* "learn2learn/data/meta_dataset.pyx":96
  *             indices_to_labels = defaultdict(int)
  *             for i in range(len(self.dataset)):
  *                 try:             # <<<<<<<<<<<<<<
  *                     label = self.dataset[i][1]
  *                     # if label is a Tensor, then take get the scalar value
  */
         __Pyx_XGIVEREF(__pyx_t_14);
         __Pyx_XGIVEREF(__pyx_t_15);
         __Pyx_XGIVEREF(__pyx_t_16);
         __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
         goto __pyx_L1_error;
         __pyx_L23_try_end:;
       }
 
-      /* "learn2learn/data/meta_dataset.pyx":104
+      /* "learn2learn/data/meta_dataset.pyx":105
  *                         'Requires scalar labels. \n' + str(e))
  * 
  *                 labels_to_indices[label].append(i)             # <<<<<<<<<<<<<<
  *                 indices_to_labels[i] = label
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_13 = __Pyx_PyObject_Append(__pyx_t_9, __pyx_t_4); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_Append(__pyx_t_9, __pyx_t_4); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":105
+      /* "learn2learn/data/meta_dataset.pyx":106
  * 
  *                 labels_to_indices[label].append(i)
  *                 indices_to_labels[i] = label             # <<<<<<<<<<<<<<
  * 
  *         self.labels_to_indices = labels_to_indices
  */
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_indices_to_labels, __pyx_v_i, __pyx_v_label, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1) < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_v_indices_to_labels, __pyx_v_i, __pyx_v_label, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1) < 0)) __PYX_ERR(0, 106, __pyx_L1_error)
     }
   }
   __pyx_L3:;
 
-  /* "learn2learn/data/meta_dataset.pyx":107
+  /* "learn2learn/data/meta_dataset.pyx":108
  *                 indices_to_labels[i] = label
  * 
  *         self.labels_to_indices = labels_to_indices             # <<<<<<<<<<<<<<
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":108
+  /* "learn2learn/data/meta_dataset.pyx":109
  * 
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels             # <<<<<<<<<<<<<<
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":109
+  /* "learn2learn/data/meta_dataset.pyx":110
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())             # <<<<<<<<<<<<<<
  * 
  *         self._bookkeeping = {
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_1) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_1) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":112
+  /* "learn2learn/data/meta_dataset.pyx":113
  * 
  *         self._bookkeeping = {
  *             'labels_to_indices': self.labels_to_indices,             # <<<<<<<<<<<<<<
  *             'indices_to_labels': self.indices_to_labels,
  *             'labels': self.labels
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_labels_to_indices, __pyx_t_4) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_labels_to_indices, __pyx_t_4) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":113
+  /* "learn2learn/data/meta_dataset.pyx":114
  *         self._bookkeeping = {
  *             'labels_to_indices': self.labels_to_indices,
  *             'indices_to_labels': self.indices_to_labels,             # <<<<<<<<<<<<<<
  *             'labels': self.labels
  *         }
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_indices_to_labels, __pyx_t_4) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_indices_to_labels, __pyx_t_4) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":114
+  /* "learn2learn/data/meta_dataset.pyx":115
  *             'labels_to_indices': self.labels_to_indices,
  *             'indices_to_labels': self.indices_to_labels,
  *             'labels': self.labels             # <<<<<<<<<<<<<<
  *         }
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_labels, __pyx_t_4) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_labels, __pyx_t_4) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":111
+  /* "learn2learn/data/meta_dataset.pyx":112
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *         self._bookkeeping = {             # <<<<<<<<<<<<<<
  *             'labels_to_indices': self.labels_to_indices,
  *             'indices_to_labels': self.indices_to_labels,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping, __pyx_t_1) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":70
+  /* "learn2learn/data/meta_dataset.pyx":71
  *         return len(self.dataset)
  * 
  *     def create_bookkeeping(self, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  *         """
  *         Iterates over the entire dataset and creates a map of target to indices.
  */
 
@@ -2979,15 +2983,15 @@
   __Pyx_XDECREF(__pyx_v_labels_to_indices);
   __Pyx_XDECREF(__pyx_v_indices_to_labels);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":117
+/* "learn2learn/data/meta_dataset.pyx":118
  *         }
  * 
  *     def load_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()
  */
 
@@ -3023,32 +3027,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("load_bookkeeping", 1, 2, 2, 1); __PYX_ERR(0, 117, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("load_bookkeeping", 1, 2, 2, 1); __PYX_ERR(0, 118, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "load_bookkeeping") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "load_bookkeeping") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_path = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("load_bookkeeping", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("load_bookkeeping", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.load_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_11MetaDataset_8load_bookkeeping(__pyx_self, __pyx_v_self, __pyx_v_path);
 
@@ -3073,148 +3077,148 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("load_bookkeeping", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":118
+  /* "learn2learn/data/meta_dataset.pyx":119
  * 
  *     def load_bookkeeping(self, path):
  *         if not os.path.exists(path):             # <<<<<<<<<<<<<<
  *             self.create_bookkeeping()
  *             self.serialize_bookkeeping(path)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_path);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (__pyx_t_5) {
 
-    /* "learn2learn/data/meta_dataset.pyx":119
+    /* "learn2learn/data/meta_dataset.pyx":120
  *     def load_bookkeeping(self, path):
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()             # <<<<<<<<<<<<<<
  *             self.serialize_bookkeeping(path)
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":120
+    /* "learn2learn/data/meta_dataset.pyx":121
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()
  *             self.serialize_bookkeeping(path)             # <<<<<<<<<<<<<<
  *         else:
  *             with open(path, 'rb') as f:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_serialize_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_serialize_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_path);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":118
+    /* "learn2learn/data/meta_dataset.pyx":119
  * 
  *     def load_bookkeeping(self, path):
  *         if not os.path.exists(path):             # <<<<<<<<<<<<<<
  *             self.create_bookkeeping()
  *             self.serialize_bookkeeping(path)
  */
     goto __pyx_L3;
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":122
+  /* "learn2learn/data/meta_dataset.pyx":123
  *             self.serialize_bookkeeping(path)
  *         else:
  *             with open(path, 'rb') as f:             # <<<<<<<<<<<<<<
  *                 self._bookkeeping = pickle.load(f)
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  */
   /*else*/ {
     /*with:*/ {
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_path);
       __Pyx_GIVEREF(__pyx_v_path);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_path);
       __Pyx_INCREF(__pyx_n_u_rb);
       __Pyx_GIVEREF(__pyx_n_u_rb);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_rb);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L4_error)
+      __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L4_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __pyx_t_1;
       __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       /*try:*/ {
         {
@@ -3224,45 +3228,45 @@
           __Pyx_XGOTREF(__pyx_t_8);
           __Pyx_XGOTREF(__pyx_t_9);
           __Pyx_XGOTREF(__pyx_t_10);
           /*try:*/ {
             __pyx_v_f = __pyx_t_3;
             __pyx_t_3 = 0;
 
-            /* "learn2learn/data/meta_dataset.pyx":123
+            /* "learn2learn/data/meta_dataset.pyx":124
  *         else:
  *             with open(path, 'rb') as f:
  *                 self._bookkeeping = pickle.load(f)             # <<<<<<<<<<<<<<
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  *             self.indices_to_labels = self._bookkeeping['indices_to_labels']
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pickle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L8_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pickle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_load); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L8_error)
+            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_load); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __pyx_t_2 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
               __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
               if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
                 __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_1, function);
               }
             }
             __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_f) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_f);
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L8_error)
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping, __pyx_t_3) < 0) __PYX_ERR(0, 123, __pyx_L8_error)
+            if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping, __pyx_t_3) < 0) __PYX_ERR(0, 124, __pyx_L8_error)
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-            /* "learn2learn/data/meta_dataset.pyx":122
+            /* "learn2learn/data/meta_dataset.pyx":123
  *             self.serialize_bookkeeping(path)
  *         else:
  *             with open(path, 'rb') as f:             # <<<<<<<<<<<<<<
  *                 self._bookkeeping = pickle.load(f)
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  */
           }
@@ -3273,36 +3277,36 @@
           __pyx_L8_error:;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           /*except:*/ {
             __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.load_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 122, __pyx_L10_except_error)
+            if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 123, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_7 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 122, __pyx_L10_except_error)
+            __pyx_t_7 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_7);
             __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 122, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 123, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (__pyx_t_5 < 0) __PYX_ERR(0, 122, __pyx_L10_except_error)
+            if (__pyx_t_5 < 0) __PYX_ERR(0, 123, __pyx_L10_except_error)
             __pyx_t_4 = ((!(__pyx_t_5 != 0)) != 0);
             if (__pyx_t_4) {
               __Pyx_GIVEREF(__pyx_t_3);
               __Pyx_GIVEREF(__pyx_t_1);
               __Pyx_XGIVEREF(__pyx_t_2);
               __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_1, __pyx_t_2);
               __pyx_t_3 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0; 
-              __PYX_ERR(0, 122, __pyx_L10_except_error)
+              __PYX_ERR(0, 123, __pyx_L10_except_error)
             }
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             goto __pyx_L9_exception_handled;
           }
           __pyx_L10_except_error:;
@@ -3320,77 +3324,77 @@
         }
       }
       /*finally:*/ {
         /*normal exit:*/{
           if (__pyx_t_6) {
             __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__2, NULL);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 122, __pyx_L1_error)
+            if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 123, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_10);
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           }
           goto __pyx_L7;
         }
         __pyx_L7:;
       }
       goto __pyx_L17;
       __pyx_L4_error:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L1_error;
       __pyx_L17:;
     }
 
-    /* "learn2learn/data/meta_dataset.pyx":124
+    /* "learn2learn/data/meta_dataset.pyx":125
  *             with open(path, 'rb') as f:
  *                 self._bookkeeping = pickle.load(f)
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']             # <<<<<<<<<<<<<<
  *             self.indices_to_labels = self._bookkeeping['indices_to_labels']
  *             self.labels = self._bookkeeping['labels']
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_labels_to_indices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_labels_to_indices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_t_1) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_t_1) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":125
+    /* "learn2learn/data/meta_dataset.pyx":126
  *                 self._bookkeeping = pickle.load(f)
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  *             self.indices_to_labels = self._bookkeeping['indices_to_labels']             # <<<<<<<<<<<<<<
  *             self.labels = self._bookkeeping['labels']
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_indices_to_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_indices_to_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_t_2) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_t_2) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":126
+    /* "learn2learn/data/meta_dataset.pyx":127
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  *             self.indices_to_labels = self._bookkeeping['indices_to_labels']
  *             self.labels = self._bookkeeping['labels']             # <<<<<<<<<<<<<<
  * 
  *     def serialize_bookkeeping(self, path):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_1) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "learn2learn/data/meta_dataset.pyx":117
+  /* "learn2learn/data/meta_dataset.pyx":118
  *         }
  * 
  *     def load_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()
  */
 
@@ -3407,15 +3411,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":128
+/* "learn2learn/data/meta_dataset.pyx":129
  *             self.labels = self._bookkeeping['labels']
  * 
  *     def serialize_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         with open(path, 'wb') as f:
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  */
 
@@ -3451,32 +3455,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("serialize_bookkeeping", 1, 2, 2, 1); __PYX_ERR(0, 128, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("serialize_bookkeeping", 1, 2, 2, 1); __PYX_ERR(0, 129, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "serialize_bookkeeping") < 0)) __PYX_ERR(0, 128, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "serialize_bookkeeping") < 0)) __PYX_ERR(0, 129, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_path = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("serialize_bookkeeping", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 128, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("serialize_bookkeeping", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 129, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.serialize_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_11MetaDataset_10serialize_bookkeeping(__pyx_self, __pyx_v_self, __pyx_v_path);
 
@@ -3501,50 +3505,50 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("serialize_bookkeeping", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":129
+  /* "learn2learn/data/meta_dataset.pyx":130
  * 
  *     def serialize_bookkeeping(self, path):
  *         with open(path, 'wb') as f:             # <<<<<<<<<<<<<<
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  * 
  */
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_path);
     __Pyx_GIVEREF(__pyx_v_path);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_path);
     __Pyx_INCREF(__pyx_n_u_wb);
     __Pyx_GIVEREF(__pyx_n_u_wb);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_wb);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L3_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
@@ -3554,47 +3558,47 @@
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __pyx_v_f = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "learn2learn/data/meta_dataset.pyx":130
+          /* "learn2learn/data/meta_dataset.pyx":131
  *     def serialize_bookkeeping(self, path):
  *         with open(path, 'wb') as f:
  *             pickle.dump(self._bookkeeping, f, protocol=-1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pickle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pickle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dump); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dump); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L7_error)
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bookkeeping); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L7_error)
+          __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
           __Pyx_INCREF(__pyx_v_f);
           __Pyx_GIVEREF(__pyx_v_f);
           PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_f);
           __pyx_t_4 = 0;
-          __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L7_error)
+          __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
-          if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_protocol, __pyx_int_neg_1) < 0) __PYX_ERR(0, 130, __pyx_L7_error)
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L7_error)
+          if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_protocol, __pyx_int_neg_1) < 0) __PYX_ERR(0, 131, __pyx_L7_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          /* "learn2learn/data/meta_dataset.pyx":129
+          /* "learn2learn/data/meta_dataset.pyx":130
  * 
  *     def serialize_bookkeeping(self, path):
  *         with open(path, 'wb') as f:             # <<<<<<<<<<<<<<
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  * 
  */
         }
@@ -3605,36 +3609,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("learn2learn.data.meta_dataset.MetaDataset.serialize_bookkeeping", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 129, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 130, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L9_except_error)
+          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 129, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 130, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 129, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 130, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_5);
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_5, __pyx_t_4, __pyx_t_1);
             __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 129, __pyx_L9_except_error)
+            __PYX_ERR(0, 130, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -3652,30 +3656,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 129, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 130, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":128
+  /* "learn2learn/data/meta_dataset.pyx":129
  *             self.labels = self._bookkeeping['labels']
  * 
  *     def serialize_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         with open(path, 'wb') as f:
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  */
 
@@ -3692,15 +3696,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":161
+/* "learn2learn/data/meta_dataset.pyx":162
  *     """
  * 
  *     def __init__(self, datasets):             # <<<<<<<<<<<<<<
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  */
 
@@ -3736,32 +3740,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_datasets)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 161, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 162, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_datasets = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 162, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.UnionMetaDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_16UnionMetaDataset___init__(__pyx_self, __pyx_v_self, __pyx_v_datasets);
 
@@ -3801,113 +3805,113 @@
   int __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_datasets);
 
-  /* "learn2learn/data/meta_dataset.pyx":162
+  /* "learn2learn/data/meta_dataset.pyx":163
  * 
  *     def __init__(self, datasets):
  *         datasets = [             # <<<<<<<<<<<<<<
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  *             for ds in datasets
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "learn2learn/data/meta_dataset.pyx":164
+    /* "learn2learn/data/meta_dataset.pyx":165
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  *             for ds in datasets             # <<<<<<<<<<<<<<
  *         ]
  *         self.datasets = datasets
  */
     if (likely(PyList_CheckExact(__pyx_v_datasets)) || PyTuple_CheckExact(__pyx_v_datasets)) {
       __pyx_t_2 = __pyx_v_datasets; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_datasets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_datasets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 164, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 165, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 164, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 165, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 164, __pyx_L5_error)
+            else __PYX_ERR(0, 165, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_ds, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":163
+      /* "learn2learn/data/meta_dataset.pyx":164
  *     def __init__(self, datasets):
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds             # <<<<<<<<<<<<<<
  *             for ds in datasets
  *         ]
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 163, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 164, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PyObject_IsInstance(__pyx_8genexpr1__pyx_v_ds, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 163, __pyx_L5_error)
+      __pyx_t_7 = PyObject_IsInstance(__pyx_8genexpr1__pyx_v_ds, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (((!(__pyx_t_7 != 0)) != 0)) {
-        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 163, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 164, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_8, function);
           }
         }
         __pyx_t_6 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_8genexpr1__pyx_v_ds) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_8genexpr1__pyx_v_ds);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 163, __pyx_L5_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 164, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_5 = __pyx_t_6;
         __pyx_t_6 = 0;
       } else {
         __Pyx_INCREF(__pyx_8genexpr1__pyx_v_ds);
         __pyx_t_5 = __pyx_8genexpr1__pyx_v_ds;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 162, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 163, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":164
+      /* "learn2learn/data/meta_dataset.pyx":165
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  *             for ds in datasets             # <<<<<<<<<<<<<<
  *         ]
  *         self.datasets = datasets
  */
     }
@@ -3918,210 +3922,210 @@
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_ds); __pyx_8genexpr1__pyx_v_ds = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_datasets, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":166
+  /* "learn2learn/data/meta_dataset.pyx":167
  *             for ds in datasets
  *         ]
  *         self.datasets = datasets             # <<<<<<<<<<<<<<
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_datasets, __pyx_v_datasets) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_datasets, __pyx_v_datasets) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":167
+  /* "learn2learn/data/meta_dataset.pyx":168
  *         ]
  *         self.datasets = datasets
  *         labels_to_indices = defaultdict(list)             # <<<<<<<<<<<<<<
  *         indices_to_labels = defaultdict(int)
  *         labels_count = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, ((PyObject *)(&PyList_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)(&PyList_Type)));
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_labels_to_indices = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":168
+  /* "learn2learn/data/meta_dataset.pyx":169
  *         self.datasets = datasets
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)             # <<<<<<<<<<<<<<
  *         labels_count = 0
  *         indices_count = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)(&PyInt_Type)));
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_indices_to_labels = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":169
+  /* "learn2learn/data/meta_dataset.pyx":170
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)
  *         labels_count = 0             # <<<<<<<<<<<<<<
  *         indices_count = 0
  *         for dataset in datasets:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_labels_count = __pyx_int_0;
 
-  /* "learn2learn/data/meta_dataset.pyx":170
+  /* "learn2learn/data/meta_dataset.pyx":171
  *         indices_to_labels = defaultdict(int)
  *         labels_count = 0
  *         indices_count = 0             # <<<<<<<<<<<<<<
  *         for dataset in datasets:
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_indices_count = __pyx_int_0;
 
-  /* "learn2learn/data/meta_dataset.pyx":171
+  /* "learn2learn/data/meta_dataset.pyx":172
  *         labels_count = 0
  *         indices_count = 0
  *         for dataset in datasets:             # <<<<<<<<<<<<<<
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}
  *             for idx, label in dataset.indices_to_labels.items():
  */
   if (likely(PyList_CheckExact(__pyx_v_datasets)) || PyTuple_CheckExact(__pyx_v_datasets)) {
     __pyx_t_1 = __pyx_v_datasets; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_datasets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_datasets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 172, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 172, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_4(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 171, __pyx_L1_error)
+          else __PYX_ERR(0, 172, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_dataset, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":172
+    /* "learn2learn/data/meta_dataset.pyx":173
  *         indices_count = 0
  *         for dataset in datasets:
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}             # <<<<<<<<<<<<<<
  *             for idx, label in dataset.indices_to_labels.items():
  *                 label = labels_nooffset[label]
  */
     { /* enter inner scope */
-      __pyx_t_2 = PyDict_New(); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L13_error)
+      __pyx_t_2 = PyDict_New(); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L13_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_int_0);
       __pyx_t_5 = __pyx_int_0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L13_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L13_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
         __pyx_t_8 = __pyx_t_6; __Pyx_INCREF(__pyx_t_8); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
       } else {
-        __pyx_t_10 = -1; __pyx_t_8 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __pyx_t_10 = -1; __pyx_t_8 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L13_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_11 = Py_TYPE(__pyx_t_8)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __pyx_t_11 = Py_TYPE(__pyx_t_8)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 173, __pyx_L13_error)
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       for (;;) {
         if (likely(!__pyx_t_11)) {
           if (likely(PyList_CheckExact(__pyx_t_8))) {
             if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_8)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_6 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_6 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 173, __pyx_L13_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_6 = PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L13_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           } else {
             if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_8)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_6); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 173, __pyx_L13_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_6 = PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L13_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           }
         } else {
           __pyx_t_6 = __pyx_t_11(__pyx_t_8);
           if (unlikely(!__pyx_t_6)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 172, __pyx_L13_error)
+              else __PYX_ERR(0, 173, __pyx_L13_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_6);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_label, __pyx_t_6);
         __pyx_t_6 = 0;
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_i, __pyx_t_5);
-        __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L13_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_5);
         __pyx_t_5 = __pyx_t_6;
         __pyx_t_6 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_t_2, (PyObject*)__pyx_8genexpr2__pyx_v_label, (PyObject*)__pyx_8genexpr2__pyx_v_i))) __PYX_ERR(0, 172, __pyx_L13_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_2, (PyObject*)__pyx_8genexpr2__pyx_v_label, (PyObject*)__pyx_8genexpr2__pyx_v_i))) __PYX_ERR(0, 173, __pyx_L13_error)
       }
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_i); __pyx_8genexpr2__pyx_v_i = 0;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_label); __pyx_8genexpr2__pyx_v_label = 0;
       goto __pyx_L16_exit_scope;
       __pyx_L13_error:;
@@ -4129,192 +4133,192 @@
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_label); __pyx_8genexpr2__pyx_v_label = 0;
       goto __pyx_L1_error;
       __pyx_L16_exit_scope:;
     } /* exit inner scope */
     __Pyx_XDECREF_SET(__pyx_v_labels_nooffset, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":173
+    /* "learn2learn/data/meta_dataset.pyx":174
  *         for dataset in datasets:
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}
  *             for idx, label in dataset.indices_to_labels.items():             # <<<<<<<<<<<<<<
  *                 label = labels_nooffset[label]
  *                 indices_to_labels[indices_count + idx] = labels_count + label
  */
     __pyx_t_10 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (unlikely(__pyx_t_5 == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 173, __pyx_L1_error)
+      __PYX_ERR(0, 174, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_items, (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_items, (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_2);
     __pyx_t_2 = __pyx_t_8;
     __pyx_t_8 = 0;
     while (1) {
       __pyx_t_14 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_12, &__pyx_t_10, &__pyx_t_8, &__pyx_t_5, NULL, __pyx_t_13);
       if (unlikely(__pyx_t_14 == 0)) break;
-      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 173, __pyx_L1_error)
+      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 174, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_label, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":174
+      /* "learn2learn/data/meta_dataset.pyx":175
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}
  *             for idx, label in dataset.indices_to_labels.items():
  *                 label = labels_nooffset[label]             # <<<<<<<<<<<<<<
  *                 indices_to_labels[indices_count + idx] = labels_count + label
  *                 labels_to_indices[labels_count + label].append(indices_count + idx)
  */
-      __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_labels_nooffset, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_labels_nooffset, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF_SET(__pyx_v_label, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":175
+      /* "learn2learn/data/meta_dataset.pyx":176
  *             for idx, label in dataset.indices_to_labels.items():
  *                 label = labels_nooffset[label]
  *                 indices_to_labels[indices_count + idx] = labels_count + label             # <<<<<<<<<<<<<<
  *                 labels_to_indices[labels_count + label].append(indices_count + idx)
  *             indices_count += len(dataset.indices_to_labels)
  */
-      __pyx_t_5 = PyNumber_Add(__pyx_v_labels_count, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_Add(__pyx_v_labels_count, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = PyNumber_Add(__pyx_v_indices_count, __pyx_v_idx); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 175, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_Add(__pyx_v_indices_count, __pyx_v_idx); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 176, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      if (unlikely(PyObject_SetItem(__pyx_v_indices_to_labels, __pyx_t_8, __pyx_t_5) < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_indices_to_labels, __pyx_t_8, __pyx_t_5) < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":176
+      /* "learn2learn/data/meta_dataset.pyx":177
  *                 label = labels_nooffset[label]
  *                 indices_to_labels[indices_count + idx] = labels_count + label
  *                 labels_to_indices[labels_count + label].append(indices_count + idx)             # <<<<<<<<<<<<<<
  *             indices_count += len(dataset.indices_to_labels)
  *             labels_count += len(dataset.labels_to_indices)
  */
-      __pyx_t_5 = PyNumber_Add(__pyx_v_labels_count, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_Add(__pyx_v_labels_count, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 176, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyNumber_Add(__pyx_v_indices_count, __pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_Add(__pyx_v_indices_count, __pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_15 = __Pyx_PyObject_Append(__pyx_t_8, __pyx_t_5); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 176, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_Append(__pyx_t_8, __pyx_t_5); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":177
+    /* "learn2learn/data/meta_dataset.pyx":178
  *                 indices_to_labels[indices_count + idx] = labels_count + label
  *                 labels_to_indices[labels_count + label].append(indices_count + idx)
  *             indices_count += len(dataset.indices_to_labels)             # <<<<<<<<<<<<<<
  *             labels_count += len(dataset.labels_to_indices)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_12 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_indices_count, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_indices_count, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_indices_count, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":178
+    /* "learn2learn/data/meta_dataset.pyx":179
  *                 labels_to_indices[labels_count + label].append(indices_count + idx)
  *             indices_count += len(dataset.indices_to_labels)
  *             labels_count += len(dataset.labels_to_indices)             # <<<<<<<<<<<<<<
  * 
  *         self.labels_to_indices = labels_to_indices
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_12 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_12 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_labels_count, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_labels_count, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_labels_count, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":171
+    /* "learn2learn/data/meta_dataset.pyx":172
  *         labels_count = 0
  *         indices_count = 0
  *         for dataset in datasets:             # <<<<<<<<<<<<<<
  *             labels_nooffset = {label: i for i, label in enumerate(dataset.labels)}
  *             for idx, label in dataset.indices_to_labels.items():
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":180
+  /* "learn2learn/data/meta_dataset.pyx":181
  *             labels_count += len(dataset.labels_to_indices)
  * 
  *         self.labels_to_indices = labels_to_indices             # <<<<<<<<<<<<<<
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":181
+  /* "learn2learn/data/meta_dataset.pyx":182
  * 
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels             # <<<<<<<<<<<<<<
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":182
+  /* "learn2learn/data/meta_dataset.pyx":183
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_5 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_5) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_5) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":161
+  /* "learn2learn/data/meta_dataset.pyx":162
  *     """
  * 
  *     def __init__(self, datasets):             # <<<<<<<<<<<<<<
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  */
 
@@ -4344,15 +4348,15 @@
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_label);
   __Pyx_XDECREF(__pyx_v_datasets);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":184
+/* "learn2learn/data/meta_dataset.pyx":185
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         ds_count = 0
  *         for dataset in self.datasets:
  */
 
@@ -4388,32 +4392,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_item)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 185, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 185, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_item = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 185, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.UnionMetaDataset.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_2__getitem__(__pyx_self, __pyx_v_self, __pyx_v_item);
 
@@ -4436,177 +4440,177 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":185
+  /* "learn2learn/data/meta_dataset.pyx":186
  * 
  *     def __getitem__(self, item):
  *         ds_count = 0             # <<<<<<<<<<<<<<
  *         for dataset in self.datasets:
  *             if ds_count + len(dataset) > item:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_ds_count = __pyx_int_0;
 
-  /* "learn2learn/data/meta_dataset.pyx":186
+  /* "learn2learn/data/meta_dataset.pyx":187
  *     def __getitem__(self, item):
  *         ds_count = 0
  *         for dataset in self.datasets:             # <<<<<<<<<<<<<<
  *             if ds_count + len(dataset) > item:
  *                 data = list(dataset[item - ds_count])
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_datasets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_datasets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 186, __pyx_L1_error)
+          else __PYX_ERR(0, 187, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_dataset, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":187
+    /* "learn2learn/data/meta_dataset.pyx":188
  *         ds_count = 0
  *         for dataset in self.datasets:
  *             if ds_count + len(dataset) > item:             # <<<<<<<<<<<<<<
  *                 data = list(dataset[item - ds_count])
  *                 data[1] = self.indices_to_labels[item]
  */
-    __pyx_t_5 = PyObject_Length(__pyx_v_dataset); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_dataset); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyNumber_Add(__pyx_v_ds_count, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_v_ds_count, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_v_item, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_v_item, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "learn2learn/data/meta_dataset.pyx":188
+      /* "learn2learn/data/meta_dataset.pyx":189
  *         for dataset in self.datasets:
  *             if ds_count + len(dataset) > item:
  *                 data = list(dataset[item - ds_count])             # <<<<<<<<<<<<<<
  *                 data[1] = self.indices_to_labels[item]
  *                 return data
  */
-      __pyx_t_1 = PyNumber_Subtract(__pyx_v_item, __pyx_v_ds_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Subtract(__pyx_v_item, __pyx_v_ds_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_dataset, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_dataset, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PySequence_List(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __pyx_t_1 = PySequence_List(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_v_data = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":189
+      /* "learn2learn/data/meta_dataset.pyx":190
  *             if ds_count + len(dataset) > item:
  *                 data = list(dataset[item - ds_count])
  *                 data[1] = self.indices_to_labels[item]             # <<<<<<<<<<<<<<
  *                 return data
  *             ds_count += len(dataset)
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_data, 1, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_v_data, 1, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":190
+      /* "learn2learn/data/meta_dataset.pyx":191
  *                 data = list(dataset[item - ds_count])
  *                 data[1] = self.indices_to_labels[item]
  *                 return data             # <<<<<<<<<<<<<<
  *             ds_count += len(dataset)
  * 
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_data);
       __pyx_r = __pyx_v_data;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "learn2learn/data/meta_dataset.pyx":187
+      /* "learn2learn/data/meta_dataset.pyx":188
  *         ds_count = 0
  *         for dataset in self.datasets:
  *             if ds_count + len(dataset) > item:             # <<<<<<<<<<<<<<
  *                 data = list(dataset[item - ds_count])
  *                 data[1] = self.indices_to_labels[item]
  */
     }
 
-    /* "learn2learn/data/meta_dataset.pyx":191
+    /* "learn2learn/data/meta_dataset.pyx":192
  *                 data[1] = self.indices_to_labels[item]
  *                 return data
  *             ds_count += len(dataset)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
-    __pyx_t_5 = PyObject_Length(__pyx_v_dataset); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 191, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_dataset); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_ds_count, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_ds_count, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_ds_count, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":186
+    /* "learn2learn/data/meta_dataset.pyx":187
  *     def __getitem__(self, item):
  *         ds_count = 0
  *         for dataset in self.datasets:             # <<<<<<<<<<<<<<
  *             if ds_count + len(dataset) > item:
  *                 data = list(dataset[item - ds_count])
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":184
+  /* "learn2learn/data/meta_dataset.pyx":185
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         ds_count = 0
  *         for dataset in self.datasets:
  */
 
@@ -4624,15 +4628,15 @@
   __Pyx_XDECREF(__pyx_v_dataset);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":193
+/* "learn2learn/data/meta_dataset.pyx":194
  *             ds_count += len(dataset)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  * 
  */
 
@@ -4657,33 +4661,33 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":194
+  /* "learn2learn/data/meta_dataset.pyx":195
  * 
  *     def __len__(self):
  *         return len(self.indices_to_labels)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/meta_dataset.pyx":193
+  /* "learn2learn/data/meta_dataset.pyx":194
  *             ds_count += len(dataset)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  * 
  */
 
@@ -4694,15 +4698,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":222
+/* "learn2learn/data/meta_dataset.pyx":223
  *     """
  * 
  *     def __init__(self, dataset, labels):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)
  */
 
@@ -4741,40 +4745,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dataset)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 222, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 223, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_labels)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 222, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 223, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_dataset = values[1];
     __pyx_v_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 222, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.FilteredMetaDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset___init__(__pyx_self, __pyx_v_self, __pyx_v_dataset, __pyx_v_labels);
 
@@ -4804,376 +4808,376 @@
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_dataset);
 
-  /* "learn2learn/data/meta_dataset.pyx":223
+  /* "learn2learn/data/meta_dataset.pyx":224
  * 
  *     def __init__(self, dataset, labels):
  *         if not isinstance(dataset, MetaDataset):             # <<<<<<<<<<<<<<
  *             dataset = MetaDataset(dataset)
  *         self.dataset = dataset
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_3) {
 
-    /* "learn2learn/data/meta_dataset.pyx":224
+    /* "learn2learn/data/meta_dataset.pyx":225
  *     def __init__(self, dataset, labels):
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)             # <<<<<<<<<<<<<<
  *         self.dataset = dataset
  *         self.to_true_indices = []
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_dataset) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_dataset);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_dataset, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":223
+    /* "learn2learn/data/meta_dataset.pyx":224
  * 
  *     def __init__(self, dataset, labels):
  *         if not isinstance(dataset, MetaDataset):             # <<<<<<<<<<<<<<
  *             dataset = MetaDataset(dataset)
  *         self.dataset = dataset
  */
   }
 
-  /* "learn2learn/data/meta_dataset.pyx":225
+  /* "learn2learn/data/meta_dataset.pyx":226
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)
  *         self.dataset = dataset             # <<<<<<<<<<<<<<
  *         self.to_true_indices = []
  *         labels_to_indices = defaultdict(list)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dataset, __pyx_v_dataset) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dataset, __pyx_v_dataset) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":226
+  /* "learn2learn/data/meta_dataset.pyx":227
  *             dataset = MetaDataset(dataset)
  *         self.dataset = dataset
  *         self.to_true_indices = []             # <<<<<<<<<<<<<<
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices, __pyx_t_1) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices, __pyx_t_1) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":227
+  /* "learn2learn/data/meta_dataset.pyx":228
  *         self.dataset = dataset
  *         self.to_true_indices = []
  *         labels_to_indices = defaultdict(list)             # <<<<<<<<<<<<<<
  *         indices_to_labels = defaultdict(int)
  *         idx_count = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((PyObject *)(&PyList_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyList_Type)));
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_labels_to_indices = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":228
+  /* "learn2learn/data/meta_dataset.pyx":229
  *         self.to_true_indices = []
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)             # <<<<<<<<<<<<<<
  *         idx_count = 0
  *         for label in labels:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyInt_Type)));
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_indices_to_labels = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":229
+  /* "learn2learn/data/meta_dataset.pyx":230
  *         labels_to_indices = defaultdict(list)
  *         indices_to_labels = defaultdict(int)
  *         idx_count = 0             # <<<<<<<<<<<<<<
  *         for label in labels:
  *             for true_idx in dataset.labels_to_indices[label]:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_idx_count = __pyx_int_0;
 
-  /* "learn2learn/data/meta_dataset.pyx":230
+  /* "learn2learn/data/meta_dataset.pyx":231
  *         indices_to_labels = defaultdict(int)
  *         idx_count = 0
  *         for label in labels:             # <<<<<<<<<<<<<<
  *             for true_idx in dataset.labels_to_indices[label]:
  *                 self.to_true_indices.append(true_idx)
  */
   if (likely(PyList_CheckExact(__pyx_v_labels)) || PyTuple_CheckExact(__pyx_v_labels)) {
     __pyx_t_1 = __pyx_v_labels; __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 231, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 231, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 231, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_7(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 230, __pyx_L1_error)
+          else __PYX_ERR(0, 231, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_label, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":231
+    /* "learn2learn/data/meta_dataset.pyx":232
  *         idx_count = 0
  *         for label in labels:
  *             for true_idx in dataset.labels_to_indices[label]:             # <<<<<<<<<<<<<<
  *                 self.to_true_indices.append(true_idx)
  *                 labels_to_indices[label].append(idx_count)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
       __pyx_t_4 = __pyx_t_5; __Pyx_INCREF(__pyx_t_4); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
     } else {
-      __pyx_t_8 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
+      __pyx_t_8 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_9 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 231, __pyx_L1_error)
+      __pyx_t_9 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 232, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     for (;;) {
       if (likely(!__pyx_t_9)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_8); __Pyx_INCREF(__pyx_t_5); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 231, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_8); __Pyx_INCREF(__pyx_t_5); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_8); __Pyx_INCREF(__pyx_t_5); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 231, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_8); __Pyx_INCREF(__pyx_t_5); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_9(__pyx_t_4);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 231, __pyx_L1_error)
+            else __PYX_ERR(0, 232, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_v_true_idx, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":232
+      /* "learn2learn/data/meta_dataset.pyx":233
  *         for label in labels:
  *             for true_idx in dataset.labels_to_indices[label]:
  *                 self.to_true_indices.append(true_idx)             # <<<<<<<<<<<<<<
  *                 labels_to_indices[label].append(idx_count)
  *                 indices_to_labels[idx_count] = dataset.indices_to_labels[true_idx]
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 233, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_v_true_idx); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 232, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_v_true_idx); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 233, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":233
+      /* "learn2learn/data/meta_dataset.pyx":234
  *             for true_idx in dataset.labels_to_indices[label]:
  *                 self.to_true_indices.append(true_idx)
  *                 labels_to_indices[label].append(idx_count)             # <<<<<<<<<<<<<<
  *                 indices_to_labels[idx_count] = dataset.indices_to_labels[true_idx]
  *                 idx_count += 1
  */
-      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 233, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_labels_to_indices, __pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_v_idx_count); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 233, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_v_idx_count); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 234, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":234
+      /* "learn2learn/data/meta_dataset.pyx":235
  *                 self.to_true_indices.append(true_idx)
  *                 labels_to_indices[label].append(idx_count)
  *                 indices_to_labels[idx_count] = dataset.indices_to_labels[true_idx]             # <<<<<<<<<<<<<<
  *                 idx_count += 1
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_dataset, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_true_idx); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_true_idx); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 235, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_v_indices_to_labels, __pyx_v_idx_count, __pyx_t_11) < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_indices_to_labels, __pyx_v_idx_count, __pyx_t_11) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":235
+      /* "learn2learn/data/meta_dataset.pyx":236
  *                 labels_to_indices[label].append(idx_count)
  *                 indices_to_labels[idx_count] = dataset.indices_to_labels[true_idx]
  *                 idx_count += 1             # <<<<<<<<<<<<<<
  * 
  *         self.labels_to_indices = labels_to_indices
  */
-      __pyx_t_11 = __Pyx_PyInt_AddObjC(__pyx_v_idx_count, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 235, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_AddObjC(__pyx_v_idx_count, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF_SET(__pyx_v_idx_count, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "learn2learn/data/meta_dataset.pyx":231
+      /* "learn2learn/data/meta_dataset.pyx":232
  *         idx_count = 0
  *         for label in labels:
  *             for true_idx in dataset.labels_to_indices[label]:             # <<<<<<<<<<<<<<
  *                 self.to_true_indices.append(true_idx)
  *                 labels_to_indices[label].append(idx_count)
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "learn2learn/data/meta_dataset.pyx":230
+    /* "learn2learn/data/meta_dataset.pyx":231
  *         indices_to_labels = defaultdict(int)
  *         idx_count = 0
  *         for label in labels:             # <<<<<<<<<<<<<<
  *             for true_idx in dataset.labels_to_indices[label]:
  *                 self.to_true_indices.append(true_idx)
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":237
+  /* "learn2learn/data/meta_dataset.pyx":238
  *                 idx_count += 1
  * 
  *         self.labels_to_indices = labels_to_indices             # <<<<<<<<<<<<<<
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices, __pyx_v_labels_to_indices) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":238
+  /* "learn2learn/data/meta_dataset.pyx":239
  * 
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels             # <<<<<<<<<<<<<<
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels, __pyx_v_indices_to_labels) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":239
+  /* "learn2learn/data/meta_dataset.pyx":240
  *         self.labels_to_indices = labels_to_indices
  *         self.indices_to_labels = indices_to_labels
  *         self.labels = list(self.labels_to_indices.keys())             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_to_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_keys); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_keys); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_11);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_11, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_11 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_11) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_11) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":222
+  /* "learn2learn/data/meta_dataset.pyx":223
  *     """
  * 
  *     def __init__(self, dataset, labels):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)
  */
 
@@ -5195,15 +5199,15 @@
   __Pyx_XDECREF(__pyx_v_true_idx);
   __Pyx_XDECREF(__pyx_v_dataset);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":241
+/* "learn2learn/data/meta_dataset.pyx":242
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         true_idx = self.to_true_indices[item]
  *         return self.dataset[true_idx]
  */
 
@@ -5239,32 +5243,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_item)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 241, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 242, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 242, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_item = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 241, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 242, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.meta_dataset.FilteredMetaDataset.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_2__getitem__(__pyx_self, __pyx_v_self, __pyx_v_item);
 
@@ -5280,47 +5284,47 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":242
+  /* "learn2learn/data/meta_dataset.pyx":243
  * 
  *     def __getitem__(self, item):
  *         true_idx = self.to_true_indices[item]             # <<<<<<<<<<<<<<
  *         return self.dataset[true_idx]
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_to_true_indices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_true_idx = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":243
+  /* "learn2learn/data/meta_dataset.pyx":244
  *     def __getitem__(self, item):
  *         true_idx = self.to_true_indices[item]
  *         return self.dataset[true_idx]             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_true_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_true_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/meta_dataset.pyx":241
+  /* "learn2learn/data/meta_dataset.pyx":242
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         true_idx = self.to_true_indices[item]
  *         return self.dataset[true_idx]
  */
 
@@ -5333,15 +5337,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_true_idx);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/meta_dataset.pyx":245
+/* "learn2learn/data/meta_dataset.pyx":246
  *         return self.dataset[true_idx]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  */
 
 /* Python wrapper */
@@ -5365,31 +5369,31 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":246
+  /* "learn2learn/data/meta_dataset.pyx":247
  * 
  *     def __len__(self):
  *         return len(self.indices_to_labels)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/meta_dataset.pyx":245
+  /* "learn2learn/data/meta_dataset.pyx":246
  *         return self.dataset[true_idx]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  */
 
   /* function exit code */
@@ -5505,21 +5509,23 @@
   {&__pyx_n_s_indices_to_labels, __pyx_k_indices_to_labels, sizeof(__pyx_k_indices_to_labels), 0, 0, 1, 1},
   {&__pyx_n_u_indices_to_labels, __pyx_k_indices_to_labels, sizeof(__pyx_k_indices_to_labels), 0, 1, 0, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_item, __pyx_k_item, sizeof(__pyx_k_item), 0, 0, 1, 1},
   {&__pyx_n_u_item, __pyx_k_item, sizeof(__pyx_k_item), 0, 1, 0, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_keys, __pyx_k_keys, sizeof(__pyx_k_keys), 0, 0, 1, 1},
+  {&__pyx_n_s_l2l, __pyx_k_l2l, sizeof(__pyx_k_l2l), 0, 0, 1, 1},
   {&__pyx_n_s_label, __pyx_k_label, sizeof(__pyx_k_label), 0, 0, 1, 1},
   {&__pyx_n_s_labels, __pyx_k_labels, sizeof(__pyx_k_labels), 0, 0, 1, 1},
   {&__pyx_n_u_labels, __pyx_k_labels, sizeof(__pyx_k_labels), 0, 1, 0, 1},
   {&__pyx_n_s_labels_count, __pyx_k_labels_count, sizeof(__pyx_k_labels_count), 0, 0, 1, 1},
   {&__pyx_n_s_labels_nooffset, __pyx_k_labels_nooffset, sizeof(__pyx_k_labels_nooffset), 0, 0, 1, 1},
   {&__pyx_n_s_labels_to_indices, __pyx_k_labels_to_indices, sizeof(__pyx_k_labels_to_indices), 0, 0, 1, 1},
   {&__pyx_n_u_labels_to_indices, __pyx_k_labels_to_indices, sizeof(__pyx_k_labels_to_indices), 0, 1, 0, 1},
+  {&__pyx_n_s_learn2learn, __pyx_k_learn2learn, sizeof(__pyx_k_learn2learn), 0, 0, 1, 1},
   {&__pyx_n_s_learn2learn_data_meta_dataset, __pyx_k_learn2learn_data_meta_dataset, sizeof(__pyx_k_learn2learn_data_meta_dataset), 0, 0, 1, 1},
   {&__pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_k_learn2learn_data_meta_dataset_py, sizeof(__pyx_k_learn2learn_data_meta_dataset_py), 0, 0, 1, 0},
   {&__pyx_n_s_len, __pyx_k_len, sizeof(__pyx_k_len), 0, 0, 1, 1},
   {&__pyx_n_s_load, __pyx_k_load, sizeof(__pyx_k_load), 0, 0, 1, 1},
   {&__pyx_n_s_load_bookkeeping, __pyx_k_load_bookkeeping, sizeof(__pyx_k_load_bookkeeping), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
@@ -5544,198 +5550,198 @@
   {&__pyx_n_s_torch, __pyx_k_torch, sizeof(__pyx_k_torch), 0, 0, 1, 1},
   {&__pyx_n_s_torch_utils_data, __pyx_k_torch_utils_data, sizeof(__pyx_k_torch_utils_data), 0, 0, 1, 1},
   {&__pyx_n_s_true_idx, __pyx_k_true_idx, sizeof(__pyx_k_true_idx), 0, 0, 1, 1},
   {&__pyx_n_u_wb, __pyx_k_wb, sizeof(__pyx_k_wb), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 100, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 122, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 173, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "learn2learn/data/meta_dataset.pyx":51
+  /* "learn2learn/data/meta_dataset.pyx":52
  * 
  *         if not isinstance(dataset, Dataset):
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 "MetaDataset only accepts a torch dataset as input")
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_MetaDataset_only_accepts_a_torch); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_MetaDataset_only_accepts_a_torch); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "learn2learn/data/meta_dataset.pyx":122
+  /* "learn2learn/data/meta_dataset.pyx":123
  *             self.serialize_bookkeeping(path)
  *         else:
  *             with open(path, 'rb') as f:             # <<<<<<<<<<<<<<
  *                 self._bookkeeping = pickle.load(f)
  *             self.labels_to_indices = self._bookkeeping['labels_to_indices']
  */
-  __pyx_tuple__2 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "learn2learn/data/meta_dataset.pyx":48
+  /* "learn2learn/data/meta_dataset.pyx":49
  *     """
  * 
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(dataset, Dataset):
  */
-  __pyx_tuple__3 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_dataset, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_dataset, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __pyx_tuple__5 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "learn2learn/data/meta_dataset.pyx":64
+  /* "learn2learn/data/meta_dataset.pyx":65
  *             )
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.dataset[item]
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_item); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_item); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 65, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":67
+  /* "learn2learn/data/meta_dataset.pyx":68
  *         return self.dataset[item]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.dataset)
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 68, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":70
+  /* "learn2learn/data/meta_dataset.pyx":71
  *         return len(self.dataset)
  * 
  *     def create_bookkeeping(self, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  *         """
  *         Iterates over the entire dataset and creates a map of target to indices.
  */
-  __pyx_tuple__10 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_idx, __pyx_n_s_label, __pyx_n_s_i, __pyx_n_s_e, __pyx_n_s_label, __pyx_n_s_indices, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_idx, __pyx_n_s_label, __pyx_n_s_i, __pyx_n_s_e, __pyx_n_s_label, __pyx_n_s_indices, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_create_bookkeeping, 70, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_tuple__12 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_create_bookkeeping, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "learn2learn/data/meta_dataset.pyx":117
+  /* "learn2learn/data/meta_dataset.pyx":118
  *         }
  * 
  *     def load_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_f); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_f); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_load_bookkeeping, 117, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_load_bookkeeping, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 118, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":128
+  /* "learn2learn/data/meta_dataset.pyx":129
  *             self.labels = self._bookkeeping['labels']
  * 
  *     def serialize_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         with open(path, 'wb') as f:
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_f); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_f); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_serialize_bookkeeping, 128, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_serialize_bookkeeping, 129, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 129, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":161
+  /* "learn2learn/data/meta_dataset.pyx":162
  *     """
  * 
  *     def __init__(self, datasets):             # <<<<<<<<<<<<<<
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  */
-  __pyx_tuple__17 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_datasets, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_labels_count, __pyx_n_s_indices_count, __pyx_n_s_dataset, __pyx_n_s_labels_nooffset, __pyx_n_s_idx, __pyx_n_s_label, __pyx_n_s_ds, __pyx_n_s_i, __pyx_n_s_label); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_datasets, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_labels_count, __pyx_n_s_indices_count, __pyx_n_s_dataset, __pyx_n_s_labels_nooffset, __pyx_n_s_idx, __pyx_n_s_label, __pyx_n_s_ds, __pyx_n_s_i, __pyx_n_s_label); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 162, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":184
+  /* "learn2learn/data/meta_dataset.pyx":185
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         ds_count = 0
  *         for dataset in self.datasets:
  */
-  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_item, __pyx_n_s_ds_count, __pyx_n_s_dataset, __pyx_n_s_data); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_item, __pyx_n_s_ds_count, __pyx_n_s_dataset, __pyx_n_s_data); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 184, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 185, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 185, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":193
+  /* "learn2learn/data/meta_dataset.pyx":194
  *             ds_count += len(dataset)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 193, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 194, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 194, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":222
+  /* "learn2learn/data/meta_dataset.pyx":223
  *     """
  * 
  *     def __init__(self, dataset, labels):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)
  */
-  __pyx_tuple__23 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_dataset, __pyx_n_s_labels, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_idx_count, __pyx_n_s_label, __pyx_n_s_true_idx); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_dataset, __pyx_n_s_labels, __pyx_n_s_labels_to_indices, __pyx_n_s_indices_to_labels, __pyx_n_s_idx_count, __pyx_n_s_label, __pyx_n_s_true_idx); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_init, 223, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 223, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":241
+  /* "learn2learn/data/meta_dataset.pyx":242
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         true_idx = self.to_true_indices[item]
  *         return self.dataset[true_idx]
  */
-  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_item, __pyx_n_s_true_idx); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_item, __pyx_n_s_true_idx); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_getitem, 242, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 242, __pyx_L1_error)
 
-  /* "learn2learn/data/meta_dataset.pyx":245
+  /* "learn2learn/data/meta_dataset.pyx":246
  *         return self.dataset[true_idx]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 245, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_meta_dataset_py, __pyx_n_s_len, 246, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6086,26 +6092,26 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "learn2learn/data/meta_dataset.pyx":12
  * 
  * import numpy as np
  * import torch             # <<<<<<<<<<<<<<
  * from torch.utils.data import Dataset
- * 
+ * import learn2learn as l2l
  */
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_torch, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_torch, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "learn2learn/data/meta_dataset.pyx":13
  * import numpy as np
  * import torch
  * from torch.utils.data import Dataset             # <<<<<<<<<<<<<<
- * 
+ * import learn2learn as l2l
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Dataset);
   __Pyx_GIVEREF(__pyx_n_s_Dataset);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Dataset);
@@ -6114,256 +6120,268 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Dataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dataset, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":16
+  /* "learn2learn/data/meta_dataset.pyx":14
+ * import torch
+ * from torch.utils.data import Dataset
+ * import learn2learn as l2l             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_learn2learn, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_l2l, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "learn2learn/data/meta_dataset.pyx":17
  * 
  * 
  * class MetaDataset(Dataset):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_MetaDataset, __pyx_n_s_MetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Wraps_a_classificat); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_MetaDataset, __pyx_n_s_MetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Wraps_a_classificat); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "learn2learn/data/meta_dataset.pyx":48
+  /* "learn2learn/data/meta_dataset.pyx":49
  *     """
  * 
  *     def __init__(self, dataset, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(dataset, Dataset):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_1__init__, 0, __pyx_n_s_MetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_1__init__, 0, __pyx_n_s_MetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__5);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":64
+  /* "learn2learn/data/meta_dataset.pyx":65
  *             )
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.dataset[item]
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_3__getitem__, 0, __pyx_n_s_MetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_3__getitem__, 0, __pyx_n_s_MetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":67
+  /* "learn2learn/data/meta_dataset.pyx":68
  *         return self.dataset[item]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.dataset)
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_5__len__, 0, __pyx_n_s_MetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_5__len__, 0, __pyx_n_s_MetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":70
+  /* "learn2learn/data/meta_dataset.pyx":71
  *         return len(self.dataset)
  * 
  *     def create_bookkeeping(self, labels_to_indices=None, indices_to_labels=None):             # <<<<<<<<<<<<<<
  *         """
  *         Iterates over the entire dataset and creates a map of target to indices.
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_7create_bookkeeping, 0, __pyx_n_s_MetaDataset_create_bookkeeping, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_7create_bookkeeping, 0, __pyx_n_s_MetaDataset_create_bookkeeping, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__12);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_create_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_create_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":117
+  /* "learn2learn/data/meta_dataset.pyx":118
  *         }
  * 
  *     def load_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         if not os.path.exists(path):
  *             self.create_bookkeeping()
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_9load_bookkeeping, 0, __pyx_n_s_MetaDataset_load_bookkeeping, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_9load_bookkeeping, 0, __pyx_n_s_MetaDataset_load_bookkeeping, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_load_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_load_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":128
+  /* "learn2learn/data/meta_dataset.pyx":129
  *             self.labels = self._bookkeeping['labels']
  * 
  *     def serialize_bookkeeping(self, path):             # <<<<<<<<<<<<<<
  *         with open(path, 'wb') as f:
  *             pickle.dump(self._bookkeeping, f, protocol=-1)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_11serialize_bookkeeping, 0, __pyx_n_s_MetaDataset_serialize_bookkeepin, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_11MetaDataset_11serialize_bookkeeping, 0, __pyx_n_s_MetaDataset_serialize_bookkeepin, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_serialize_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_serialize_bookkeeping, __pyx_t_4) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":16
+  /* "learn2learn/data/meta_dataset.pyx":17
  * 
  * 
  * class MetaDataset(Dataset):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MetaDataset, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MetaDataset, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":133
+  /* "learn2learn/data/meta_dataset.pyx":134
  * 
  * 
  * class UnionMetaDataset(MetaDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_UnionMetaDataset, __pyx_n_s_UnionMetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Takes_multiple_Meta); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_UnionMetaDataset, __pyx_n_s_UnionMetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Takes_multiple_Meta); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "learn2learn/data/meta_dataset.pyx":161
+  /* "learn2learn/data/meta_dataset.pyx":162
  *     """
  * 
  *     def __init__(self, datasets):             # <<<<<<<<<<<<<<
  *         datasets = [
  *             MetaDataset(ds) if not isinstance(ds, MetaDataset) else ds
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_1__init__, 0, __pyx_n_s_UnionMetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_1__init__, 0, __pyx_n_s_UnionMetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":184
+  /* "learn2learn/data/meta_dataset.pyx":185
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         ds_count = 0
  *         for dataset in self.datasets:
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_3__getitem__, 0, __pyx_n_s_UnionMetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_3__getitem__, 0, __pyx_n_s_UnionMetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":193
+  /* "learn2learn/data/meta_dataset.pyx":194
  *             ds_count += len(dataset)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_5__len__, 0, __pyx_n_s_UnionMetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_16UnionMetaDataset_5__len__, 0, __pyx_n_s_UnionMetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":133
+  /* "learn2learn/data/meta_dataset.pyx":134
  * 
  * 
  * class UnionMetaDataset(MetaDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_UnionMetaDataset, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_UnionMetaDataset, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnionMetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnionMetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":197
+  /* "learn2learn/data/meta_dataset.pyx":198
  * 
  * 
  * class FilteredMetaDataset(MetaDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_FilteredMetaDataset, __pyx_n_s_FilteredMetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Takes_in_a_MetaData); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_FilteredMetaDataset, __pyx_n_s_FilteredMetaDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_kp_s_Description_Takes_in_a_MetaData); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "learn2learn/data/meta_dataset.pyx":222
+  /* "learn2learn/data/meta_dataset.pyx":223
  *     """
  * 
  *     def __init__(self, dataset, labels):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, MetaDataset):
  *             dataset = MetaDataset(dataset)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_1__init__, 0, __pyx_n_s_FilteredMetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_1__init__, 0, __pyx_n_s_FilteredMetaDataset___init, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":241
+  /* "learn2learn/data/meta_dataset.pyx":242
  *         self.labels = list(self.labels_to_indices.keys())
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         true_idx = self.to_true_indices[item]
  *         return self.dataset[true_idx]
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_3__getitem__, 0, __pyx_n_s_FilteredMetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_3__getitem__, 0, __pyx_n_s_FilteredMetaDataset___getitem, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_getitem, __pyx_t_4) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":245
+  /* "learn2learn/data/meta_dataset.pyx":246
  *         return self.dataset[true_idx]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.indices_to_labels)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_5__len__, 0, __pyx_n_s_FilteredMetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12meta_dataset_19FilteredMetaDataset_5__len__, 0, __pyx_n_s_FilteredMetaDataset___len, NULL, __pyx_n_s_learn2learn_data_meta_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_len, __pyx_t_4) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "learn2learn/data/meta_dataset.pyx":197
+  /* "learn2learn/data/meta_dataset.pyx":198
  * 
  * 
  * class FilteredMetaDataset(MetaDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_FilteredMetaDataset, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_FilteredMetaDataset, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FilteredMetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FilteredMetaDataset, __pyx_t_4) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "learn2learn/data/meta_dataset.pyx":1
  * # cython: language_version=3             # <<<<<<<<<<<<<<
```

### Comparing `learn2learn-0.1.7/learn2learn/data/meta_dataset.pyx` & `learn2learn-0.2.0/learn2learn/data/meta_dataset.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pickle
 import random
 from collections import defaultdict
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset
+import learn2learn as l2l
 
 
 class MetaDataset(Dataset):
     """
 
     **Description**
```

### Comparing `learn2learn-0.1.7/learn2learn/data/task_dataset.c` & `learn2learn-0.2.0/learn2learn/data/task_dataset.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-/* Generated by Cython 0.29.17 */
+/* Generated by Cython 0.29.24 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "learn2learn.data.task_dataset",
         "sources": [
             "learn2learn/data/task_dataset.pyx"
         ]
     },
     "module_name": "learn2learn.data.task_dataset"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_17"
-#define CYTHON_HEX_VERSION 0x001D11F0
+#define CYTHON_ABI "0_29_24"
+#define CYTHON_HEX_VERSION 0x001D18F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -434,24 +436,36 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
+  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
+  #else
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -506,14 +520,21 @@
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -545,15 +566,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -586,19 +607,18 @@
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
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -834,15 +854,15 @@
 struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription {
   PyObject_HEAD
   long index;
   PyObject *transforms;
 };
 
 
-/* "learn2learn/data/task_dataset.pyx":100
+/* "learn2learn/data/task_dataset.pyx":110
  * 
  * 
  * cdef class CythonTaskDataset:             # <<<<<<<<<<<<<<
  * 
  *     cdef public:
  */
 struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset {
@@ -1112,28 +1132,28 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
 /* CallableCheck.proto */
 #if CYTHON_USE_TYPE_SLOTS && PY_MAJOR_VERSION >= 3
-#define __Pyx_PyCallable_Check(obj)   ((obj)->ob_type->tp_call != NULL)
+#define __Pyx_PyCallable_Check(obj)   (Py_TYPE(obj)->tp_call != NULL)
 #else
 #define __Pyx_PyCallable_Check(obj)   PyCallable_Check(obj)
 #endif
 
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1321,23 +1341,28 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1374,58 +1399,67 @@
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_StopIteration;
 static PyObject *__pyx_builtin_NotImplementedError;
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_l2l[] = "l2l";
 static const char __pyx_k_new[] = "__new__";
+static const char __pyx_k_args[] = "args";
 static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_super[] = "super";
+static const char __pyx_k_utils[] = "utils";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Dataset[] = "Dataset";
+static const char __pyx_k_Taskset[] = "Taskset";
 static const char __pyx_k_collate[] = "collate";
 static const char __pyx_k_dataset[] = "dataset";
+static const char __pyx_k_message[] = "message";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_randint[] = "randint";
 static const char __pyx_k_get_task[] = "get_task";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_severity[] = "severity";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_num_tasks[] = "num_tasks";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_warn_once[] = "warn_once";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_transforms[] = "transforms";
 static const char __pyx_k_MetaDataset[] = "MetaDataset";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_TaskDataset[] = "TaskDataset";
+static const char __pyx_k_deprecation[] = "deprecation";
 static const char __pyx_k_learn2learn[] = "learn2learn";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_task_collate[] = "task_collate";
 static const char __pyx_k_StopIteration[] = "StopIteration";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_Taskset___init[] = "Taskset.__init__";
 static const char __pyx_k_DataDescription[] = "DataDescription";
 static const char __pyx_k_default_collate[] = "default_collate";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_task_transforms[] = "task_transforms";
 static const char __pyx_k_torch_utils_data[] = "torch.utils.data";
 static const char __pyx_k_CythonTaskDataset[] = "CythonTaskDataset";
@@ -1438,14 +1472,15 @@
 static const char __pyx_k_learn2learn_data_task_dataset[] = "learn2learn.data.task_dataset";
 static const char __pyx_k_General_wrapper_to_help_create[] = "\nGeneral wrapper to help create tasks.\n";
 static const char __pyx_k_pyx_unpickle_CythonTaskDataset[] = "__pyx_unpickle_CythonTaskDataset";
 static const char __pyx_k_Source_https_github_com_learnab[] = "\n    [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/data/task_dataset.py)\n\n    **Description**\n\n    Creates a set of tasks from a given Dataset.\n\n    In addition to the Dataset, TaskDataset accepts a list of task transformations (`task_transforms`)\n    which define the kind of tasks sampled from the dataset.\n\n    The tasks are lazily sampled upon indexing (or calling the `.sample()` method), and their\n    descriptions cached for later use.\n    If `num_tasks` is -1, the TaskDataset will not cache task descriptions and instead continuously resample\n    new ones.\n    In this case, the length of the TaskDataset is set to 1.\n\n    For more information on tasks and task descriptions, please refer to the\n    documentation of task transforms.\n\n    **Arguments**\n\n    * **dataset** (Dataset) - Dataset of data to compute tasks.\n    * **task_transforms** (list, *optional*, default=None) - List of task transformations.\n    * **num_tasks** (int, *optional*, default=-1) - Number of tasks to generate.\n\n    **Example**\n    ~~~python\n    dataset = l2l.data.MetaDataset(MyDataset())\n    transforms = [\n        l2l.data.transforms.NWays(dataset, n=5),\n        l2l.data.transforms.KShots(dataset, k=1),\n        l2l.data.transforms.LoadData(dataset),\n    ]\n    taskset = TaskDataset(dataset, transforms, num_tasks=20000)\n    for task in taskset:\n        X, y = task\n    ~~~\n    ";
 static const char __pyx_k_Adding_datasets_not_yet_supporte[] = "Adding datasets not yet supported for TaskDatasets.";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x8b[] = "Incompatible checksums (%s vs 0x8bc64ce = (_task_id, dataset, num_tasks, sampled_descriptions, task_collate, task_transforms))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xc3[] = "Incompatible checksums (%s vs 0xc3e47ae = (index, transforms))";
+static const char __pyx_k_TaskDataset_is_deprecated_use_Ta[] = "TaskDataset is deprecated, use Taskset instead.";
 static const char __pyx_k_learn2learn_data_task_dataset_py[] = "learn2learn/data/task_dataset.pyx";
 static const char __pyx_k_num_tasks_needs_to_be_1_infinity[] = "num_tasks needs to be -1 (infinity) or positive.";
 static PyObject *__pyx_kp_u_Adding_datasets_not_yet_supporte;
 static PyObject *__pyx_n_s_CythonTaskDataset;
 static PyObject *__pyx_n_s_DataDescription;
 static PyObject *__pyx_n_s_Dataset;
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x8b;
@@ -1453,33 +1488,40 @@
 static PyObject *__pyx_n_s_MetaDataset;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_kp_s_Source_https_github_com_learnab;
 static PyObject *__pyx_n_s_StopIteration;
 static PyObject *__pyx_n_s_TaskDataset;
 static PyObject *__pyx_n_s_TaskDataset___init;
+static PyObject *__pyx_kp_u_TaskDataset_is_deprecated_use_Ta;
+static PyObject *__pyx_n_s_Taskset;
+static PyObject *__pyx_n_s_Taskset___init;
 static PyObject *__pyx_n_s_ValueError;
+static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_collate;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_dataset;
 static PyObject *__pyx_n_s_default_collate;
+static PyObject *__pyx_n_u_deprecation;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_get_task;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_init;
+static PyObject *__pyx_n_s_kwargs;
 static PyObject *__pyx_n_s_l2l;
 static PyObject *__pyx_n_s_learn2learn;
 static PyObject *__pyx_n_s_learn2learn_data_task_dataset;
 static PyObject *__pyx_kp_s_learn2learn_data_task_dataset_py;
 static PyObject *__pyx_n_s_main;
+static PyObject *__pyx_n_s_message;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_num_tasks;
 static PyObject *__pyx_kp_u_num_tasks_needs_to_be_1_infinity;
 static PyObject *__pyx_n_s_pickle;
@@ -1499,32 +1541,36 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_sample_task_description;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_severity;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_super;
 static PyObject *__pyx_n_s_task_collate;
 static PyObject *__pyx_n_s_task_transforms;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_torch_utils_data;
 static PyObject *__pyx_n_s_torch_utils_data__utils;
 static PyObject *__pyx_n_s_transforms;
 static PyObject *__pyx_n_s_update;
+static PyObject *__pyx_n_s_utils;
+static PyObject *__pyx_n_s_warn_once;
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription___init__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, long __pyx_v_index); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_5index___get__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self); /* proto */
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_5index_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_10transforms___get__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self); /* proto */
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_10transforms_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_10transforms_4__del__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_2__reduce_cython__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_4__setstate_cython__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_dataset, PyObject *__pyx_v_task_transforms, PyObject *__pyx_v_num_tasks, PyObject *__pyx_v_task_collate); /* proto */
+static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_7Taskset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_dataset, PyObject *__pyx_v_task_transforms, PyObject *__pyx_v_num_tasks, PyObject *__pyx_v_task_collate); /* proto */
+static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static int __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset___init__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_dataset, PyObject *__pyx_v_task_transforms, int __pyx_v_num_tasks, PyObject *__pyx_v_task_collate); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_2sample_task_description(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_4get_task(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_task_description); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_6sample(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_8__len__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_10__getitem__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_i); /* proto */
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_12__iter__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self); /* proto */
@@ -1557,17 +1603,19 @@
 static PyObject *__pyx_int_205408174;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_codeobj__3;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
 /* "learn2learn/data/task_dataset.pyx":23
  * @cython.nonecheck(False)
  * @cython.infer_types(False)
  * cdef list fast_allocate(long n):             # <<<<<<<<<<<<<<
  *     cdef list result = [None] * n
@@ -1580,14 +1628,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   long __pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fast_allocate", 0);
 
   /* "learn2learn/data/task_dataset.pyx":24
  * @cython.infer_types(False)
  * cdef list fast_allocate(long n):
  *     cdef list result = [None] * n             # <<<<<<<<<<<<<<
  *     cdef long i
@@ -1674,14 +1725,17 @@
  *         self.transforms = []
  */
 
 /* Python wrapper */
 static int __pyx_pw_11learn2learn_4data_12task_dataset_15DataDescription_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_11learn2learn_4data_12task_dataset_15DataDescription_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   long __pyx_v_index;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_index,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -1724,14 +1778,17 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription___init__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, long __pyx_v_index) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "learn2learn/data/task_dataset.pyx":46
  * 
  *     def __init__(self, long index):
  *         self.index = index             # <<<<<<<<<<<<<<
  *         self.transforms = []
@@ -1795,14 +1852,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_5index___get__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->index); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -1831,14 +1891,17 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_5index_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   long __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
   __pyx_t_1 = __Pyx_PyInt_As_long(__pyx_v_value); if (unlikely((__pyx_t_1 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 7, __pyx_L1_error)
   __pyx_v_self->index = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -1899,14 +1962,17 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_10transforms_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
   if (!(likely(PyList_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(1, 8, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->transforms);
   __Pyx_DECREF(__pyx_v_self->transforms);
@@ -1981,14 +2047,17 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.index, self.transforms)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
@@ -2212,14 +2281,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_15DataDescription_4__setstate_cython__(struct __pyx_obj_11learn2learn_4data_12task_dataset_DataDescription *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_DataDescription, (type(self), 0xc3e47ae, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_DataDescription__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
@@ -2248,28 +2320,31 @@
   return __pyx_r;
 }
 
 /* "learn2learn/data/task_dataset.pyx":91
  *     """
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_11learn2learn_4data_12task_dataset_11TaskDataset___init__[] = "TaskDataset.__init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None)";
-static PyMethodDef __pyx_mdef_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11learn2learn_4data_12task_dataset_11TaskDataset___init__};
-static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_7Taskset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_11learn2learn_4data_12task_dataset_7Taskset___init__[] = "Taskset.__init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None)";
+static PyMethodDef __pyx_mdef_11learn2learn_4data_12task_dataset_7Taskset_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11learn2learn_4data_12task_dataset_7Taskset_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11learn2learn_4data_12task_dataset_7Taskset___init__};
+static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_7Taskset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_dataset = 0;
   PyObject *__pyx_v_task_transforms = 0;
   PyObject *__pyx_v_num_tasks = 0;
   PyObject *__pyx_v_task_collate = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_dataset,&__pyx_n_s_task_transforms,&__pyx_n_s_num_tasks,&__pyx_n_s_task_collate,0};
     PyObject* values[5] = {0,0,0,0,0};
     values[2] = ((PyObject *)((PyObject *)Py_None));
@@ -2345,41 +2420,44 @@
     __pyx_v_num_tasks = values[3];
     __pyx_v_task_collate = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 91, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("learn2learn.data.task_dataset.TaskDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("learn2learn.data.task_dataset.Taskset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(__pyx_self, __pyx_v_self, __pyx_v_dataset, __pyx_v_task_transforms, __pyx_v_num_tasks, __pyx_v_task_collate);
+  __pyx_r = __pyx_pf_11learn2learn_4data_12task_dataset_7Taskset___init__(__pyx_self, __pyx_v_self, __pyx_v_dataset, __pyx_v_task_transforms, __pyx_v_num_tasks, __pyx_v_task_collate);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_dataset, PyObject *__pyx_v_task_transforms, PyObject *__pyx_v_num_tasks, PyObject *__pyx_v_task_collate) {
+static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_7Taskset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_dataset, PyObject *__pyx_v_task_transforms, PyObject *__pyx_v_num_tasks, PyObject *__pyx_v_task_collate) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "learn2learn/data/task_dataset.pyx":92
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):
- *         super(TaskDataset, self).__init__(             # <<<<<<<<<<<<<<
+ *         super(Taskset, self).__init__(             # <<<<<<<<<<<<<<
  *             dataset=dataset,
  *             task_transforms=task_transforms,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TaskDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Taskset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
@@ -2390,25 +2468,25 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "learn2learn/data/task_dataset.pyx":93
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,             # <<<<<<<<<<<<<<
  *             task_transforms=task_transforms,
  *             num_tasks=num_tasks,
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dataset, __pyx_v_dataset) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
 
   /* "learn2learn/data/task_dataset.pyx":94
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,
  *             task_transforms=task_transforms,             # <<<<<<<<<<<<<<
  *             num_tasks=num_tasks,
  *             task_collate=task_collate,
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_task_transforms, __pyx_v_task_transforms) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
 
@@ -2429,62 +2507,254 @@
  * 
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_task_collate, __pyx_v_task_collate) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
 
   /* "learn2learn/data/task_dataset.pyx":92
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):
- *         super(TaskDataset, self).__init__(             # <<<<<<<<<<<<<<
+ *         super(Taskset, self).__init__(             # <<<<<<<<<<<<<<
  *             dataset=dataset,
  *             task_transforms=task_transforms,
  */
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "learn2learn/data/task_dataset.pyx":91
  *     """
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("learn2learn.data.task_dataset.Taskset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "learn2learn/data/task_dataset.pyx":102
+ * class TaskDataset(Taskset):
+ * 
+ *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_11learn2learn_4data_12task_dataset_11TaskDataset___init__[] = "TaskDataset.__init__(self, *args, **kwargs)";
+static PyMethodDef __pyx_mdef_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11learn2learn_4data_12task_dataset_11TaskDataset___init__};
+static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_self = 0;
+  PyObject *__pyx_v_args = 0;
+  PyObject *__pyx_v_kwargs = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kwargs);
+  if (PyTuple_GET_SIZE(__pyx_args) > 1) {
+    __pyx_v_args = PyTuple_GetSlice(__pyx_args, 1, PyTuple_GET_SIZE(__pyx_args));
+    if (unlikely(!__pyx_v_args)) {
+      __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+      __Pyx_RefNannyFinishContext();
+      return NULL;
+    }
+    __Pyx_GOTREF(__pyx_v_args);
+  } else {
+    __pyx_v_args = __pyx_empty_tuple; __Pyx_INCREF(__pyx_empty_tuple);
+  }
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
+    PyObject* values[1] = {0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        default:
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "__init__") < 0)) __PYX_ERR(0, 102, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+    }
+    __pyx_v_self = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 102, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
+  __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("learn2learn.data.task_dataset.TaskDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(__pyx_self, __pyx_v_self, __pyx_v_args, __pyx_v_kwargs);
+
+  /* function exit code */
+  __Pyx_XDECREF(__pyx_v_args);
+  __Pyx_XDECREF(__pyx_v_kwargs);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_11TaskDataset___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__init__", 0);
+
+  /* "learn2learn/data/task_dataset.pyx":103
+ * 
+ *     def __init__(self, *args, **kwargs):
+ *         super(TaskDataset, self).__init__(*args, **kwargs)             # <<<<<<<<<<<<<<
+ *         l2l.utils.warn_once(
+ *             message='TaskDataset is deprecated, use Taskset instead.',
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TaskDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self);
+  __Pyx_GIVEREF(__pyx_v_self);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_self);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_v_args, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "learn2learn/data/task_dataset.pyx":104
+ *     def __init__(self, *args, **kwargs):
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(             # <<<<<<<<<<<<<<
+ *             message='TaskDataset is deprecated, use Taskset instead.',
+ *             severity='deprecation',
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_l2l); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_utils); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn_once); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "learn2learn/data/task_dataset.pyx":105
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(
+ *             message='TaskDataset is deprecated, use Taskset instead.',             # <<<<<<<<<<<<<<
+ *             severity='deprecation',
+ *         )
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_message, __pyx_kp_u_TaskDataset_is_deprecated_use_Ta) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_severity, __pyx_n_u_deprecation) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+
+  /* "learn2learn/data/task_dataset.pyx":104
+ *     def __init__(self, *args, **kwargs):
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(             # <<<<<<<<<<<<<<
+ *             message='TaskDataset is deprecated, use Taskset instead.',
+ *             severity='deprecation',
+ */
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "learn2learn/data/task_dataset.pyx":102
+ * class TaskDataset(Taskset):
+ * 
+ *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("learn2learn.data.task_dataset.TaskDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":110
+/* "learn2learn/data/task_dataset.pyx":120
  *         int _task_id
  * 
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, l2l.data.MetaDataset):
  *             dataset = l2l.data.MetaDataset(dataset)
  */
 
 /* Python wrapper */
 static int __pyx_pw_11learn2learn_4data_12task_dataset_17CythonTaskDataset_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_11learn2learn_4data_12task_dataset_17CythonTaskDataset_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_dataset = 0;
   PyObject *__pyx_v_task_transforms = 0;
   int __pyx_v_num_tasks;
   PyObject *__pyx_v_task_collate = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dataset,&__pyx_n_s_task_transforms,&__pyx_n_s_num_tasks,&__pyx_n_s_task_collate,0};
     PyObject* values[4] = {0,0,0,0};
     values[1] = ((PyObject *)Py_None);
@@ -2525,15 +2795,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_task_collate);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 120, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -2543,23 +2813,23 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_dataset = values[0];
     __pyx_v_task_transforms = values[1];
     if (values[2]) {
-      __pyx_v_num_tasks = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_num_tasks == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
+      __pyx_v_num_tasks = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_num_tasks == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L3_error)
     } else {
       __pyx_v_num_tasks = ((int)-1);
     }
     __pyx_v_task_collate = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 120, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("learn2learn.data.task_dataset.CythonTaskDataset.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset___init__(((struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self), __pyx_v_dataset, __pyx_v_task_transforms, __pyx_v_num_tasks, __pyx_v_task_collate);
 
@@ -2572,149 +2842,152 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_dataset);
   __Pyx_INCREF(__pyx_v_task_transforms);
   __Pyx_INCREF(__pyx_v_task_collate);
 
-  /* "learn2learn/data/task_dataset.pyx":111
+  /* "learn2learn/data/task_dataset.pyx":121
  * 
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):
  *         if not isinstance(dataset, l2l.data.MetaDataset):             # <<<<<<<<<<<<<<
  *             dataset = l2l.data.MetaDataset(dataset)
  *         if task_transforms is None:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_l2l); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_l2l); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_3 = PyObject_IsInstance(__pyx_v_dataset, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = ((!(__pyx_t_3 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "learn2learn/data/task_dataset.pyx":112
+    /* "learn2learn/data/task_dataset.pyx":122
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):
  *         if not isinstance(dataset, l2l.data.MetaDataset):
  *             dataset = l2l.data.MetaDataset(dataset)             # <<<<<<<<<<<<<<
  *         if task_transforms is None:
  *             task_transforms = []
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_l2l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_l2l); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_MetaDataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_dataset) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_dataset);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_dataset, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":111
+    /* "learn2learn/data/task_dataset.pyx":121
  * 
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):
  *         if not isinstance(dataset, l2l.data.MetaDataset):             # <<<<<<<<<<<<<<
  *             dataset = l2l.data.MetaDataset(dataset)
  *         if task_transforms is None:
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":113
+  /* "learn2learn/data/task_dataset.pyx":123
  *         if not isinstance(dataset, l2l.data.MetaDataset):
  *             dataset = l2l.data.MetaDataset(dataset)
  *         if task_transforms is None:             # <<<<<<<<<<<<<<
  *             task_transforms = []
  *         if task_collate is None:
  */
   __pyx_t_4 = (__pyx_v_task_transforms == Py_None);
   __pyx_t_3 = (__pyx_t_4 != 0);
   if (__pyx_t_3) {
 
-    /* "learn2learn/data/task_dataset.pyx":114
+    /* "learn2learn/data/task_dataset.pyx":124
  *             dataset = l2l.data.MetaDataset(dataset)
  *         if task_transforms is None:
  *             task_transforms = []             # <<<<<<<<<<<<<<
  *         if task_collate is None:
  *             task_collate = collate.default_collate
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_task_transforms, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":113
+    /* "learn2learn/data/task_dataset.pyx":123
  *         if not isinstance(dataset, l2l.data.MetaDataset):
  *             dataset = l2l.data.MetaDataset(dataset)
  *         if task_transforms is None:             # <<<<<<<<<<<<<<
  *             task_transforms = []
  *         if task_collate is None:
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":115
+  /* "learn2learn/data/task_dataset.pyx":125
  *         if task_transforms is None:
  *             task_transforms = []
  *         if task_collate is None:             # <<<<<<<<<<<<<<
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:
  */
   __pyx_t_3 = (__pyx_v_task_collate == Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "learn2learn/data/task_dataset.pyx":116
+    /* "learn2learn/data/task_dataset.pyx":126
  *             task_transforms = []
  *         if task_collate is None:
  *             task_collate = collate.default_collate             # <<<<<<<<<<<<<<
  *         if num_tasks < -1 or num_tasks == 0:
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_collate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_collate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_default_collate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_default_collate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_task_collate, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":115
+    /* "learn2learn/data/task_dataset.pyx":125
  *         if task_transforms is None:
  *             task_transforms = []
  *         if task_collate is None:             # <<<<<<<<<<<<<<
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":117
+  /* "learn2learn/data/task_dataset.pyx":127
  *         if task_collate is None:
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:             # <<<<<<<<<<<<<<
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')
  *         self.dataset = dataset
  */
   __pyx_t_3 = ((__pyx_v_num_tasks < -1L) != 0);
@@ -2724,109 +2997,109 @@
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_3 = ((__pyx_v_num_tasks == 0) != 0);
   __pyx_t_4 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_4)) {
 
-    /* "learn2learn/data/task_dataset.pyx":118
+    /* "learn2learn/data/task_dataset.pyx":128
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')             # <<<<<<<<<<<<<<
  *         self.dataset = dataset
  *         self.num_tasks = num_tasks
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 118, __pyx_L1_error)
+    __PYX_ERR(0, 128, __pyx_L1_error)
 
-    /* "learn2learn/data/task_dataset.pyx":117
+    /* "learn2learn/data/task_dataset.pyx":127
  *         if task_collate is None:
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:             # <<<<<<<<<<<<<<
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')
  *         self.dataset = dataset
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":119
+  /* "learn2learn/data/task_dataset.pyx":129
  *         if num_tasks < -1 or num_tasks == 0:
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')
  *         self.dataset = dataset             # <<<<<<<<<<<<<<
  *         self.num_tasks = num_tasks
  *         self.task_transforms = task_transforms
  */
   __Pyx_INCREF(__pyx_v_dataset);
   __Pyx_GIVEREF(__pyx_v_dataset);
   __Pyx_GOTREF(__pyx_v_self->dataset);
   __Pyx_DECREF(__pyx_v_self->dataset);
   __pyx_v_self->dataset = __pyx_v_dataset;
 
-  /* "learn2learn/data/task_dataset.pyx":120
+  /* "learn2learn/data/task_dataset.pyx":130
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')
  *         self.dataset = dataset
  *         self.num_tasks = num_tasks             # <<<<<<<<<<<<<<
  *         self.task_transforms = task_transforms
  *         self.sampled_descriptions = {}  # Maps indices to tasks' description dict
  */
   __pyx_v_self->num_tasks = __pyx_v_num_tasks;
 
-  /* "learn2learn/data/task_dataset.pyx":121
+  /* "learn2learn/data/task_dataset.pyx":131
  *         self.dataset = dataset
  *         self.num_tasks = num_tasks
  *         self.task_transforms = task_transforms             # <<<<<<<<<<<<<<
  *         self.sampled_descriptions = {}  # Maps indices to tasks' description dict
  *         self.task_collate = task_collate
  */
   __Pyx_INCREF(__pyx_v_task_transforms);
   __Pyx_GIVEREF(__pyx_v_task_transforms);
   __Pyx_GOTREF(__pyx_v_self->task_transforms);
   __Pyx_DECREF(__pyx_v_self->task_transforms);
   __pyx_v_self->task_transforms = __pyx_v_task_transforms;
 
-  /* "learn2learn/data/task_dataset.pyx":122
+  /* "learn2learn/data/task_dataset.pyx":132
  *         self.num_tasks = num_tasks
  *         self.task_transforms = task_transforms
  *         self.sampled_descriptions = {}  # Maps indices to tasks' description dict             # <<<<<<<<<<<<<<
  *         self.task_collate = task_collate
  *         self._task_id = 0
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->sampled_descriptions);
   __Pyx_DECREF(__pyx_v_self->sampled_descriptions);
   __pyx_v_self->sampled_descriptions = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":123
+  /* "learn2learn/data/task_dataset.pyx":133
  *         self.task_transforms = task_transforms
  *         self.sampled_descriptions = {}  # Maps indices to tasks' description dict
  *         self.task_collate = task_collate             # <<<<<<<<<<<<<<
  *         self._task_id = 0
  * 
  */
   __Pyx_INCREF(__pyx_v_task_collate);
   __Pyx_GIVEREF(__pyx_v_task_collate);
   __Pyx_GOTREF(__pyx_v_self->task_collate);
   __Pyx_DECREF(__pyx_v_self->task_collate);
   __pyx_v_self->task_collate = __pyx_v_task_collate;
 
-  /* "learn2learn/data/task_dataset.pyx":124
+  /* "learn2learn/data/task_dataset.pyx":134
  *         self.sampled_descriptions = {}  # Maps indices to tasks' description dict
  *         self.task_collate = task_collate
  *         self._task_id = 0             # <<<<<<<<<<<<<<
  * 
  *     cpdef sample_task_description(self):
  */
   __pyx_v_self->_task_id = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":110
+  /* "learn2learn/data/task_dataset.pyx":120
  *         int _task_id
  * 
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
  *         if not isinstance(dataset, l2l.data.MetaDataset):
  *             dataset = l2l.data.MetaDataset(dataset)
  */
 
@@ -2843,15 +3116,15 @@
   __Pyx_XDECREF(__pyx_v_dataset);
   __Pyx_XDECREF(__pyx_v_task_transforms);
   __Pyx_XDECREF(__pyx_v_task_collate);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":126
+/* "learn2learn/data/task_dataset.pyx":136
  *         self._task_id = 0
  * 
  *     cpdef sample_task_description(self):             # <<<<<<<<<<<<<<
  *         #  Samples a new task description.
  *         # cdef list description = fast_allocate(len(self.dataset))
  */
 
@@ -2865,25 +3138,28 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   PyObject *(*__pyx_t_8)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample_task_description", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_task_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_task_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_11learn2learn_4data_12task_dataset_17CythonTaskDataset_3sample_task_description)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -2892,15 +3168,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2913,39 +3189,39 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "learn2learn/data/task_dataset.pyx":129
+  /* "learn2learn/data/task_dataset.pyx":139
  *         #  Samples a new task description.
  *         # cdef list description = fast_allocate(len(self.dataset))
  *         description = None             # <<<<<<<<<<<<<<
  *         if callable(self.task_transforms):
  *             return self.task_transforms(description)
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_description = Py_None;
 
-  /* "learn2learn/data/task_dataset.pyx":130
+  /* "learn2learn/data/task_dataset.pyx":140
  *         # cdef list description = fast_allocate(len(self.dataset))
  *         description = None
  *         if callable(self.task_transforms):             # <<<<<<<<<<<<<<
  *             return self.task_transforms(description)
  *         for transform in self.task_transforms:
  */
   __pyx_t_1 = __pyx_v_self->task_transforms;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyCallable_Check(__pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyCallable_Check(__pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "learn2learn/data/task_dataset.pyx":131
+    /* "learn2learn/data/task_dataset.pyx":141
  *         description = None
  *         if callable(self.task_transforms):
  *             return self.task_transforms(description)             # <<<<<<<<<<<<<<
  *         for transform in self.task_transforms:
  *             description = transform(description)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -2958,80 +3234,80 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_description) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_description);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "learn2learn/data/task_dataset.pyx":130
+    /* "learn2learn/data/task_dataset.pyx":140
  *         # cdef list description = fast_allocate(len(self.dataset))
  *         description = None
  *         if callable(self.task_transforms):             # <<<<<<<<<<<<<<
  *             return self.task_transforms(description)
  *         for transform in self.task_transforms:
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":132
+  /* "learn2learn/data/task_dataset.pyx":142
  *         if callable(self.task_transforms):
  *             return self.task_transforms(description)
  *         for transform in self.task_transforms:             # <<<<<<<<<<<<<<
  *             description = transform(description)
  *         return description
  */
   if (likely(PyList_CheckExact(__pyx_v_self->task_transforms)) || PyTuple_CheckExact(__pyx_v_self->task_transforms)) {
     __pyx_t_1 = __pyx_v_self->task_transforms; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_self->task_transforms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_self->task_transforms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_8(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 132, __pyx_L1_error)
+          else __PYX_ERR(0, 142, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_transform, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":133
+    /* "learn2learn/data/task_dataset.pyx":143
  *             return self.task_transforms(description)
  *         for transform in self.task_transforms:
  *             description = transform(description)             # <<<<<<<<<<<<<<
  *         return description
  * 
  */
     __Pyx_INCREF(__pyx_v_transform);
@@ -3043,43 +3319,43 @@
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_description) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_description);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_description, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":132
+    /* "learn2learn/data/task_dataset.pyx":142
  *         if callable(self.task_transforms):
  *             return self.task_transforms(description)
  *         for transform in self.task_transforms:             # <<<<<<<<<<<<<<
  *             description = transform(description)
  *         return description
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":134
+  /* "learn2learn/data/task_dataset.pyx":144
  *         for transform in self.task_transforms:
  *             description = transform(description)
  *         return description             # <<<<<<<<<<<<<<
  * 
  *     def get_task(self, task_description):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_description);
   __pyx_r = __pyx_v_description;
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":126
+  /* "learn2learn/data/task_dataset.pyx":136
  *         self._task_id = 0
  * 
  *     cpdef sample_task_description(self):             # <<<<<<<<<<<<<<
  *         #  Samples a new task description.
  *         # cdef list description = fast_allocate(len(self.dataset))
  */
 
@@ -3113,17 +3389,20 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_2sample_task_description(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample_task_description", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_11learn2learn_4data_12task_dataset_17CythonTaskDataset_sample_task_description(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_11learn2learn_4data_12task_dataset_17CythonTaskDataset_sample_task_description(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3132,15 +3411,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":136
+/* "learn2learn/data/task_dataset.pyx":146
  *         return description
  * 
  *     def get_task(self, task_description):             # <<<<<<<<<<<<<<
  *         # Given a task description, creates the corresponding batch of data.
  *         all_data = []
  */
 
@@ -3171,142 +3450,145 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_task", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":138
+  /* "learn2learn/data/task_dataset.pyx":148
  *     def get_task(self, task_description):
  *         # Given a task description, creates the corresponding batch of data.
  *         all_data = []             # <<<<<<<<<<<<<<
  *         for data_description in task_description:
  *             data = data_description.index
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_all_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":139
+  /* "learn2learn/data/task_dataset.pyx":149
  *         # Given a task description, creates the corresponding batch of data.
  *         all_data = []
  *         for data_description in task_description:             # <<<<<<<<<<<<<<
  *             data = data_description.index
  *             for transform in data_description.transforms:
  */
   if (likely(PyList_CheckExact(__pyx_v_task_description)) || PyTuple_CheckExact(__pyx_v_task_description)) {
     __pyx_t_1 = __pyx_v_task_description; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_task_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_task_description); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 139, __pyx_L1_error)
+          else __PYX_ERR(0, 149, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_data_description, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":140
+    /* "learn2learn/data/task_dataset.pyx":150
  *         all_data = []
  *         for data_description in task_description:
  *             data = data_description.index             # <<<<<<<<<<<<<<
  *             for transform in data_description.transforms:
  *                 data = transform(data)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_description, __pyx_n_s_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_description, __pyx_n_s_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":141
+    /* "learn2learn/data/task_dataset.pyx":151
  *         for data_description in task_description:
  *             data = data_description.index
  *             for transform in data_description.transforms:             # <<<<<<<<<<<<<<
  *                 data = transform(data)
  *             all_data.append(data)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_description, __pyx_n_s_transforms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_description, __pyx_n_s_transforms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
       __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 141, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 151, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 151, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_5))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 141, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 141, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_7(__pyx_t_5);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 141, __pyx_L1_error)
+            else __PYX_ERR(0, 151, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_transform, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "learn2learn/data/task_dataset.pyx":142
+      /* "learn2learn/data/task_dataset.pyx":152
  *             data = data_description.index
  *             for transform in data_description.transforms:
  *                 data = transform(data)             # <<<<<<<<<<<<<<
  *             all_data.append(data)
  *         return self.task_collate(all_data)
  */
       __Pyx_INCREF(__pyx_v_transform);
@@ -3318,50 +3600,50 @@
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
       __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "learn2learn/data/task_dataset.pyx":141
+      /* "learn2learn/data/task_dataset.pyx":151
  *         for data_description in task_description:
  *             data = data_description.index
  *             for transform in data_description.transforms:             # <<<<<<<<<<<<<<
  *                 data = transform(data)
  *             all_data.append(data)
  */
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":143
+    /* "learn2learn/data/task_dataset.pyx":153
  *             for transform in data_description.transforms:
  *                 data = transform(data)
  *             all_data.append(data)             # <<<<<<<<<<<<<<
  *         return self.task_collate(all_data)
  * 
  */
-    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_all_data, __pyx_v_data); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_all_data, __pyx_v_data); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 153, __pyx_L1_error)
 
-    /* "learn2learn/data/task_dataset.pyx":139
+    /* "learn2learn/data/task_dataset.pyx":149
  *         # Given a task description, creates the corresponding batch of data.
  *         all_data = []
  *         for data_description in task_description:             # <<<<<<<<<<<<<<
  *             data = data_description.index
  *             for transform in data_description.transforms:
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":144
+  /* "learn2learn/data/task_dataset.pyx":154
  *                 data = transform(data)
  *             all_data.append(data)
  *         return self.task_collate(all_data)             # <<<<<<<<<<<<<<
  * 
  *     def sample(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3374,22 +3656,22 @@
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_all_data) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_all_data);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":136
+  /* "learn2learn/data/task_dataset.pyx":146
  *         return description
  * 
  *     def get_task(self, task_description):             # <<<<<<<<<<<<<<
  *         # Given a task description, creates the corresponding batch of data.
  *         all_data = []
  */
 
@@ -3408,15 +3690,15 @@
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_transform);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":146
+/* "learn2learn/data/task_dataset.pyx":156
  *         return self.task_collate(all_data)
  * 
  *     def sample(self):             # <<<<<<<<<<<<<<
  *         """
  *         **Description**
  */
 
@@ -3441,30 +3723,33 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":157
+  /* "learn2learn/data/task_dataset.pyx":167
  *         ~~~
  *         """
  *         i = random.randint(0, len(self) - 1)             # <<<<<<<<<<<<<<
  *         return self[i]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_randint); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_randint); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_4 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_4 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -3473,64 +3758,64 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_int_0, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_int_0, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_i = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":158
+  /* "learn2learn/data/task_dataset.pyx":168
  *         """
  *         i = random.randint(0, len(self) - 1)
  *         return self[i]             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":146
+  /* "learn2learn/data/task_dataset.pyx":156
  *         return self.task_collate(all_data)
  * 
  *     def sample(self):             # <<<<<<<<<<<<<<
  *         """
  *         **Description**
  */
 
@@ -3546,15 +3831,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":160
+/* "learn2learn/data/task_dataset.pyx":170
  *         return self[i]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             # Ok to return 1, since __iter__ will run forever
  */
 
@@ -3573,68 +3858,68 @@
 
 static Py_ssize_t __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_8__len__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":161
+  /* "learn2learn/data/task_dataset.pyx":171
  * 
  *     def __len__(self):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             # Ok to return 1, since __iter__ will run forever
  *             # and __getitem__ will always resample.
  */
   __pyx_t_1 = ((__pyx_v_self->num_tasks == -1L) != 0);
   if (__pyx_t_1) {
 
-    /* "learn2learn/data/task_dataset.pyx":164
+    /* "learn2learn/data/task_dataset.pyx":174
  *             # Ok to return 1, since __iter__ will run forever
  *             # and __getitem__ will always resample.
  *             return 1             # <<<<<<<<<<<<<<
  *         return self.num_tasks
  * 
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "learn2learn/data/task_dataset.pyx":161
+    /* "learn2learn/data/task_dataset.pyx":171
  * 
  *     def __len__(self):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             # Ok to return 1, since __iter__ will run forever
  *             # and __getitem__ will always resample.
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":165
+  /* "learn2learn/data/task_dataset.pyx":175
  *             # and __getitem__ will always resample.
  *             return 1
  *         return self.num_tasks             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, i):
  */
   __pyx_r = __pyx_v_self->num_tasks;
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":160
+  /* "learn2learn/data/task_dataset.pyx":170
  *         return self[i]
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             # Ok to return 1, since __iter__ will run forever
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":167
+/* "learn2learn/data/task_dataset.pyx":177
  *         return self.num_tasks
  * 
  *     def __getitem__(self, i):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  */
 
@@ -3657,153 +3942,156 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":168
+  /* "learn2learn/data/task_dataset.pyx":178
  * 
  *     def __getitem__(self, i):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             return self.get_task(self.sample_task_description())
  *         if i not in self.sampled_descriptions:
  */
   __pyx_t_1 = ((__pyx_v_self->num_tasks == -1L) != 0);
   if (__pyx_t_1) {
 
-    /* "learn2learn/data/task_dataset.pyx":169
+    /* "learn2learn/data/task_dataset.pyx":179
  *     def __getitem__(self, i):
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())             # <<<<<<<<<<<<<<
  *         if i not in self.sampled_descriptions:
  *             self.sampled_descriptions[i] = self.sample_task_description()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "learn2learn/data/task_dataset.pyx":168
+    /* "learn2learn/data/task_dataset.pyx":178
  * 
  *     def __getitem__(self, i):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             return self.get_task(self.sample_task_description())
  *         if i not in self.sampled_descriptions:
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":170
+  /* "learn2learn/data/task_dataset.pyx":180
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  *         if i not in self.sampled_descriptions:             # <<<<<<<<<<<<<<
  *             self.sampled_descriptions[i] = self.sample_task_description()
  *         task_description = self.sampled_descriptions[i]
  */
   if (unlikely(__pyx_v_self->sampled_descriptions == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 170, __pyx_L1_error)
+    __PYX_ERR(0, 180, __pyx_L1_error)
   }
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_i, __pyx_v_self->sampled_descriptions, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_i, __pyx_v_self->sampled_descriptions, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_t_6 = (__pyx_t_1 != 0);
   if (__pyx_t_6) {
 
-    /* "learn2learn/data/task_dataset.pyx":171
+    /* "learn2learn/data/task_dataset.pyx":181
  *             return self.get_task(self.sample_task_description())
  *         if i not in self.sampled_descriptions:
  *             self.sampled_descriptions[i] = self.sample_task_description()             # <<<<<<<<<<<<<<
  *         task_description = self.sampled_descriptions[i]
  *         return self.get_task(task_description)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (unlikely(__pyx_v_self->sampled_descriptions == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 171, __pyx_L1_error)
+      __PYX_ERR(0, 181, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__pyx_v_self->sampled_descriptions, __pyx_v_i, __pyx_t_2) < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->sampled_descriptions, __pyx_v_i, __pyx_t_2) < 0)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":170
+    /* "learn2learn/data/task_dataset.pyx":180
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  *         if i not in self.sampled_descriptions:             # <<<<<<<<<<<<<<
  *             self.sampled_descriptions[i] = self.sample_task_description()
  *         task_description = self.sampled_descriptions[i]
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":172
+  /* "learn2learn/data/task_dataset.pyx":182
  *         if i not in self.sampled_descriptions:
  *             self.sampled_descriptions[i] = self.sample_task_description()
  *         task_description = self.sampled_descriptions[i]             # <<<<<<<<<<<<<<
  *         return self.get_task(task_description)
  * 
  */
   if (unlikely(__pyx_v_self->sampled_descriptions == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 172, __pyx_L1_error)
+    __PYX_ERR(0, 182, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->sampled_descriptions, __pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->sampled_descriptions, __pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_task_description = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":173
+  /* "learn2learn/data/task_dataset.pyx":183
  *             self.sampled_descriptions[i] = self.sample_task_description()
  *         task_description = self.sampled_descriptions[i]
  *         return self.get_task(task_description)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_task_description) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_task_description);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":167
+  /* "learn2learn/data/task_dataset.pyx":177
  *         return self.num_tasks
  * 
  *     def __getitem__(self, i):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  */
 
@@ -3818,15 +4106,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_task_description);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":175
+/* "learn2learn/data/task_dataset.pyx":185
  *         return self.get_task(task_description)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self._task_id = 0
  *         return self
  */
 
@@ -3844,51 +4132,51 @@
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_12__iter__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":176
+  /* "learn2learn/data/task_dataset.pyx":186
  * 
  *     def __iter__(self):
  *         self._task_id = 0             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->_task_id = 0;
 
-  /* "learn2learn/data/task_dataset.pyx":177
+  /* "learn2learn/data/task_dataset.pyx":187
  *     def __iter__(self):
  *         self._task_id = 0
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "learn2learn/data/task_dataset.pyx":175
+  /* "learn2learn/data/task_dataset.pyx":185
  *         return self.get_task(task_description)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self._task_id = 0
  *         return self
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":179
+/* "learn2learn/data/task_dataset.pyx":189
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  */
 
@@ -3910,132 +4198,135 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":180
+  /* "learn2learn/data/task_dataset.pyx":190
  * 
  *     def __next__(self):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             return self.get_task(self.sample_task_description())
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->num_tasks == -1L) != 0);
   if (__pyx_t_1) {
 
-    /* "learn2learn/data/task_dataset.pyx":181
+    /* "learn2learn/data/task_dataset.pyx":191
  *     def __next__(self):
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())             # <<<<<<<<<<<<<<
  * 
  *         if self._task_id < self.num_tasks:
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_task); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_11learn2learn_4data_12task_dataset_CythonTaskDataset *)__pyx_v_self->__pyx_vtab)->sample_task_description(__pyx_v_self, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "learn2learn/data/task_dataset.pyx":180
+    /* "learn2learn/data/task_dataset.pyx":190
  * 
  *     def __next__(self):
  *         if self.num_tasks == -1:             # <<<<<<<<<<<<<<
  *             return self.get_task(self.sample_task_description())
  * 
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":183
+  /* "learn2learn/data/task_dataset.pyx":193
  *             return self.get_task(self.sample_task_description())
  * 
  *         if self._task_id < self.num_tasks:             # <<<<<<<<<<<<<<
  *             task = self[self._task_id]
  *             self._task_id += 1
  */
   __pyx_t_1 = ((__pyx_v_self->_task_id < __pyx_v_self->num_tasks) != 0);
   if (likely(__pyx_t_1)) {
 
-    /* "learn2learn/data/task_dataset.pyx":184
+    /* "learn2learn/data/task_dataset.pyx":194
  * 
  *         if self._task_id < self.num_tasks:
  *             task = self[self._task_id]             # <<<<<<<<<<<<<<
  *             self._task_id += 1
  *             return task
  */
-    __pyx_t_2 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self), __pyx_v_self->_task_id, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self), __pyx_v_self->_task_id, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_task = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "learn2learn/data/task_dataset.pyx":185
+    /* "learn2learn/data/task_dataset.pyx":195
  *         if self._task_id < self.num_tasks:
  *             task = self[self._task_id]
  *             self._task_id += 1             # <<<<<<<<<<<<<<
  *             return task
  *         else:
  */
     __pyx_v_self->_task_id = (__pyx_v_self->_task_id + 1);
 
-    /* "learn2learn/data/task_dataset.pyx":186
+    /* "learn2learn/data/task_dataset.pyx":196
  *             task = self[self._task_id]
  *             self._task_id += 1
  *             return task             # <<<<<<<<<<<<<<
  *         else:
  *             raise StopIteration
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_task);
     __pyx_r = __pyx_v_task;
     goto __pyx_L0;
 
-    /* "learn2learn/data/task_dataset.pyx":183
+    /* "learn2learn/data/task_dataset.pyx":193
  *             return self.get_task(self.sample_task_description())
  * 
  *         if self._task_id < self.num_tasks:             # <<<<<<<<<<<<<<
  *             task = self[self._task_id]
  *             self._task_id += 1
  */
   }
 
-  /* "learn2learn/data/task_dataset.pyx":188
+  /* "learn2learn/data/task_dataset.pyx":198
  *             return task
  *         else:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  * 
  *     def __add__(self, other):
  */
   /*else*/ {
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 198, __pyx_L1_error)
   }
 
-  /* "learn2learn/data/task_dataset.pyx":179
+  /* "learn2learn/data/task_dataset.pyx":189
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.num_tasks == -1:
  *             return self.get_task(self.sample_task_description())
  */
 
@@ -4050,15 +4341,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_task);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":190
+/* "learn2learn/data/task_dataset.pyx":200
  *             raise StopIteration
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         msg = 'Adding datasets not yet supported for TaskDatasets.'
  *         raise NotImplementedError(msg)
  */
 
@@ -4076,37 +4367,40 @@
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_16__add__(CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_other) {
   PyObject *__pyx_v_msg = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__add__", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":191
+  /* "learn2learn/data/task_dataset.pyx":201
  * 
  *     def __add__(self, other):
  *         msg = 'Adding datasets not yet supported for TaskDatasets.'             # <<<<<<<<<<<<<<
  *         raise NotImplementedError(msg)
  */
   __Pyx_INCREF(__pyx_kp_u_Adding_datasets_not_yet_supporte);
   __pyx_v_msg = __pyx_kp_u_Adding_datasets_not_yet_supporte;
 
-  /* "learn2learn/data/task_dataset.pyx":192
+  /* "learn2learn/data/task_dataset.pyx":202
  *     def __add__(self, other):
  *         msg = 'Adding datasets not yet supported for TaskDatasets.'
  *         raise NotImplementedError(msg)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_v_msg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_v_msg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 192, __pyx_L1_error)
+  __PYX_ERR(0, 202, __pyx_L1_error)
 
-  /* "learn2learn/data/task_dataset.pyx":190
+  /* "learn2learn/data/task_dataset.pyx":200
  *             raise StopIteration
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         msg = 'Adding datasets not yet supported for TaskDatasets.'
  *         raise NotImplementedError(msg)
  */
 
@@ -4117,15 +4411,15 @@
   __pyx_r = NULL;
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":103
+/* "learn2learn/data/task_dataset.pyx":113
  * 
  *     cdef public:
  *         object dataset             # <<<<<<<<<<<<<<
  *         object task_transforms
  *         object task_collate
  */
 
@@ -4212,15 +4506,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":104
+/* "learn2learn/data/task_dataset.pyx":114
  *     cdef public:
  *         object dataset
  *         object task_transforms             # <<<<<<<<<<<<<<
  *         object task_collate
  *         dict sampled_descriptions
  */
 
@@ -4307,15 +4601,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":105
+/* "learn2learn/data/task_dataset.pyx":115
  *         object dataset
  *         object task_transforms
  *         object task_collate             # <<<<<<<<<<<<<<
  *         dict sampled_descriptions
  *         int num_tasks
  */
 
@@ -4402,15 +4696,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":106
+/* "learn2learn/data/task_dataset.pyx":116
  *         object task_transforms
  *         object task_collate
  *         dict sampled_descriptions             # <<<<<<<<<<<<<<
  *         int num_tasks
  *         int _task_id
  */
 
@@ -4456,16 +4750,19 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_20sampled_descriptions_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 116, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->sampled_descriptions);
   __Pyx_DECREF(__pyx_v_self->sampled_descriptions);
   __pyx_v_self->sampled_descriptions = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -4507,15 +4804,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":107
+/* "learn2learn/data/task_dataset.pyx":117
  *         object task_collate
  *         dict sampled_descriptions
  *         int num_tasks             # <<<<<<<<<<<<<<
  *         int _task_id
  * 
  */
 
@@ -4532,17 +4829,20 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_9num_tasks___get__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->num_tasks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->num_tasks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4568,30 +4868,33 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_9num_tasks_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
   __pyx_v_self->num_tasks = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("learn2learn.data.task_dataset.CythonTaskDataset.num_tasks.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "learn2learn/data/task_dataset.pyx":108
+/* "learn2learn/data/task_dataset.pyx":118
  *         dict sampled_descriptions
  *         int num_tasks
  *         int _task_id             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, dataset, task_transforms=None, int num_tasks=-1, task_collate=None):
  */
 
@@ -4608,17 +4911,20 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_8_task_id___get__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_task_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_task_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4644,16 +4950,19 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_8_task_id_2__set__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L1_error)
   __pyx_v_self->_task_id = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("learn2learn.data.task_dataset.CythonTaskDataset._task_id.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -4691,14 +5000,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self._task_id, self.dataset, self.num_tasks, self.sampled_descriptions, self.task_collate, self.task_transforms)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
@@ -4960,14 +5272,17 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_11learn2learn_4data_12task_dataset_17CythonTaskDataset_20__setstate_cython__(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_CythonTaskDataset, (type(self), 0x8bc64ce, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_CythonTaskDataset__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
@@ -5006,14 +5321,17 @@
 static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_11learn2learn_4data_12task_dataset___pyx_unpickle_DataDescription[] = "__pyx_unpickle_DataDescription(__pyx_type, long __pyx_checksum, __pyx_state)";
 static PyMethodDef __pyx_mdef_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription = {"__pyx_unpickle_DataDescription", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11learn2learn_4data_12task_dataset___pyx_unpickle_DataDescription};
 static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_DataDescription (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -5083,14 +5401,17 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DataDescription", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum != 0xc3e47ae:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
@@ -5272,14 +5593,17 @@
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DataDescription__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_DataDescription__set_state(DataDescription __pyx_result, tuple __pyx_state):
  *     __pyx_result.index = __pyx_state[0]; __pyx_result.transforms = __pyx_state[1]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
@@ -5406,14 +5730,17 @@
 static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_11learn2learn_4data_12task_dataset_2__pyx_unpickle_CythonTaskDataset[] = "__pyx_unpickle_CythonTaskDataset(__pyx_type, long __pyx_checksum, __pyx_state)";
 static PyMethodDef __pyx_mdef_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset = {"__pyx_unpickle_CythonTaskDataset", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11learn2learn_4data_12task_dataset_2__pyx_unpickle_CythonTaskDataset};
 static PyObject *__pyx_pw_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_CythonTaskDataset (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -5483,14 +5810,17 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CythonTaskDataset", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum != 0x8bc64ce:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
@@ -5672,14 +6002,17 @@
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CythonTaskDataset__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_CythonTaskDataset__set_state(CythonTaskDataset __pyx_result, tuple __pyx_state):
  *     __pyx_result._task_id = __pyx_state[0]; __pyx_result.dataset = __pyx_state[1]; __pyx_result.num_tasks = __pyx_state[2]; __pyx_result.sampled_descriptions = __pyx_state[3]; __pyx_result.task_collate = __pyx_state[4]; __pyx_result.task_transforms = __pyx_state[5]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 6 and hasattr(__pyx_result, '__dict__'):
@@ -6374,33 +6707,40 @@
   {&__pyx_n_s_MetaDataset, __pyx_k_MetaDataset, sizeof(__pyx_k_MetaDataset), 0, 0, 1, 1},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_kp_s_Source_https_github_com_learnab, __pyx_k_Source_https_github_com_learnab, sizeof(__pyx_k_Source_https_github_com_learnab), 0, 0, 1, 0},
   {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
   {&__pyx_n_s_TaskDataset, __pyx_k_TaskDataset, sizeof(__pyx_k_TaskDataset), 0, 0, 1, 1},
   {&__pyx_n_s_TaskDataset___init, __pyx_k_TaskDataset___init, sizeof(__pyx_k_TaskDataset___init), 0, 0, 1, 1},
+  {&__pyx_kp_u_TaskDataset_is_deprecated_use_Ta, __pyx_k_TaskDataset_is_deprecated_use_Ta, sizeof(__pyx_k_TaskDataset_is_deprecated_use_Ta), 0, 1, 0, 0},
+  {&__pyx_n_s_Taskset, __pyx_k_Taskset, sizeof(__pyx_k_Taskset), 0, 0, 1, 1},
+  {&__pyx_n_s_Taskset___init, __pyx_k_Taskset___init, sizeof(__pyx_k_Taskset___init), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_collate, __pyx_k_collate, sizeof(__pyx_k_collate), 0, 0, 1, 1},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_dataset, __pyx_k_dataset, sizeof(__pyx_k_dataset), 0, 0, 1, 1},
   {&__pyx_n_s_default_collate, __pyx_k_default_collate, sizeof(__pyx_k_default_collate), 0, 0, 1, 1},
+  {&__pyx_n_u_deprecation, __pyx_k_deprecation, sizeof(__pyx_k_deprecation), 0, 1, 0, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_get_task, __pyx_k_get_task, sizeof(__pyx_k_get_task), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
+  {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
   {&__pyx_n_s_l2l, __pyx_k_l2l, sizeof(__pyx_k_l2l), 0, 0, 1, 1},
   {&__pyx_n_s_learn2learn, __pyx_k_learn2learn, sizeof(__pyx_k_learn2learn), 0, 0, 1, 1},
   {&__pyx_n_s_learn2learn_data_task_dataset, __pyx_k_learn2learn_data_task_dataset, sizeof(__pyx_k_learn2learn_data_task_dataset), 0, 0, 1, 1},
   {&__pyx_kp_s_learn2learn_data_task_dataset_py, __pyx_k_learn2learn_data_task_dataset_py, sizeof(__pyx_k_learn2learn_data_task_dataset_py), 0, 0, 1, 0},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+  {&__pyx_n_s_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_num_tasks, __pyx_k_num_tasks, sizeof(__pyx_k_num_tasks), 0, 0, 1, 1},
   {&__pyx_kp_u_num_tasks_needs_to_be_1_infinity, __pyx_k_num_tasks_needs_to_be_1_infinity, sizeof(__pyx_k_num_tasks_needs_to_be_1_infinity), 0, 1, 0, 0},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
@@ -6420,79 +6760,94 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_sample_task_description, __pyx_k_sample_task_description, sizeof(__pyx_k_sample_task_description), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_severity, __pyx_k_severity, sizeof(__pyx_k_severity), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
   {&__pyx_n_s_task_collate, __pyx_k_task_collate, sizeof(__pyx_k_task_collate), 0, 0, 1, 1},
   {&__pyx_n_s_task_transforms, __pyx_k_task_transforms, sizeof(__pyx_k_task_transforms), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_torch_utils_data, __pyx_k_torch_utils_data, sizeof(__pyx_k_torch_utils_data), 0, 0, 1, 1},
   {&__pyx_n_s_torch_utils_data__utils, __pyx_k_torch_utils_data__utils, sizeof(__pyx_k_torch_utils_data__utils), 0, 0, 1, 1},
   {&__pyx_n_s_transforms, __pyx_k_transforms, sizeof(__pyx_k_transforms), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+  {&__pyx_n_s_utils, __pyx_k_utils, sizeof(__pyx_k_utils), 0, 0, 1, 1},
+  {&__pyx_n_s_warn_once, __pyx_k_warn_once, sizeof(__pyx_k_warn_once), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 92, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 118, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 188, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 202, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "learn2learn/data/task_dataset.pyx":118
+  /* "learn2learn/data/task_dataset.pyx":128
  *             task_collate = collate.default_collate
  *         if num_tasks < -1 or num_tasks == 0:
  *             raise ValueError('num_tasks needs to be -1 (infinity) or positive.')             # <<<<<<<<<<<<<<
  *         self.dataset = dataset
  *         self.num_tasks = num_tasks
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_num_tasks_needs_to_be_1_infinity); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_num_tasks_needs_to_be_1_infinity); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "learn2learn/data/task_dataset.pyx":91
  *     """
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,
  */
   __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_dataset, __pyx_n_s_task_transforms, __pyx_n_s_num_tasks, __pyx_n_s_task_collate); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
   __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_task_dataset_py, __pyx_n_s_init, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 91, __pyx_L1_error)
   __pyx_tuple__4 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)__pyx_int_neg_1), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
+  /* "learn2learn/data/task_dataset.pyx":102
+ * class TaskDataset(Taskset):
+ * 
+ *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(
+ */
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_learn2learn_data_task_dataset_py, __pyx_n_s_init, 102, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 102, __pyx_L1_error)
+
   /* "(tree fragment)":1
  * def __pyx_unpickle_DataDescription(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DataDescription, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CythonTaskDataset, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DataDescription, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CythonTaskDataset, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6537,38 +6892,41 @@
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
   if (PyType_Ready(&__pyx_type_11learn2learn_4data_12task_dataset_DataDescription) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_11learn2learn_4data_12task_dataset_DataDescription.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11learn2learn_4data_12task_dataset_DataDescription.tp_dictoffset && __pyx_type_11learn2learn_4data_12task_dataset_DataDescription.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11learn2learn_4data_12task_dataset_DataDescription.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DataDescription, (PyObject *)&__pyx_type_11learn2learn_4data_12task_dataset_DataDescription) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11learn2learn_4data_12task_dataset_DataDescription) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __pyx_ptype_11learn2learn_4data_12task_dataset_DataDescription = &__pyx_type_11learn2learn_4data_12task_dataset_DataDescription;
   __pyx_vtabptr_11learn2learn_4data_12task_dataset_CythonTaskDataset = &__pyx_vtable_11learn2learn_4data_12task_dataset_CythonTaskDataset;
   __pyx_vtable_11learn2learn_4data_12task_dataset_CythonTaskDataset.sample_task_description = (PyObject *(*)(struct __pyx_obj_11learn2learn_4data_12task_dataset_CythonTaskDataset *, int __pyx_skip_dispatch))__pyx_f_11learn2learn_4data_12task_dataset_17CythonTaskDataset_sample_task_description;
-  if (PyType_Ready(&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_dictoffset && __pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_dict, __pyx_vtabptr_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CythonTaskDataset, (PyObject *)&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset.tp_dict, __pyx_vtabptr_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CythonTaskDataset, (PyObject *)&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_ptype_11learn2learn_4data_12task_dataset_CythonTaskDataset = &__pyx_type_11learn2learn_4data_12task_dataset_CythonTaskDataset;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -6594,25 +6952,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
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
 __Pyx_PyMODINIT_FUNC inittask_dataset(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC inittask_dataset(void)
@@ -6689,14 +7049,17 @@
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'task_dataset' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -6736,19 +7099,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
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
   __pyx_m = Py_InitModule4("task_dataset", __pyx_methods, __pyx_k_General_wrapper_to_help_create, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -6777,22 +7138,22 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "learn2learn.data.task_dataset")) {
       if (unlikely(PyDict_SetItemString(modules, "learn2learn.data.task_dataset", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
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
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -6874,87 +7235,133 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_l2l, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "learn2learn/data/task_dataset.pyx":50
  * 
  * 
- * class TaskDataset(CythonTaskDataset):             # <<<<<<<<<<<<<<
+ * class Taskset(CythonTaskDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_11learn2learn_4data_12task_dataset_CythonTaskDataset));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_11learn2learn_4data_12task_dataset_CythonTaskDataset));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_ptype_11learn2learn_4data_12task_dataset_CythonTaskDataset));
   __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_TaskDataset, __pyx_n_s_TaskDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_task_dataset, __pyx_kp_s_Source_https_github_com_learnab); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_Taskset, __pyx_n_s_Taskset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_task_dataset, __pyx_kp_s_Source_https_github_com_learnab); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "learn2learn/data/task_dataset.pyx":91
  *     """
  * 
  *     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):             # <<<<<<<<<<<<<<
- *         super(TaskDataset, self).__init__(
+ *         super(Taskset, self).__init__(
  *             dataset=dataset,
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__, 0, __pyx_n_s_TaskDataset___init, NULL, __pyx_n_s_learn2learn_data_task_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12task_dataset_7Taskset_1__init__, 0, __pyx_n_s_Taskset___init, NULL, __pyx_n_s_learn2learn_data_task_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "learn2learn/data/task_dataset.pyx":50
  * 
  * 
- * class TaskDataset(CythonTaskDataset):             # <<<<<<<<<<<<<<
+ * class Taskset(CythonTaskDataset):             # <<<<<<<<<<<<<<
  * 
  *     """
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_TaskDataset, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_Taskset, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TaskDataset, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Taskset, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+  /* "learn2learn/data/task_dataset.pyx":100
+ * 
+ * 
+ * class TaskDataset(Taskset):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, *args, **kwargs):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Taskset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_TaskDataset, __pyx_n_s_TaskDataset, (PyObject *) NULL, __pyx_n_s_learn2learn_data_task_dataset, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  /* "learn2learn/data/task_dataset.pyx":102
+ * class TaskDataset(Taskset):
+ * 
+ *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         super(TaskDataset, self).__init__(*args, **kwargs)
+ *         l2l.utils.warn_once(
+ */
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_11learn2learn_4data_12task_dataset_11TaskDataset_1__init__, 0, __pyx_n_s_TaskDataset___init, NULL, __pyx_n_s_learn2learn_data_task_dataset, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "learn2learn/data/task_dataset.pyx":100
+ * 
+ * 
+ * class TaskDataset(Taskset):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, *args, **kwargs):
+ */
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_TaskDataset, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TaskDataset, __pyx_t_4) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "(tree fragment)":1
  * def __pyx_unpickle_DataDescription(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription, NULL, __pyx_n_s_learn2learn_data_task_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_DataDescription, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11learn2learn_4data_12task_dataset_1__pyx_unpickle_DataDescription, NULL, __pyx_n_s_learn2learn_data_task_dataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_DataDescription, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_DataDescription__set_state(<DataDescription> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_DataDescription__set_state(DataDescription __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.index = __pyx_state[0]; __pyx_result.transforms = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset, NULL, __pyx_n_s_learn2learn_data_task_dataset); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_CythonTaskDataset, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11learn2learn_4data_12task_dataset_3__pyx_unpickle_CythonTaskDataset, NULL, __pyx_n_s_learn2learn_data_task_dataset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_CythonTaskDataset, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "learn2learn/data/task_dataset.pyx":1
  * # cython: language_version=3             # <<<<<<<<<<<<<<
  * #!/usr/bin/env python3
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -7167,15 +7574,15 @@
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
@@ -7225,15 +7632,15 @@
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
@@ -8564,15 +8971,16 @@
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
     {0, 0, 0,  0, 0}
 };
 static PyObject *
 __Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
 {
 #if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromString(m->func.m_ml->ml_name);
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
 #else
     return PyString_FromString(m->func.m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
@@ -8669,26 +9077,28 @@
         for (i = 0; i < m->defaults_pyobjects; i++)
             Py_VISIT(pydefaults[i]);
     }
     return 0;
 }
 static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
 {
+#if PY_MAJOR_VERSION < 3
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
         Py_INCREF(func);
         return func;
     }
     if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
         if (type == NULL)
             type = (PyObject *)(Py_TYPE(obj));
         return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
     }
     if (obj == Py_None)
         obj = NULL;
+#endif
     return __Pyx_PyMethod_New(func, obj, type);
 }
 static PyObject*
 __Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromFormat("<cyfunction %U at %p>",
@@ -9160,45 +9570,14 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -9214,47 +9593,61 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
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
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
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
@@ -9433,17 +9826,62 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
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
```

### Comparing `learn2learn-0.1.7/learn2learn/data/task_dataset.pyx` & `learn2learn-0.2.0/learn2learn/data/task_dataset.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
 
     def __init__(self, long index):
         self.index = index
         self.transforms = []
 
 
-class TaskDataset(CythonTaskDataset):
+class Taskset(CythonTaskDataset):
 
     """
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/data/task_dataset.py)
 
     **Description**
 
     Creates a set of tasks from a given Dataset.
@@ -85,22 +85,32 @@
     taskset = TaskDataset(dataset, transforms, num_tasks=20000)
     for task in taskset:
         X, y = task
     ~~~
     """
 
     def __init__(self, dataset, task_transforms=None, num_tasks=-1, task_collate=None):
-        super(TaskDataset, self).__init__(
+        super(Taskset, self).__init__(
             dataset=dataset,
             task_transforms=task_transforms,
             num_tasks=num_tasks,
             task_collate=task_collate,
         )
 
 
+class TaskDataset(Taskset):
+
+    def __init__(self, *args, **kwargs):
+        super(TaskDataset, self).__init__(*args, **kwargs)
+        l2l.utils.warn_once(
+            message='TaskDataset is deprecated, use Taskset instead.',
+            severity='deprecation',
+        )
+
+
 cdef class CythonTaskDataset:
 
     cdef public:
         object dataset
         object task_transforms
         object task_collate
         dict sampled_descriptions
```

### Comparing `learn2learn-0.1.7/learn2learn/data/transforms.c` & `learn2learn-0.2.0/learn2learn/data/transforms.c`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/data/transforms.pyx` & `learn2learn-0.2.0/learn2learn/data/transforms.pyx`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/data/utils.py` & `learn2learn-0.2.0/learn2learn/data/utils.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/README.md` & `learn2learn-0.2.0/learn2learn/gym/README.md`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/async_vec_env.py` & `learn2learn-0.2.0/learn2learn/gym/async_vec_env.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/__init__.py` & `learn2learn-0.2.0/learn2learn/gym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/meta_env.py` & `learn2learn-0.2.0/learn2learn/gym/envs/meta_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 
     **Description**
 
     Interface for l2l envs. Environments have a certain number of task specific parameters that uniquely
     identify the environment. Tasks are then a dictionary with the names of these parameters as keys and the
     values of these parameters as values. Environments must then implement functions to get, set and sample tasks.
     The flow is then
-    ```
+
+    ~~~python
     env = EnvClass()
     tasks = env.sample_tasks(num_tasks)
     for task in tasks:
         env.set_task(task)
-        *training code here*
+        # *training code here*
         ...
-    ```
+    ~~~
 
     **Credit**
 
     Adapted from Tristan Deleu and Jonas Rothfuss' implementations.
 
     """
 
     def __init__(self, task=None):
-        super(Env, self).__init__()
+        super(MetaEnv, self).__init__()
         if task is None:
             task = self.sample_tasks(1)[0]
         self.set_task(task)
 
     def sample_tasks(self, num_tasks):
         """
         **Description**
```

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/metaworld/metaworld.py` & `learn2learn-0.2.0/learn2learn/gym/envs/metaworld/metaworld.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/ant_direction.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/ant_direction.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/ant_forward_backward.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/ant_forward_backward.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/dummy_mujoco_env.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/dummy_mujoco_env.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/halfcheetah_forward_backward.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/halfcheetah_forward_backward.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/humanoid_direction.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/humanoid_direction.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/mujoco/humanoid_forward_backward.py` & `learn2learn-0.2.0/learn2learn/gym/envs/mujoco/humanoid_forward_backward.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/particles/particles_2d.py` & `learn2learn-0.2.0/learn2learn/gym/envs/particles/particles_2d.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/gym/envs/subproc_vec_env.py` & `learn2learn-0.2.0/learn2learn/gym/envs/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/nn/kroneckers.py` & `learn2learn-0.2.0/learn2learn/nn/kroneckers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     Returns alpha * (mat2.t() X mat1) @ vec(mat3) + beta * vec(bias)
     (Assuming bias is not None.)
     """
     res = mat1 @ mat3 @ mat2
     res.mul_(alpha)
     if bias is not None:
-        res.add_(beta, bias)
+        res.add_(alpha=beta, other=bias)
     return res
 
 
 class KroneckerLinear(nn.Module):
 
     r"""
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/nn/kroneckers.py)
@@ -165,20 +165,21 @@
 
     **References**
 
     1. Jose et al. 2018. "Kronecker recurrent units".
 
     **Example**
     ~~~python
-    m, n = 2, 3
-    x = torch.randn(6)
-    h = torch.randn(6)
+    n, m = 2, 3
+    x = torch.randn(n, m)
+    h = torch.randn(n, m)
+    c = torch.zeros(n, m)
     kronecker = KroneckerLSTM(n, m)
-    y, new_h = kronecker(x, h)
-    y.shape  # (6, )
+    y, new_h = kronecker(x, (h, c))
+    y.shape  # (2, 3)
     ~~~
     """
 
     def __init__(self, n, m, bias=True, sigma=None):
         super(KroneckerLSTM, self).__init__()
         self.W_ii = KroneckerLinear(n, m, bias=bias)
         self.W_hi = KroneckerLinear(n, m, bias=bias)
```

### Comparing `learn2learn-0.1.7/learn2learn/nn/metaoptnet.py` & `learn2learn-0.2.0/learn2learn/nn/metaoptnet.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/nn/misc.py` & `learn2learn-0.2.0/learn2learn/nn/misc.py`

 * *Files 27% similar despite different names*

```diff
@@ -82,7 +82,62 @@
         elif shape is None:
             shape = (1, )
         alpha = torch.ones(*shape) * alpha
         self.alpha = torch.nn.Parameter(alpha)
 
     def forward(self, x):
         return x * self.alpha
+
+
+def freeze(module):
+    """
+    [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/nn/misc.py)
+
+    **Description**
+
+    Prevents all parameters in `module` to get gradients.
+
+    Note: the module is modified in-place.
+
+    **Arguments**
+
+    * **module** (Module) - The module to freeze.
+
+    **Example**
+    ~~~python
+    linear = torch.nn.Linear(128, 4)
+    l2l.nn.freeze(linear)
+    ~~~
+    """
+    for p in module.parameters():
+        p.detach_()
+        if hasattr(p, 'requires_grad'):
+            p.requires_grad = False
+    return module
+
+
+def unfreeze(module):
+    """
+    [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/nn/misc.py)
+
+    **Description**
+
+    Enables all parameters in `module` to compute gradients.
+
+    Note: the module is modified in-place.
+
+    **Arguments**
+
+    * **module** (Module) - The module to unfreeze.
+
+    **Example**
+
+    ~~~python
+    linear = torch.nn.Linear(128, 4)
+    l2l.nn.freeze(linear)
+    l2l.nn.unfreeze(linear)
+    ~~~
+    """
+    for p in module.parameters():
+        if hasattr(p, 'requires_grad'):
+            p.requires_grad = True
+    return module
```

### Comparing `learn2learn-0.1.7/learn2learn/nn/protonet.py` & `learn2learn-0.2.0/learn2learn/nn/protonet.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/learnable_optimizer.py` & `learn2learn-0.2.0/learn2learn/optim/learnable_optimizer.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/parameter_update.py` & `learn2learn-0.2.0/learn2learn/optim/parameter_update.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/transforms/__init__.py` & `learn2learn-0.2.0/learn2learn/optim/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/transforms/kronecker_transform.py` & `learn2learn-0.2.0/learn2learn/optim/transforms/kronecker_transform.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/transforms/metacurvature_transform.py` & `learn2learn-0.2.0/learn2learn/optim/transforms/metacurvature_transform.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/transforms/module_transform.py` & `learn2learn-0.2.0/learn2learn/optim/transforms/module_transform.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/transforms/transform_dictionary.py` & `learn2learn-0.2.0/learn2learn/optim/transforms/transform_dictionary.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/optim/update_rules/differentiable_sgd.py` & `learn2learn-0.2.0/learn2learn/optim/update_rules/differentiable_sgd.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/text/datasets/news_classification.py` & `learn2learn-0.2.0/learn2learn/text/datasets/news_classification.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/utils/__init__.py` & `learn2learn-0.2.0/learn2learn/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import copy
 import torch
 import argparse
 import dataclasses
+import warnings
 
 
 def magic_box(x):
     """
 
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/utils.py)
 
@@ -46,14 +47,18 @@
     return x
 
 
 def clone_parameters(param_list):
     return [p.clone() for p in param_list]
 
 
+def clone_named_parameters(param_dict):
+    return {k: p.clone() for k, p in param_dict.items()}
+
+
 def clone_module(module, memo=None):
     """
 
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/utils.py)
 
     **Description**
 
@@ -128,15 +133,15 @@
                 buff = module._buffers[buffer_key]
                 buff_ptr = buff.data_ptr
                 if buff_ptr in memo:
                     clone._buffers[buffer_key] = memo[buff_ptr]
                 else:
                     cloned = buff.clone()
                     clone._buffers[buffer_key] = cloned
-                    memo[param_ptr] = cloned
+                    memo[buff_ptr] = cloned
 
     # Then, recurse for each submodule
     if hasattr(clone, '_modules'):
         for module_key in clone._modules:
             clone._modules[module_key] = clone_module(
                 module._modules[module_key],
                 memo=memo,
@@ -167,17 +172,17 @@
     * **keep_requires_grad** (bool) - By default, all parameters of the detached module will have
     `requires_grad` set to `False`. If this flag is set to `True`, then the `requires_grad` field
     will be the same as the pre-detached module.
 
     **Example**
 
     ~~~python
-    net = nn.Sequential(Linear(20, 10), nn.ReLU(), nn.Linear(10, 2))
+    net = nn.Sequential(nn.Linear(20, 10), nn.ReLU(), nn.Linear(10, 2))
     clone = clone_module(net)
-    detach_module(clone)
+    detach_module(clone, keep_requires_grad=True)
     error = loss(clone(X), y)
     error.backward()  # Gradients are back-propagate on clone, not net.
     ~~~
     """
     if not isinstance(module, torch.nn.Module):
         return
     # First, re-write all parameters
@@ -365,7 +370,31 @@
         raise ImportError(msg)
 
     def __getattr__(self, *args, **kwargs):
         self.raise_import()
 
     def __call__(self, *args, **kwargs):
         self.raise_import()
+
+
+class _SingleWarning(object):
+
+    def __init__(self):
+        self.warned_messages = []
+        self.warning_categories = {
+            'default': UserWarning,
+            'deprecation': DeprecationWarning,
+        }
+
+    def __call__(self, message, severity=None):
+        if message not in self.warned_messages:
+            if severity is None:
+                severity = 'default'
+            if severity == 'error':
+                raise RuntimeError(message)
+            elif isinstance(severity, str):
+                severity = self.warning_categories[severity]
+            warnings.warn(message, category=severity)
+            self.warned_messages.append(message)
+
+
+warn_once = _SingleWarning()
```

### Comparing `learn2learn-0.1.7/learn2learn/utils/lightning.py` & `learn2learn-0.2.0/learn2learn/utils/lightning.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         length = self.epoch_length
         return EpisodicBatcher.epochify(
             self.test_tasks,
             length,
         )
 
 
-class NoLeaveProgressBar(pl.callbacks.ProgressBar):
+class NoLeaveProgressBar(pl.callbacks.TQDMProgressBar):
 
     def init_test_tqdm(self):
         bar = tqdm.tqdm(
             desc='Testing',
             position=(2 * self.process_position),
             disable=self.is_disabled,
             leave=False,
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/__init__.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 """
 The benchmark modules provides a convenient interface to standardized benchmarks in the literature.
-It provides train/validation/test TaskDatasets and TaskTransforms for pre-defined datasets.
+It provides train/validation/test Tasksets and TaskTransforms for pre-defined datasets.
 
 This utility is useful for researchers to compare new algorithms against existing benchmarks.
-For a more fine-grained control over tasks and data, we recommend directly using `l2l.data.TaskDataset` and `l2l.data.TaskTransforms`.
+For a more fine-grained control over tasks and data, we recommend directly using `l2l.data.Taskset` and `l2l.data.TaskTransforms`.
 """
 
 import os
 import learn2learn as l2l
 
 from collections import namedtuple
 from .omniglot_benchmark import omniglot_tasksets
@@ -66,25 +66,25 @@
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/vision/benchmarks/)
 
     **Description**
 
     Returns the tasksets for a particular benchmark, using literature standard data and task transformations.
 
     The returned object is a namedtuple with attributes `train`, `validation`, `test` which
-    correspond to their respective TaskDatasets.
+    correspond to their respective Tasksets.
     See `examples/vision/maml_miniimagenet.py` for an example.
 
     **Arguments**
 
     * **name** (str) - The name of the benchmark. Full list in `list_tasksets()`.
     * **train_ways** (int, *optional*, default=5) - The number of classes per train tasks.
     * **train_samples** (int, *optional*, default=10) - The number of samples per train tasks.
     * **test_ways** (int, *optional*, default=5) - The number of classes per test tasks. Also used for validation tasks.
     * **test_samples** (int, *optional*, default=10) - The number of samples per test tasks. Also used for validation tasks.
-    * **num_tasks** (int, *optional*, default=-1) - The number of tasks in each TaskDataset.
+    * **num_tasks** (int, *optional*, default=-1) - The number of tasks in each Taskset.
     * **device** (torch.Device, *optional*, default=None) - If not None, tasksets are loaded as Tensors on `device`.
     * **root** (str, *optional*, default='~/data') - Where the data is stored.
 
     **Example**
     ~~~python
     train_tasks, validation_tasks, test_tasks = l2l.vision.benchmarks.get_tasksets('omniglot')
     batch = train_tasks.sample()
@@ -105,23 +105,23 @@
                                            root=root,
                                            device=device,
                                            **kwargs)
     train_dataset, validation_dataset, test_dataset = datasets
     train_transforms, validation_transforms, test_transforms = transforms
 
     # Instantiate the tasksets
-    train_tasks = l2l.data.TaskDataset(
+    train_tasks = l2l.data.Taskset(
         dataset=train_dataset,
         task_transforms=train_transforms,
         num_tasks=num_tasks,
     )
-    validation_tasks = l2l.data.TaskDataset(
+    validation_tasks = l2l.data.Taskset(
         dataset=validation_dataset,
         task_transforms=validation_transforms,
         num_tasks=num_tasks,
     )
-    test_tasks = l2l.data.TaskDataset(
+    test_tasks = l2l.data.Taskset(
         dataset=test_dataset,
         task_transforms=test_transforms,
         num_tasks=num_tasks,
     )
     return BenchmarkTasksets(train_tasks, validation_tasks, test_tasks)
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/cifarfs_benchmark.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/cifarfs_benchmark.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/fc100_benchmark.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/fc100_benchmark.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/mini_imagenet_benchmark.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/mini_imagenet_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             ToTensor(),
             normalize,
         ])
         test_data_transforms = Compose([
             normalize,
         ])
     else:
-        raise('Invalid data_augmentation argument.')
+        raise ValueError('Invalid data_augmentation argument.')
 
     train_dataset = l2l.vision.datasets.MiniImagenet(
         root=root,
         mode='train',
         download=True,
     )
     valid_dataset = l2l.vision.datasets.MiniImagenet(
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/omniglot_benchmark.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/omniglot_benchmark.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/benchmarks/tiered_imagenet_benchmark.py` & `learn2learn-0.2.0/learn2learn/vision/benchmarks/tiered_imagenet_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             normalize,
         ])
         test_data_transforms = Compose([
             to_tensor,
             normalize,
         ])
     else:
-        raise('Invalid data_augmentation argument.')
+        raise ValueError('Invalid data_augmentation argument.')
 
     train_dataset = l2l.vision.datasets.TieredImagenet(
         root=root,
         mode='train',
         transform=ToTensor(),
         download=True,
     )
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/__init__.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/cifarfs.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/cifarfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import shutil
 import zipfile
 import numpy as np
 import torch
 import torch.utils.data as data
 
 from torchvision.datasets import ImageFolder
-from learn2learn.data.utils import download_file_from_google_drive
+from learn2learn.data.utils import (
+    download_file_from_google_drive,
+    download_file,
+)
 
 
 class CIFARFS(ImageFolder):
 
     """
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/vision/datasets/cifarfs.py)
 
@@ -80,19 +83,28 @@
 
     def _download(self):
         # Download the zip, unzip it, and clean up
         print('Downloading CIFARFS to ', self.root)
         if not os.path.exists(self.root):
             os.mkdir(self.root)
         zip_file = os.path.join(self.root, 'cifarfs.zip')
-        download_file_from_google_drive('1pTsCCMDj45kzFYgrnO67BWVbKs48Q3NI',
-                                        zip_file)
-        with zipfile.ZipFile(zip_file, 'r') as zfile:
-            zfile.extractall(self.raw_path)
-        os.remove(zip_file)
+        try:
+            download_file(
+                source='https://zenodo.org/record/7978538/files/cifar100.zip',
+                destination=zip_file,
+            )
+            with zipfile.ZipFile(zip_file, 'r') as zfile:
+                zfile.extractall(self.raw_path)
+            os.remove(zip_file)
+        except Exception:
+            download_file_from_google_drive('1pTsCCMDj45kzFYgrnO67BWVbKs48Q3NI',
+                                            zip_file)
+            with zipfile.ZipFile(zip_file, 'r') as zfile:
+                zfile.extractall(self.raw_path)
+            os.remove(zip_file)
 
     def _process_zip(self):
         print('Creating CIFARFS splits')
         if not os.path.exists(self.processed_root):
             os.mkdir(self.processed_root)
         split_path = os.path.join(self.raw_path, 'cifar100', 'splits', 'bertinetto')
         train_split_file = os.path.join(split_path, 'train.txt')
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/cu_birds200.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/cu_birds200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python3
 
 import os
 import tarfile
 import torch
 
 from PIL import Image
-from learn2learn.data.utils import download_file_from_google_drive
+from learn2learn.data.utils import (
+    download_file_from_google_drive,
+    download_file,
+)
 
 DATA_DIR = 'cubirds200'
 DATA_FILENAME = 'CUB_200_2011.tgz'
 ARCHIVE_ID = '1hbzc_P1FuxMkcabkgn9ZKinBwW683j45'
+ZENODO_URL = 'https://zenodo.org/record/8000562/files/CUB_200_2011.tgz'
 
 SPLITS = {
     'train': [
         '190.Red_cockaded_Woodpecker',
         '144.Common_Tern',
         '014.Indigo_Bunting',
         '012.Yellow_headed_Blackbird',
@@ -307,15 +311,15 @@
     * **bounding_box_crop** (bool, *optional*, default=False) - Whether to crop each image using bounding box information.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.CUBirds200(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
     def __init__(
         self,
         root,
@@ -349,19 +353,26 @@
 
     def download(self):
         # Download and extract the data
         data_path = os.path.join(self.root, DATA_DIR)
         os.makedirs(data_path, exist_ok=True)
         tar_path = os.path.join(data_path, DATA_FILENAME)
         print('Downloading CUBirds200 dataset. (1.1Gb)')
-        download_file_from_google_drive(ARCHIVE_ID, tar_path)
-        tar_file = tarfile.open(tar_path)
-        tar_file.extractall(data_path)
-        tar_file.close()
-        os.remove(tar_path)
+        try:
+            download_file(ZENODO_URL, tar_path)
+            tar_file = tarfile.open(tar_path)
+            tar_file.extractall(data_path)
+            tar_file.close()
+            os.remove(tar_path)
+        except Exception:
+            download_file_from_google_drive(ARCHIVE_ID, tar_path)
+            tar_file = tarfile.open(tar_path)
+            tar_file.extractall(data_path)
+            tar_file.close()
+            os.remove(tar_path)
 
     def load_data(self, mode='train'):
         classes = sum(SPLITS.values(), []) if mode == 'all' else SPLITS[mode]
         images_path = os.path.join(
             self.root,
             DATA_DIR,
             'CUB_200_2011',
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/describable_textures.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/describable_textures.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     * **download** (bool, *optional*, default=False) - Whether to download the dataset.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.DescribableTextures(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
     def __init__(
         self,
         root,
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/fc100.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/fc100.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import pickle
 import zipfile
 
 import torch.utils.data as data
 
 from PIL import Image
 
-from learn2learn.data.utils import download_file_from_google_drive, download_file
-
-
-GOOGLE_DRIVE_FILE_ID = '1_ZsLyqI487NRDQhwvI7rg86FK3YAZvz1'
-DROPBOX_LINK = 'https://www.dropbox.com/s/ftsjuwsu6lfp0fz/FC100.zip?dl=1'
+from learn2learn.data.utils import (
+    download_file_from_google_drive,
+    download_file,
+)
 
 
 class FC100(data.Dataset):
     """
     [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/vision/datasets/fc100.py)
 
     **Description**
@@ -45,19 +44,23 @@
     * **target_transform** (Transform, *optional*, default=None) - Target pre-processing.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.FC100(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
+    GOOGLE_DRIVE_FILE_ID = '1_ZsLyqI487NRDQhwvI7rg86FK3YAZvz1'
+    DROPBOX_LINK = 'https://www.dropbox.com/s/ftsjuwsu6lfp0fz/FC100.zip?dl=1'
+    ZENODO_LINK = 'https://zenodo.org/record/7978538/files/fc100.zip'
+
     def __init__(self,
                  root,
                  mode='train',
                  transform=None,
                  target_transform=None,
                  download=False):
         super(FC100, self).__init__()
@@ -81,25 +84,31 @@
             archive = u.load()
         self.images = archive['data']
         self.labels = archive['labels']
 
     def download(self):
         archive_path = os.path.join(self.root, 'fc100.zip')
         print('Downloading FC100. (160Mb)')
-        try:  # Download from Google Drive first
-            download_file_from_google_drive(GOOGLE_DRIVE_FILE_ID,
-                                            archive_path)
-            archive_file = zipfile.ZipFile(archive_path)
-            archive_file.extractall(self.root)
-            os.remove(archive_path)
-        except zipfile.BadZipFile:
-            download_file(DROPBOX_LINK, archive_path)
+        try:
+            download_file(FC100.ZENODO_LINK, archive_path)
             archive_file = zipfile.ZipFile(archive_path)
             archive_file.extractall(self.root)
             os.remove(archive_path)
+        except Exception:
+            try:  # Download from Google Drive first
+                download_file_from_google_drive(FC100.GOOGLE_DRIVE_FILE_ID,
+                                                archive_path)
+                archive_file = zipfile.ZipFile(archive_path)
+                archive_file.extractall(self.root)
+                os.remove(archive_path)
+            except zipfile.BadZipFile:
+                download_file(FC100.DROPBOX_LINK, archive_path)
+                archive_file = zipfile.ZipFile(archive_path)
+                archive_file.extractall(self.root)
+                os.remove(archive_path)
 
     def __getitem__(self, idx):
         image = self.images[idx]
         image = Image.fromarray(image)
         label = self.labels[idx]
         if self.transform is not None:
             image = self.transform(image)
@@ -112,13 +121,14 @@
 
     def _check_exists(self):
         return os.path.exists(os.path.join(self.root,
                                            'FC100_train.pickle'))
 
 
 if __name__ == '__main__':
+    __import__('pdb').set_trace()
     dataset = FC100(root='~/data')
     img, tgt = dataset[43]
     dataset = FC100(root='~/data', mode='validation')
     img, tgt = dataset[43]
     dataset = FC100(root='~/data', mode='test')
     img, tgt = dataset[43]
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/fgvc_aircraft.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/fgvc_aircraft.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     * **bounding_box_crop** (bool, *optional*, default=False) - Whether to crop each image using bounding box information.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.FGVCAircraft(root='./data', mode='train', download=True)
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
     def __init__(
         self,
         root,
@@ -111,15 +111,16 @@
         bounding_box_crop=False,
     ):
         root = os.path.expanduser(root)
         self.root = os.path.expanduser(root)
         self.transform = transform
         self.target_transform = target_transform
         self.bounding_box_crop = bounding_box_crop
-        self._bookkeeping_path = os.path.join(self.root, 'fgvc-aircraft-' + mode + '-bookkeeping.pkl')
+        self._bookkeeping_path = os.path.join(
+            self.root, 'fgvc-aircraft-' + mode + '-bookkeeping.pkl')
 
         if not self._check_exists() and download:
             self.download()
 
         assert mode in ['train', 'validation', 'test', 'all'], \
             'mode should be one of: train, validation, test, all.'
         self.load_data(mode)
@@ -143,21 +144,41 @@
             print('Downloading FGVC Aircraft dataset. (2.75Gb)')
             req = requests.get(DATASET_URL)
             with open(tar_path, 'wb') as archive:
                 for chunk in req.iter_content(chunk_size=32768):
                     if chunk:
                         archive.write(chunk)
         with tarfile.open(tar_path) as tar_file:
-            tar_file.extractall(data_path)
-        family_names = ['images_family_train.txt',
-                        'images_family_val.txt',
-                        'images_family_test.txt']
+            def is_within_directory(directory, target):
+
+                abs_directory = os.path.abspath(directory)
+                abs_target = os.path.abspath(target)
+
+                prefix = os.path.commonprefix([abs_directory, abs_target])
+
+                return prefix == abs_directory
+
+            def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+
+                for member in tar.getmembers():
+                    member_path = os.path.join(path, member.name)
+                    if not is_within_directory(path, member_path):
+                        raise Exception("Attempted Path Traversal in Tar File")
+
+                tar.extractall(path, members, numeric_owner=numeric_owner)
+
+            safe_extract(tar_file, data_path)
+        family_names = [
+            'images_variant_train.txt',
+            'images_variant_val.txt',
+            'images_variant_test.txt',
+        ]
         images_labels = []
         for family in family_names:
-            with open(os.path.join(data_path, DATA_DIR, family_names[0]), 'r') as family_file:
+            with open(os.path.join(data_path, DATA_DIR, family), 'r') as family_file:
                 for line in family_file.readlines():
                     image, label = line.split(' ', 1)
                     images_labels.append((image.strip(), label.strip()))
         labels_path = os.path.join(data_path, LABELS_PATH)
         with open(labels_path, 'wb') as labels_file:
             pickle.dump(images_labels, labels_file)
         os.remove(tar_path)
@@ -187,15 +208,16 @@
                         int(line[3]),
                         int(line[4]),
                     )
 
         # read images from disk
         for image, label in image_labels:
             if label in split:
-                image_path = os.path.join(data_path, IMAGES_DIR, image + '.jpg')
+                image_path = os.path.join(
+                    data_path, IMAGES_DIR, image + '.jpg')
                 if self.bounding_box_crop:
                     self.bounding_boxes[image_path] = bbox_content[image]
                 label = split.index(label)
                 data.append((image_path, label))
         self.data = data
 
     def __getitem__(self, i):
@@ -211,20 +233,36 @@
         return image, label
 
     def __len__(self):
         return len(self.data)
 
 
 if __name__ == '__main__':
-    assert len(SPLITS['all']) == len(SPLITS['train']) + len(SPLITS['valid']) + len(SPLITS['test'])
+    assert len(SPLITS['all']) == len(SPLITS['train']) + \
+        len(SPLITS['valid']) + len(SPLITS['test'])
     aircraft = FGVCAircraft('~/data', download=True, bounding_box_crop=True)
     img = aircraft[0]
     print(len(aircraft))
 
     import numpy as np
     import tqdm
     print('cropped:')
     data = FGVCAircraft('~/data', download=True, bounding_box_crop=True)
     min_size = float('inf')
     for img, label in tqdm.tqdm(data):
         min_size = min(min_size, *np.array(img).shape[:2])
     print('min_size:', min_size)
+
+    data = FGVCAircraft(
+        root="test_data/",
+        mode="all",
+        download=True,
+        bounding_box_crop=False,
+    )
+
+    label_set = set()
+
+    with tqdm.tqdm(total=len(data)) as pbar:
+        for item in data:
+            label_set.add(item[1])
+            pbar.update(1)
+            pbar.set_description(f"Found {len(label_set)} labels")
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/fgvc_fungi.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/fgvc_fungi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1455,15 +1455,15 @@
     * **download** (bool, *optional*, default=False) - Whether to download the dataset.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.FGVCFungi(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
     def __init__(self, root, mode='all', transform=None, target_transform=None, download=False):
         root = os.path.expanduser(root)
         self.root = os.path.expanduser(root)
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/full_omniglot.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/full_omniglot.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/mini_imagenet.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/mini_imagenet.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 import os
 import pickle
 
 import numpy as np
 import torch
 import torch.utils.data as data
 
-from learn2learn.data.utils import download_file_from_google_drive, download_file
+from learn2learn.data.utils import (
+    download_file_from_google_drive,
+    download_file,
+)
 
 
 def download_pkl(google_drive_id, data_root, mode):
     filename = 'mini-imagenet-cache-' + mode
     file_path = os.path.join(data_root, filename)
 
     if not os.path.exists(file_path + '.pkl'):
@@ -83,51 +86,61 @@
         self.transform = transform
         self.target_transform = target_transform
         self.mode = mode
         self._bookkeeping_path = os.path.join(self.root, 'mini-imagenet-bookkeeping-' + mode + '.pkl')
         if self.mode == 'test':
             google_drive_file_id = '1wpmY-hmiJUUlRBkO9ZDCXAcIpHEFdOhD'
             dropbox_file_link = 'https://www.dropbox.com/s/ye9jeb5tyz0x01b/mini-imagenet-cache-test.pkl?dl=1'
+            zenodo_file_link = 'https://zenodo.org/record/7978538/files/mini-imagenet-cache-test.pkl'
         elif self.mode == 'train':
             google_drive_file_id = '1I3itTXpXxGV68olxM5roceUMG8itH9Xj'
             dropbox_file_link = 'https://www.dropbox.com/s/9g8c6w345s2ek03/mini-imagenet-cache-train.pkl?dl=1'
+            zenodo_file_link = 'https://zenodo.org/record/7978538/files/mini-imagenet-cache-train.pkl'
         elif self.mode == 'validation':
             google_drive_file_id = '1KY5e491bkLFqJDp0-UWou3463Mo8AOco'
             dropbox_file_link = 'https://www.dropbox.com/s/ip1b7se3gij3r1b/mini-imagenet-cache-validation.pkl?dl=1'
+            zenodo_file_link = 'https://zenodo.org/record/7978538/files/mini-imagenet-cache-validation.pkl'
         else:
-            raise ('ValueError', 'Needs to be train, test or validation')
+            raise ValueError('Needs to be train, test or validation')
 
         pickle_file = os.path.join(self.root, 'mini-imagenet-cache-' + mode + '.pkl')
         try:
             if not self._check_exists() and download:
                 print('Downloading mini-ImageNet --', mode)
-                download_pkl(google_drive_file_id, self.root, mode)
-            with open(pickle_file, 'rb') as f:
-                self.data = pickle.load(f)
-        except pickle.UnpicklingError:
-            if not self._check_exists() and download:
-                print('Download failed. Re-trying mini-ImageNet --', mode)
                 download_file(dropbox_file_link, pickle_file)
             with open(pickle_file, 'rb') as f:
                 self.data = pickle.load(f)
+        except Exception:
+            try:
+                if not self._check_exists() and download:
+                    print('Downloading mini-ImageNet --', mode)
+                    download_pkl(google_drive_file_id, self.root, mode)
+                with open(pickle_file, 'rb') as f:
+                    self.data = pickle.load(f)
+            except pickle.UnpicklingError:
+                if not self._check_exists() and download:
+                    print('Download failed. Re-trying mini-ImageNet --', mode)
+                    download_file(dropbox_file_link, pickle_file)
+                with open(pickle_file, 'rb') as f:
+                    self.data = pickle.load(f)
 
         self.x = torch.from_numpy(self.data["image_data"]).permute(0, 3, 1, 2).float()
         self.y = np.ones(len(self.x))
 
         # TODO Remove index_classes from here
         self.class_idx = index_classes(self.data['class_dict'].keys())
         for class_name, idxs in self.data['class_dict'].items():
             for idx in idxs:
                 self.y[idx] = self.class_idx[class_name]
 
     def __getitem__(self, idx):
         data = self.x[idx]
         if self.transform:
             data = self.transform(data)
-        return data, self.y[idx]
+        return data, int(self.y[idx])
 
     def __len__(self):
         return len(self.x)
 
     def _check_exists(self):
         return os.path.exists(os.path.join(self.root, 'mini-imagenet-cache-' + self.mode + '.pkl'))
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/quickdraw.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/quickdraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
     * **download** (bool, *optional*, default=False) - Whether to download the dataset.
 
     **Example**
 
     ~~~python
     train_dataset = l2l.vision.datasets.Quickdraw(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
     def __init__(
         self,
         root,
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/datasets/tiered_imagenet.py` & `learn2learn-0.2.0/learn2learn/vision/datasets/vgg_flowers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,139 @@
 #!/usr/bin/env python3
 
 import os
-import io
-import pickle
 import tarfile
-
-import numpy as np
-import torch
-import torch.utils.data as data
+import requests
+import scipy.io
 
 from PIL import Image
+from torch.utils.data import Dataset
+
+from learn2learn.data.utils import download_file
+
+DATA_DIR = 'vgg_flower102'
+IMAGES_URL = 'http://www.robots.ox.ac.uk/~vgg/data/flowers/102/102flowers.tgz'
+LABELS_URL = 'http://www.robots.ox.ac.uk/~vgg/data/flowers/102/imagelabels.mat'
+IMAGES_DIR = 'jpg'
+LABELS_PATH = 'imagelabels.mat'
+
+# Splits from "Meta-Datasets", Triantafillou et al, 2020
+SPLITS = {
+    'train': [90, 38, 80, 30, 29, 12, 43, 27, 4, 64, 31, 99, 8, 67, 95, 77,
+              78, 61, 88, 74, 55, 32, 21, 13, 79, 70, 51, 69, 14, 60, 11, 39,
+              63, 37, 36, 28, 48, 7, 93, 2, 18, 24, 6, 3, 44, 76, 75, 72, 52,
+              84, 73, 34, 54, 66, 59, 50, 91, 68, 100, 71, 81, 101, 92, 22,
+              33, 87, 1, 49, 20, 25, 58],
+    'validation': [10, 16, 17, 23, 26, 47, 53, 56, 57, 62, 82, 83, 86, 97, 102],
+    'test': [5, 9, 15, 19, 35, 40, 41, 42, 45, 46, 65, 85, 89, 94, 96, 98],
+    'all': list(range(1, 103)),
+}
 
-from learn2learn.data.utils import download_file_from_google_drive
 
+class VGGFlower102(Dataset):
 
-class TieredImagenet(data.Dataset):
     """
-    [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/vision/datasets/tiered_imagenet.py)
+    [[Source]](https://github.com/learnables/learn2learn/blob/master/learn2learn/vision/datasets/vgg_flowers.py)
 
     **Description**
 
-    The *tiered*-ImageNet dataset was originally introduced by Ren et al, 2018 and we download the data directly from the link provided in their repository.
+    The VGG Flowers dataset was originally introduced by Nilsback and Zisserman, 2006 and then re-purposed for few-shot learning in Triantafillou et al., 2020.
 
-    Like *mini*-ImageNet, *tiered*-ImageNet builds on top of ILSVRC-12, but consists of 608 classes (779,165 images) instead of 100.
-    The train-validation-test split is made such that classes from similar categories are in the same splits.
-    There are 34 categories each containing between 10 and 30 classes.
-    Of these categories, 20 (351 classes; 448,695 images) are used for training,
-    6 (97 classes; 124,261 images) for validation, and 8 (160 class; 206,209 images) for testing.
+    The dataset consists of 102 classes of flowers, with each class consisting of 40 to 258 images.
+    We provide the raw (unprocessed) images, and follow the train-validation-test splits of Triantafillou et al.
 
     **References**
 
-    1. Ren et al, 2018. "Meta-Learning for Semi-Supervised Few-Shot Classification." ICLR '18.
-    2. Ren Mengye. 2018. "few-shot-ssl-public". [https://github.com/renmengye/few-shot-ssl-public](https://github.com/renmengye/few-shot-ssl-public)
+    1. Nilsback, M. and A. Zisserman. 2006. "A Visual Vocabulary for Flower Classification." CVPR '06.
+    2. Triantafillou et al. 2020. "Meta-Dataset: A Dataset of Datasets for Learning to Learn from Few Examples." ICLR '20.
+    3. [https://www.robots.ox.ac.uk/~vgg/data/flowers/](https://www.robots.ox.ac.uk/~vgg/data/flowers/)
 
     **Arguments**
 
     * **root** (str) - Path to download the data.
     * **mode** (str, *optional*, default='train') - Which split to use.
         Must be 'train', 'validation', or 'test'.
     * **transform** (Transform, *optional*, default=None) - Input pre-processing.
     * **target_transform** (Transform, *optional*, default=None) - Target pre-processing.
     * **download** (bool, *optional*, default=False) - Whether to download the dataset.
 
     **Example**
 
     ~~~python
-    train_dataset = l2l.vision.datasets.TieredImagenet(root='./data', mode='train', download=True)
+    train_dataset = l2l.vision.datasets.VGGFlower102(root='./data', mode='train')
     train_dataset = l2l.data.MetaDataset(train_dataset)
-    train_generator = l2l.data.TaskDataset(dataset=train_dataset, num_tasks=1000)
+    train_generator = l2l.data.Taskset(dataset=train_dataset, num_tasks=1000)
     ~~~
 
     """
 
-    def __init__(self, root, mode='train', transform=None, target_transform=None, download=False):
-        super(TieredImagenet, self).__init__()
+    def __init__(self, root, mode='all', transform=None, target_transform=None, download=False):
+        root = os.path.expanduser(root)
         self.root = os.path.expanduser(root)
-        if not os.path.exists(self.root):
-            os.mkdir(self.root)
         self.transform = transform
         self.target_transform = target_transform
-        if mode not in ['train', 'validation', 'test']:
-            raise ValueError('mode must be train, validation, or test.')
-        self.mode = mode
-        self._bookkeeping_path = os.path.join(self.root, 'tiered-imagenet-bookkeeping-' + mode + '.pkl')
-        google_drive_file_id = '1g1aIDy2Ar_MViF2gDXFYDBTR-HYecV07'
+        self._bookkeeping_path = os.path.join(self.root, 'vgg-flower102-' + mode + '-bookkeeping.pkl')
 
         if not self._check_exists() and download:
-            self.download(google_drive_file_id, self.root)
+            self.download()
+
+        self.load_data(mode)
 
-        short_mode = 'val' if mode == 'validation' else mode
-        tiered_imaganet_path = os.path.join(self.root, 'tiered-imagenet')
-        images_path = os.path.join(tiered_imaganet_path, short_mode + '_images_png.pkl')
-        with open(images_path, 'rb') as images_file:
-            self.images = pickle.load(images_file)
-        labels_path = os.path.join(tiered_imaganet_path, short_mode + '_labels.pkl')
-        with open(labels_path, 'rb') as labels_file:
-            self.labels = pickle.load(labels_file)
-            self.labels = self.labels['label_specific']
-
-    def download(self, file_id, destination):
-        archive_path = os.path.join(destination, 'tiered_imagenet.tar')
-        print('Downloading tiered ImageNet. (12Gb) Please be patient.')
-        download_file_from_google_drive(file_id, archive_path)
-        archive_file = tarfile.open(archive_path)
-        archive_file.extractall(destination)
-        os.remove(archive_path)
-
-    def __getitem__(self, idx):
-        image = Image.open(io.BytesIO(self.images[idx]))
-        label = self.labels[idx]
-        if self.transform is not None:
+    def _check_exists(self):
+        data_path = os.path.join(self.root, DATA_DIR)
+        return os.path.exists(data_path)
+
+    def download(self):
+        if not os.path.exists(self.root):
+            os.mkdir(self.root)
+        data_path = os.path.join(self.root, DATA_DIR)
+        if not os.path.exists(data_path):
+            os.mkdir(data_path)
+        tar_path = os.path.join(data_path, os.path.basename(IMAGES_URL))
+        print('Downloading VGG Flower102 dataset (330Mb)')
+        download_file(IMAGES_URL, tar_path)
+        tar_file = tarfile.open(tar_path)
+        tar_file.extractall(data_path)
+        tar_file.close()
+        os.remove(tar_path)
+
+        label_path = os.path.join(data_path, os.path.basename(LABELS_URL))
+        req = requests.get(LABELS_URL)
+        with open(label_path, 'wb') as label_file:
+            label_file.write(req.content)
+
+    def load_data(self, mode='train'):
+        data_path = os.path.join(self.root, DATA_DIR)
+        images_path = os.path.join(data_path, IMAGES_DIR)
+        labels_path = os.path.join(data_path, LABELS_PATH)
+        labels_mat = scipy.io.loadmat(labels_path)
+        image_labels = []
+        split = SPLITS[mode]
+        for idx, label in enumerate(labels_mat['labels'][0], start=1):
+            if label in split:
+                image = str(idx).zfill(5)
+                image = f'image_{image}.jpg'
+                image = os.path.join(images_path, image)
+                label = split.index(label)
+                image_labels.append((image, label))
+        self.data = image_labels
+
+    def __getitem__(self, i):
+        image, label = self.data[i]
+        image = Image.open(image)
+        if self.transform:
             image = self.transform(image)
-        if self.target_transform is not None:
+        if self.target_transform:
             label = self.target_transform(label)
         return image, label
 
     def __len__(self):
-        return len(self.labels)
-
-    def _check_exists(self):
-        return os.path.exists(os.path.join(self.root,
-                                           'tiered-imagenet',
-                                           'train_images_png.pkl'))
+        return len(self.data)
 
 
 if __name__ == '__main__':
-    dataset = TieredImagenet(root='~/data')
-    img, tgt = dataset[43]
-    dataset = TieredImagenet(root='~/data', mode='validation')
-    img, tgt = dataset[43]
-    dataset = TieredImagenet(root='~/data', mode='test')
-    img, tgt = dataset[43]
+    assert len(SPLITS['train']) == 71
+    assert len(SPLITS['validation']) == 15
+    assert len(SPLITS['test']) == 16
+    assert len(SPLITS['all']) == 102
+    flowers = VGGFlower102('~/vgg_data', download=True)
+    print(len(flowers))
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/models/__init__.py` & `learn2learn-0.2.0/learn2learn/vision/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ConvBase,
     OmniglotFC,
     OmniglotCNN,
     MiniImagenetCNN,
     CNN4,
     CNN4Backbone,
 )
+
 from .resnet12 import ResNet12, ResNet12Backbone
 from .wrn28 import WRN28, WRN28Backbone
 
 __all__ = [
     'get_pretrained_backbone',
     'fc_init_',
     'maml_init_',
```

### Comparing `learn2learn-0.1.7/learn2learn/vision/models/cnn4.py` & `learn2learn-0.2.0/learn2learn/vision/models/cnn4.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/models/resnet12.py` & `learn2learn-0.2.0/learn2learn/vision/models/resnet12.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/models/wrn28.py` & `learn2learn-0.2.0/learn2learn/vision/models/wrn28.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn/vision/transforms.py` & `learn2learn-0.2.0/learn2learn/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/learn2learn.egg-info/PKG-INFO` & `learn2learn-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,206 +1,209 @@
 Metadata-Version: 2.1
 Name: learn2learn
-Version: 0.1.7
+Version: 0.2.0
 Summary: PyTorch Library for Meta-Learning Research
 Home-page: https://github.com/learnables/learn2learn
 Author: Debajyoti Datta, Ian bunner, Seb Arnold, Praateek Mahajan
 Author-email: smr.arnold@gmail.com
 License: MIT
-Download-URL: https://github.com/learnables/learn2learn/archive/0.1.7.zip
-Description: <p align="center"><img src="https://raw.githubusercontent.com/learnables/learn2learn/gh-pages/assets/img/l2l-full.png" height="120px" /></p>
-        
-        --------------------------------------------------------------------------------
-        
-        ![Test Status](https://github.com/learnables/learn2learn/workflows/Testing/badge.svg?branch=master)
-        [![arXiv](https://img.shields.io/badge/arXiv-2008.12284-b31b1b.svg)](https://arxiv.org/abs/2008.12284)
-        
-        learn2learn is a software library for meta-learning research.
-        
-        learn2learn builds on top of PyTorch to accelerate two aspects of the meta-learning research cycle:
-        
-        * *fast prototyping*, essential in letting researchers quickly try new ideas, and
-        * *correct reproducibility*, ensuring that these ideas are evaluated fairly.
-        
-        learn2learn provides low-level utilities and unified interface to create new algorithms and domains, together with high-quality implementations of existing algorithms and standardized benchmarks.
-        It retains compatibility with [torchvision](https://pytorch.org/vision/), [torchaudio](https://pytorch.org/audio/), [torchtext](https://pytorch.org/text/), [cherry](http://cherry-rl.net/), and any other PyTorch-based library you might be using.
-        
-        To learn more, see our whitepaper: [arXiv:2008.12284](https://arxiv.org/abs/2008.12284)
-        
-        **Overview**
-        
-        * [`learn2learn.data`](http://learn2learn.net/docs/learn2learn.data/): `TaskDataset` and transforms to create few-shot tasks from any PyTorch dataset.
-        * [`learn2learn.vision`](http://learn2learn.net/docs/learn2learn.vision/): Models, datasets, and benchmarks for computer vision and few-shot learning.
-        * [`learn2learn.gym`](http://learn2learn.net/docs/learn2learn.gym/): Environment and utilities for meta-reinforcement learning.
-        * [`learn2learn.algorithms`](http://learn2learn.net/docs/learn2learn.algorithms/): High-level wrappers for existing meta-learning algorithms.
-        * [`learn2learn.optim`](http://learn2learn.net/docs/learn2learn.optim/): Utilities and algorithms for differentiable optimization and meta-descent.
-        
-        **Resources**
-        
-        * Website: [http://learn2learn.net/](http://learn2learn.net/)
-        * Documentation: [http://learn2learn.net/docs/learn2learn](http://learn2learn.net/docs/learn2learn)
-        * Tutorials: [http://learn2learn.net/tutorials/getting_started/](http://learn2learn.net/tutorials/getting_started/)
-        * Examples: [https://github.com/learnables/learn2learn/tree/master/examples](https://github.com/learnables/learn2learn/tree/master/examples)
-        * GitHub: [https://github.com/learnables/learn2learn/](https://github.com/learnables/learn2learn/)
-        * Slack: [http://slack.learn2learn.net/](http://slack.learn2learn.net/)
-        
-        ## Installation
-        
-        ~~~bash
-        pip install learn2learn
-        ~~~
-        
-        ## Snippets & Examples
-        
-        The following snippets provide a sneak peek at the functionalities of learn2learn.
-        
-        ### High-level Wrappers
-        
-        <details>
-        <summary><b>Few-Shot Learning with MAML</b></summary>
-        
-        For more algorithms (ProtoNets, ANIL, Meta-SGD, Reptile, Meta-Curvature, KFO) refer to the <a href="https://github.com/learnables/learn2learn/tree/master/examples/vision">examples</a> folder.
-        Most of them can be implemented with with the `GBML` wrapper. (<a href="http://learn2learn.net/docs/learn2learn.algorithms/#gbml">documentation</a>).
-            
-        ~~~python
-        maml = l2l.algorithms.MAML(model, lr=0.1)
-        opt = torch.optim.SGD(maml.parameters(), lr=0.001)
-        for iteration in range(10):
-            opt.zero_grad()
-            task_model = maml.clone()  # torch.clone() for nn.Modules
-            adaptation_loss = compute_loss(task_model)
-            task_model.adapt(adaptation_loss)  # computes gradient, update task_model in-place
-            evaluation_loss = compute_loss(task_model)
-            evaluation_loss.backward()  # gradients w.r.t. maml.parameters()
-            opt.step()
-        ~~~
-        </details>
-        
-        <details>
-        <summary><b>Meta-Descent with Hypergradient</b></summary>
-            
-        Learn any kind of optimization algorithm with the `LearnableOptimizer`. (<a href="https://github.com/learnables/learn2learn/tree/master/examples/optimization">example</a> and <a href="http://learn2learn.net/docs/learn2learn.optim/#learnableoptimizer">documentation</a>)
-        
-        ~~~python
-        linear = nn.Linear(784, 10)
-        transform = l2l.optim.ModuleTransform(l2l.nn.Scale)
-        metaopt = l2l.optim.LearnableOptimizer(linear, transform, lr=0.01)  # metaopt has .step()
-        opt = torch.optim.SGD(metaopt.parameters(), lr=0.001)  # metaopt also has .parameters()
-        
-        metaopt.zero_grad()
-        opt.zero_grad()
-        error = loss(linear(X), y)
-        error.backward()
-        opt.step()  # update metaopt
-        metaopt.step()  # update linear
-        ~~~
-        </details>
-        
-        ### Learning Domains
-        
-        <details>
-        <summary><b>Custom Few-Shot Dataset</b></summary>
-        
-        Many standardized datasets (Omniglot, mini-/tiered-ImageNet, FC100, CIFAR-FS) are readily available in `learn2learn.vision.datasets`.
-        (<a href="http://learn2learn.net/docs/learn2learn.vision/#learn2learnvisiondatasets">documentation</a>)
-        
-        ~~~python
-        dataset = l2l.data.MetaDataset(MyDataset())  # any PyTorch dataset
-        transforms = [  # Easy to define your own transform
-            l2l.data.transforms.NWays(dataset, n=5),
-            l2l.data.transforms.KShots(dataset, k=1),
-            l2l.data.transforms.LoadData(dataset),
-        ]
-        taskset = TaskDataset(dataset, transforms, num_tasks=20000)
-        for task in taskset:
-            X, y = task
-            # Meta-train on the task
-        ~~~
-        </details>
-        
-        
-        <details>
-        <summary><b>Environments and Utilities for Meta-RL</b></summary>
-        
-        Parallelize your own meta-environments with `AsyncVectorEnv`, or use the standardized ones.
-        (<a href="http://learn2learn.net/docs/learn2learn.gym/#metaenv">documentation</a>)
-        
-        ~~~python
-        def make_env():
-            env = l2l.gym.HalfCheetahForwardBackwardEnv()
-            env = cherry.envs.ActionSpaceScaler(env)
-            return env
-        
-        env = l2l.gym.AsyncVectorEnv([make_env for _ in range(16)])  # uses 16 threads
-        for task_config in env.sample_tasks(20):
-            env.set_task(task)  # all threads receive the same task
-            state = env.reset()  # use standard Gym API
-            action = my_policy(env)
-            env.step(action)
-        ~~~
-        </details>
-        
-        ### Low-Level Utilities
-        
-        <details>
-        <summary><b>Differentiable Optimization</b></summary>
-        
-        Learn and differentiate through updates of PyTorch Modules.
-        (<a href="http://learn2learn.net/docs/learn2learn.optim/#parameterupdate">documentation</a>)
-            
-        ~~~python
-        
-        model = MyModel()
-        transform = l2l.optim.KroneckerTransform(l2l.nn.KroneckerLinear)
-        learned_update = l2l.optim.ParameterUpdate(  # learnable update function
-                model.parameters(), transform)
-        clone = l2l.clone_module(model)  # torch.clone() for nn.Modules
-        error = loss(clone(X), y)
-        updates = learned_update(  # similar API as torch.autograd.grad
-            error,
-            clone.parameters(),
-            create_graph=True,
-        )
-        l2l.update_module(clone, updates=updates)
-        loss(clone(X), y).backward()  # Gradients w.r.t model.parameters() and learned_update.parameters()
-        ~~~
-        </details>
-        
-        ## Changelog
-        
-        A human-readable changelog is available in the [CHANGELOG.md](CHANGELOG.md) file.
-        
-        ## Citation
-        
-        To cite the `learn2learn` repository in your academic publications, please use the following reference.
-        
-        > Arnold, Sebastien M. R., Praateek Mahajan, Debajyoti Datta, Ian Bunner, and Konstantinos Saitas Zarkias. 2020. “learn2learn: A Library for Meta-Learning Research.” arXiv [cs.LG]. http://arxiv.org/abs/2008.12284.
-        
-        You can also use the following Bibtex entry.
-        
-        ~~~bib
-        @article{Arnold2020-ss,
-          title         = "learn2learn: A Library for {Meta-Learning} Research",
-          author        = "Arnold, S{\'e}bastien M R and Mahajan, Praateek and Datta,
-                           Debajyoti and Bunner, Ian and Zarkias, Konstantinos Saitas",
-          month         =  aug,
-          year          =  2020,
-          url           = "http://arxiv.org/abs/2008.12284",
-          archivePrefix = "arXiv",
-          primaryClass  = "cs.LG",
-          eprint        = "2008.12284"
-        }
-        
-        ~~~
-        
-        ### Acknowledgements & Friends
-        
-        1. [TorchMeta](https://github.com/tristandeleu/pytorch-meta) is similar library, with a focus on datasets for supervised meta-learning. 
-        2. [higher](https://github.com/facebookresearch/higher) is a PyTorch library that enables differentiating through optimization inner-loops. While they monkey-patch `nn.Module` to be stateless, learn2learn retains the stateful PyTorch look-and-feel. For more information, refer to [their ArXiv paper](https://arxiv.org/abs/1910.01727).
-        3. We are thankful to the following open-source implementations which helped guide the design of learn2learn:
-            * Tristan Deleu's [pytorch-maml-rl](https://github.com/tristandeleu/pytorch-maml-rl)
-            * Jonas Rothfuss' [ProMP](https://github.com/jonasrothfuss/ProMP/)
-            * Kwonjoon Lee's [MetaOptNet](https://github.com/kjunelee/MetaOptNet)
-            * Han-Jia Ye's and Hexiang Hu's [FEAT](https://github.com/Sha-Lab/FEAT)
-        
+Download-URL: https://github.com/learnables/learn2learn/archive/0.2.0.zip
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center"><img src="https://raw.githubusercontent.com/learnables/learn2learn/gh-pages/assets/img/l2l-full.png" height="120px" /></p>
+
+--------------------------------------------------------------------------------
+
+![Test Status](https://github.com/learnables/learn2learn/workflows/Testing/badge.svg?branch=master)
+[![arXiv](https://img.shields.io/badge/arXiv-2008.12284-b31b1b.svg)](https://arxiv.org/abs/2008.12284)
+
+learn2learn is a software library for meta-learning research.
+
+learn2learn builds on top of PyTorch to accelerate two aspects of the meta-learning research cycle:
+
+* *fast prototyping*, essential in letting researchers quickly try new ideas, and
+* *correct reproducibility*, ensuring that these ideas are evaluated fairly.
+
+learn2learn provides low-level utilities and unified interface to create new algorithms and domains, together with high-quality implementations of existing algorithms and standardized benchmarks.
+It retains compatibility with [torchvision](https://pytorch.org/vision/), [torchaudio](https://pytorch.org/audio/), [torchtext](https://pytorch.org/text/), [cherry](http://cherry-rl.net/), and any other PyTorch-based library you might be using.
+
+To learn more, see our whitepaper: [arXiv:2008.12284](https://arxiv.org/abs/2008.12284)
+
+**Overview**
+
+* [`learn2learn.data`](http://learn2learn.net/docs/learn2learn.data/): `Taskset` and transforms to create few-shot tasks from any PyTorch dataset.
+* [`learn2learn.vision`](http://learn2learn.net/docs/learn2learn.vision/): Models, datasets, and benchmarks for computer vision and few-shot learning.
+* [`learn2learn.gym`](http://learn2learn.net/docs/learn2learn.gym/): Environment and utilities for meta-reinforcement learning.
+* [`learn2learn.algorithms`](http://learn2learn.net/docs/learn2learn.algorithms/): High-level wrappers for existing meta-learning algorithms.
+* [`learn2learn.optim`](http://learn2learn.net/docs/learn2learn.optim/): Utilities and algorithms for differentiable optimization and meta-descent.
+
+**Resources**
+
+* Website: [http://learn2learn.net/](http://learn2learn.net/)
+* Documentation: [http://learn2learn.net/docs/learn2learn](http://learn2learn.net/docs/learn2learn)
+* Tutorials: [http://learn2learn.net/tutorials/getting_started/](http://learn2learn.net/tutorials/getting_started/)
+* Examples: [https://github.com/learnables/learn2learn/tree/master/examples](https://github.com/learnables/learn2learn/tree/master/examples)
+* GitHub: [https://github.com/learnables/learn2learn/](https://github.com/learnables/learn2learn/)
+* Slack: [http://slack.learn2learn.net/](http://slack.learn2learn.net/)
+
+## Installation
+
+~~~bash
+pip install learn2learn
+~~~
+
+## Snippets & Examples
+
+The following snippets provide a sneak peek at the functionalities of learn2learn.
+
+### High-level Wrappers
+
+<details>
+<summary><b>Few-Shot Learning with MAML</b></summary>
+
+For more algorithms (ProtoNets, ANIL, Meta-SGD, Reptile, Meta-Curvature, KFO) refer to the <a href="https://github.com/learnables/learn2learn/tree/master/examples/vision">examples</a> folder.
+Most of them can be implemented with with the `GBML` wrapper. (<a href="http://learn2learn.net/docs/learn2learn.algorithms/#gbml">documentation</a>).
+    
+~~~python
+maml = l2l.algorithms.MAML(model, lr=0.1)
+opt = torch.optim.SGD(maml.parameters(), lr=0.001)
+for iteration in range(10):
+    opt.zero_grad()
+    task_model = maml.clone()  # torch.clone() for nn.Modules
+    adaptation_loss = compute_loss(task_model)
+    task_model.adapt(adaptation_loss)  # computes gradient, update task_model in-place
+    evaluation_loss = compute_loss(task_model)
+    evaluation_loss.backward()  # gradients w.r.t. maml.parameters()
+    opt.step()
+~~~
+</details>
+
+<details>
+<summary><b>Meta-Descent with Hypergradient</b></summary>
+    
+Learn any kind of optimization algorithm with the `LearnableOptimizer`. (<a href="https://github.com/learnables/learn2learn/tree/master/examples/optimization">example</a> and <a href="http://learn2learn.net/docs/learn2learn.optim/#learnableoptimizer">documentation</a>)
+
+~~~python
+linear = nn.Linear(784, 10)
+transform = l2l.optim.ModuleTransform(l2l.nn.Scale)
+metaopt = l2l.optim.LearnableOptimizer(linear, transform, lr=0.01)  # metaopt has .step()
+opt = torch.optim.SGD(metaopt.parameters(), lr=0.001)  # metaopt also has .parameters()
+
+metaopt.zero_grad()
+opt.zero_grad()
+error = loss(linear(X), y)
+error.backward()
+opt.step()  # update metaopt
+metaopt.step()  # update linear
+~~~
+</details>
+
+### Learning Domains
+
+<details>
+<summary><b>Custom Few-Shot Dataset</b></summary>
+
+Many standardized datasets (Omniglot, mini-/tiered-ImageNet, FC100, CIFAR-FS) are readily available in `learn2learn.vision.datasets`.
+(<a href="http://learn2learn.net/docs/learn2learn.vision/#learn2learnvisiondatasets">documentation</a>)
+
+~~~python
+dataset = l2l.data.MetaDataset(MyDataset())  # any PyTorch dataset
+transforms = [  # Easy to define your own transform
+    l2l.data.transforms.NWays(dataset, n=5),
+    l2l.data.transforms.KShots(dataset, k=1),
+    l2l.data.transforms.LoadData(dataset),
+]
+taskset = Taskset(dataset, transforms, num_tasks=20000)
+for task in taskset:
+    X, y = task
+    # Meta-train on the task
+~~~
+</details>
+
+
+<details>
+<summary><b>Environments and Utilities for Meta-RL</b></summary>
+
+Parallelize your own meta-environments with `AsyncVectorEnv`, or use the standardized ones.
+(<a href="http://learn2learn.net/docs/learn2learn.gym/#metaenv">documentation</a>)
+
+~~~python
+def make_env():
+    env = l2l.gym.HalfCheetahForwardBackwardEnv()
+    env = cherry.envs.ActionSpaceScaler(env)
+    return env
+
+env = l2l.gym.AsyncVectorEnv([make_env for _ in range(16)])  # uses 16 threads
+for task_config in env.sample_tasks(20):
+    env.set_task(task)  # all threads receive the same task
+    state = env.reset()  # use standard Gym API
+    action = my_policy(env)
+    env.step(action)
+~~~
+</details>
+
+### Low-Level Utilities
+
+<details>
+<summary><b>Differentiable Optimization</b></summary>
+
+Learn and differentiate through updates of PyTorch Modules.
+(<a href="http://learn2learn.net/docs/learn2learn.optim/#parameterupdate">documentation</a>)
+    
+~~~python
+
+model = MyModel()
+transform = l2l.optim.KroneckerTransform(l2l.nn.KroneckerLinear)
+learned_update = l2l.optim.ParameterUpdate(  # learnable update function
+        model.parameters(), transform)
+clone = l2l.clone_module(model)  # torch.clone() for nn.Modules
+error = loss(clone(X), y)
+updates = learned_update(  # similar API as torch.autograd.grad
+    error,
+    clone.parameters(),
+    create_graph=True,
+)
+l2l.update_module(clone, updates=updates)
+loss(clone(X), y).backward()  # Gradients w.r.t model.parameters() and learned_update.parameters()
+~~~
+</details>
+
+## Changelog
+
+A human-readable changelog is available in the [CHANGELOG.md](CHANGELOG.md) file.
+
+## Citation
+
+To cite the `learn2learn` repository in your academic publications, please use the following reference.
+
+> Arnold, Sebastien M. R., Praateek Mahajan, Debajyoti Datta, Ian Bunner, and Konstantinos Saitas Zarkias. 2020. “learn2learn: A Library for Meta-Learning Research.” arXiv [cs.LG]. http://arxiv.org/abs/2008.12284.
+
+You can also use the following Bibtex entry.
+
+~~~bib
+@article{Arnold2020-ss,
+  title         = "learn2learn: A Library for {Meta-Learning} Research",
+  author        = "Arnold, S{\'e}bastien M R and Mahajan, Praateek and Datta,
+                   Debajyoti and Bunner, Ian and Zarkias, Konstantinos Saitas",
+  month         =  aug,
+  year          =  2020,
+  url           = "http://arxiv.org/abs/2008.12284",
+  archivePrefix = "arXiv",
+  primaryClass  = "cs.LG",
+  eprint        = "2008.12284"
+}
+
+~~~
+
+### Acknowledgements & Friends
+
+1. [TorchMeta](https://github.com/tristandeleu/pytorch-meta) is similar library, with a focus on datasets for supervised meta-learning. 
+2. [higher](https://github.com/facebookresearch/higher) is a PyTorch library that enables differentiating through optimization inner-loops. While they monkey-patch `nn.Module` to be stateless, learn2learn retains the stateful PyTorch look-and-feel. For more information, refer to [their ArXiv paper](https://arxiv.org/abs/1910.01727).
+3. We are thankful to the following open-source implementations which helped guide the design of learn2learn:
+    * Tristan Deleu's [pytorch-maml-rl](https://github.com/tristandeleu/pytorch-maml-rl)
+    * Jonas Rothfuss' [ProMP](https://github.com/jonasrothfuss/ProMP/)
+    * Kwonjoon Lee's [MetaOptNet](https://github.com/kjunelee/MetaOptNet)
+    * Han-Jia Ye's and Hexiang Hu's [FEAT](https://github.com/Sha-Lab/FEAT)
+
+
```

### Comparing `learn2learn-0.1.7/learn2learn.egg-info/SOURCES.txt` & `learn2learn-0.2.0/learn2learn.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+.gitignore
+CHANGELOG.md
+CITATION.cff
 LICENSE
 MANIFEST.in
+Makefile
 README.md
+mkdocs.yml
+requirements-dev.txt
+requirements.txt
 setup.cfg
 setup.py
 .eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Code.pxd
 .eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/FlowControl.pxd
 .eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/ParseTreeTransforms.pxd
 .eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Parsing.pxd
 .eggs/Cython-0.29.15-py3.7.egg/Cython/Compiler/Scanning.pxd
@@ -354,14 +361,113 @@
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Printing.c
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/Profile.c
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/StringTools.c
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCyUtilityLoader.pyx
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestCythonScope.pyx
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TestUtilityLoader.c
 .eggs/Cython-0.29.24-py3.9-macosx-10.9-x86_64.egg/Cython/Utility/TypeConversion.c
+.github/pull_request_template.md
+.github/workflows/codeql.yml
+.github/workflows/python_unittest.yaml
+docs/CNAME
+docs/changelog.md
+docs/community.md
+docs/index.md
+docs/paper_list.md
+docs/assets/css/l2l_material.css
+docs/assets/img/halfcheetah.gif
+docs/assets/img/l2l-full.png
+docs/assets/img/learn2learn.png
+docs/assets/img/learn2learn.svg
+docs/assets/img/learn2learn_white.png
+docs/assets/img/community/amazon_science.png
+docs/assets/img/community/pytorch_lightning.png
+docs/assets/img/community/uiuc.png
+docs/assets/img/community/usc.png
+docs/assets/img/examples/ant_fwdbwd_rewards.png
+docs/assets/img/examples/cheetah_fwdbwd_rewards.png
+docs/assets/img/favicons/android-icon-144x144.png
+docs/assets/img/favicons/android-icon-192x192.png
+docs/assets/img/favicons/android-icon-36x36.png
+docs/assets/img/favicons/android-icon-48x48.png
+docs/assets/img/favicons/android-icon-72x72.png
+docs/assets/img/favicons/android-icon-96x96.png
+docs/assets/img/favicons/apple-icon-114x114.png
+docs/assets/img/favicons/apple-icon-120x120.png
+docs/assets/img/favicons/apple-icon-144x144.png
+docs/assets/img/favicons/apple-icon-152x152.png
+docs/assets/img/favicons/apple-icon-180x180.png
+docs/assets/img/favicons/apple-icon-57x57.png
+docs/assets/img/favicons/apple-icon-60x60.png
+docs/assets/img/favicons/apple-icon-72x72.png
+docs/assets/img/favicons/apple-icon-76x76.png
+docs/assets/img/favicons/apple-icon-precomposed.png
+docs/assets/img/favicons/apple-icon.png
+docs/assets/img/favicons/favicon-16x16.png
+docs/assets/img/favicons/favicon-32x32.png
+docs/assets/img/favicons/favicon-96x96.png
+docs/assets/img/favicons/favicon.ico
+docs/assets/img/favicons/manifest.json
+docs/assets/img/favicons/ms-icon-144x144.png
+docs/assets/img/favicons/ms-icon-150x150.png
+docs/assets/img/favicons/ms-icon-310x310.png
+docs/assets/img/favicons/ms-icon-70x70.png
+docs/docs/learn2learn.algorithms.md
+docs/docs/learn2learn.data.md
+docs/docs/learn2learn.gym.md
+docs/docs/learn2learn.md
+docs/docs/learn2learn.nn.md
+docs/docs/learn2learn.optim.md
+docs/docs/learn2learn.vision.md
+docs/examples/README.md
+docs/examples/optim.md
+docs/examples/rl.md
+docs/examples/vision.md
+docs/tutorials/getting_started.md
+docs/tutorials/anil_tutorial/ANIL_tutorial.md
+docs/tutorials/anil_tutorial/MAML_vs_ANIL.png
+docs/tutorials/anil_tutorial/rapid_learning_or_feature_reuse.png
+docs/tutorials/task_transform_tutorial/few-shot.png
+docs/tutorials/task_transform_tutorial/l2l-task-transform.png
+docs/tutorials/task_transform_tutorial/transform_tutorial.md
+examples/maml_sine.py
+examples/maml_toy.py
+examples/metamodule_toy.py
+examples/optimization/README.md
+examples/optimization/hypergrad_mnist.py
+examples/rl/README.md
+examples/rl/__init__.py
+examples/rl/cavia_trpo.py
+examples/rl/dist_promp.py
+examples/rl/maml_dice.py
+examples/rl/maml_trpo.py
+examples/rl/maml_trpo_metaworld.py
+examples/rl/metasgd_a2c.py
+examples/rl/policies.py
+examples/rl/promp.py
+examples/text/gpt2_adapters.py
+examples/text/nanogpt_lora.py
+examples/text/nanogpt_model.py
+examples/vision/Makefile
+examples/vision/README.md
+examples/vision/anil_fc100.py
+examples/vision/anilkfo_cifarfs.py
+examples/vision/distributed_maml.py
+examples/vision/maml_miniimagenet.py
+examples/vision/maml_omniglot.py
+examples/vision/meta_mnist.py
+examples/vision/metacurvature_fc100.py
+examples/vision/protonet_miniimagenet.py
+examples/vision/reptile_miniimagenet.py
+examples/vision/supervised_pretraining.py
+examples/vision/lightning/Makefile
+examples/vision/lightning/main.py
+examples/vision/mamlpp/MAMLpp.py
+examples/vision/mamlpp/cnn4_bnrs.py
+examples/vision/mamlpp/maml++_miniimagenet.py
 learn2learn/__init__.py
 learn2learn/_version.py
 learn2learn.egg-info/PKG-INFO
 learn2learn.egg-info/SOURCES.txt
 learn2learn.egg-info/dependency_links.txt
 learn2learn.egg-info/not-zip-safe
 learn2learn.egg-info/requires.txt
@@ -376,14 +482,15 @@
 learn2learn/algorithms/lightning/lightning_episodic_module.py
 learn2learn/algorithms/lightning/lightning_maml.py
 learn2learn/algorithms/lightning/lightning_metaoptnet.py
 learn2learn/algorithms/lightning/lightning_protonet.py
 learn2learn/data/__init__.py
 learn2learn/data/meta_dataset.c
 learn2learn/data/meta_dataset.pyx
+learn2learn/data/samplers.py
 learn2learn/data/task_dataset.c
 learn2learn/data/task_dataset.pxd
 learn2learn/data/task_dataset.pyx
 learn2learn/data/transforms.c
 learn2learn/data/transforms.pyx
 learn2learn/data/utils.py
 learn2learn/gym/README.md
@@ -404,14 +511,17 @@
 learn2learn/gym/envs/particles/__init__.py
 learn2learn/gym/envs/particles/particles_2d.py
 learn2learn/nn/__init__.py
 learn2learn/nn/kroneckers.py
 learn2learn/nn/metaoptnet.py
 learn2learn/nn/misc.py
 learn2learn/nn/protonet.py
+learn2learn/nn/metalayers/__init__.py
+learn2learn/nn/metalayers/metamodule.py
+learn2learn/nn/metalayers/parameter_transform.py
 learn2learn/optim/__init__.py
 learn2learn/optim/learnable_optimizer.py
 learn2learn/optim/parameter_update.py
 learn2learn/optim/transforms/__init__.py
 learn2learn/optim/transforms/kronecker_transform.py
 learn2learn/optim/transforms/metacurvature_transform.py
 learn2learn/optim/transforms/module_transform.py
@@ -443,14 +553,17 @@
 learn2learn/vision/datasets/quickdraw.py
 learn2learn/vision/datasets/tiered_imagenet.py
 learn2learn/vision/datasets/vgg_flowers.py
 learn2learn/vision/models/__init__.py
 learn2learn/vision/models/cnn4.py
 learn2learn/vision/models/resnet12.py
 learn2learn/vision/models/wrn28.py
+scripts/bibtex_to_gsheets.py
+scripts/compile_paper_list.py
+scripts/credentials.json
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/maml_miniimagenet_test_notravis.py
 tests/integration/maml_omniglot_test.py
 tests/integration/protonets_miniimagenet_test_notravis.py
 tests/unit/__init__.py
 tests/unit/utils_test.py
```

### Comparing `learn2learn-0.1.7/setup.py` & `learn2learn-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/integration/maml_miniimagenet_test_notravis.py` & `learn2learn-0.2.0/tests/integration/maml_miniimagenet_test_notravis.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,39 +72,45 @@
     train_transforms = [
         l2l.data.transforms.NWays(train_dataset, ways),
         l2l.data.transforms.KShots(train_dataset, 2*shots),
         l2l.data.transforms.LoadData(train_dataset),
         l2l.data.transforms.RemapLabels(train_dataset),
         l2l.data.transforms.ConsecutiveLabels(train_dataset),
     ]
-    train_tasks = l2l.data.TaskDataset(train_dataset,
-                                       task_transforms=train_transforms,
-                                       num_tasks=20000)
+    train_tasks = l2l.data.Taskset(
+        train_dataset,
+        task_transforms=train_transforms,
+        num_tasks=20000,
+    )
 
     valid_transforms = [
         l2l.data.transforms.NWays(valid_dataset, ways),
         l2l.data.transforms.KShots(valid_dataset, 2*shots),
         l2l.data.transforms.LoadData(valid_dataset),
         l2l.data.transforms.ConsecutiveLabels(train_dataset),
         l2l.data.transforms.RemapLabels(valid_dataset),
     ]
-    valid_tasks = l2l.data.TaskDataset(valid_dataset,
-                                       task_transforms=valid_transforms,
-                                       num_tasks=600)
+    valid_tasks = l2l.data.Taskset(
+        valid_dataset,
+        task_transforms=valid_transforms,
+        num_tasks=600,
+    )
 
     test_transforms = [
         l2l.data.transforms.NWays(test_dataset, ways),
         l2l.data.transforms.KShots(test_dataset, 2*shots),
         l2l.data.transforms.LoadData(test_dataset),
         l2l.data.transforms.RemapLabels(test_dataset),
         l2l.data.transforms.ConsecutiveLabels(train_dataset),
     ]
-    test_tasks = l2l.data.TaskDataset(test_dataset,
-                                      task_transforms=test_transforms,
-                                      num_tasks=600)
+    test_tasks = l2l.data.Taskset(
+        test_dataset,
+        task_transforms=test_transforms,
+        num_tasks=600,
+    )
 
     # Create model
     model = l2l.vision.models.MiniImagenetCNN(ways)
     model.to(device)
     maml = l2l.algorithms.MAML(model, lr=fast_lr, first_order=False)
     opt = optim.Adam(maml.parameters(), meta_lr)
     loss = nn.CrossEntropyLoss(size_average=True, reduction='mean')
```

### Comparing `learn2learn-0.1.7/tests/integration/maml_omniglot_test.py` & `learn2learn-0.2.0/tests/integration/maml_omniglot_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,45 +81,51 @@
                                              k=2*shots,
                                              filter_labels=classes[:1100]),
         l2l.data.transforms.LoadData(dataset),
         l2l.data.transforms.RemapLabels(dataset),
         l2l.data.transforms.ConsecutiveLabels(dataset),
         l2l.vision.transforms.RandomClassRotation(dataset, [0.0, 90.0, 180.0, 270.0])
     ]
-    train_tasks = l2l.data.TaskDataset(dataset,
-                                       task_transforms=train_transforms,
-                                       num_tasks=20000)
+    train_tasks = l2l.data.Taskset(
+        dataset,
+        task_transforms=train_transforms,
+        num_tasks=20000,
+    )
 
     valid_transforms = [
         l2l.data.transforms.FusedNWaysKShots(dataset,
                                              n=ways,
                                              k=2*shots,
                                              filter_labels=classes[1100:1200]),
         l2l.data.transforms.LoadData(dataset),
         l2l.data.transforms.RemapLabels(dataset),
         l2l.data.transforms.ConsecutiveLabels(dataset),
         l2l.vision.transforms.RandomClassRotation(dataset, [0.0, 90.0, 180.0, 270.0])
     ]
-    valid_tasks = l2l.data.TaskDataset(dataset,
-                                       task_transforms=valid_transforms,
-                                       num_tasks=1024)
+    valid_tasks = l2l.data.Taskset(
+        dataset,
+        task_transforms=valid_transforms,
+        num_tasks=1024,
+    )
 
     test_transforms = [
         l2l.data.transforms.FusedNWaysKShots(dataset,
                                              n=ways,
                                              k=2*shots,
                                              filter_labels=classes[1200:]),
         l2l.data.transforms.LoadData(dataset),
         l2l.data.transforms.RemapLabels(dataset),
         l2l.data.transforms.ConsecutiveLabels(dataset),
         l2l.vision.transforms.RandomClassRotation(dataset, [0.0, 90.0, 180.0, 270.0])
     ]
-    test_tasks = l2l.data.TaskDataset(dataset,
-                                      task_transforms=test_transforms,
-                                      num_tasks=1024)
+    test_tasks = l2l.data.Taskset(
+        dataset,
+        task_transforms=test_transforms,
+        num_tasks=1024,
+    )
 
     # Create model
     model = l2l.vision.models.OmniglotFC(28 ** 2, ways)
     model.to(device)
     maml = l2l.algorithms.MAML(model, lr=fast_lr, first_order=False)
     opt = optim.Adam(maml.parameters(), meta_lr)
     loss = nn.CrossEntropyLoss(reduction='mean')
```

### Comparing `learn2learn-0.1.7/tests/integration/protonets_miniimagenet_test_notravis.py` & `learn2learn-0.2.0/tests/integration/protonets_miniimagenet_test_notravis.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,39 +126,43 @@
     train_dataset = l2l.data.MetaDataset(train_dataset)
     train_transforms = [
         l2l.data.transforms.NWays(train_dataset, args.train_way),
         l2l.data.transforms.KShots(train_dataset, args.train_query + args.shot),
         l2l.data.transforms.LoadData(train_dataset),
         l2l.data.transforms.RemapLabels(train_dataset),
     ]
-    train_tasks = l2l.data.TaskDataset(train_dataset, task_transforms=train_transforms)
+    train_tasks = l2l.data.Taskset(train_dataset, task_transforms=train_transforms)
 #    train_loader = DataLoader(train_tasks, pin_memory=True, shuffle=True)
 
     valid_dataset = l2l.data.MetaDataset(valid_dataset)
     valid_transforms = [
         l2l.data.transforms.NWays(valid_dataset, args.test_way),
         l2l.data.transforms.KShots(valid_dataset, args.test_query + args.test_shot),
         l2l.data.transforms.LoadData(valid_dataset),
         l2l.data.transforms.RemapLabels(valid_dataset),
     ]
-    valid_tasks = l2l.data.TaskDataset(valid_dataset,
-                                       task_transforms=valid_transforms,
-                                       num_tasks=200)
+    valid_tasks = l2l.data.Taskset(
+        valid_dataset,
+        task_transforms=valid_transforms,
+        num_tasks=200,
+    )
 #    valid_loader = DataLoader(valid_tasks, pin_memory=True, shuffle=True)
 
     test_dataset = l2l.data.MetaDataset(test_dataset)
     test_transforms = [
         l2l.data.transforms.NWays(test_dataset, args.test_way),
         l2l.data.transforms.KShots(test_dataset, args.test_query + args.test_shot),
         l2l.data.transforms.LoadData(test_dataset),
         l2l.data.transforms.RemapLabels(test_dataset),
     ]
-    test_tasks = l2l.data.TaskDataset(test_dataset,
-                                      task_transforms=test_transforms,
-                                      num_tasks=200)
+    test_tasks = l2l.data.Taskset(
+        test_dataset,
+        task_transforms=test_transforms,
+        num_tasks=200,
+    )
 #    test_loader = DataLoader(test_tasks, pin_memory=True, shuffle=True)
 
     optimizer = torch.optim.Adam(model.parameters(), lr=0.001)
     lr_scheduler = torch.optim.lr_scheduler.StepLR(
         optimizer, step_size=20, gamma=0.5)
 
     for epoch in range(1, args.max_epoch + 1):
```

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/gbml_test.py` & `learn2learn-0.2.0/tests/unit/algorithms/gbml_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/lightning_anil_test_notravis.py` & `learn2learn-0.2.0/tests/unit/algorithms/lightning_anil_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/lightning_maml_test_notravis.py` & `learn2learn-0.2.0/tests/unit/algorithms/lightning_maml_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/lightning_metaoptnet_test_notravis.py` & `learn2learn-0.2.0/tests/unit/algorithms/lightning_metaoptnet_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/lightning_protonet_test_notravis.py` & `learn2learn-0.2.0/tests/unit/algorithms/lightning_protonet_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/maml_test.py` & `learn2learn-0.2.0/tests/unit/algorithms/maml_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/algorithms/metasgd_test.py` & `learn2learn-0.2.0/tests/unit/algorithms/metasgd_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/data/metadataset_test.py` & `learn2learn-0.2.0/tests/unit/data/metadataset_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/data/task_dataset_test.py` & `learn2learn-0.2.0/tests/unit/data/task_dataset_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 from unittest import TestCase
 
 import numpy as np
 import torch
 from torch.utils.data import TensorDataset, DataLoader
 
-from learn2learn.data import MetaDataset, TaskDataset
+from learn2learn.data import MetaDataset, Taskset
 from learn2learn.data.transforms import LoadData
 
 
 NUM_TASKS = 10
 NUM_DATA = 128
 X_SHAPE = 16
 Y_SHAPE = 10
@@ -28,28 +28,28 @@
         diff += (a-b).pow(2).sum().item()
     return diff < EPSILON
 
 def random_subset(task_description):
     return random.choices(task_description, k=SUBSET_SIZE)
 
 
-class TestTaskDataset(TestCase):
+class TestTaskset(TestCase):
 
     def test_instanciation(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = TensorDataset(data, labels)
-        task_dataset = TaskDataset(dataset, task_transforms=[LoadData(dataset)], num_tasks=NUM_TASKS)
+        task_dataset = Taskset(dataset, task_transforms=[LoadData(dataset)], num_tasks=NUM_TASKS)
         self.assertEqual(len(task_dataset), NUM_TASKS)
 
     def test_task_caching(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = TensorDataset(data, labels)
-        task_dataset = TaskDataset(dataset, task_transforms=[LoadData(dataset)], num_tasks=NUM_TASKS)
+        task_dataset = Taskset(dataset, task_transforms=[LoadData(dataset)], num_tasks=NUM_TASKS)
         tasks = []
         for i, task in enumerate(task_dataset, 1):
             tasks.append(task)
         self.assertEqual(i, NUM_TASKS)
         for ref, task in zip(tasks, task_dataset):
             self.assertTrue(task_equal(ref, task))
 
@@ -58,47 +58,48 @@
             task = task_dataset[i]
             self.assertTrue(task_equal(ref, task))
 
     def test_infinite_tasks(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = TensorDataset(data, labels)
-        task_dataset = TaskDataset(dataset, task_transforms=[LoadData(dataset), random_subset])
+        task_dataset = Taskset(dataset, task_transforms=[LoadData(dataset), random_subset])
         self.assertEqual(len(task_dataset), 1)
         prev = task_dataset.sample()
         for i, task in enumerate(task_dataset):
             self.assertFalse(task_equal(prev, task))
             prev = task
             if i > 4:
                 break
 
     def test_task_transforms(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = TensorDataset(data, labels)
-        task_dataset = TaskDataset(dataset,
-                                   task_transforms=[LoadData(dataset), random_subset],
-                                   num_tasks=NUM_TASKS)
+        task_dataset = Taskset(dataset,
+                               task_transforms=[LoadData(dataset), random_subset],
+                               num_tasks=NUM_TASKS)
         for task in task_dataset:
             # Tests transforms on the task_description
             self.assertEqual(len(task[0]), SUBSET_SIZE)
             self.assertEqual(len(task[1]), SUBSET_SIZE)
 
             # Tests transforms on the data
             self.assertEqual(task[0].size(1), X_SHAPE)
             self.assertLessEqual(task[1].max(), Y_SHAPE - 1)
             self.assertGreaterEqual(task[1].max(), 0)
 
     def test_dataloader(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = TensorDataset(data, labels)
-        task_dataset = TaskDataset(dataset,
-                                   task_transforms=[LoadData(dataset), random_subset],
-                                   num_tasks=NUM_TASKS)
+        task_dataset = Taskset(
+            dataset,
+            task_transforms=[LoadData(dataset), random_subset],
+            num_tasks=NUM_TASKS)
         task_loader = DataLoader(task_dataset,
                                  shuffle=True,
                                  batch_size=META_BSZ,
                                  num_workers=WORKERS,
                                  drop_last=True)
         for task_batch in task_loader:
             self.assertEqual(task_batch[0].shape, (META_BSZ, X_SHAPE))
```

### Comparing `learn2learn-0.1.7/tests/unit/data/transforms_test.py` & `learn2learn-0.2.0/tests/unit/data/transforms_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 from unittest import TestCase
 
 import numpy as np
 import torch
 from torch.utils.data import TensorDataset
 
-from learn2learn.data import MetaDataset, TaskDataset
+from learn2learn.data import MetaDataset, Taskset
 from learn2learn.data.transforms import NWays, KShots, LoadData, FilterLabels, RemapLabels
 
 NUM_TASKS = 128
 NUM_DATA = 512
 X_SHAPE = 16
 Y_SHAPE = 10
 EPSILON = 1e-6
@@ -24,70 +24,75 @@
 class TestTransforms(TestCase):
 
     def test_n_ways(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = MetaDataset(TensorDataset(data, labels))
         for ways in range(1, 10):
-            task_dataset = TaskDataset(dataset, 
-                                       task_transforms=[NWays(dataset, n=ways), LoadData(dataset)],
-                                       num_tasks=NUM_TASKS)
+            task_dataset = Taskset(
+                dataset,
+                task_transforms=[NWays(dataset, n=ways), LoadData(dataset)],
+                num_tasks=NUM_TASKS)
             for task in task_dataset:
                 bins = task[1].bincount()
                 num_classes = len(bins) - (bins == 0).sum()
                 self.assertEqual(num_classes, ways)
 
     def test_k_shots(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = MetaDataset(TensorDataset(data, labels))
         for replacement in [False, True]:
             for shots in range(1, 10):
-                task_dataset = TaskDataset(dataset, 
-                                           task_transforms=[KShots(dataset, k=shots, replacement=replacement),
-                                                            LoadData(dataset)],
-                                           num_tasks=NUM_TASKS)
+                task_dataset = Taskset(
+                    dataset,
+                    task_transforms=[KShots(dataset, k=shots, replacement=replacement),
+                                     LoadData(dataset)],
+                    num_tasks=NUM_TASKS)
                 for task in task_dataset:
                     bins = task[1].bincount()
                     correct = (bins == shots).sum()
                     self.assertEqual(correct, Y_SHAPE)
 
     def test_load_data(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = MetaDataset(TensorDataset(data, labels))
-        task_dataset = TaskDataset(dataset, 
-                                   task_transforms=[LoadData(dataset)],
-                                   num_tasks=NUM_TASKS)
+        task_dataset = Taskset(
+            dataset,
+            task_transforms=[LoadData(dataset)],
+            num_tasks=NUM_TASKS)
         for task in task_dataset:
             self.assertTrue(isinstance(task[0], torch.Tensor))
             self.assertTrue(isinstance(task[1], torch.Tensor))
 
     def test_filter_labels(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         chosen_labels = random.sample(list(range(Y_SHAPE)), k=Y_SHAPE//2)
         dataset = MetaDataset(TensorDataset(data, labels))
-        task_dataset = TaskDataset(dataset, 
-                                   task_transforms=[FilterLabels(dataset, chosen_labels), LoadData(dataset)],
-                                   num_tasks=NUM_TASKS)
+        task_dataset = Taskset(
+            dataset,
+            task_transforms=[FilterLabels(dataset, chosen_labels), LoadData(dataset)],
+            num_tasks=NUM_TASKS)
         for task in task_dataset:
             for label in task[1]:
                 self.assertTrue(label in chosen_labels)
 
     def test_remap_labels(self):
         data = torch.randn(NUM_DATA, X_SHAPE)
         labels = torch.randint(0, Y_SHAPE, (NUM_DATA, ))
         dataset = MetaDataset(TensorDataset(data, labels))
         for ways in range(1, 5):
-            task_dataset = TaskDataset(dataset,
-                                       task_transforms=[NWays(dataset, ways),
-                                                        LoadData(dataset),
-                                                        RemapLabels(dataset)],
-                                       num_tasks=NUM_TASKS)
+            task_dataset = Taskset(
+                dataset,
+                task_transforms=[NWays(dataset, ways),
+                                 LoadData(dataset),
+                                 RemapLabels(dataset)],
+                num_tasks=NUM_TASKS)
             for task in task_dataset:
                 for label in range(ways):
                     self.assertTrue(label in task[1])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `learn2learn-0.1.7/tests/unit/data/util_datasets.py` & `learn2learn-0.2.0/tests/unit/data/util_datasets.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/data/utils_test.py` & `learn2learn-0.2.0/tests/unit/data/utils_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/nn/kroneckers_test.py` & `learn2learn-0.2.0/tests/unit/nn/kroneckers_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/nn/metaoptnet_test_notravis.py` & `learn2learn-0.2.0/tests/unit/nn/metaoptnet_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/nn/misc.py` & `learn2learn-0.2.0/tests/unit/nn/misc.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/nn/protonet_test.py` & `learn2learn-0.2.0/tests/unit/nn/protonet_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/utils_test.py` & `learn2learn-0.2.0/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/benchmarks_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/benchmarks_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/cu_birds200_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/cu_birds200_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/describable_textures_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/describable_textures_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/fc100_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/fc100_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/fgvc_aircraft_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/fgvc_aircraft_test_notravis.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,10 +26,17 @@
         self.assertTrue(os.path.exists(path))
 
         aircraft = l2l.vision.datasets.FGVCAircraft(root=root, mode='test')
         image, label = aircraft[12]
         path = os.path.join(root, 'fgvc_aircraft')
         self.assertTrue(os.path.exists(path))
 
+        full_aircrafts = l2l.vision.datasets.FGVCAircraft(root=root, mode='all')
+
+        label_set = set()
+        for item in full_aircrafts:
+            label_set.add(item[1])
+        self.assertTrue(len(label_set) == 100)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `learn2learn-0.1.7/tests/unit/vision/pretrained_backbones_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/pretrained_backbones_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/quickdraw_test_no.py` & `learn2learn-0.2.0/tests/unit/vision/quickdraw_test_no.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/tiered_imagenet_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/tiered_imagenet_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/transform_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/transform_test_notravis.py`

 * *Files identical despite different names*

### Comparing `learn2learn-0.1.7/tests/unit/vision/vgg_flowers_test_notravis.py` & `learn2learn-0.2.0/tests/unit/vision/vgg_flowers_test_notravis.py`

 * *Files identical despite different names*

