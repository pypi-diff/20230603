# Comparing `tmp/archs4py-0.1.8.tar.gz` & `tmp/archs4py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.1.8.tar", last modified: Sat Jun  3 04:19:32 2023, max compression
+gzip compressed data, was "archs4py-0.1.9.tar", last modified: Sat Jun  3 04:22:22 2023, max compression
```

## Comparing `archs4py-0.1.8.tar` & `archs4py-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:19:32.640880 archs4py-0.1.8/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.8/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:19:32.640702 archs4py-0.1.8/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.8/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:19:32.638853 archs4py-0.1.8/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.8/archs4py/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:19:32.640267 archs4py-0.1.8/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.8/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.8/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.8/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.8/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.8/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:19:32.640095 archs4py-0.1.8/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:19:32.000000 archs4py-0.1.8/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 04:19:32.000000 archs4py-0.1.8/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 04:19:32.000000 archs4py-0.1.8/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      110 2023-06-03 04:19:32.000000 archs4py-0.1.8/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 04:19:32.000000 archs4py-0.1.8/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 04:19:32.640935 archs4py-0.1.8/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)      876 2023-06-03 04:18:49.000000 archs4py-0.1.8/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333773 archs4py-0.1.9/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.9/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:22:22.333638 archs4py-0.1.9/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.9/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.332304 archs4py-0.1.9/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.9/archs4py/__init__.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333337 archs4py-0.1.9/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.9/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.9/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.9/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.9/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.9/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333195 archs4py-0.1.9/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      110 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 04:22:22.333820 archs4py-0.1.9/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1018 2023-06-03 04:22:12.000000 archs4py-0.1.9/setup.py
```

### Comparing `archs4py-0.1.8/LICENSE` & `archs4py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/PKG-INFO` & `archs4py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.8
+Version: 0.1.9
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `archs4py-0.1.8/README.md` & `archs4py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py/data/config.json` & `archs4py-0.1.9/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py/data.py` & `archs4py-0.1.9/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py/download.py` & `archs4py-0.1.9/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py/meta.py` & `archs4py-0.1.9/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py/utils.py` & `archs4py-0.1.9/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.8/archs4py.egg-info/PKG-INFO` & `archs4py-0.1.9/archs4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.8
+Version: 0.1.9
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `archs4py-0.1.8/setup.py` & `archs4py-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.1.8",
+    version="0.1.9",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
@@ -18,10 +18,19 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_data={
         "archs4py": ["data/*"]
     },
     include_package_data=True,
-    install_requires=list(map(str.strip, open('requirements.txt', 'r').readlines())),
+    install_requires=[
+        'h5py==3.8.0',
+        'numpy==1.24.3',
+        'pandas==2.0.2',
+        'qnorm==0.8.1',
+        'setuptools==67.8.0',
+        'tqdm==4.65.0',
+        'wget==3.2',
+        's3fs==2023.5.0',
+    ],
     python_requires='>=3.7',
 )
```

