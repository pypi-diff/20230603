# Comparing `tmp/relevanceai-4.0.4.tar.gz` & `tmp/relevanceai-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-4.0.4.tar", last modified: Sat Jun  3 18:40:54 2023, max compression
+gzip compressed data, was "relevanceai-4.0.5.tar", last modified: Sat Jun  3 18:49:53 2023, max compression
```

## Comparing `relevanceai-4.0.4.tar` & `relevanceai-4.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:40:54.140147 relevanceai-4.0.4/
--rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.4/LICENSE
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:40:54.140014 relevanceai-4.0.4/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.4/README.md
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:40:54.138250 relevanceai-4.0.4/relevanceai/
--rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 18:40:30.000000 relevanceai-4.0.4/relevanceai/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.4/relevanceai/_request.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.4/relevanceai/auth.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.4/relevanceai/chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.4/relevanceai/datasets.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.4/relevanceai/env.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.4/relevanceai/params.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:40:54.139855 relevanceai-4.0.4/relevanceai/steps/
--rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.4/relevanceai/steps/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2595 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/_base.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/api_call.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/execute_javascript.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/generate_vector_embedding.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/prompt_completion.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/redis_vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.4/relevanceai/steps/run_chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2803 2023-06-03 18:39:29.000000 relevanceai-4.0.4/relevanceai/steps/run_step.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.4/relevanceai/steps/vectorize_and_search.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:40:54.138766 relevanceai-4.0.4/relevanceai.egg-info/
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:40:54.000000 relevanceai-4.0.4/relevanceai.egg-info/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 18:40:54.000000 relevanceai-4.0.4/relevanceai.egg-info/SOURCES.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 18:40:54.000000 relevanceai-4.0.4/relevanceai.egg-info/dependency_links.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 18:40:54.000000 relevanceai-4.0.4/relevanceai.egg-info/requires.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 18:40:54.000000 relevanceai-4.0.4/relevanceai.egg-info/top_level.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 18:40:54.140191 relevanceai-4.0.4/setup.cfg
--rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.4/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:49:53.304161 relevanceai-4.0.5/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.5/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:49:53.304029 relevanceai-4.0.5/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.5/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:49:53.301319 relevanceai-4.0.5/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 18:49:41.000000 relevanceai-4.0.5/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.5/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.5/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.5/relevanceai/chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.5/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.5/relevanceai/env.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.5/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:49:53.303810 relevanceai-4.0.5/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.5/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2669 2023-06-03 18:49:06.000000 relevanceai-4.0.5/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.5/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2815 2023-06-03 18:49:28.000000 relevanceai-4.0.5/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.5/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 18:49:53.301984 relevanceai-4.0.5/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 18:49:53.000000 relevanceai-4.0.5/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 18:49:53.000000 relevanceai-4.0.5/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 18:49:53.000000 relevanceai-4.0.5/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 18:49:53.000000 relevanceai-4.0.5/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 18:49:53.000000 relevanceai-4.0.5/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 18:49:53.304194 relevanceai-4.0.5/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.5/setup.py
```

### Comparing `relevanceai-4.0.4/LICENSE` & `relevanceai-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/PKG-INFO` & `relevanceai-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.4
+Version: 4.0.5
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.4/README.md` & `relevanceai-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/auth.py` & `relevanceai-4.0.5/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/chain.py` & `relevanceai-4.0.5/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/datasets.py` & `relevanceai-4.0.5/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/env.py` & `relevanceai-4.0.5/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/params.py` & `relevanceai-4.0.5/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/__init__.py` & `relevanceai-4.0.5/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/_base.py` & `relevanceai-4.0.5/relevanceai/steps/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 from relevanceai.auth import Auth
 from relevanceai._request import handle_response
 from relevanceai.params import Parameters, ParamBase
 
 
 class StepBase:
     def __init__(
-        self, name="step", description="a step", parameters={}, id="new", auth=None
+        self,
+        name="step",
+        description="a step",
+        parameters={},
+        id="new",
+        auth=None,
+        *args,
+        **kwargs,
     ):
         self.name = name
         self.description = description
         if isinstance(parameters, Parameters):
             self.parameters = parameters.to_json()
         elif isinstance(parameters, ParamBase):
             self.parameters = parameters.to_json()
```

### Comparing `relevanceai-4.0.4/relevanceai/steps/api_call.py` & `relevanceai-4.0.5/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/execute_javascript.py` & `relevanceai-4.0.5/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-4.0.5/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/prompt_completion.py` & `relevanceai-4.0.5/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/redis_vector_search.py` & `relevanceai-4.0.5/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/run_chain.py` & `relevanceai-4.0.5/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/run_step.py` & `relevanceai-4.0.5/relevanceai/steps/run_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from relevanceai._request import handle_response
 from relevanceai.auth import config, Auth
 from relevanceai.steps._base import StepBase
 
 
-def list_all_steps(auth: Auth = None, raw=True):
+def list_all_steps(auth: Auth = None, raw=False):
     if auth is None:
         auth = config.auth
     response = requests.get(
         f"https://api-{auth.region}.stack.tryrelevance.com/latest/studios/transformations/list",
     )
     res = handle_response(response)
     if raw:
@@ -28,15 +28,15 @@
             }
         )
     return results_list
 
 
 class RunStep(StepBase):
     def __init__(self, step_id: str, step_name: str = None, *args, **kwargs):
-        self.list_of_steps = list_all_steps(raw=True)
+        self.list_of_steps = list_all_steps(raw=True)["results"]
         self.step_id = step_id
         for step in self.list_of_steps:
             if step["transformation_id"] == self.step_id:
                 self.step_definition = step
         self.step_name = (
             self.step_definition["name"] if step_name is None else step_name
         )
```

### Comparing `relevanceai-4.0.4/relevanceai/steps/vector_search.py` & `relevanceai-4.0.5/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai/steps/vectorize_and_search.py` & `relevanceai-4.0.5/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/relevanceai.egg-info/PKG-INFO` & `relevanceai-4.0.5/relevanceai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.4
+Version: 4.0.5
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.4/relevanceai.egg-info/SOURCES.txt` & `relevanceai-4.0.5/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.4/setup.py` & `relevanceai-4.0.5/setup.py`

 * *Files identical despite different names*

