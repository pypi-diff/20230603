# Comparing `tmp/tfliteiorewriter-0.0.2.tar.gz` & `tmp/tfliteiorewriter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfliteiorewriter-0.0.2.tar", last modified: Sat Jun  3 08:40:27 2023, max compression
+gzip compressed data, was "tfliteiorewriter-1.0.0.tar", last modified: Sat Jun  3 08:48:26 2023, max compression
```

## Comparing `tfliteiorewriter-0.0.2.tar` & `tfliteiorewriter-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/tfliteiorewriter/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/tfliteiorewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 08:40:26.000000 tfliteiorewriter-0.0.2/tfliteiorewriter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 08:40:12.000000 tfliteiorewriter-0.0.2/tfliteiorewriter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:40:27.091420 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:40:27.000000 tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.889346 tfliteiorewriter-1.0.0/tfliteiorewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 08:48:16.000000 tfliteiorewriter-1.0.0/tfliteiorewriter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:48:26.893346 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:48:26.000000 tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/top_level.txt
```

### Comparing `tfliteiorewriter-0.0.2/.github/workflows/codeql-analysis.yml` & `tfliteiorewriter-1.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/.github/workflows/python-publish.yml` & `tfliteiorewriter-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/Dockerfile` & `tfliteiorewriter-1.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/LICENSE` & `tfliteiorewriter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/PKG-INFO` & `tfliteiorewriter-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 0.0.2
+Version: 1.0.0
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,25 +59,25 @@
 
     Username (xxxx): {Enter}
     Password: {Personal Access Token}
     Login Succeeded
 
     $ docker run --rm -it \
     -v `pwd`:/home/user \
-    ghcr.io/pinto0309/tfliteiorewriter:latest
+    ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
     sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
     pip install -U tfliteiorewriter
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
 usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
```

### Comparing `tfliteiorewriter-0.0.2/README.md` & `tfliteiorewriter-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 
     Username (xxxx): {Enter}
     Password: {Personal Access Token}
     Login Succeeded
 
     $ docker run --rm -it \
     -v `pwd`:/home/user \
-    ghcr.io/pinto0309/tfliteiorewriter:latest
+    ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
     sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
     pip install -U tfliteiorewriter
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
 usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
```

### Comparing `tfliteiorewriter-0.0.2/pyproject.toml` & `tfliteiorewriter-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/tfliteiorewriter/main.py` & `tfliteiorewriter-1.0.0/tfliteiorewriter/main.py`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-0.0.2/tfliteiorewriter.egg-info/PKG-INFO` & `tfliteiorewriter-1.0.0/tfliteiorewriter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 0.0.2
+Version: 1.0.0
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,25 +59,25 @@
 
     Username (xxxx): {Enter}
     Password: {Personal Access Token}
     Login Succeeded
 
     $ docker run --rm -it \
     -v `pwd`:/home/user \
-    ghcr.io/pinto0309/tfliteiorewriter:latest
+    ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
     sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
     pip install -U tfliteiorewriter
 
-    tfliteiorewriter -i xxxx.tflite
+    $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
 usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
```

