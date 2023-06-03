# Comparing `tmp/vector_vault-1.7.2.tar.gz` & `tmp/vector_vault-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.2.tar", last modified: Sat Jun  3 03:29:35 2023, max compression
+gzip compressed data, was "vector_vault-1.7.3.tar", last modified: Sat Jun  3 03:44:21 2023, max compression
```

## Comparing `vector_vault-1.7.2.tar` & `vector_vault-1.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:29:35.322096 vector_vault-1.7.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:29:35.321929 vector_vault-1.7.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 03:29:35.322133 vector_vault-1.7.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 03:29:30.000000 vector_vault-1.7.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:29:35.318640 vector_vault-1.7.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:29:35.000000 vector_vault-1.7.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 03:29:35.000000 vector_vault-1.7.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 03:29:35.000000 vector_vault-1.7.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 03:29:35.000000 vector_vault-1.7.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 03:29:35.000000 vector_vault-1.7.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:29:35.321494 vector_vault-1.7.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 03:04:00.000000 vector_vault-1.7.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 03:04:06.000000 vector_vault-1.7.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.2/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26858 2023-06-03 03:29:20.000000 vector_vault-1.7.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:44:21.589516 vector_vault-1.7.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:44:21.589354 vector_vault-1.7.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 03:44:21.589552 vector_vault-1.7.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 03:44:16.000000 vector_vault-1.7.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:44:21.586918 vector_vault-1.7.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 03:44:21.000000 vector_vault-1.7.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 03:44:21.000000 vector_vault-1.7.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 03:44:21.000000 vector_vault-1.7.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 03:44:21.000000 vector_vault-1.7.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 03:44:21.000000 vector_vault-1.7.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 03:44:21.589072 vector_vault-1.7.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 03:04:00.000000 vector_vault-1.7.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 03:04:06.000000 vector_vault-1.7.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.3/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26776 2023-06-03 03:44:03.000000 vector_vault-1.7.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.3/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.2/LICENSE` & `vector_vault-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/PKG-INFO` & `vector_vault-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.2
+Version: 1.7.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.2/README.md` & `vector_vault-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/setup.py` & `vector_vault-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.2",
+    version="1.7.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.2
+Version: 1.7.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.2/vectorvault/__init__.py` & `vector_vault-1.7.3/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/ai.py` & `vector_vault-1.7.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/cloudmanager.py` & `vector_vault-1.7.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/creds.py` & `vector_vault-1.7.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/download.py` & `vector_vault-1.7.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/itemize.py` & `vector_vault-1.7.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/signup.py` & `vector_vault-1.7.3/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/vault.py` & `vector_vault-1.7.3/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,47 +548,42 @@
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
                             input_ += text['data']
                         for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
                             yield word
-                        for item in context:
-                            if type(metatag) is not list:
-                                for tag in item['metadata']:
-                                    yield str(item['metadata'][f'{tag}'])
-                            else:
-                                if metatag_prefixes:
-                                    if metatag_suffixes:
-                                        for i in range(len(metatag)):
-                                            yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
-                                    else:
-                                        for i in range(len(metatag)):
-                                            yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
-                            
-                            yield item['data']
+                        
+                        if return_context:
+                            for item in context:
+                                if type(metatag) is not list:
+                                    for tag in item['metadata']:
+                                        yield str(item['metadata'][f'{tag}'])
+                                else:
+                                    if metatag_prefixes:
+                                        if metatag_suffixes:
+                                            for i in range(len(metatag)):
+                                                yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
+                                        else:
+                                            for i in range(len(metatag)):
+                                                yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
+                                yield item['data']
                     else:
                         for word in self.ai.llm(segment, history, model=model, stream=True):
                             yield word
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
                     
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
-        if return_context == False:
-            return response
-        elif return_context == True:
-            return {'response': response, 'context': context}
-        
-
     def print_stream(self, function):
         full_text= ''
         newlinetime=1
         for word in function:
             full_text += word
             print(word, end='', flush=True) 
             if len(full_text) / 80 > newlinetime:
```

### Comparing `vector_vault-1.7.2/vectorvault/vecreq.py` & `vector_vault-1.7.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.2/vectorvault/wrap.py` & `vector_vault-1.7.3/vectorvault/wrap.py`

 * *Files identical despite different names*

