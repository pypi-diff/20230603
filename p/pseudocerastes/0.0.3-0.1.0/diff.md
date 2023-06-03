# Comparing `tmp/pseudocerastes-0.0.3.tar.gz` & `tmp/pseudocerastes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudocerastes-0.0.3.tar", last modified: Sat Jun  3 14:52:15 2023, max compression
+gzip compressed data, was "pseudocerastes-0.1.0.tar", last modified: Sat Jun  3 14:53:45 2023, max compression
```

## Comparing `pseudocerastes-0.0.3.tar` & `pseudocerastes-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-05-20 19:01:15.000000 pseudocerastes-0.0.3/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-05-20 19:01:15.000000 pseudocerastes-0.0.3/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      823 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       60 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/README.md
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-05-20 19:01:15.000000 pseudocerastes-0.0.3/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1131 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:52:15.700369 pseudocerastes-0.0.3/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/src/pseudocerastes/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       30 2023-05-20 19:01:15.000000 pseudocerastes-0.0.3/src/pseudocerastes/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      456 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/src/pseudocerastes/common.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/src/pseudocerastes/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-05-20 19:01:15.000000 pseudocerastes-0.0.3/src/pseudocerastes/core/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      933 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/src/pseudocerastes/core/html.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1470 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/src/pseudocerastes/core/parser.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:52:15.704369 pseudocerastes-0.0.3/src/pseudocerastes.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      823 2023-06-03 14:52:15.000000 pseudocerastes-0.0.3/src/pseudocerastes.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      395 2023-06-03 14:52:15.000000 pseudocerastes-0.0.3/src/pseudocerastes.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-06-03 14:52:15.000000 pseudocerastes-0.0.3/src/pseudocerastes.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       15 2023-06-03 14:52:15.000000 pseudocerastes-0.0.3/src/pseudocerastes.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-06-03 14:52:07.000000 pseudocerastes-0.0.3/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-05-20 19:01:15.000000 pseudocerastes-0.1.0/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-05-20 19:01:15.000000 pseudocerastes-0.1.0/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      823 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       60 2023-06-03 14:52:07.000000 pseudocerastes-0.1.0/README.md
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-05-20 19:01:15.000000 pseudocerastes-0.1.0/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1131 2023-06-03 14:52:07.000000 pseudocerastes-0.1.0/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:53:45.205511 pseudocerastes-0.1.0/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/src/pseudocerastes/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       30 2023-05-20 19:01:15.000000 pseudocerastes-0.1.0/src/pseudocerastes/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      456 2023-06-03 14:52:07.000000 pseudocerastes-0.1.0/src/pseudocerastes/common.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/src/pseudocerastes/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-05-20 19:01:15.000000 pseudocerastes-0.1.0/src/pseudocerastes/core/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      933 2023-06-03 14:52:07.000000 pseudocerastes-0.1.0/src/pseudocerastes/core/html.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1470 2023-06-03 14:52:07.000000 pseudocerastes-0.1.0/src/pseudocerastes/core/parser.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-06-03 14:53:45.213512 pseudocerastes-0.1.0/src/pseudocerastes.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      823 2023-06-03 14:53:45.000000 pseudocerastes-0.1.0/src/pseudocerastes.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      395 2023-06-03 14:53:45.000000 pseudocerastes-0.1.0/src/pseudocerastes.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-06-03 14:53:45.000000 pseudocerastes-0.1.0/src/pseudocerastes.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       15 2023-06-03 14:53:45.000000 pseudocerastes-0.1.0/src/pseudocerastes.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-06-03 14:53:37.000000 pseudocerastes-0.1.0/version.txt
```

### Comparing `pseudocerastes-0.0.3/LICENSE` & `pseudocerastes-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pseudocerastes-0.0.3/PKG-INFO` & `pseudocerastes-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pseudocerastes
-Version: 0.0.3
+Version: 0.1.0
 Summary: A simple html parsing tool
 Home-page: https://github.com/LostSavannah/pseudocerastes
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pseudocerastes/issues
 Project-URL: Documentation, https://dev.moradev.dev/pseudocerastes/documentation
 Project-URL: Examples, https://dev.moradev.dev/pseudocerastes/examples
```

### Comparing `pseudocerastes-0.0.3/setup.py` & `pseudocerastes-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pseudocerastes-0.0.3/src/pseudocerastes/core/html.py` & `pseudocerastes-0.1.0/src/pseudocerastes/core/html.py`

 * *Files identical despite different names*

### Comparing `pseudocerastes-0.0.3/src/pseudocerastes/core/parser.py` & `pseudocerastes-0.1.0/src/pseudocerastes/core/parser.py`

 * *Files identical despite different names*

### Comparing `pseudocerastes-0.0.3/src/pseudocerastes.egg-info/PKG-INFO` & `pseudocerastes-0.1.0/src/pseudocerastes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pseudocerastes
-Version: 0.0.3
+Version: 0.1.0
 Summary: A simple html parsing tool
 Home-page: https://github.com/LostSavannah/pseudocerastes
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pseudocerastes/issues
 Project-URL: Documentation, https://dev.moradev.dev/pseudocerastes/documentation
 Project-URL: Examples, https://dev.moradev.dev/pseudocerastes/examples
```

