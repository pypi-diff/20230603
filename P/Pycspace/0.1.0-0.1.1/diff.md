# Comparing `tmp/Pycspace-0.1.0.tar.gz` & `tmp/Pycspace-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pycspace-0.1.0.tar", last modified: Sat Jun  3 06:54:44 2023, max compression
+gzip compressed data, was "Pycspace-0.1.1.tar", last modified: Sat Jun  3 10:21:32 2023, max compression
```

## Comparing `Pycspace-0.1.0.tar` & `Pycspace-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 dakada   (15179199) registered_users (60000)        0 2023-06-03 06:54:44.431283 Pycspace-0.1.0/
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)      619 2023-06-03 06:54:44.427282 Pycspace-0.1.0/PKG-INFO
-drwxrwxr-x   0 dakada   (15179199) registered_users (60000)        0 2023-06-03 06:54:44.331282 Pycspace-0.1.0/Pycspace.egg-info/
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)      619 2023-06-03 06:54:43.000000 Pycspace-0.1.0/Pycspace.egg-info/PKG-INFO
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)      177 2023-06-03 06:54:43.000000 Pycspace-0.1.0/Pycspace.egg-info/SOURCES.txt
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)        1 2023-06-03 06:54:43.000000 Pycspace-0.1.0/Pycspace.egg-info/dependency_links.txt
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)        9 2023-06-03 06:54:43.000000 Pycspace-0.1.0/Pycspace.egg-info/requires.txt
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)        1 2023-06-03 06:54:43.000000 Pycspace-0.1.0/Pycspace.egg-info/top_level.txt
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)       17 2023-05-07 08:24:25.000000 Pycspace-0.1.0/README.md
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)       38 2023-06-03 06:54:44.431283 Pycspace-0.1.0/setup.cfg
--rw-rw-r--   0 dakada   (15179199) registered_users (60000)     3587 2023-06-03 06:52:35.000000 Pycspace-0.1.0/setup.py
+drwxrwxr-x   0 dakada   (15179199) registered_users (60000)        0 2023-06-03 10:21:32.359413 Pycspace-0.1.1/
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)      650 2023-06-03 10:21:32.355413 Pycspace-0.1.1/PKG-INFO
+drwxrwxr-x   0 dakada   (15179199) registered_users (60000)        0 2023-06-03 10:21:32.343412 Pycspace-0.1.1/Pycspace.egg-info/
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)      650 2023-06-03 10:21:32.000000 Pycspace-0.1.1/Pycspace.egg-info/PKG-INFO
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)      177 2023-06-03 10:21:32.000000 Pycspace-0.1.1/Pycspace.egg-info/SOURCES.txt
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)        1 2023-06-03 10:21:32.000000 Pycspace-0.1.1/Pycspace.egg-info/dependency_links.txt
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)        9 2023-06-03 10:21:32.000000 Pycspace-0.1.1/Pycspace.egg-info/requires.txt
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)        1 2023-06-03 10:21:32.000000 Pycspace-0.1.1/Pycspace.egg-info/top_level.txt
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)       48 2023-06-03 10:00:19.000000 Pycspace-0.1.1/README.md
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)       38 2023-06-03 10:21:32.359413 Pycspace-0.1.1/setup.cfg
+-rw-rw-r--   0 dakada   (15179199) registered_users (60000)     3587 2023-06-03 10:15:55.000000 Pycspace-0.1.1/setup.py
```

### Comparing `Pycspace-0.1.0/PKG-INFO` & `Pycspace-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pycspace
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pycloud
 Home-page: https://github.com/dakadayyds/pycspace
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -13,11 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-# dakada2
-114514
+# Pycloud
 
 
+## 一个强大的云处理器
+
+
+***
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pycspace-0.1.0/Pycspace.egg-info/PKG-INFO` & `Pycspace-0.1.1/Pycspace.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pycspace
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pycloud
 Home-page: https://github.com/dakadayyds/pycspace
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -13,11 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-# dakada2
-114514
+# Pycloud
 
 
+## 一个强大的云处理器
+
+
+***
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pycspace-0.1.0/setup.py` & `Pycspace-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'Pycspace'
 DESCRIPTION = 'Pycloud'
 URL = 'https://github.com/dakadayyds/pycspace'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests'
 ]
 
 # What packages are optional?
```

