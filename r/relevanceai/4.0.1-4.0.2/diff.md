# Comparing `tmp/relevanceai-4.0.1.tar.gz` & `tmp/relevanceai-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-4.0.1.tar", last modified: Sat Jun  3 15:51:34 2023, max compression
+gzip compressed data, was "relevanceai-4.0.2.tar", last modified: Sat Jun  3 18:26:18 2023, max compression
```

## Comparing `relevanceai-4.0.1.tar` & `relevanceai-4.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.502320 relevanceai-4.0.1/
--rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.1/LICENSE
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 15:51:34.502177 relevanceai-4.0.1/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.1/README.md
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.500171 relevanceai-4.0.1/relevanceai/
--rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 15:51:32.000000 relevanceai-4.0.1/relevanceai/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/_request.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/auth.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 08:24:41.000000 relevanceai-4.0.1/relevanceai/datasets.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/env.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/params.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.501997 relevanceai-4.0.1/relevanceai/steps/
--rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.1/relevanceai/steps/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2595 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/_base.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/api_call.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/execute_javascript.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/generate_vector_embedding.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/prompt_completion.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/redis_vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.1/relevanceai/steps/run_chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2750 2023-06-03 15:22:51.000000 relevanceai-4.0.1/relevanceai/steps/run_step.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/vectorize_and_search.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.500745 relevanceai-4.0.1/relevanceai.egg-info/
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/SOURCES.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/dependency_links.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/requires.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/top_level.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 15:51:34.502357 relevanceai-4.0.1/setup.cfg
--rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.1/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:26:18.639081 relevanceai-4.0.2/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.2/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:26:18.638942 relevanceai-4.0.2/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.2/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:26:18.636865 relevanceai-4.0.2/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 18:25:47.000000 relevanceai-4.0.2/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.2/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.2/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.2/relevanceai/chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.2/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.2/relevanceai/env.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.2/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:26:18.638781 relevanceai-4.0.2/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.2/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2595 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.2/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2742 2023-06-03 18:24:12.000000 relevanceai-4.0.2/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.2/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:26:18.637490 relevanceai-4.0.2/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:26:18.000000 relevanceai-4.0.2/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 18:26:18.000000 relevanceai-4.0.2/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 18:26:18.000000 relevanceai-4.0.2/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 18:26:18.000000 relevanceai-4.0.2/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 18:26:18.000000 relevanceai-4.0.2/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 18:26:18.639121 relevanceai-4.0.2/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.2/setup.py
```

### Comparing `relevanceai-4.0.1/LICENSE` & `relevanceai-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/PKG-INFO` & `relevanceai-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.1
+Version: 4.0.2
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.1/README.md` & `relevanceai-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/auth.py` & `relevanceai-4.0.2/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/chain.py` & `relevanceai-4.0.2/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/datasets.py` & `relevanceai-4.0.2/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/env.py` & `relevanceai-4.0.2/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/params.py` & `relevanceai-4.0.2/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/__init__.py` & `relevanceai-4.0.2/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/_base.py` & `relevanceai-4.0.2/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/api_call.py` & `relevanceai-4.0.2/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/execute_javascript.py` & `relevanceai-4.0.2/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-4.0.2/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/prompt_completion.py` & `relevanceai-4.0.2/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/redis_vector_search.py` & `relevanceai-4.0.2/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/run_chain.py` & `relevanceai-4.0.2/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/run_step.py` & `relevanceai-4.0.2/relevanceai/steps/run_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     if auth is None:
         auth = config.auth
     response = requests.get(
         f"https://api-{auth.region}.stack.tryrelevance.com/latest/studios/transformations/list",
     )
     res = handle_response(response)
     results_list = []
-    for s in res["transformations"]:
+    for s in res["results"]:
         results_list.append(
             {
                 "id": s["transformation_id"],
                 "name": s["name"],
                 "description": s["description"],
                 "input_schema": s["input_schema"]["properties"].keys(),
                 "output_schema": s["output_schema"]["properties"].keys(),
```

### Comparing `relevanceai-4.0.1/relevanceai/steps/vector_search.py` & `relevanceai-4.0.2/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai/steps/vectorize_and_search.py` & `relevanceai-4.0.2/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/relevanceai.egg-info/PKG-INFO` & `relevanceai-4.0.2/relevanceai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.1
+Version: 4.0.2
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.1/relevanceai.egg-info/SOURCES.txt` & `relevanceai-4.0.2/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.1/setup.py` & `relevanceai-4.0.2/setup.py`

 * *Files identical despite different names*

