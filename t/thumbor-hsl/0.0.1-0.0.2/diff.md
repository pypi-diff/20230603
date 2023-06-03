# Comparing `tmp/thumbor_hsl-0.0.1.tar.gz` & `tmp/thumbor_hsl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thumbor_hsl-0.0.1.tar", last modified: Sat Jun  3 12:21:38 2023, max compression
+gzip compressed data, was "thumbor_hsl-0.0.2.tar", last modified: Sat Jun  3 12:32:55 2023, max compression
```

## Comparing `thumbor_hsl-0.0.1.tar` & `thumbor_hsl-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/thumbor_hsl/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/thumbor_hsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/thumbor_hsl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/thumbor_hsl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-03 12:21:25.000000 thumbor_hsl-0.0.1/thumbor_hsl/loaders/http_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:21:38.989274 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-03 12:21:38.000000 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-03 12:21:38.000000 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:21:38.000000 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 12:21:38.000000 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 12:21:38.000000 thumbor_hsl-0.0.1/thumbor_hsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/loaders/http_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/top_level.txt
```

### Comparing `thumbor_hsl-0.0.1/LICENSE` & `thumbor_hsl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbor_hsl-0.0.1/PKG-INFO` & `thumbor_hsl-0.0.2/thumbor_hsl.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: thumbor_hsl
-Version: 0.0.1
-Summary: A modified `http` loader for thumbor which introduces an additional statd counter to track headers
-Home-page: https://github.com/BowlingX/thumbor-http-header-stats-loader
+Name: thumbor-hsl
+Version: 0.0.2
+Summary: A modified `http` loader for thumbor which provides additional statistics (like width, height and url parsing)
+Home-page: https://github.com/BowlingX/thumbor-http-stats-loader
 Author: David Heidrich
 Author-email: me@bowlingx.com
 License: MIT
 License-File: LICENSE
 
 thumbor-http-stats-loader
 --------------------------------
@@ -28,8 +28,8 @@
     HSL_REGEX_MATCH_URL="someQuery=(\d+)"
 
 For a given url, e.g. `https://my-image?someQuery=10` the result of `10` will be appended to the counter.
 
 
 ## Install
 
-    pip install https://github.com/BowlingX/thumbor-http-header-stats-loader/archive/1.0.0.zip  
+    pip install thumbor_hsl
```

### Comparing `thumbor_hsl-0.0.1/setup.py` & `thumbor_hsl-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,17 +7,18 @@
     """print long description"""
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='thumbor_hsl',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
-    url='https://github.com/BowlingX/thumbor-http-header-stats-loader',
+    url='https://github.com/BowlingX/thumbor-http-stats-loader',
     license='MIT',
     author='David Heidrich',
     author_email='me@bowlingx.com',
     install_requires=['thumbor>=7.0.0a2,<8'],
-    description='A modified `http` loader for thumbor which introduces an additional statd counter to track headers',
+    description='A modified `http` loader for thumbor which provides additional statistics '
+                '(like width, height and url parsing)',
     long_description=readme(),
 )
```

### Comparing `thumbor_hsl-0.0.1/thumbor_hsl/loaders/http_loader.py` & `thumbor_hsl-0.0.2/thumbor_hsl/loaders/http_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_hsl-0.0.1/thumbor_hsl.egg-info/PKG-INFO` & `thumbor_hsl-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: thumbor-hsl
-Version: 0.0.1
-Summary: A modified `http` loader for thumbor which introduces an additional statd counter to track headers
-Home-page: https://github.com/BowlingX/thumbor-http-header-stats-loader
+Name: thumbor_hsl
+Version: 0.0.2
+Summary: A modified `http` loader for thumbor which provides additional statistics (like width, height and url parsing)
+Home-page: https://github.com/BowlingX/thumbor-http-stats-loader
 Author: David Heidrich
 Author-email: me@bowlingx.com
 License: MIT
 License-File: LICENSE
 
 thumbor-http-stats-loader
 --------------------------------
@@ -28,8 +28,8 @@
     HSL_REGEX_MATCH_URL="someQuery=(\d+)"
 
 For a given url, e.g. `https://my-image?someQuery=10` the result of `10` will be appended to the counter.
 
 
 ## Install
 
-    pip install https://github.com/BowlingX/thumbor-http-header-stats-loader/archive/1.0.0.zip  
+    pip install thumbor_hsl
```

