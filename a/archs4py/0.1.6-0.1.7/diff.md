# Comparing `tmp/archs4py-0.1.6.tar.gz` & `tmp/archs4py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.1.6.tar", last modified: Sat Jun  3 02:36:16 2023, max compression
+gzip compressed data, was "archs4py-0.1.7.tar", last modified: Sat Jun  3 03:14:04 2023, max compression
```

## Comparing `archs4py-0.1.6.tar` & `archs4py-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177864 archs4py-0.1.6/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.6/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 02:36:16.177701 archs4py-0.1.6/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.6/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.176147 archs4py-0.1.6/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.6/archs4py/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177301 archs4py-0.1.6/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.6/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.6/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.6/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.6/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.6/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177150 archs4py-0.1.6/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      111 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 02:36:16.177922 archs4py-0.1.6/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)      876 2023-06-03 02:36:12.000000 archs4py-0.1.6/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 03:14:04.799393 archs4py-0.1.7/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.7/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6749 2023-06-03 03:14:04.799260 archs4py-0.1.7/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.7/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 03:14:04.797915 archs4py-0.1.7/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.7/archs4py/__init__.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 03:14:04.798903 archs4py-0.1.7/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.7/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.7/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.7/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.7/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.7/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 03:14:04.798781 archs4py-0.1.7/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6749 2023-06-03 03:14:04.000000 archs4py-0.1.7/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 03:14:04.000000 archs4py-0.1.7/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 03:14:04.000000 archs4py-0.1.7/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      110 2023-06-03 03:14:04.000000 archs4py-0.1.7/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 03:14:04.000000 archs4py-0.1.7/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 03:14:04.799490 archs4py-0.1.7/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)      876 2023-06-03 03:09:45.000000 archs4py-0.1.7/setup.py
```

### Comparing `archs4py-0.1.6/LICENSE` & `archs4py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/PKG-INFO` & `archs4py-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.6
+Version: 0.1.7
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -164,7 +166,9 @@
 
 ```python
 import archs4 as a4
 
 print(a4.versions())
 
 ```
+
+
```

### Comparing `archs4py-0.1.6/README.md` & `archs4py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py/data/config.json` & `archs4py-0.1.7/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py/data.py` & `archs4py-0.1.7/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py/download.py` & `archs4py-0.1.7/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py/meta.py` & `archs4py-0.1.7/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py/utils.py` & `archs4py-0.1.7/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.6/archs4py.egg-info/PKG-INFO` & `archs4py-0.1.7/archs4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.6
+Version: 0.1.7
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -164,7 +166,9 @@
 
 ```python
 import archs4 as a4
 
 print(a4.versions())
 
 ```
+
+
```

### Comparing `archs4py-0.1.6/setup.py` & `archs4py-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.1.6",
+    version="0.1.7",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
```

