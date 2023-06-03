# Comparing `tmp/tfliteiorewriter-1.0.1.tar.gz` & `tmp/tfliteiorewriter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfliteiorewriter-1.0.1.tar", last modified: Sat Jun  3 09:03:59 2023, max compression
+gzip compressed data, was "tfliteiorewriter-1.0.2.tar", last modified: Sat Jun  3 12:04:44 2023, max compression
```

## Comparing `tfliteiorewriter-1.0.1.tar` & `tfliteiorewriter-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.480971 tfliteiorewriter-1.0.1/tfliteiorewriter/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 09:03:48.000000 tfliteiorewriter-1.0.1/tfliteiorewriter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:59.484971 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 09:03:59.000000 tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.844712 tfliteiorewriter-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.848712 tfliteiorewriter-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.848712 tfliteiorewriter-1.0.2/tfliteiorewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-03 12:04:32.000000 tfliteiorewriter-1.0.2/tfliteiorewriter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:04:44.852712 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 12:04:44.000000 tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/top_level.txt
```

### Comparing `tfliteiorewriter-1.0.1/.github/workflows/codeql-analysis.yml` & `tfliteiorewriter-1.0.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.1/.github/workflows/python-publish.yml` & `tfliteiorewriter-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.1/Dockerfile` & `tfliteiorewriter-1.0.2/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 SHELL ["/bin/bash", "-c"]
 
 RUN apt-get update \
     && apt-get install -y \
         python3-pip \
         python-is-python3 \
-        flatbuffers-compiler \
         sudo \
+        wget \
     && pip install -U pip \
     && pip install -U tfliteiorewriter \
     && pip install -U tfliteiorewriter \
     && apt clean \
     && rm -rf /var/lib/apt/lists/*
 
 ENV USERNAME=user
@@ -26,8 +26,14 @@
         --groups adm,sudo \
         ${USERNAME} \
     && echo "${USERNAME}:${USERNAME}" | chpasswd \
     && cat /dev/null > /etc/sudoers.d/${USERNAME} \
     && echo "%${USERNAME}    ALL=(ALL)   NOPASSWD:    ALL" >> \
         /etc/sudoers.d/${USERNAME}
 USER ${USERNAME}
-WORKDIR /home/${USERNAME}
+WORKDIR /home/${USERNAME}
+
+RUN wget https://github.com/PINTO0309/onnx2tf/releases/download/1.7.3/flatc.tar.gz \
+    && tar -zxvf flatc.tar.gz \
+    && sudo chmod +x flatc \
+    && sudo mv flatc /usr/bin/ \
+    && rm flatc.tar.gz
```

### Comparing `tfliteiorewriter-1.0.1/LICENSE` & `tfliteiorewriter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.1/PKG-INFO` & `tfliteiorewriter-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.1
+Version: 1.0.2
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,22 +65,27 @@
     -v `pwd`:/home/user \
     ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
-    sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
+    $ sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
-    pip install -U tfliteiorewriter
+    $ pip install -U tfliteiorewriter
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
-usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
+usage: tfliteiorewriter
+  [-h]
+  -i INPUT_TFLITE_FILE_PATH
+  [-v]
+  [-o OUTPUT_FOLDER_PATH]
+  [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
 
   -i INPUT_TFLITE_FILE_PATH, --input_tflite_file_path INPUT_TFLITE_FILE_PATH
       Input tflite file path.
```

### Comparing `tfliteiorewriter-1.0.1/README.md` & `tfliteiorewriter-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,27 @@
     -v `pwd`:/home/user \
     ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
-    sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
+    $ sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
-    pip install -U tfliteiorewriter
+    $ pip install -U tfliteiorewriter
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
-usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
+usage: tfliteiorewriter
+  [-h]
+  -i INPUT_TFLITE_FILE_PATH
+  [-v]
+  [-o OUTPUT_FOLDER_PATH]
+  [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
 
   -i INPUT_TFLITE_FILE_PATH, --input_tflite_file_path INPUT_TFLITE_FILE_PATH
       Input tflite file path.
```

### Comparing `tfliteiorewriter-1.0.1/pyproject.toml` & `tfliteiorewriter-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.1/tfliteiorewriter/main.py` & `tfliteiorewriter-1.0.2/tfliteiorewriter/main.py`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.1/tfliteiorewriter.egg-info/PKG-INFO` & `tfliteiorewriter-1.0.2/tfliteiorewriter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.1
+Version: 1.0.2
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,22 +65,27 @@
     -v `pwd`:/home/user \
     ghcr.io/pinto0309/tflite-input-output-rewriter:latest
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 2. Local
     ```bash
-    sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
+    $ sudo apt-get update && sudo apt-get install -y flatbuffers-compiler
     # Other than debian/ubuntu: https://github.com/google/flatbuffers/releases
-    pip install -U tfliteiorewriter
+    $ pip install -U tfliteiorewriter
 
     $ tfliteiorewriter -i xxxx.tflite
     ```
 ```
-usage: tfliteiorewriter [-h] -i INPUT_TFLITE_FILE_PATH [-v] [-o OUTPUT_FOLDER_PATH] [-r RENAME RENAME]
+usage: tfliteiorewriter
+  [-h]
+  -i INPUT_TFLITE_FILE_PATH
+  [-v]
+  [-o OUTPUT_FOLDER_PATH]
+  [-r RENAME RENAME]
 
 optional arguments:
   -h, --help
       show this help message and exit
 
   -i INPUT_TFLITE_FILE_PATH, --input_tflite_file_path INPUT_TFLITE_FILE_PATH
       Input tflite file path.
```

