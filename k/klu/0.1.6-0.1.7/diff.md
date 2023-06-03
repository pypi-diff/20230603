# Comparing `tmp/klu-0.1.6.tar.gz` & `tmp/klu-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.6.tar", max compression
+gzip compressed data, was "klu-0.1.7.tar", max compression
```

## Comparing `klu-0.1.6.tar` & `klu-0.1.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1070 2023-06-01 11:32:44.968401 klu-0.1.6/LICENSE
--rw-r--r--   0        0        0     2840 2023-06-01 11:32:44.968401 klu-0.1.6/README.md
--rw-r--r--   0        0        0      150 2023-06-01 11:32:44.968401 klu-0.1.6/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/__init__.py
--rw-r--r--   0        0        0    11322 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/client.py
--rw-r--r--   0        0        0      280 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/constants.py
--rw-r--r--   0        0        0      547 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/errors.py
--rw-r--r--   0        0        0     1980 2023-06-01 11:32:44.968401 klu-0.1.6/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/__init__.py
--rw-r--r--   0        0        0     2998 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/config.py
--rw-r--r--   0        0        0      118 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/constants.py
--rw-r--r--   0        0        0     1406 2023-06-01 11:32:44.968401 klu-0.1.6/klu/api/sse_client.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/__init__.py
--rw-r--r--   0        0        0     7753 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/client.py
--rw-r--r--   0        0        0      259 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/constants.py
--rw-r--r--   0        0        0      318 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/errors.py
--rw-r--r--   0        0        0     1464 2023-06-01 11:32:44.968401 klu-0.1.6/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/client/__init__.py
--rw-r--r--   0        0        0      794 2023-06-01 11:32:44.968401 klu-0.1.6/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/__init__.py
--rw-r--r--   0        0        0     3086 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/client.py
--rw-r--r--   0        0        0     2975 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/errors.py
--rw-r--r--   0        0        0     2209 2023-06-01 11:32:44.968401 klu-0.1.6/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/__init__.py
--rw-r--r--   0        0        0     2332 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/client.py
--rw-r--r--   0        0        0       25 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/constants.py
--rw-r--r--   0        0        0      274 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/errors.py
--rw-r--r--   0        0        0     3199 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8672 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/client.py
--rw-r--r--   0        0        0      287 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/constants.py
--rw-r--r--   0        0        0      309 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/errors.py
--rw-r--r--   0        0        0     3415 2023-06-01 11:32:44.968401 klu-0.1.6/klu/data_index/models.py
--rw-r--r--   0        0        0       19 2023-06-01 11:32:44.968401 klu-0.1.6/klu/klu.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/__init__.py
--rw-r--r--   0        0        0     3505 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/client.py
--rw-r--r--   0        0        0       28 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/constants.py
--rw-r--r--   0        0        0      447 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/errors.py
--rw-r--r--   0        0        0     1397 2023-06-01 11:32:44.968401 klu-0.1.6/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/__init__.py
--rw-r--r--   0        0        0     1488 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/client.py
--rw-r--r--   0        0        0       32 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/constants.py
--rw-r--r--   0        0        0     1264 2023-06-01 11:32:44.968401 klu-0.1.6/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      752 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/file_upload.py
--rw-r--r--   0        0        0     2407 2023-06-01 11:32:44.972401 klu-0.1.6/klu/utils/paginator.py
--rw-r--r--   0        0        0        0 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/__init__.py
--rw-r--r--   0        0        0     8052 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/client.py
--rw-r--r--   0        0        0      321 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/errors.py
--rw-r--r--   0        0        0      943 2023-06-01 11:32:44.972401 klu-0.1.6/klu/workspace/models.py
--rw-r--r--   0        0        0     1952 2023-06-01 11:32:44.972401 klu-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 17:41:15.902941 klu-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2840 2023-06-03 17:41:15.902941 klu-0.1.7/README.md
+-rw-r--r--   0        0        0      150 2023-06-03 17:41:15.902941 klu-0.1.7/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/__init__.py
+-rw-r--r--   0        0        0    11322 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/client.py
+-rw-r--r--   0        0        0      280 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/constants.py
+-rw-r--r--   0        0        0      547 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/errors.py
+-rw-r--r--   0        0        0     1980 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/__init__.py
+-rw-r--r--   0        0        0     2998 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/config.py
+-rw-r--r--   0        0        0      118 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/constants.py
+-rw-r--r--   0        0        0     1406 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/sse_client.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/__init__.py
+-rw-r--r--   0        0        0     7753 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/constants.py
+-rw-r--r--   0        0        0      318 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/errors.py
+-rw-r--r--   0        0        0     1464 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/client/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-03 17:41:15.902941 klu-0.1.7/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/__init__.py
+-rw-r--r--   0        0        0     3086 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/client.py
+-rw-r--r--   0        0        0     2975 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/errors.py
+-rw-r--r--   0        0        0     2209 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/__init__.py
+-rw-r--r--   0        0        0     2291 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/client.py
+-rw-r--r--   0        0        0       25 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/constants.py
+-rw-r--r--   0        0        0      274 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/errors.py
+-rw-r--r--   0        0        0     3199 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8672 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/client.py
+-rw-r--r--   0        0        0      287 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/constants.py
+-rw-r--r--   0        0        0      309 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3415 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/models.py
+-rw-r--r--   0        0        0       19 2023-06-03 17:41:15.902941 klu-0.1.7/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/__init__.py
+-rw-r--r--   0        0        0     3505 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/client.py
+-rw-r--r--   0        0        0       28 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/constants.py
+-rw-r--r--   0        0        0      447 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/errors.py
+-rw-r--r--   0        0        0     1397 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/__init__.py
+-rw-r--r--   0        0        0     1488 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/client.py
+-rw-r--r--   0        0        0       32 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/constants.py
+-rw-r--r--   0        0        0     1264 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      752 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2407 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     8052 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/errors.py
+-rw-r--r--   0        0        0      943 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/models.py
+-rw-r--r--   0        0        0     1952 2023-06-03 17:41:15.906941 klu-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.7/PKG-INFO
```

### Comparing `klu-0.1.6/LICENSE` & `klu-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/README.md` & `klu-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/action/client.py` & `klu-0.1.7/klu/action/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/action/errors.py` & `klu-0.1.7/klu/action/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/action/models.py` & `klu-0.1.7/klu/action/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/api/client.py` & `klu-0.1.7/klu/api/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/api/sse_client.py` & `klu-0.1.7/klu/api/sse_client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/application/client.py` & `klu-0.1.7/klu/application/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/application/models.py` & `klu-0.1.7/klu/application/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/client/klu.py` & `klu-0.1.7/klu/client/klu.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/common/client.py` & `klu-0.1.7/klu/common/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/common/errors.py` & `klu-0.1.7/klu/common/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/common/models.py` & `klu-0.1.7/klu/common/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/data/client.py` & `klu-0.1.7/klu/data/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,43 @@
 
 class DataClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, DATA_ENDPOINT, Data)
 
     async def create(
         self,
-        issue: str,
         input: str,
         output: str,
-        action: str,
         rating: int,
-        correction: str,
         action_guid: str,
-        session_guid: str,
+        issue: Optional[str] = None,
+        correction: Optional[str] = None,
         meta_data: Optional[dict] = None,
+        session_guid: Optional[str] = None,
     ) -> Data:
         """
         Creates new data instance for an action_id provided.
 
         Args:
             issue (str): Data issue
             input (str): Input value of action execution
             output (str): The result of action execution
-            action (str): Data action value
             rating (int): Data rating
             action_guid (str): Guid of an action data belongs to
             session_guid (str): Guid of a session data belongs to
             meta_data (dict): Data meta_data
             correction (str): Data correction
 
         Returns:
             Created Data object
         """
         return await super().create(
             issue=issue,
             input=input,
             output=output,
-            action=action,
             rating=rating,
             meta_data=meta_data,
             correction=correction,
             action_guid=action_guid,
             session_guid=session_guid,
         )
```

### Comparing `klu-0.1.6/klu/data/models.py` & `klu-0.1.7/klu/data/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/data_index/client.py` & `klu-0.1.7/klu/data_index/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/data_index/models.py` & `klu-0.1.7/klu/data_index/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/model/client.py` & `klu-0.1.7/klu/model/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/model/models.py` & `klu-0.1.7/klu/model/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/session/client.py` & `klu-0.1.7/klu/session/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/session/models.py` & `klu-0.1.7/klu/session/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/utils/file_upload.py` & `klu-0.1.7/klu/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/utils/paginator.py` & `klu-0.1.7/klu/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/workspace/client.py` & `klu-0.1.7/klu/workspace/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/klu/workspace/models.py` & `klu-0.1.7/klu/workspace/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.6/pyproject.toml` & `klu-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.6"
+version = "0.1.7"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
 authors = ["Stefan Sabev <stefan@klu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `klu-0.1.6/PKG-INFO` & `klu-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klu
-Version: 0.1.6
+Version: 0.1.7
 Summary: SDK for building AI Enabled apps.
 Home-page: https://github.com/ssabev/klu
 License: MIT
 Author: Stefan Sabev
 Author-email: stefan@klu.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

