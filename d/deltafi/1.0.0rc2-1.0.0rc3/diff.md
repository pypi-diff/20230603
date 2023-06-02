# Comparing `tmp/deltafi-1.0.0rc2.tar.gz` & `tmp/deltafi-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-1.0.0rc2.tar", max compression
+gzip compressed data, was "deltafi-1.0.0rc3.tar", max compression
```

## Comparing `deltafi-1.0.0rc2.tar` & `deltafi-1.0.0rc3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc2/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc2/deltafi/__init__.py
--rw-r--r--   0        0        0     7326 2023-05-17 20:43:32.059753 deltafi-1.0.0rc2/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc2/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc2/deltafi/actiontype.py
--rw-r--r--   0        0        0    11019 2023-05-17 20:43:32.060753 deltafi-1.0.0rc2/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc2/deltafi/exception.py
--rw-r--r--   0        0        0     6284 2023-05-17 20:43:32.060753 deltafi-1.0.0rc2/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc2/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc2/deltafi/metric.py
--rw-r--r--   0        0        0     8553 2023-05-08 15:00:28.699314 deltafi-1.0.0rc2/deltafi/plugin.py
--rw-r--r--   0        0        0     9972 2023-05-17 20:43:32.061753 deltafi-1.0.0rc2/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc2/deltafi/storage.py
--rw-r--r--   0        0        0     1281 2023-05-18 11:25:38.491144 deltafi-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/deltafi/__init__.py
+-rw-r--r--   0        0        0     7326 2023-06-01 15:10:46.434796 deltafi-1.0.0rc3/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc3/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11019 2023-06-01 15:10:46.435796 deltafi-1.0.0rc3/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc3/deltafi/exception.py
+-rw-r--r--   0        0        0     6284 2023-06-01 15:10:46.435796 deltafi-1.0.0rc3/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc3/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc3/deltafi/metric.py
+-rw-r--r--   0        0        0     8553 2023-05-08 15:00:28.699314 deltafi-1.0.0rc3/deltafi/plugin.py
+-rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.0rc3/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc3/deltafi/storage.py
+-rw-r--r--   0        0        0     1281 2023-06-02 22:02:57.540036 deltafi-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc3/PKG-INFO
```

### Comparing `deltafi-1.0.0rc2/deltafi/__init__.py` & `deltafi-1.0.0rc3/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/action.py` & `deltafi-1.0.0rc3/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/actioneventqueue.py` & `deltafi-1.0.0rc3/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/actiontype.py` & `deltafi-1.0.0rc3/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/domain.py` & `deltafi-1.0.0rc3/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/exception.py` & `deltafi-1.0.0rc3/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/input.py` & `deltafi-1.0.0rc3/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/logger.py` & `deltafi-1.0.0rc3/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/metric.py` & `deltafi-1.0.0rc3/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/plugin.py` & `deltafi-1.0.0rc3/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/deltafi/result.py` & `deltafi-1.0.0rc3/deltafi/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     def add_metric(self, metric: Metric):
         self.metrics.append(metric)
 
 
 class DomainResult(Result):
     def __init__(self, context: Context):
         super().__init__('domain', 'DOMAIN', context)
-        self.indexed_metadata = {}
+        self.annotations = {}
 
-    def index_metadata(self, key: str, value: str):
-        self.indexed_metadata[key] = value
+    def annotate(self, key: str, value: str):
+        self.annotations[key] = value
         return self
 
     def response(self):
         return {
-            'indexedMetadata': self.indexed_metadata
+            'annotations': self.annotations
         }
 
 
 class EgressResult(Result):
     def __init__(self, context: Context, destination: str, bytes_egressed: int):
         super().__init__(None, 'EGRESS', context)
         self.add_metric(Metric(FILES_OUT, 1, {ENDPOINT_TAG: destination}))
@@ -70,32 +70,32 @@
         return None
 
 
 class EnrichResult(Result):
     def __init__(self, context: Context):
         super().__init__('enrich', 'ENRICH', context)
         self.enrichments = []
-        self.indexed_metadata = {}
+        self.annotations = {}
 
     def enrich(self, name: str, value: str, media_type: str):
         self.enrichments.append({
             'name': name,
             'value': value,
             'mediaType': media_type
         })
         return self
 
-    def index_metadata(self, key: str, value: str):
-        self.indexed_metadata[key] = value
+    def annotate(self, key: str, value: str):
+        self.annotations[key] = value
         return self
 
     def response(self):
         return {
             'enrichments': self.enrichments,
-            'indexedMetadata': self.indexed_metadata
+            'annotations': self.annotations
         }
 
 
 class ErrorResult(Result):
     def __init__(self, context: Context, error_cause: str, error_context: str):
         super().__init__('error', 'ERROR', context)
         self.error_cause = error_cause
@@ -165,14 +165,16 @@
 
 class LoadResult(Result):
     def __init__(self, context: Context):
         super().__init__('load', 'LOAD', context)
         self.content = []
         self.metadata = {}
         self.domains = []
+        self.annotations = {}
+        self.delete_metadata_keys = []
 
     # content can be a single Content or a List[Content]
     def add_content(self, content):
         if content:
             if type(content) == list:
                 self.content.extend(content)
             else:
@@ -197,19 +199,29 @@
     def add_domain(self, name: str, value: str, media_type: str):
         self.domains.append({
             'name': name,
             'value': value,
             'mediaType': media_type})
         return self
 
+    def annotate(self, key: str, value: str):
+        self.annotations[key] = value
+        return self
+
+    def delete_metadata_key(self, key: str):
+        self.delete_metadata_keys.append(key)
+        return self
+
     def response(self):
         return {
             'domains': self.domains,
             'content': [content.json() for content in self.content],
-            'metadata': self.metadata
+            'metadata': self.metadata,
+            'annotations': self.annotations,
+            'deleteMetadataKeys': self.delete_metadata_keys
         }
 
 
 class ChildLoadResult:
     def __init__(self, load_result: LoadResult = None):
         self._did = str(uuid.uuid4())
         self.load_result = load_result
@@ -269,14 +281,16 @@
 
 
 class TransformResult(Result):
     def __init__(self, context: Context):
         super().__init__('transform', 'TRANSFORM', context)
         self.content = []
         self.metadata = {}
+        self.annotations = {}
+        self.delete_metadata_keys = []
 
     # content can be a single Content or a List[Content]
     def add_content(self, content):
         if content:
             if type(content) == list:
                 self.content.extend(content)
             else:
@@ -294,18 +308,28 @@
         self.content.append(Content(name=name, segments=[segment], media_type=media_type, content_service=self.context.content_service))
         return self
 
     def add_metadata(self, key: str, value: str):
         self.metadata[key] = value
         return self
 
+    def annotate(self, key: str, value: str):
+        self.annotations[key] = value
+        return self
+
+    def delete_metadata_key(self, key: str):
+        self.delete_metadata_keys.append(key)
+        return self
+
     def response(self):
         return {
             'content': [content.json() for content in self.content],
-            'metadata': self.metadata
+            'metadata': self.metadata,
+            'annotations': self.annotations,
+            'deleteMetadataKeys': self.delete_metadata_keys
         }
 
 
 class ValidateResult(Result):
     def __init__(self, context: Context):
         super().__init__(None, 'VALIDATE', context)
```

### Comparing `deltafi-1.0.0rc2/deltafi/storage.py` & `deltafi-1.0.0rc3/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc2/pyproject.toml` & `deltafi-1.0.0rc3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "1.0.0-RC2"
+version = "1.0.0-RC3"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-1.0.0rc2/PKG-INFO` & `deltafi-1.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

