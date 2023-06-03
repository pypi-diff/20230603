# Comparing `tmp/vector_vault-1.7.0.tar.gz` & `tmp/vector_vault-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.0.tar", last modified: Fri Jun  2 08:27:06 2023, max compression
+gzip compressed data, was "vector_vault-1.7.1.tar", last modified: Sat Jun  3 03:04:43 2023, max compression
```

## Comparing `vector_vault-1.7.0.tar` & `vector_vault-1.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.842913 vector_vault-1.7.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 08:27:06.842729 vector_vault-1.7.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-02 08:27:06.842955 vector_vault-1.7.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-02 08:27:00.000000 vector_vault-1.7.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.839743 vector_vault-1.7.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.842321 vector_vault-1.7.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-02 08:26:16.000000 vector_vault-1.7.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-02 08:26:22.000000 vector_vault-1.7.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    27022 2023-06-02 08:26:36.000000 vector_vault-1.7.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.0/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:04:43.753326 vector_vault-1.7.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:04:43.753163 vector_vault-1.7.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 03:04:43.753361 vector_vault-1.7.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 03:04:34.000000 vector_vault-1.7.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:04:43.750125 vector_vault-1.7.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:04:43.000000 vector_vault-1.7.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 03:04:43.000000 vector_vault-1.7.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 03:04:43.000000 vector_vault-1.7.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 03:04:43.000000 vector_vault-1.7.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 03:04:43.000000 vector_vault-1.7.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:04:43.752904 vector_vault-1.7.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 03:04:00.000000 vector_vault-1.7.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 03:04:06.000000 vector_vault-1.7.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26993 2023-06-03 03:04:23.000000 vector_vault-1.7.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.1/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.0/LICENSE` & `vector_vault-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/PKG-INFO` & `vector_vault-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.0
+Version: 1.7.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.0/README.md` & `vector_vault-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/setup.py` & `vector_vault-1.7.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.0",
+    version="1.7.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.1/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.0
+Version: 1.7.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.0/vectorvault/__init__.py` & `vector_vault-1.7.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/ai.py` & `vector_vault-1.7.1/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/cloudmanager.py` & `vector_vault-1.7.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/creds.py` & `vector_vault-1.7.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/download.py` & `vector_vault-1.7.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/itemize.py` & `vector_vault-1.7.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/signup.py` & `vector_vault-1.7.1/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/vault.py` & `vector_vault-1.7.1/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,32 +67,31 @@
         self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
         total_saved_items = 0
 
         with ThreadPoolExecutor() as executor:
-            for item in self.items:
-                item_text, item_id, item_meta = get_item(item)
-                executor.submit(self.cloud_manager.upload, item_id, item_text, item_meta)
+            futures = {executor.submit(self.cloud_manager.upload, *get_item(item)) for item in self.items}
+            for future in as_completed(futures):
                 total_saved_items += 1
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
             byte = os.path.getsize(temp_file.name)
             self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault, self.user, self.api, byte))
 
         self.items.clear()
         self.x_checked = False
         self.vecs_loaded = False
         self.saved_already = False
 
         if self.verbose:
             print(f"upload time --- {(time.time() - start_time)} seconds --- {total_saved_items} items saved")
-        
+            
     def clear_cache(self):
         self.reload_vectors()
         self.x_checked = True
         self.vecs_loaded = True
         self.saved_already = False
 
     def delete(self):
```

### Comparing `vector_vault-1.7.0/vectorvault/vecreq.py` & `vector_vault-1.7.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.0/vectorvault/wrap.py` & `vector_vault-1.7.1/vectorvault/wrap.py`

 * *Files identical despite different names*

