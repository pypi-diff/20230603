# Comparing `tmp/vector_vault-1.7.5.tar.gz` & `tmp/vector_vault-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.5.tar", last modified: Sat Jun  3 06:47:45 2023, max compression
+gzip compressed data, was "vector_vault-1.7.6.tar", last modified: Sat Jun  3 06:57:48 2023, max compression
```

## Comparing `vector_vault-1.7.5.tar` & `vector_vault-1.7.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:47:45.463158 vector_vault-1.7.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:47:45.463005 vector_vault-1.7.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 06:47:45.463196 vector_vault-1.7.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 06:47:40.000000 vector_vault-1.7.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:47:45.459661 vector_vault-1.7.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:47:45.000000 vector_vault-1.7.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 06:47:45.000000 vector_vault-1.7.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 06:47:45.000000 vector_vault-1.7.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 06:47:45.000000 vector_vault-1.7.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 06:47:45.000000 vector_vault-1.7.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:47:45.462645 vector_vault-1.7.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 06:47:29.000000 vector_vault-1.7.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 06:47:22.000000 vector_vault-1.7.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.5/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    27467 2023-06-03 06:47:17.000000 vector_vault-1.7.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.135571 vector_vault-1.7.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:57:48.135391 vector_vault-1.7.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 06:57:48.135605 vector_vault-1.7.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 06:57:44.000000 vector_vault-1.7.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.132430 vector_vault-1.7.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.134996 vector_vault-1.7.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 06:47:29.000000 vector_vault-1.7.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 06:47:22.000000 vector_vault-1.7.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.6/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    27483 2023-06-03 06:57:38.000000 vector_vault-1.7.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.6/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.6/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.5/LICENSE` & `vector_vault-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/PKG-INFO` & `vector_vault-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.5
+Version: 1.7.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.5/README.md` & `vector_vault-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/setup.py` & `vector_vault-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.5",
+    version="1.7.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.6/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.5
+Version: 1.7.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.5/vectorvault/__init__.py` & `vector_vault-1.7.6/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/ai.py` & `vector_vault-1.7.6/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/cloudmanager.py` & `vector_vault-1.7.6/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/creds.py` & `vector_vault-1.7.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/download.py` & `vector_vault-1.7.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/itemize.py` & `vector_vault-1.7.6/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/signup.py` & `vector_vault-1.7.6/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/vault.py` & `vector_vault-1.7.6/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # from Vector Vault.
 
 import numpy as np
 import tempfile
 import os
 import time
 import re
-import json
 import openai
+import json
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from .cloudmanager import CloudManager
 from .ai import AI
 from .itemize import itemize, name_vecs, get_item, get_vectors
 from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
@@ -603,8 +603,8 @@
                 if len(full_text) / 80 > newlinetime:
                     newlinetime += 1
                     print('\n', end='', flush=True)
     
             
     def cloud_stream(self, function):
         for word in function:
-            yield json.dumps({'data': word})
+            yield f"data: {json.dumps({'data': word})} \n\n"
```

### Comparing `vector_vault-1.7.5/vectorvault/vecreq.py` & `vector_vault-1.7.6/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.5/vectorvault/wrap.py` & `vector_vault-1.7.6/vectorvault/wrap.py`

 * *Files identical despite different names*

