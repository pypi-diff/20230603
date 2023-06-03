# Comparing `tmp/firegs-0.2.tar.gz` & `tmp/firegs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firegs-0.2.tar", last modified: Sat Jun  3 16:02:33 2023, max compression
+gzip compressed data, was "firegs-0.3.tar", last modified: Sat Jun  3 16:20:23 2023, max compression
```

## Comparing `firegs-0.2.tar` & `firegs-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:02:33.725684 firegs-0.2/
--rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.2/LICENSE
--rw-r--r--   0 ask        (501) staff       (20)     1367 2023-06-03 16:02:33.725542 firegs-0.2/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.2/README.md
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:02:33.724145 firegs-0.2/firegs/
--rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.2/firegs/__init__.py
--rw-r--r--   0 ask        (501) staff       (20)     5642 2023-06-03 15:57:54.000000 firegs-0.2/firegs/script.py
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:02:33.725330 firegs-0.2/firegs.egg-info/
--rw-r--r--   0 ask        (501) staff       (20)     1367 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      244 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/SOURCES.txt
--rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/dependency_links.txt
--rw-r--r--   0 ask        (501) staff       (20)       47 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/entry_points.txt
--rw-r--r--   0 ask        (501) staff       (20)      119 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/requires.txt
--rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:02:33.000000 firegs-0.2/firegs.egg-info/top_level.txt
--rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:02:33.725740 firegs-0.2/setup.cfg
--rw-r--r--   0 ask        (501) staff       (20)      876 2023-06-03 16:02:12.000000 firegs-0.2/setup.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.288804 firegs-0.3/
+-rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.3/LICENSE
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:20:23.288631 firegs-0.3/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.3/README.md
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.287197 firegs-0.3/firegs/
+-rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.3/firegs/__init__.py
+-rw-r--r--   0 ask        (501) staff       (20)     5642 2023-06-03 15:57:54.000000 firegs-0.3/firegs/script.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.288378 firegs-0.3/firegs.egg-info/
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      244 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/SOURCES.txt
+-rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/dependency_links.txt
+-rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/entry_points.txt
+-rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/requires.txt
+-rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/top_level.txt
+-rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:20:23.288851 firegs-0.3/setup.cfg
+-rw-r--r--   0 ask        (501) staff       (20)      834 2023-06-03 16:19:11.000000 firegs-0.3/setup.py
```

### Comparing `firegs-0.2/LICENSE` & `firegs-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `firegs-0.2/PKG-INFO` & `firegs-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.2
+Version: 0.3
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FireGS
 
@@ -47,9 +45,7 @@
 ```
 
 ## License
 
 FireGS is released under the MIT License. See the LICENSE file for more details.
 
 
-
-
```

### Comparing `firegs-0.2/README.md` & `firegs-0.3/README.md`

 * *Files identical despite different names*

### Comparing `firegs-0.2/firegs/script.py` & `firegs-0.3/firegs/script.py`

 * *Files identical despite different names*

### Comparing `firegs-0.2/firegs.egg-info/PKG-INFO` & `firegs-0.3/firegs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.2
+Version: 0.3
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FireGS
 
@@ -47,9 +45,7 @@
 ```
 
 ## License
 
 FireGS is released under the MIT License. See the LICENSE file for more details.
 
 
-
-
```

### Comparing `firegs-0.2/setup.py` & `firegs-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="firegs",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     install_requires=[
         'requests',
         'google-auth',
         'google-auth-httplib2',
         'google-auth-oauthlib',
         'google-api-python-client',
-        'google-auth-transport-requests',
     ],
     entry_points={
         'console_scripts': [
             'firegs = firegs.script:main',
         ],
     },
     author="Android Dev Notes",
```

