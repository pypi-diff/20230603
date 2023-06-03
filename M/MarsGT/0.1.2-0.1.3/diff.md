# Comparing `tmp/MarsGT-0.1.2.tar.gz` & `tmp/MarsGT-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MarsGT-0.1.2.tar", last modified: Sat Jun  3 07:23:55 2023, max compression
+gzip compressed data, was "dist/MarsGT-0.1.3.tar", last modified: Sat Jun  3 07:35:29 2023, max compression
```

## Comparing `MarsGT-0.1.2.tar` & `MarsGT-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.133795 MarsGT-0.1.2/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.2/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.097783 MarsGT-0.1.2/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.2/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 06:21:55.000000 MarsGT-0.1.2/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6007 2023-06-03 06:21:56.000000 MarsGT-0.1.2/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21321 2023-06-03 06:21:56.000000 MarsGT-0.1.2/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 06:21:57.000000 MarsGT-0.1.2/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:23:55.115785 MarsGT-0.1.2/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      323 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 07:23:54.000000 MarsGT-0.1.2/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:23:55.131785 MarsGT-0.1.2/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.2/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 07:23:55.134787 MarsGT-0.1.2/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1077 2023-06-03 07:22:43.000000 MarsGT-0.1.2/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.373832 MarsGT-0.1.3/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.3/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.349812 MarsGT-0.1.3/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.3/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 06:21:55.000000 MarsGT-0.1.3/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6007 2023-06-03 06:21:56.000000 MarsGT-0.1.3/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21321 2023-06-03 06:21:56.000000 MarsGT-0.1.3/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 06:21:57.000000 MarsGT-0.1.3/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.367813 MarsGT-0.1.3/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      317 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:35:29.371821 MarsGT-0.1.3/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.3/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 07:35:29.374813 MarsGT-0.1.3/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1071 2023-06-03 07:33:41.000000 MarsGT-0.1.3/setup.py
```

### Comparing `MarsGT-0.1.2/MarsGT/conv.py` & `MarsGT-0.1.3/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.2/MarsGT/egrn.py` & `MarsGT-0.1.3/MarsGT/egrn.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.2/MarsGT/marsgt_model.py` & `MarsGT-0.1.3/MarsGT/marsgt_model.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.2/MarsGT/utils.py` & `MarsGT-0.1.3/MarsGT/utils.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.2/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.1.3/MarsGT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.2
+Version: 0.1.3
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
```

### Comparing `MarsGT-0.1.2/PKG-INFO` & `MarsGT-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.2
+Version: 0.1.3
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
```

### Comparing `MarsGT-0.1.2/README.md` & `MarsGT-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.2/setup.py` & `MarsGT-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="MarsGT",
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'anndata==0.8.0',
         'dill==0.3.4',
         'matplotlib==3.5.1',
         'numpy==1.22.3',
         'pandas==1.4.2',
         'scipy==1.9.1',
         'seaborn==0.11.2',
         'scikit-learn==1.1.2',
-        'torch==1.12.0+cu102',
+        'torch==1.12.0',
         'torch-geometric==2.1.0.post1',
         'torchmetrics==0.9.3',
         'xlwt==1.3.0',
         'tqdm==4.64.0',
         'scanpy==1.9.1',
         'leidenalg==0.8.10',
     ],
```

