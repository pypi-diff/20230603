# Comparing `tmp/archs4py-0.1.5.tar.gz` & `tmp/archs4py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.1.5.tar", last modified: Sat Jun  3 02:30:12 2023, max compression
+gzip compressed data, was "archs4py-0.1.6.tar", last modified: Sat Jun  3 02:36:16 2023, max compression
```

## Comparing `archs4py-0.1.5.tar` & `archs4py-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:30:12.130873 archs4py-0.1.5/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.5/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     6749 2023-06-03 02:30:12.130684 archs4py-0.1.5/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     6262 2023-06-03 02:29:32.000000 archs4py-0.1.5/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:30:12.127956 archs4py-0.1.5/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.5/archs4py/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:30:12.130160 archs4py-0.1.5/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.5/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.5/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.5/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.5/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.5/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:30:12.129997 archs4py-0.1.5/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6749 2023-06-03 02:30:12.000000 archs4py-0.1.5/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 02:30:12.000000 archs4py-0.1.5/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 02:30:12.000000 archs4py-0.1.5/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      111 2023-06-03 02:30:12.000000 archs4py-0.1.5/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 02:30:12.000000 archs4py-0.1.5/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 02:30:12.130933 archs4py-0.1.5/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)      876 2022-11-16 22:18:58.000000 archs4py-0.1.5/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177864 archs4py-0.1.6/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.6/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 02:36:16.177701 archs4py-0.1.6/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.6/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.176147 archs4py-0.1.6/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.6/archs4py/__init__.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177301 archs4py-0.1.6/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.6/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.6/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.6/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.6/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.6/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 02:36:16.177150 archs4py-0.1.6/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      111 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 02:36:16.000000 archs4py-0.1.6/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 02:36:16.177922 archs4py-0.1.6/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)      876 2023-06-03 02:36:12.000000 archs4py-0.1.6/setup.py
```

### Comparing `archs4py-0.1.5/LICENSE` & `archs4py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/PKG-INFO` & `archs4py-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
 
 ```
-pip3 install git+https://github.com/MaayanLab/archs4py.git
+pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
```

### Comparing `archs4py-0.1.5/README.md` & `archs4py-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
 
 ```
-pip3 install git+https://github.com/MaayanLab/archs4py.git
+pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
```

### Comparing `archs4py-0.1.5/archs4py/data/config.json` & `archs4py-0.1.6/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/archs4py/data.py` & `archs4py-0.1.6/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/archs4py/download.py` & `archs4py-0.1.6/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/archs4py/meta.py` & `archs4py-0.1.6/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/archs4py/utils.py` & `archs4py-0.1.6/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.5/archs4py.egg-info/PKG-INFO` & `archs4py-0.1.6/archs4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
 
 ```
-pip3 install git+https://github.com/MaayanLab/archs4py.git
+pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
```

### Comparing `archs4py-0.1.5/setup.py` & `archs4py-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.1.5",
+    version="0.1.6",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
```

