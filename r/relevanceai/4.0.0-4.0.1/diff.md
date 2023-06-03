# Comparing `tmp/relevanceai-4.0.0.tar.gz` & `tmp/relevanceai-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-4.0.0.tar", last modified: Sat Jun  3 06:36:38 2023, max compression
+gzip compressed data, was "relevanceai-4.0.1.tar", last modified: Sat Jun  3 15:51:34 2023, max compression
```

## Comparing `relevanceai-4.0.0.tar` & `relevanceai-4.0.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-03 06:36:22.000000 relevanceai-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 06:36:38.395334 relevanceai-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-03 06:36:22.000000 relevanceai-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/execute_javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/prompt_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/redis_vector_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/vector_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/vectorize_and_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 06:36:38.395334 relevanceai-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 06:36:22.000000 relevanceai-4.0.0/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.502320 relevanceai-4.0.1/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.1/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 15:51:34.502177 relevanceai-4.0.1/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.1/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.500171 relevanceai-4.0.1/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 15:51:32.000000 relevanceai-4.0.1/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 08:24:41.000000 relevanceai-4.0.1/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/env.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.1/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.501997 relevanceai-4.0.1/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-06-03 15:02:39.000000 relevanceai-4.0.1/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2595 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.1/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2750 2023-06-03 15:22:51.000000 relevanceai-4.0.1/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.1/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 15:51:34.500745 relevanceai-4.0.1/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      746 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 15:51:34.000000 relevanceai-4.0.1/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 15:51:34.502357 relevanceai-4.0.1/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.1/setup.py
```

### Comparing `relevanceai-4.0.0/LICENSE` & `relevanceai-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/auth.py` & `relevanceai-4.0.1/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/chain.py` & `relevanceai-4.0.1/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/datasets.py` & `relevanceai-4.0.1/relevanceai/datasets.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,14 @@
                 authenticate=False,
             )
         except ImportError:
             raise ImportError(
                 "vecdb is not installed. Please install vecdb with `pip install vecdb`"
             )
         self.db = Dataset(api=self.vecdb_client.api, dataset_id=self.id)
-    
 
     def insert(
         self,
         documents: List = None,
         ids: List[str] = None,
         data: List[str] = None,
         metadata: List[Dict[str, Any]] = None,
@@ -59,15 +58,14 @@
                 metadata=metadata,
                 vector=vector,
                 encoders=encoders,
                 *args,
                 **kwargs,
             )
 
-
     def search(
         self,
         text: str,
         field: str = "text_vector_",
         page_size: int = 5,
         model: str = "all-mpnet-base-v2",
         return_as_step: bool = False,
@@ -76,29 +74,27 @@
             field = f"{field}_vector_"
         if return_as_step:
             return VectorSimilaritySearch(
                 dataset_id=self.id,
                 query=text,
                 vector_field=field,
                 model=model,
-                page_size=page_size
+                page_size=page_size,
             )
         else:
             return VectorSimilaritySearch(
                 dataset_id=self.id,
                 query=text,
                 vector_field=field,
                 model=model,
-                page_size=page_size
+                page_size=page_size,
             ).run()
 
-
     def delete(self):
-        return self.db.delete()
-
+        return self.db.api._delete_dataset(self.id)
 
     def all(self):
         return self.db.get_all()
 
 
 def list_datasets(auth: Auth = None):
     auth: Auth = config.auth if auth is None else auth
```

### Comparing `relevanceai-4.0.0/relevanceai/env.py` & `relevanceai-4.0.1/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/params.py` & `relevanceai-4.0.1/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/_base.py` & `relevanceai-4.0.1/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/api_call.py` & `relevanceai-4.0.1/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/execute_javascript.py` & `relevanceai-4.0.1/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/prompt_completion.py` & `relevanceai-4.0.1/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/redis_vector_search.py` & `relevanceai-4.0.1/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/vector_search.py` & `relevanceai-4.0.1/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai/steps/vectorize_and_search.py` & `relevanceai-4.0.1/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.0/relevanceai.egg-info/SOURCES.txt` & `relevanceai-4.0.1/relevanceai.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 relevanceai.egg-info/dependency_links.txt
 relevanceai.egg-info/requires.txt
 relevanceai.egg-info/top_level.txt
 relevanceai/steps/__init__.py
 relevanceai/steps/_base.py
 relevanceai/steps/api_call.py
 relevanceai/steps/execute_javascript.py
+relevanceai/steps/generate_vector_embedding.py
 relevanceai/steps/prompt_completion.py
 relevanceai/steps/redis_vector_search.py
+relevanceai/steps/run_chain.py
+relevanceai/steps/run_step.py
 relevanceai/steps/vector_search.py
 relevanceai/steps/vectorize_and_search.py
```

### Comparing `relevanceai-4.0.0/setup.py` & `relevanceai-4.0.1/setup.py`

 * *Files identical despite different names*

