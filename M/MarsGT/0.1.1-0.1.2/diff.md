# Comparing `tmp/MarsGT-0.1.1.tar.gz` & `tmp/MarsGT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MarsGT-0.1.1.tar", last modified: Sat Jun  3 07:00:04 2023, max compression
+gzip compressed data, was "dist/MarsGT-0.1.2.tar", last modified: Sat Jun  3 07:23:55 2023, max compression
```

## Comparing `MarsGT-0.1.1.tar` & `MarsGT-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:00:04.736046 MarsGT-0.1.1/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.1/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:00:04.710050 MarsGT-0.1.1/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.1/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 06:21:55.000000 MarsGT-0.1.1/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6007 2023-06-03 06:21:56.000000 MarsGT-0.1.1/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21321 2023-06-03 06:21:56.000000 MarsGT-0.1.1/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 06:21:57.000000 MarsGT-0.1.1/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:00:04.731046 MarsGT-0.1.1/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      965 2023-06-03 07:00:04.000000 MarsGT-0.1.1/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 07:00:04.000000 MarsGT-0.1.1/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 07:00:04.000000 MarsGT-0.1.1/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      290 2023-06-03 07:00:04.000000 MarsGT-0.1.1/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 07:00:04.000000 MarsGT-0.1.1/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      965 2023-06-03 07:00:04.734067 MarsGT-0.1.1/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.1/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 07:00:04.736066 MarsGT-0.1.1/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1012 2023-06-03 06:59:43.000000 MarsGT-0.1.1/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.133795 MarsGT-0.1.2/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.2/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.097783 MarsGT-0.1.2/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.2/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 06:21:55.000000 MarsGT-0.1.2/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6007 2023-06-03 06:21:56.000000 MarsGT-0.1.2/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21321 2023-06-03 06:21:56.000000 MarsGT-0.1.2/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 06:21:57.000000 MarsGT-0.1.2/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.115785 MarsGT-0.1.2/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      323 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:23:55.131785 MarsGT-0.1.2/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.2/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 07:23:55.134787 MarsGT-0.1.2/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1077 2023-06-03 07:22:43.000000 MarsGT-0.1.2/setup.py
```

### Comparing `MarsGT-0.1.1/MarsGT/conv.py` & `MarsGT-0.1.2/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.1/MarsGT/egrn.py` & `MarsGT-0.1.2/MarsGT/egrn.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.1/MarsGT/marsgt_model.py` & `MarsGT-0.1.2/MarsGT/marsgt_model.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.1/MarsGT/utils.py` & `MarsGT-0.1.2/MarsGT/utils.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.1/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.1.2/MarsGT.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.1
+Version: 0.1.2
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: torch_sparse
+Provides-Extra: torch_scatter
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
 DeepMARS, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
```

### Comparing `MarsGT-0.1.1/PKG-INFO` & `MarsGT-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.1
+Version: 0.1.2
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: torch_sparse
+Provides-Extra: torch_scatter
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
 DeepMARS, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
```

### Comparing `MarsGT-0.1.1/README.md` & `MarsGT-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.1/setup.py` & `MarsGT-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="MarsGT",
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'anndata==0.8.0',
         'dill==0.3.4',
         'matplotlib==3.5.1',
         'numpy==1.22.3',
         'pandas==1.4.2',
@@ -18,18 +18,20 @@
         'scikit-learn==1.1.2',
         'torch==1.12.0+cu102',
         'torch-geometric==2.1.0.post1',
         'torchmetrics==0.9.3',
         'xlwt==1.3.0',
         'tqdm==4.64.0',
         'scanpy==1.9.1',
-        'torch-sparse==0.6.14',
-        'torch-scatter==2.0.9',
         'leidenalg==0.8.10',
     ],
+    extras_require={
+        "torch_sparse": ["torch-sparse==0.6.14"], 
+        "torch_scatter": ["torch-scatter==2.0.9"]
+    },
     python_requires='==3.8.0',
     description="MarsGT: A Python library for rare cell identification (Internal testing only)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License"
     ]
```

