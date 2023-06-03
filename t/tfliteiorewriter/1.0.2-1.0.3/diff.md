# Comparing `tmp/tfliteiorewriter-1.0.2.tar.gz` & `tmp/tfliteiorewriter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfliteiorewriter-1.0.2.tar", last modified: Sat Jun  3 12:04:44 2023, max compression
+gzip compressed data, was "tfliteiorewriter-1.0.3.tar", last modified: Sat Jun  3 15:50:00 2023, max compression
```

## Comparing `tfliteiorewriter-1.0.2.tar` & `tfliteiorewriter-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.844712 tfliteiorewriter-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.848712 tfliteiorewriter-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.848712 tfliteiorewriter-1.0.2/tfliteiorewriter/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/tfliteiorewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/top_level.txt
```

### Comparing `tfliteiorewriter-1.0.2/.github/workflows/codeql-analysis.yml` & `tfliteiorewriter-1.0.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.2/.github/workflows/python-publish.yml` & `tfliteiorewriter-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.2/Dockerfile` & `tfliteiorewriter-1.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.2/LICENSE` & `tfliteiorewriter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.2/PKG-INFO` & `tfliteiorewriter-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.2
+Version: 1.0.3
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
-- flatbuffers-compiler
+- flatbuffers-compiler (Note: Official binaries are degraded by lack of precision when processing INT8 quantized tflite files.)
 - requests
 
 ## Motivation
 The purpose is to solve the following problems by forcibly rewriting tflite's input/output OP names.
 
 - When TFLite models are generated, TensorFlow automatically prefixes the input OP name with `serving_default_`, resulting in very difficult-to-read models. Also, an unnecessary index `:n` is added to the end of the name.
```

### Comparing `tfliteiorewriter-1.0.2/README.md` & `tfliteiorewriter-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
-- flatbuffers-compiler
+- flatbuffers-compiler (Note: Official binaries are degraded by lack of precision when processing INT8 quantized tflite files.)
 - requests
 
 ## Motivation
 The purpose is to solve the following problems by forcibly rewriting tflite's input/output OP names.
 
 - When TFLite models are generated, TensorFlow automatically prefixes the input OP name with `serving_default_`, resulting in very difficult-to-read models. Also, an unnecessary index `:n` is added to the end of the name.
```

### Comparing `tfliteiorewriter-1.0.2/pyproject.toml` & `tfliteiorewriter-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.2/tfliteiorewriter/main.py` & `tfliteiorewriter-1.0.3/tfliteiorewriter/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         output_json_file_path = f'{output_path}/{output_json_file_name}'
         flat_json = None
 
         with open(input_json_file_path, 'r') as f:
             flat_json = json.load(f)
 
         # Checks if signature_defs are recorded in tflite
-        if 'signature_defs' not in flat_json:
+        if 'signature_defs' not in flat_json or not flat_json['signature_defs']:
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} ' +
                 f'Processing is aborted because signature_defs is not recorded in tflite.'
             )
             sys.exit(0)
 
         flat_subgraphs = flat_json['subgraphs'][0]
```

### Comparing `tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/PKG-INFO` & `tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.2
+Version: 1.0.3
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 # tflite-input-output-rewriter
 This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tfliteiorewriter?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tfliteiorewriter) ![GitHub](https://img.shields.io/github/license/PINTO0309/tflite-input-output-rewriter?color=2BAF2B) [![Python](https://img.shields.io/badge/Python-3.8-2BAF2B)](https://img.shields.io/badge/Python-3.8-2BAF2B) [![PyPI](https://img.shields.io/pypi/v/tfliteiorewriter?color=2BAF2B)](https://pypi.org/project/tfliteiorewriter/)
 
 ## Environment
 - Ubuntu 20.04+
-- flatbuffers-compiler
+- flatbuffers-compiler (Note: Official binaries are degraded by lack of precision when processing INT8 quantized tflite files.)
 - requests
 
 ## Motivation
 The purpose is to solve the following problems by forcibly rewriting tflite's input/output OP names.
 
 - When TFLite models are generated, TensorFlow automatically prefixes the input OP name with `serving_default_`, resulting in very difficult-to-read models. Also, an unnecessary index `:n` is added to the end of the name.
```

