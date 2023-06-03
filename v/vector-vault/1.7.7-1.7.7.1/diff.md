# Comparing `tmp/vector_vault-1.7.7.tar.gz` & `tmp/vector_vault-1.7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.7.tar", last modified: Sat Jun  3 21:45:42 2023, max compression
+gzip compressed data, was "vector_vault-1.7.7.1.tar", last modified: Sat Jun  3 21:52:41 2023, max compression
```

## Comparing `vector_vault-1.7.7.tar` & `vector_vault-1.7.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.657993 vector_vault-1.7.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 21:45:42.657856 vector_vault-1.7.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 21:45:42.658029 vector_vault-1.7.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 21:45:34.000000 vector_vault-1.7.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.654966 vector_vault-1.7.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.657437 vector_vault-1.7.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7707 2023-06-03 21:28:12.000000 vector_vault-1.7.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 21:45:10.000000 vector_vault-1.7.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 21:45:08.000000 vector_vault-1.7.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.7/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26431 2023-06-03 21:45:19.000000 vector_vault-1.7.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:52:41.258855 vector_vault-1.7.7.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.7.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20083 2023-06-03 21:52:41.258711 vector_vault-1.7.7.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.7.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 21:52:41.258891 vector_vault-1.7.7.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1077 2023-06-03 21:52:34.000000 vector_vault-1.7.7.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:52:41.255843 vector_vault-1.7.7.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20083 2023-06-03 21:52:41.000000 vector_vault-1.7.7.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 21:52:41.000000 vector_vault-1.7.7.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 21:52:41.000000 vector_vault-1.7.7.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 21:52:41.000000 vector_vault-1.7.7.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 21:52:41.000000 vector_vault-1.7.7.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:52:41.258417 vector_vault-1.7.7.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.7.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7709 2023-06-03 21:52:22.000000 vector_vault-1.7.7.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 21:45:10.000000 vector_vault-1.7.7.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.7.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.7.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 21:45:08.000000 vector_vault-1.7.7.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.7.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26431 2023-06-03 21:45:19.000000 vector_vault-1.7.7.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.7.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.7.1/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.7/LICENSE` & `vector_vault-1.7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/PKG-INFO` & `vector_vault-1.7.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.7
+Version: 1.7.7.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.7/README.md` & `vector_vault-1.7.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/setup.py` & `vector_vault-1.7.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.7",
+    version="1.7.7.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.7.1/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.7
+Version: 1.7.7.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.7/vectorvault/__init__.py` & `vector_vault-1.7.7.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/ai.py` & `vector_vault-1.7.7.1/vectorvault/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,23 @@
                             yield content
                         
                     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', stream=False):
         prompt_template = """
         Use the following pieces of context to answer the question at the end. 
-        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't give any disclaimers or warnings at the end.
+        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't give any disclaimers or warnings.
 
         Our Conversation History (if any): {history}
 
-        Context - Context - Context: {context}
+        Context: {context}
 
         Question: {question}
 
-        (answer the question directly. Most importantly, answer interesting, engaging, and helpful) 
+        (answer the question directly. Be the voice of the context, and most importantly, answer interesting, engaging, and helpful) 
         Answer:"""
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
```

### Comparing `vector_vault-1.7.7/vectorvault/cloudmanager.py` & `vector_vault-1.7.7.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/creds.py` & `vector_vault-1.7.7.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/download.py` & `vector_vault-1.7.7.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/itemize.py` & `vector_vault-1.7.7.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/signup.py` & `vector_vault-1.7.7.1/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/vault.py` & `vector_vault-1.7.7.1/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/vecreq.py` & `vector_vault-1.7.7.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.7/vectorvault/wrap.py` & `vector_vault-1.7.7.1/vectorvault/wrap.py`

 * *Files identical despite different names*

