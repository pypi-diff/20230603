# Comparing `tmp/relevanceai-4.0.6.tar.gz` & `tmp/relevanceai-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-4.0.6.tar", last modified: Sat Jun  3 18:51:58 2023, max compression
+gzip compressed data, was "relevanceai-4.0.7.tar", last modified: Sat Jun  3 18:56:24 2023, max compression
```

## Comparing `relevanceai-4.0.6.tar` & `relevanceai-4.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:51:58.179974 relevanceai-4.0.6/
--rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.6/LICENSE
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:51:58.179834 relevanceai-4.0.6/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.6/README.md
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:51:58.177511 relevanceai-4.0.6/relevanceai/
--rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 18:50:48.000000 relevanceai-4.0.6/relevanceai/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.6/relevanceai/_request.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.6/relevanceai/auth.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.6/relevanceai/chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.6/relevanceai/datasets.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.6/relevanceai/env.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.6/relevanceai/params.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:51:58.179657 relevanceai-4.0.6/relevanceai/steps/
--rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.6/relevanceai/steps/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2669 2023-06-03 18:49:06.000000 relevanceai-4.0.6/relevanceai/steps/_base.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/api_call.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/execute_javascript.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/generate_vector_embedding.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/prompt_completion.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/redis_vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.6/relevanceai/steps/run_chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2815 2023-06-03 18:49:28.000000 relevanceai-4.0.6/relevanceai/steps/run_step.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.6/relevanceai/steps/vectorize_and_search.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:51:58.178074 relevanceai-4.0.6/relevanceai.egg-info/
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:51:58.000000 relevanceai-4.0.6/relevanceai.egg-info/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 18:51:58.000000 relevanceai-4.0.6/relevanceai.egg-info/SOURCES.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 18:51:58.000000 relevanceai-4.0.6/relevanceai.egg-info/dependency_links.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 18:51:58.000000 relevanceai-4.0.6/relevanceai.egg-info/requires.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 18:51:58.000000 relevanceai-4.0.6/relevanceai.egg-info/top_level.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 18:51:58.180008 relevanceai-4.0.6/setup.cfg
--rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.6/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:56:24.752933 relevanceai-4.0.7/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.7/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:56:24.752672 relevanceai-4.0.7/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.7/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:56:24.750491 relevanceai-4.0.7/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 18:56:15.000000 relevanceai-4.0.7/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.7/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.7/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.7/relevanceai/chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.7/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.7/relevanceai/env.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.7/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:56:24.752482 relevanceai-4.0.7/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.7/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2669 2023-06-03 18:49:06.000000 relevanceai-4.0.7/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.7/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2816 2023-06-03 18:56:08.000000 relevanceai-4.0.7/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.7/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:56:24.751068 relevanceai-4.0.7/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:56:24.000000 relevanceai-4.0.7/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 18:56:24.000000 relevanceai-4.0.7/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 18:56:24.000000 relevanceai-4.0.7/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 18:56:24.000000 relevanceai-4.0.7/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 18:56:24.000000 relevanceai-4.0.7/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 18:56:24.753003 relevanceai-4.0.7/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.7/setup.py
```

### Comparing `relevanceai-4.0.6/LICENSE` & `relevanceai-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/PKG-INFO` & `relevanceai-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.6
+Version: 4.0.7
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.6/README.md` & `relevanceai-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/auth.py` & `relevanceai-4.0.7/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/chain.py` & `relevanceai-4.0.7/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/datasets.py` & `relevanceai-4.0.7/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/env.py` & `relevanceai-4.0.7/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/params.py` & `relevanceai-4.0.7/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/__init__.py` & `relevanceai-4.0.7/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/_base.py` & `relevanceai-4.0.7/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/api_call.py` & `relevanceai-4.0.7/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/execute_javascript.py` & `relevanceai-4.0.7/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-4.0.7/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/prompt_completion.py` & `relevanceai-4.0.7/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/redis_vector_search.py` & `relevanceai-4.0.7/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/run_chain.py` & `relevanceai-4.0.7/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/run_step.py` & `relevanceai-4.0.7/relevanceai/steps/run_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,14 @@
     @property
     def steps(self):
         params = {}
         for i in self.inputted:
             params[i] = getattr(self, i)
         return [
             {
-                "transformation": "run_chain",
+                "transformation": self.step_id,
                 "name": self.step_name,
                 "foreach": "",
                 "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
                 "params": params,
             }
         ]
```

### Comparing `relevanceai-4.0.6/relevanceai/steps/vector_search.py` & `relevanceai-4.0.7/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai/steps/vectorize_and_search.py` & `relevanceai-4.0.7/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/relevanceai.egg-info/PKG-INFO` & `relevanceai-4.0.7/relevanceai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.6
+Version: 4.0.7
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.6/relevanceai.egg-info/SOURCES.txt` & `relevanceai-4.0.7/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.6/setup.py` & `relevanceai-4.0.7/setup.py`

 * *Files identical despite different names*

