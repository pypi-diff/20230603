# Comparing `tmp/tfliteiorewriter-1.0.0.tar.gz` & `tmp/tfliteiorewriter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfliteiorewriter-1.0.0.tar", last modified: Sat Jun  3 08:48:26 2023, max compression
+gzip compressed data, was "tfliteiorewriter-1.0.1.tar", last modified: Sat Jun  3 09:03:59 2023, max compression
```

## Comparing `tfliteiorewriter-1.0.0.tar` & `tfliteiorewriter-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/tfliteiorewriter/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/tfliteiorewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/top_level.txt
```

### Comparing `tfliteiorewriter-1.0.0/.github/workflows/codeql-analysis.yml` & `tfliteiorewriter-1.0.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/.github/workflows/python-publish.yml` & `tfliteiorewriter-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/Dockerfile` & `tfliteiorewriter-1.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/LICENSE` & `tfliteiorewriter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/PKG-INFO` & `tfliteiorewriter-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.0
+Version: 1.0.1
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
-[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tfliteiorewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
+[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
 - flatbuffers-compiler
 - requests
 
 ## Motivation
```

### Comparing `tfliteiorewriter-1.0.0/README.md` & `tfliteiorewriter-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
-[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tfliteiorewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
+[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
 - flatbuffers-compiler
 - requests
 
 ## Motivation
```

### Comparing `tfliteiorewriter-1.0.0/pyproject.toml` & `tfliteiorewriter-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/tfliteiorewriter/main.py` & `tfliteiorewriter-1.0.1/tfliteiorewriter/main.py`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/PKG-INFO` & `tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.0
+Version: 1.0.1
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
-[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tfliteiorewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
+[![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
 - flatbuffers-compiler
 - requests
 
 ## Motivation
```

