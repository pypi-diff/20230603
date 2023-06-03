# Comparing `tmp/cognica-0.1.1.tar.gz` & `tmp/cognica-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.1.tar", last modified: Tue May 30 06:00:43 2023, max compression
+gzip compressed data, was "cognica-0.1.2.tar", last modified: Sat Jun  3 01:37:43 2023, max compression
```

## Comparing `cognica-0.1.1.tar` & `cognica-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-05-30 06:00:43.508277 cognica-0.1.1/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.1/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-05-30 06:00:43.508096 cognica-0.1.1/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.1/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1337 2023-05-30 06:00:28.000000 cognica-0.1.1/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-05-30 06:00:43.508338 cognica-0.1.1/setup.cfg
--rw-r--r--   0 jaepil     (501) staff       (20)     2034 2023-05-30 06:00:35.000000 cognica-0.1.1/setup.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-05-30 06:00:43.504405 cognica-0.1.1/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-05-30 06:00:43.505705 cognica-0.1.1/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.1/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.1/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    14245 2023-05-29 01:46:31.000000 cognica-0.1.1/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.1/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.1/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-05-30 06:00:43.507873 cognica-0.1.1/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.1/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11244 2023-05-29 00:52:18.000000 cognica-0.1.1/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-05-29 00:52:18.000000 cognica-0.1.1/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-04-05 07:21:53.000000 cognica-0.1.1/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2376 2023-04-05 07:21:53.000000 cognica-0.1.1/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-03-29 15:06:15.000000 cognica-0.1.1/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7123 2023-04-05 07:21:53.000000 cognica-0.1.1/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-03-29 15:06:33.000000 cognica-0.1.1/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     5589 2023-04-05 07:21:53.000000 cognica-0.1.1/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-03-29 15:06:44.000000 cognica-0.1.1/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.1/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-05-30 06:00:43.506473 cognica-0.1.1/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-05-30 06:00:43.000000 cognica-0.1.1/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      840 2023-05-30 06:00:43.000000 cognica-0.1.1/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-05-30 06:00:43.000000 cognica-0.1.1/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-05-30 06:00:43.000000 cognica-0.1.1/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-05-30 06:00:43.000000 cognica-0.1.1/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:37:43.751469 cognica-0.1.2/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.2/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-06-03 01:37:43.750605 cognica-0.1.2/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.2/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1337 2023-06-03 01:36:47.000000 cognica-0.1.2/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-03 01:37:43.751557 cognica-0.1.2/setup.cfg
+-rw-r--r--   0 jaepil     (501) staff       (20)     2034 2023-06-03 01:37:01.000000 cognica-0.1.2/setup.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:37:43.745605 cognica-0.1.2/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:37:43.747102 cognica-0.1.2/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.2/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.2/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    15678 2023-06-03 01:26:57.000000 cognica-0.1.2/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.2/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.2/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:37:43.750322 cognica-0.1.2/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.2/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    12686 2023-06-03 01:33:38.000000 cognica-0.1.2/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.2/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.2/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.2/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.2/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.2/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.2/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.2/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.2/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.2/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:37:43.747905 cognica-0.1.2/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-06-03 01:37:43.000000 cognica-0.1.2/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      840 2023-06-03 01:37:43.000000 cognica-0.1.2/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-03 01:37:43.000000 cognica-0.1.2/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-03 01:37:43.000000 cognica-0.1.2/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-03 01:37:43.000000 cognica-0.1.2/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.1/LICENSE` & `cognica-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/PKG-INFO` & `cognica-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for Cognica database
 Home-page: https://github.com/cognicadb/cognica-python
 Author: Cognica, Inc.
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cognica-0.1.1/README.md` & `cognica-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/pyproject.toml` & `cognica-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
```

### Comparing `cognica-0.1.1/setup.py` & `cognica-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "key-value",
         "document store",
         "full-text search",
         "vector search",
         "search engine",
         "database",
     ],
-    version="0.1.1",
+    version="0.1.2",
     packages=setuptools.find_namespace_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/cognicadb/cognica-python",
     project_urls={
         "Documentation": "https://github.com/cognicadb/cognica-python",
         "Changes": "https://github.com/cognicadb/cognica-python/releases",
         "Code": "https://github.com/cognicadb/cognica-python",
```

### Comparing `cognica-0.1.1/src/cognica/__init__.py` & `cognica-0.1.2/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/channel.py` & `cognica-0.1.2/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/document_db.py` & `cognica-0.1.2/src/cognica/document_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Cognica
 #
 # Copyright (c) 2023 Cognica, Inc.
 #
 
 # pylint: disable=no-member,missing-class-docstring,missing-function-docstring
+# pylint: disable=invalid-name,no-else-return
 
 import io
 import json
 import time
 import typing as t
 
 import grpc
@@ -128,15 +129,21 @@
         limit=None,
         index_columns=None,
         columns=None,
         dtypes=None,
         to_pandas=True,
         to_polars=False,
         to_arrow=False,
-    ) -> pd.DataFrame | pl.DataFrame | pa.Table:
+        enable_profile=False,
+    ) -> (
+        pd.DataFrame
+        | pl.DataFrame
+        | pa.Table
+        | tuple[pd.DataFrame | pl.DataFrame | pa.Table, dict]
+    ):
         if to_polars or to_arrow:
             to_pandas = False
 
         query = _to_json(query)
         req = FindRequest(
             query=Query(collection_name=collection, query=query),
             limit=limit,
@@ -157,21 +164,41 @@
             )
         elif to_polars:
             df = self._to_pl_dataframe(buffer=resp.buffer, columns=columns)
         elif to_arrow:
             df = self._to_arrow_table(buffer=resp.buffer, columns=columns)
         else:
             df = self._to_arrow_table(buffer=resp.buffer, columns=columns)
-        del resp
 
-        return df
+        if enable_profile:
+            profile = {
+                "duration": {
+                    "query": resp.profile.query_duration_us,
+                    "serialization": resp.profile.serialization_duration_us,
+                    "unit": "us",
+                }
+            }
+            del resp
+            return df, profile
+        else:
+            del resp
+            return df
 
     def find_batch(
-        self, requests, to_pandas=True, to_polars=False, to_arrow=False
-    ) -> list[pd.DataFrame] | list[pa.Table]:
+        self,
+        requests,
+        to_pandas=True,
+        to_polars=False,
+        to_arrow=False,
+        enable_profile=False,
+    ) -> (
+        list[pd.DataFrame]
+        | list[pa.Table]
+        | tuple[list[pd.DataFrame] | list[pa.Table], list[dict]]
+    ):
         if not requests:
             return []
 
         if to_polars or to_arrow:
             to_pandas = False
 
         batch_items = []
@@ -184,41 +211,56 @@
                 columns=req.columns,
                 dtypes=req.dtypes,
             )
             batch_items.append(item)
         batch_req = FindBatchRequest(requests=batch_items)
 
         dfs = []
+        profiles = []
         resp: FindBatchResponse = self._invoke(
             self._stub.find_batch, batch_req, wait_for_ready=True
         )
-        for req, parquet_buffer in zip(requests, resp.buffers):  # type: ignore
+        for req, response in zip(requests, resp.responses):  # type: ignore
             if to_pandas:
                 df = self._to_pd_dataframe(
-                    buffer=parquet_buffer.buffer,
+                    buffer=response.buffer,
                     index_columns=req.index_columns,
                     columns=req.columns,
                     dtypes=req.dtypes,
                 )
             elif to_polars:
                 df = self._to_pl_dataframe(
-                    buffer=resp.buffer, columns=req.columns
+                    buffer=response.buffer, columns=req.columns
                 )
             elif to_arrow:
                 df = self._to_arrow_table(
-                    buffer=resp.buffer, columns=req.columns
+                    buffer=response.buffer, columns=req.columns
                 )
             else:
                 df = self._to_arrow_table(
-                    buffer=parquet_buffer.buffer, columns=req.columns
+                    buffer=response.buffer, columns=req.columns
                 )
             dfs.append(df)
+            if enable_profile:
+                profile = {
+                    "duration": {
+                        "query": response.profile.query_duration_us,
+                        "serialization": (
+                            response.profile.serialization_duration_us
+                        ),
+                        "unit": "us",
+                    }
+                }
+                profiles.append(profile)
         del resp
 
-        return dfs
+        if enable_profile:
+            return dfs, profiles
+        else:
+            return dfs
 
     def insert(self, collection, docs) -> None:
         if not isinstance(docs, list):
             docs = [docs]
 
         items = []
         for doc in docs:
@@ -265,28 +307,34 @@
                 {
                     "collection_name": resp.collection.collection_name,
                     "primary_key": {
                         "index_id": resp.collection.primary_key.index_id,
                         "index_name": resp.collection.primary_key.index_name,
                         "fields": list(resp.collection.primary_key.fields),
                         "unique": resp.collection.primary_key.unique,
-                        "index_type": resp.collection.primary_key.index_type,
-                        "status": resp.collection.primary_key.status,
+                        "index_type": IndexType.Name(
+                            resp.collection.primary_key.index_type
+                        ),
+                        "status": IndexStatus.Name(
+                            resp.collection.primary_key.status
+                        ),
                         "options": json.loads(
                             resp.collection.primary_key.options.json or "{}"
                         ),
                     },
                     "secondary_keys": [
                         {
                             "index_id": secondary_key.index_id,
                             "index_name": secondary_key.index_name,
                             "fields": list(secondary_key.fields),
                             "unique": secondary_key.unique,
-                            "index_type": secondary_key.index_type,
-                            "status": secondary_key.status,
+                            "index_type": IndexType.Name(
+                                secondary_key.index_type
+                            ),
+                            "status": IndexStatus.Name(secondary_key.status),
                             "options": json.loads(
                                 secondary_key.options.json or "{}"
                             ),
                         }
                         for secondary_key in resp.collection.secondary_keys
                     ],
                 }
```

### Comparing `cognica-0.1.1/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.2/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/key_value_db.py` & `cognica-0.1.2/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.2/src/cognica/protobuf/document_db_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,95 +7,97 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import cognica.protobuf.document_pb2 as document__pb2
+import document_pb2 as document__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf3\x01\n\tIndexDesc\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x07 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x08 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\x9e\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x37\n\x0bprimary_key\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\x12:\n\x0esecondary_keys\x18\x03 \x03(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\";\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"9\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"u\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"e\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x36\n\nindex_desc\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"6\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"4\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\x84\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x36\n\nindex_desc\x18\x04 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"E\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"?\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"B\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"1\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"1\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"1\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"=\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x18\n\x16ListCollectionsRequest\"T\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf3\x01\n\tIndexDesc\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x07 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x08 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\x9e\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x37\n\x0bprimary_key\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\x12:\n\x0esecondary_keys\x18\x03 \x03(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"e\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x36\n\nindex_desc\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xbb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x36\n\nindex_desc\x18\x04 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\x12\x35\n\x07profile\x18\x05 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_db_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
   _FINDREQUEST_DTYPESENTRY._options = None
   _FINDREQUEST_DTYPESENTRY._serialized_options = b'8\001'
-  _INDEXTYPE._serialized_start=2837
-  _INDEXTYPE._serialized_end=2938
-  _INDEXSTATUS._serialized_start=2941
-  _INDEXSTATUS._serialized_end=3082
+  _INDEXTYPE._serialized_start=3738
+  _INDEXTYPE._serialized_end=3839
+  _INDEXSTATUS._serialized_start=3842
+  _INDEXSTATUS._serialized_end=3983
   _INDEXDESC._serialized_start=63
   _INDEXDESC._serialized_end=306
   _COLLECTIONINFO._serialized_start=309
   _COLLECTIONINFO._serialized_end=467
-  _CREATECOLLECTIONREQUEST._serialized_start=469
-  _CREATECOLLECTIONREQUEST._serialized_end=555
-  _CREATECOLLECTIONRESPONSE._serialized_start=557
-  _CREATECOLLECTIONRESPONSE._serialized_end=616
-  _DROPCOLLECTIONREQUEST._serialized_start=618
-  _DROPCOLLECTIONREQUEST._serialized_end=666
-  _DROPCOLLECTIONRESPONSE._serialized_start=668
-  _DROPCOLLECTIONRESPONSE._serialized_end=725
-  _GETCOLLECTIONREQUEST._serialized_start=727
-  _GETCOLLECTIONREQUEST._serialized_end=774
-  _GETCOLLECTIONRESPONSE._serialized_start=776
-  _GETCOLLECTIONRESPONSE._serialized_end=893
-  _CREATEINDEXREQUEST._serialized_start=895
-  _CREATEINDEXREQUEST._serialized_end=996
-  _CREATEINDEXRESPONSE._serialized_start=998
-  _CREATEINDEXRESPONSE._serialized_end=1052
-  _DROPINDEXREQUEST._serialized_start=1054
-  _DROPINDEXREQUEST._serialized_end=1117
-  _DROPINDEXRESPONSE._serialized_start=1119
-  _DROPINDEXRESPONSE._serialized_end=1171
-  _GETINDEXREQUEST._serialized_start=1173
-  _GETINDEXREQUEST._serialized_end=1235
-  _GETINDEXRESPONSE._serialized_start=1238
-  _GETINDEXRESPONSE._serialized_end=1370
-  _QUERY._serialized_start=1372
-  _QUERY._serialized_end=1454
-  _FINDREQUEST._serialized_start=1457
-  _FINDREQUEST._serialized_end=1685
-  _FINDREQUEST_DTYPESENTRY._serialized_start=1640
-  _FINDREQUEST_DTYPESENTRY._serialized_end=1685
-  _FINDRESPONSE._serialized_start=1687
-  _FINDRESPONSE._serialized_end=1756
-  _FINDBATCHREQUEST._serialized_start=1758
-  _FINDBATCHREQUEST._serialized_end=1832
-  _FINDBATCHRESPONSE._serialized_start=1834
-  _FINDBATCHRESPONSE._serialized_end=1911
-  _COUNTREQUEST._serialized_start=1913
-  _COUNTREQUEST._serialized_end=1974
-  _COUNTRESPONSE._serialized_start=1976
-  _COUNTRESPONSE._serialized_end=2039
-  _CONTAINSREQUEST._serialized_start=2041
-  _CONTAINSREQUEST._serialized_end=2105
-  _CONTAINSRESPONSE._serialized_start=2107
-  _CONTAINSRESPONSE._serialized_end=2173
-  _INSERTREQUEST._serialized_start=2175
-  _INSERTREQUEST._serialized_end=2240
-  _INSERTRESPONSE._serialized_start=2242
-  _INSERTRESPONSE._serialized_end=2291
-  _UPDATEREQUEST._serialized_start=2294
-  _UPDATEREQUEST._serialized_end=2437
-  _UPDATERESPONSE._serialized_start=2439
-  _UPDATERESPONSE._serialized_end=2488
-  _REMOVEREQUEST._serialized_start=2490
-  _REMOVEREQUEST._serialized_end=2555
-  _REMOVERESPONSE._serialized_start=2557
-  _REMOVERESPONSE._serialized_end=2606
-  _TRUNCATECOLLECTIONREQUEST._serialized_start=2608
-  _TRUNCATECOLLECTIONREQUEST._serialized_end=2660
-  _TRUNCATECOLLECTIONRESPONSE._serialized_start=2662
-  _TRUNCATECOLLECTIONRESPONSE._serialized_end=2723
-  _LISTCOLLECTIONSREQUEST._serialized_start=2725
-  _LISTCOLLECTIONSREQUEST._serialized_end=2749
-  _LISTCOLLECTIONSRESPONSE._serialized_start=2751
-  _LISTCOLLECTIONSRESPONSE._serialized_end=2835
-  _DOCUMENTDBSERVICE._serialized_start=3085
-  _DOCUMENTDBSERVICE._serialized_end=4683
+  _PROFILEINFO._serialized_start=469
+  _PROFILEINFO._serialized_end=596
+  _CREATECOLLECTIONREQUEST._serialized_start=598
+  _CREATECOLLECTIONREQUEST._serialized_end=684
+  _CREATECOLLECTIONRESPONSE._serialized_start=686
+  _CREATECOLLECTIONRESPONSE._serialized_end=800
+  _DROPCOLLECTIONREQUEST._serialized_start=802
+  _DROPCOLLECTIONREQUEST._serialized_end=850
+  _DROPCOLLECTIONRESPONSE._serialized_start=852
+  _DROPCOLLECTIONRESPONSE._serialized_end=964
+  _GETCOLLECTIONREQUEST._serialized_start=966
+  _GETCOLLECTIONREQUEST._serialized_end=1013
+  _GETCOLLECTIONRESPONSE._serialized_start=1016
+  _GETCOLLECTIONRESPONSE._serialized_end=1188
+  _CREATEINDEXREQUEST._serialized_start=1190
+  _CREATEINDEXREQUEST._serialized_end=1291
+  _CREATEINDEXRESPONSE._serialized_start=1293
+  _CREATEINDEXRESPONSE._serialized_end=1402
+  _DROPINDEXREQUEST._serialized_start=1404
+  _DROPINDEXREQUEST._serialized_end=1467
+  _DROPINDEXRESPONSE._serialized_start=1469
+  _DROPINDEXRESPONSE._serialized_end=1576
+  _GETINDEXREQUEST._serialized_start=1578
+  _GETINDEXREQUEST._serialized_end=1640
+  _GETINDEXRESPONSE._serialized_start=1643
+  _GETINDEXRESPONSE._serialized_end=1830
+  _QUERY._serialized_start=1832
+  _QUERY._serialized_end=1914
+  _FINDREQUEST._serialized_start=1917
+  _FINDREQUEST._serialized_end=2145
+  _FINDREQUEST_DTYPESENTRY._serialized_start=2100
+  _FINDREQUEST_DTYPESENTRY._serialized_end=2145
+  _FINDRESPONSE._serialized_start=2147
+  _FINDRESPONSE._serialized_end=2271
+  _FINDBATCHREQUEST._serialized_start=2273
+  _FINDBATCHREQUEST._serialized_end=2347
+  _FINDBATCHRESPONSE._serialized_start=2349
+  _FINDBATCHRESPONSE._serialized_end=2426
+  _COUNTREQUEST._serialized_start=2428
+  _COUNTREQUEST._serialized_end=2489
+  _COUNTRESPONSE._serialized_start=2491
+  _COUNTRESPONSE._serialized_end=2609
+  _CONTAINSREQUEST._serialized_start=2611
+  _CONTAINSREQUEST._serialized_end=2675
+  _CONTAINSRESPONSE._serialized_start=2677
+  _CONTAINSRESPONSE._serialized_end=2798
+  _INSERTREQUEST._serialized_start=2800
+  _INSERTREQUEST._serialized_end=2865
+  _INSERTRESPONSE._serialized_start=2867
+  _INSERTRESPONSE._serialized_end=2971
+  _UPDATEREQUEST._serialized_start=2974
+  _UPDATEREQUEST._serialized_end=3117
+  _UPDATERESPONSE._serialized_start=3119
+  _UPDATERESPONSE._serialized_end=3223
+  _REMOVEREQUEST._serialized_start=3225
+  _REMOVEREQUEST._serialized_end=3290
+  _REMOVERESPONSE._serialized_start=3292
+  _REMOVERESPONSE._serialized_end=3396
+  _TRUNCATECOLLECTIONREQUEST._serialized_start=3398
+  _TRUNCATECOLLECTIONREQUEST._serialized_end=3450
+  _TRUNCATECOLLECTIONRESPONSE._serialized_start=3452
+  _TRUNCATECOLLECTIONRESPONSE._serialized_end=3568
+  _LISTCOLLECTIONSREQUEST._serialized_start=3570
+  _LISTCOLLECTIONSREQUEST._serialized_end=3594
+  _LISTCOLLECTIONSRESPONSE._serialized_start=3597
+  _LISTCOLLECTIONSRESPONSE._serialized_end=3736
+  _DOCUMENTDBSERVICE._serialized_start=3986
+  _DOCUMENTDBSERVICE._serialized_end=5584
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.1/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.2/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.2/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.2/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66ts_analysis_pipeline.proto\x12\x12\x63ognica.rpc.db.fts\"k\n\x18PipelineExecutionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x03 \x03(\t\x12\r\n\x05query\x18\x04 \x01(\t\";\n\x19PipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\"Y\n\x1d\x41\x64hocPipelineExecutionRequest\x12\x14\n\x0cpipeline_def\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x02 \x03(\t\x12\r\n\x05query\x18\x03 \x01(\t\"@\n\x1e\x41\x64hocPipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t2\x80\x02\n\x1a\x46TSAnalysisPipelineService\x12h\n\x07\x65xecute\x12,.cognica.rpc.db.fts.PipelineExecutionRequest\x1a-.cognica.rpc.db.fts.PipelineExecutionResponse\"\x00\x12x\n\rexecute_adhoc\x12\x31.cognica.rpc.db.fts.AdhocPipelineExecutionRequest\x1a\x32.cognica.rpc.db.fts.AdhocPipelineExecutionResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66ts_analysis_pipeline.proto\x12\x12\x63ognica.rpc.db.fts\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"k\n\x18PipelineExecutionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x03 \x03(\t\x12\r\n\x05query\x18\x04 \x01(\t\"m\n\x19PipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12\x30\n\x07profile\x18\x03 \x01(\x0b\x32\x1f.cognica.rpc.db.fts.ProfileInfo\"Y\n\x1d\x41\x64hocPipelineExecutionRequest\x12\x14\n\x0cpipeline_def\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_names\x18\x02 \x03(\t\x12\r\n\x05query\x18\x03 \x01(\t\"r\n\x1e\x41\x64hocPipelineExecutionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\t\x12\x30\n\x07profile\x18\x03 \x01(\x0b\x32\x1f.cognica.rpc.db.fts.ProfileInfo2\x80\x02\n\x1a\x46TSAnalysisPipelineService\x12h\n\x07\x65xecute\x12,.cognica.rpc.db.fts.PipelineExecutionRequest\x1a-.cognica.rpc.db.fts.PipelineExecutionResponse\"\x00\x12x\n\rexecute_adhoc\x12\x31.cognica.rpc.db.fts.AdhocPipelineExecutionRequest\x1a\x32.cognica.rpc.db.fts.AdhocPipelineExecutionResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fts_analysis_pipeline_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
-  _PIPELINEEXECUTIONREQUEST._serialized_start=51
-  _PIPELINEEXECUTIONREQUEST._serialized_end=158
-  _PIPELINEEXECUTIONRESPONSE._serialized_start=160
-  _PIPELINEEXECUTIONRESPONSE._serialized_end=219
-  _ADHOCPIPELINEEXECUTIONREQUEST._serialized_start=221
-  _ADHOCPIPELINEEXECUTIONREQUEST._serialized_end=310
-  _ADHOCPIPELINEEXECUTIONRESPONSE._serialized_start=312
-  _ADHOCPIPELINEEXECUTIONRESPONSE._serialized_end=376
-  _FTSANALYSISPIPELINESERVICE._serialized_start=379
-  _FTSANALYSISPIPELINESERVICE._serialized_end=635
+  _PROFILEINFO._serialized_start=51
+  _PROFILEINFO._serialized_end=85
+  _PIPELINEEXECUTIONREQUEST._serialized_start=87
+  _PIPELINEEXECUTIONREQUEST._serialized_end=194
+  _PIPELINEEXECUTIONRESPONSE._serialized_start=196
+  _PIPELINEEXECUTIONRESPONSE._serialized_end=305
+  _ADHOCPIPELINEEXECUTIONREQUEST._serialized_start=307
+  _ADHOCPIPELINEEXECUTIONREQUEST._serialized_end=396
+  _ADHOCPIPELINEEXECUTIONRESPONSE._serialized_start=398
+  _ADHOCPIPELINEEXECUTIONRESPONSE._serialized_end=512
+  _FTSANALYSISPIPELINESERVICE._serialized_start=515
+  _FTSANALYSISPIPELINESERVICE._serialized_end=771
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.1/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.2/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.2/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,68 +9,70 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12key_value_db.proto\x12\x11\x63ognica.rpc.db.kv\"J\n\x08Response\x12-\n\x06status\x18\x01 \x01(\x0e\x32\x1d.cognica.rpc.db.kv.StatusType\x12\x0f\n\x07message\x18\x02 \x01(\t\"g\n\nPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\r\n\x05value\x18\x03 \x01(\x0c\x12\x0b\n\x03ttl\x18\x04 \x01(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"<\n\x0bPutResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"3\n\rRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"?\n\x0eRemoveResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\nGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"K\n\x0bGetResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\r\n\x05value\x18\x02 \x01(\x0c\"6\n\x0fMultiGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"R\n\x10MultiGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\"q\n\x11\x42\x61tchedPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\x12\x0e\n\x06values\x18\x03 \x03(\x0c\x12\x0c\n\x04ttls\x18\x04 \x03(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"D\n\x12\x42\x61tchedPutResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\";\n\x14\x42\x61tchedRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"G\n\x15\x42\x61tchedRemoveResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"8\n\x11\x42\x61tchedGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"T\n\x12\x42\x61tchedGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\".\n\x15\x43reateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"G\n\x16\x43reateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\",\n\x13\x44ropKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"E\n\x14\x44ropKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\x17TruncateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"I\n\x18TruncateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"\x16\n\x14ListKeyspacesRequest\"^\n\x15ListKeyspacesResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x16\n\x0ekeyspace_names\x18\x02 \x03(\t*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\xe4\x04\n\x11KeyValueDBService\x12\x46\n\x03put\x12\x1d.cognica.rpc.db.kv.PutRequest\x1a\x1e.cognica.rpc.db.kv.PutResponse\"\x00\x12O\n\x06remove\x12 .cognica.rpc.db.kv.RemoveRequest\x1a!.cognica.rpc.db.kv.RemoveResponse\"\x00\x12\x46\n\x03get\x12\x1d.cognica.rpc.db.kv.GetRequest\x1a\x1e.cognica.rpc.db.kv.GetResponse\"\x00\x12Q\n\x04mget\x12\".cognica.rpc.db.kv.MultiGetRequest\x1a#.cognica.rpc.db.kv.MultiGetResponse\"\x00\x12Z\n\tput_batch\x12$.cognica.rpc.db.kv.BatchedPutRequest\x1a%.cognica.rpc.db.kv.BatchedPutResponse\"\x00\x12\x63\n\x0cremove_batch\x12\'.cognica.rpc.db.kv.BatchedRemoveRequest\x1a(.cognica.rpc.db.kv.BatchedRemoveResponse\"\x00\x12Z\n\tget_batch\x12$.cognica.rpc.db.kv.BatchedGetRequest\x1a%.cognica.rpc.db.kv.BatchedGetResponse\"\x00\x32\xbd\x03\n\x16KeyspaceManagerService\x12h\n\x0f\x63reate_keyspace\x12(.cognica.rpc.db.kv.CreateKeyspaceRequest\x1a).cognica.rpc.db.kv.CreateKeyspaceResponse\"\x00\x12\x62\n\rdrop_keyspace\x12&.cognica.rpc.db.kv.DropKeyspaceRequest\x1a\'.cognica.rpc.db.kv.DropKeyspaceResponse\"\x00\x12n\n\x11truncate_keyspace\x12*.cognica.rpc.db.kv.TruncateKeyspaceRequest\x1a+.cognica.rpc.db.kv.TruncateKeyspaceResponse\"\x00\x12\x65\n\x0elist_keyspaces\x12\'.cognica.rpc.db.kv.ListKeyspacesRequest\x1a(.cognica.rpc.db.kv.ListKeyspacesResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12key_value_db.proto\x12\x11\x63ognica.rpc.db.kv\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"{\n\x08Response\x12-\n\x06status\x18\x01 \x01(\x0e\x32\x1d.cognica.rpc.db.kv.StatusType\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x07profile\x18\x03 \x01(\x0b\x32\x1e.cognica.rpc.db.kv.ProfileInfo\"g\n\nPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\r\n\x05value\x18\x03 \x01(\x0c\x12\x0b\n\x03ttl\x18\x04 \x01(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"<\n\x0bPutResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"3\n\rRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"?\n\x0eRemoveResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\nGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\"K\n\x0bGetResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\r\n\x05value\x18\x02 \x01(\x0c\"6\n\x0fMultiGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"R\n\x10MultiGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\"q\n\x11\x42\x61tchedPutRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\x12\x0e\n\x06values\x18\x03 \x03(\x0c\x12\x0c\n\x04ttls\x18\x04 \x03(\x03\x12\x19\n\x11\x63reate_if_missing\x18\x05 \x01(\x08\"D\n\x12\x42\x61tchedPutResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\";\n\x14\x42\x61tchedRemoveRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"G\n\x15\x42\x61tchedRemoveResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"8\n\x11\x42\x61tchedGetRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\x0c\"T\n\x12\x42\x61tchedGetResponse\x12.\n\tresponses\x18\x01 \x03(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x0e\n\x06values\x18\x02 \x03(\x0c\".\n\x15\x43reateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"G\n\x16\x43reateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\",\n\x13\x44ropKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"E\n\x14\x44ropKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"0\n\x17TruncateKeyspaceRequest\x12\x15\n\rkeyspace_name\x18\x01 \x01(\t\"I\n\x18TruncateKeyspaceResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\"\x16\n\x14ListKeyspacesRequest\"^\n\x15ListKeyspacesResponse\x12-\n\x08response\x18\x01 \x01(\x0b\x32\x1b.cognica.rpc.db.kv.Response\x12\x16\n\x0ekeyspace_names\x18\x02 \x03(\t*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\xe4\x04\n\x11KeyValueDBService\x12\x46\n\x03put\x12\x1d.cognica.rpc.db.kv.PutRequest\x1a\x1e.cognica.rpc.db.kv.PutResponse\"\x00\x12O\n\x06remove\x12 .cognica.rpc.db.kv.RemoveRequest\x1a!.cognica.rpc.db.kv.RemoveResponse\"\x00\x12\x46\n\x03get\x12\x1d.cognica.rpc.db.kv.GetRequest\x1a\x1e.cognica.rpc.db.kv.GetResponse\"\x00\x12Q\n\x04mget\x12\".cognica.rpc.db.kv.MultiGetRequest\x1a#.cognica.rpc.db.kv.MultiGetResponse\"\x00\x12Z\n\tput_batch\x12$.cognica.rpc.db.kv.BatchedPutRequest\x1a%.cognica.rpc.db.kv.BatchedPutResponse\"\x00\x12\x63\n\x0cremove_batch\x12\'.cognica.rpc.db.kv.BatchedRemoveRequest\x1a(.cognica.rpc.db.kv.BatchedRemoveResponse\"\x00\x12Z\n\tget_batch\x12$.cognica.rpc.db.kv.BatchedGetRequest\x1a%.cognica.rpc.db.kv.BatchedGetResponse\"\x00\x32\xbd\x03\n\x16KeyspaceManagerService\x12h\n\x0f\x63reate_keyspace\x12(.cognica.rpc.db.kv.CreateKeyspaceRequest\x1a).cognica.rpc.db.kv.CreateKeyspaceResponse\"\x00\x12\x62\n\rdrop_keyspace\x12&.cognica.rpc.db.kv.DropKeyspaceRequest\x1a\'.cognica.rpc.db.kv.DropKeyspaceResponse\"\x00\x12n\n\x11truncate_keyspace\x12*.cognica.rpc.db.kv.TruncateKeyspaceRequest\x1a+.cognica.rpc.db.kv.TruncateKeyspaceResponse\"\x00\x12\x65\n\x0elist_keyspaces\x12\'.cognica.rpc.db.kv.ListKeyspacesRequest\x1a(.cognica.rpc.db.kv.ListKeyspacesResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'key_value_db_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
-  _STATUSTYPE._serialized_start=1615
-  _STATUSTYPE._serialized_end=1666
-  _RESPONSE._serialized_start=41
-  _RESPONSE._serialized_end=115
-  _PUTREQUEST._serialized_start=117
-  _PUTREQUEST._serialized_end=220
-  _PUTRESPONSE._serialized_start=222
-  _PUTRESPONSE._serialized_end=282
-  _REMOVEREQUEST._serialized_start=284
-  _REMOVEREQUEST._serialized_end=335
-  _REMOVERESPONSE._serialized_start=337
-  _REMOVERESPONSE._serialized_end=400
-  _GETREQUEST._serialized_start=402
-  _GETREQUEST._serialized_end=450
-  _GETRESPONSE._serialized_start=452
-  _GETRESPONSE._serialized_end=527
-  _MULTIGETREQUEST._serialized_start=529
-  _MULTIGETREQUEST._serialized_end=583
-  _MULTIGETRESPONSE._serialized_start=585
-  _MULTIGETRESPONSE._serialized_end=667
-  _BATCHEDPUTREQUEST._serialized_start=669
-  _BATCHEDPUTREQUEST._serialized_end=782
-  _BATCHEDPUTRESPONSE._serialized_start=784
-  _BATCHEDPUTRESPONSE._serialized_end=852
-  _BATCHEDREMOVEREQUEST._serialized_start=854
-  _BATCHEDREMOVEREQUEST._serialized_end=913
-  _BATCHEDREMOVERESPONSE._serialized_start=915
-  _BATCHEDREMOVERESPONSE._serialized_end=986
-  _BATCHEDGETREQUEST._serialized_start=988
-  _BATCHEDGETREQUEST._serialized_end=1044
-  _BATCHEDGETRESPONSE._serialized_start=1046
-  _BATCHEDGETRESPONSE._serialized_end=1130
-  _CREATEKEYSPACEREQUEST._serialized_start=1132
-  _CREATEKEYSPACEREQUEST._serialized_end=1178
-  _CREATEKEYSPACERESPONSE._serialized_start=1180
-  _CREATEKEYSPACERESPONSE._serialized_end=1251
-  _DROPKEYSPACEREQUEST._serialized_start=1253
-  _DROPKEYSPACEREQUEST._serialized_end=1297
-  _DROPKEYSPACERESPONSE._serialized_start=1299
-  _DROPKEYSPACERESPONSE._serialized_end=1368
-  _TRUNCATEKEYSPACEREQUEST._serialized_start=1370
-  _TRUNCATEKEYSPACEREQUEST._serialized_end=1418
-  _TRUNCATEKEYSPACERESPONSE._serialized_start=1420
-  _TRUNCATEKEYSPACERESPONSE._serialized_end=1493
-  _LISTKEYSPACESREQUEST._serialized_start=1495
-  _LISTKEYSPACESREQUEST._serialized_end=1517
-  _LISTKEYSPACESRESPONSE._serialized_start=1519
-  _LISTKEYSPACESRESPONSE._serialized_end=1613
-  _KEYVALUEDBSERVICE._serialized_start=1669
-  _KEYVALUEDBSERVICE._serialized_end=2281
-  _KEYSPACEMANAGERSERVICE._serialized_start=2284
-  _KEYSPACEMANAGERSERVICE._serialized_end=2729
+  _STATUSTYPE._serialized_start=1700
+  _STATUSTYPE._serialized_end=1751
+  _PROFILEINFO._serialized_start=41
+  _PROFILEINFO._serialized_end=75
+  _RESPONSE._serialized_start=77
+  _RESPONSE._serialized_end=200
+  _PUTREQUEST._serialized_start=202
+  _PUTREQUEST._serialized_end=305
+  _PUTRESPONSE._serialized_start=307
+  _PUTRESPONSE._serialized_end=367
+  _REMOVEREQUEST._serialized_start=369
+  _REMOVEREQUEST._serialized_end=420
+  _REMOVERESPONSE._serialized_start=422
+  _REMOVERESPONSE._serialized_end=485
+  _GETREQUEST._serialized_start=487
+  _GETREQUEST._serialized_end=535
+  _GETRESPONSE._serialized_start=537
+  _GETRESPONSE._serialized_end=612
+  _MULTIGETREQUEST._serialized_start=614
+  _MULTIGETREQUEST._serialized_end=668
+  _MULTIGETRESPONSE._serialized_start=670
+  _MULTIGETRESPONSE._serialized_end=752
+  _BATCHEDPUTREQUEST._serialized_start=754
+  _BATCHEDPUTREQUEST._serialized_end=867
+  _BATCHEDPUTRESPONSE._serialized_start=869
+  _BATCHEDPUTRESPONSE._serialized_end=937
+  _BATCHEDREMOVEREQUEST._serialized_start=939
+  _BATCHEDREMOVEREQUEST._serialized_end=998
+  _BATCHEDREMOVERESPONSE._serialized_start=1000
+  _BATCHEDREMOVERESPONSE._serialized_end=1071
+  _BATCHEDGETREQUEST._serialized_start=1073
+  _BATCHEDGETREQUEST._serialized_end=1129
+  _BATCHEDGETRESPONSE._serialized_start=1131
+  _BATCHEDGETRESPONSE._serialized_end=1215
+  _CREATEKEYSPACEREQUEST._serialized_start=1217
+  _CREATEKEYSPACEREQUEST._serialized_end=1263
+  _CREATEKEYSPACERESPONSE._serialized_start=1265
+  _CREATEKEYSPACERESPONSE._serialized_end=1336
+  _DROPKEYSPACEREQUEST._serialized_start=1338
+  _DROPKEYSPACEREQUEST._serialized_end=1382
+  _DROPKEYSPACERESPONSE._serialized_start=1384
+  _DROPKEYSPACERESPONSE._serialized_end=1453
+  _TRUNCATEKEYSPACEREQUEST._serialized_start=1455
+  _TRUNCATEKEYSPACEREQUEST._serialized_end=1503
+  _TRUNCATEKEYSPACERESPONSE._serialized_start=1505
+  _TRUNCATEKEYSPACERESPONSE._serialized_end=1578
+  _LISTKEYSPACESREQUEST._serialized_start=1580
+  _LISTKEYSPACESREQUEST._serialized_end=1602
+  _LISTKEYSPACESRESPONSE._serialized_start=1604
+  _LISTKEYSPACESRESPONSE._serialized_end=1698
+  _KEYVALUEDBSERVICE._serialized_start=1754
+  _KEYVALUEDBSERVICE._serialized_end=2366
+  _KEYSPACEMANAGERSERVICE._serialized_start=2369
+  _KEYSPACEMANAGERSERVICE._serialized_end=2814
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.1/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.2/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.2/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,52 +9,54 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asentence_transformer.proto\x12 cognica.rpc.sentence_transformer\"$\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\"?\n\x16SentenceEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tsentences\x18\x02 \x03(\t\"\xa6\x01\n\x17SentenceEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\"4\n\x0cSentencePair\x12\x11\n\tsentence1\x18\x01 \x01(\t\x12\x11\n\tsentence2\x18\x02 \x01(\t\"l\n\x13\x43rossEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x41\n\tsentences\x18\x02 \x03(\x0b\x32..cognica.rpc.sentence_transformer.SentencePair\"x\n\x14\x43rossEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x0e\n\x06scores\x18\x03 \x03(\x02\"\xb0\x01\n\x12\x43LIPEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12P\n\x06\x66ormat\x18\x02 \x01(\x0e\x32@.cognica.rpc.sentence_transformer.CLIPEncoderRequest.InputFormat\x12\x0e\n\x06inputs\x18\x03 \x03(\x0c\"$\n\x0bInputFormat\x12\t\n\x05kText\x10\x00\x12\n\n\x06kImage\x10\x01\"\xa2\x01\n\x13\x43LIPEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\"Z\n\x10QAEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tquestions\x18\x02 \x03(\t\x12\x10\n\x08\x63ontexts\x18\x03 \x03(\t\x12\r\n\x05top_k\x18\x04 \x01(\x05\"\xe5\x02\n\x11QAEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12R\n\x07\x61nswers\x18\x03 \x03(\x0b\x32\x41.cognica.rpc.sentence_transformer.QAEncoderResponse.CandidateList\x1a\x46\n\tCandidate\x12\r\n\x05score\x18\x01 \x01(\x02\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\x12\x0e\n\x06\x61nswer\x18\x04 \x01(\t\x1a\x62\n\rCandidateList\x12Q\n\ncandidates\x18\x01 \x03(\x0b\x32=.cognica.rpc.sentence_transformer.QAEncoderResponse.Candidate*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\x9d\x01\n\x1aSentenceTransformerService\x12\x7f\n\x06\x65ncode\x12\x38.cognica.rpc.sentence_transformer.SentenceEncoderRequest\x1a\x39.cognica.rpc.sentence_transformer.SentenceEncoderResponse\"\x00\x32\x91\x01\n\x13\x43rossEncoderService\x12z\n\x07predict\x12\x35.cognica.rpc.sentence_transformer.CrossEncoderRequest\x1a\x36.cognica.rpc.sentence_transformer.CrossEncoderResponse\"\x00\x32\x8d\x01\n\x12\x43LIPEncoderService\x12w\n\x06\x65ncode\x12\x34.cognica.rpc.sentence_transformer.CLIPEncoderRequest\x1a\x35.cognica.rpc.sentence_transformer.CLIPEncoderResponse\"\x00\x32\x88\x01\n\x10QAEncoderService\x12t\n\x07predict\x12\x32.cognica.rpc.sentence_transformer.QAEncoderRequest\x1a\x33.cognica.rpc.sentence_transformer.QAEncoderResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asentence_transformer.proto\x12 cognica.rpc.sentence_transformer\"$\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\"\"\n\x0bProfileInfo\x12\x13\n\x0b\x64uration_us\x18\x01 \x01(\x04\"?\n\x16SentenceEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tsentences\x18\x02 \x03(\t\"\xe7\x01\n\x17SentenceEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"4\n\x0cSentencePair\x12\x11\n\tsentence1\x18\x01 \x01(\t\x12\x11\n\tsentence2\x18\x02 \x01(\t\"l\n\x13\x43rossEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x41\n\tsentences\x18\x02 \x03(\x0b\x32..cognica.rpc.sentence_transformer.SentencePair\"\xb9\x01\n\x14\x43rossEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x0e\n\x06scores\x18\x03 \x03(\x02\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"\xb0\x01\n\x12\x43LIPEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12P\n\x06\x66ormat\x18\x02 \x01(\x0e\x32@.cognica.rpc.sentence_transformer.CLIPEncoderRequest.InputFormat\x12\x0e\n\x06inputs\x18\x03 \x03(\x0c\"$\n\x0bInputFormat\x12\t\n\x05kText\x10\x00\x12\n\n\x06kImage\x10\x01\"\xe3\x01\n\x13\x43LIPEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x39\n\x07tensors\x18\x03 \x03(\x0b\x32(.cognica.rpc.sentence_transformer.Tensor\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\"Z\n\x10QAEncoderRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x11\n\tquestions\x18\x02 \x03(\t\x12\x10\n\x08\x63ontexts\x18\x03 \x03(\t\x12\r\n\x05top_k\x18\x04 \x01(\x05\"\xa6\x03\n\x11QAEncoderResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.cognica.rpc.sentence_transformer.StatusType\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12R\n\x07\x61nswers\x18\x03 \x03(\x0b\x32\x41.cognica.rpc.sentence_transformer.QAEncoderResponse.CandidateList\x12?\n\x08profiles\x18\x04 \x03(\x0b\x32-.cognica.rpc.sentence_transformer.ProfileInfo\x1a\x46\n\tCandidate\x12\r\n\x05score\x18\x01 \x01(\x02\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\x12\x0e\n\x06\x61nswer\x18\x04 \x01(\t\x1a\x62\n\rCandidateList\x12Q\n\ncandidates\x18\x01 \x03(\x0b\x32=.cognica.rpc.sentence_transformer.QAEncoderResponse.Candidate*3\n\nStatusType\x12\x07\n\x03kOK\x10\x00\x12\r\n\tkNotFound\x10\x01\x12\r\n\tkInternal\x10\n2\x9d\x01\n\x1aSentenceTransformerService\x12\x7f\n\x06\x65ncode\x12\x38.cognica.rpc.sentence_transformer.SentenceEncoderRequest\x1a\x39.cognica.rpc.sentence_transformer.SentenceEncoderResponse\"\x00\x32\x91\x01\n\x13\x43rossEncoderService\x12z\n\x07predict\x12\x35.cognica.rpc.sentence_transformer.CrossEncoderRequest\x1a\x36.cognica.rpc.sentence_transformer.CrossEncoderResponse\"\x00\x32\x8d\x01\n\x12\x43LIPEncoderService\x12w\n\x06\x65ncode\x12\x34.cognica.rpc.sentence_transformer.CLIPEncoderRequest\x1a\x35.cognica.rpc.sentence_transformer.CLIPEncoderResponse\"\x00\x32\x88\x01\n\x10QAEncoderService\x12t\n\x07predict\x12\x32.cognica.rpc.sentence_transformer.QAEncoderRequest\x1a\x33.cognica.rpc.sentence_transformer.QAEncoderResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentence_transformer_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
-  _STATUSTYPE._serialized_start=1418
-  _STATUSTYPE._serialized_end=1469
+  _STATUSTYPE._serialized_start=1715
+  _STATUSTYPE._serialized_end=1766
   _TENSOR._serialized_start=64
   _TENSOR._serialized_end=100
-  _SENTENCEENCODERREQUEST._serialized_start=102
-  _SENTENCEENCODERREQUEST._serialized_end=165
-  _SENTENCEENCODERRESPONSE._serialized_start=168
-  _SENTENCEENCODERRESPONSE._serialized_end=334
-  _SENTENCEPAIR._serialized_start=336
-  _SENTENCEPAIR._serialized_end=388
-  _CROSSENCODERREQUEST._serialized_start=390
-  _CROSSENCODERREQUEST._serialized_end=498
-  _CROSSENCODERRESPONSE._serialized_start=500
-  _CROSSENCODERRESPONSE._serialized_end=620
-  _CLIPENCODERREQUEST._serialized_start=623
-  _CLIPENCODERREQUEST._serialized_end=799
-  _CLIPENCODERREQUEST_INPUTFORMAT._serialized_start=763
-  _CLIPENCODERREQUEST_INPUTFORMAT._serialized_end=799
-  _CLIPENCODERRESPONSE._serialized_start=802
-  _CLIPENCODERRESPONSE._serialized_end=964
-  _QAENCODERREQUEST._serialized_start=966
-  _QAENCODERREQUEST._serialized_end=1056
-  _QAENCODERRESPONSE._serialized_start=1059
-  _QAENCODERRESPONSE._serialized_end=1416
-  _QAENCODERRESPONSE_CANDIDATE._serialized_start=1246
-  _QAENCODERRESPONSE_CANDIDATE._serialized_end=1316
-  _QAENCODERRESPONSE_CANDIDATELIST._serialized_start=1318
-  _QAENCODERRESPONSE_CANDIDATELIST._serialized_end=1416
-  _SENTENCETRANSFORMERSERVICE._serialized_start=1472
-  _SENTENCETRANSFORMERSERVICE._serialized_end=1629
-  _CROSSENCODERSERVICE._serialized_start=1632
-  _CROSSENCODERSERVICE._serialized_end=1777
-  _CLIPENCODERSERVICE._serialized_start=1780
-  _CLIPENCODERSERVICE._serialized_end=1921
-  _QAENCODERSERVICE._serialized_start=1924
-  _QAENCODERSERVICE._serialized_end=2060
+  _PROFILEINFO._serialized_start=102
+  _PROFILEINFO._serialized_end=136
+  _SENTENCEENCODERREQUEST._serialized_start=138
+  _SENTENCEENCODERREQUEST._serialized_end=201
+  _SENTENCEENCODERRESPONSE._serialized_start=204
+  _SENTENCEENCODERRESPONSE._serialized_end=435
+  _SENTENCEPAIR._serialized_start=437
+  _SENTENCEPAIR._serialized_end=489
+  _CROSSENCODERREQUEST._serialized_start=491
+  _CROSSENCODERREQUEST._serialized_end=599
+  _CROSSENCODERRESPONSE._serialized_start=602
+  _CROSSENCODERRESPONSE._serialized_end=787
+  _CLIPENCODERREQUEST._serialized_start=790
+  _CLIPENCODERREQUEST._serialized_end=966
+  _CLIPENCODERREQUEST_INPUTFORMAT._serialized_start=930
+  _CLIPENCODERREQUEST_INPUTFORMAT._serialized_end=966
+  _CLIPENCODERRESPONSE._serialized_start=969
+  _CLIPENCODERRESPONSE._serialized_end=1196
+  _QAENCODERREQUEST._serialized_start=1198
+  _QAENCODERREQUEST._serialized_end=1288
+  _QAENCODERRESPONSE._serialized_start=1291
+  _QAENCODERRESPONSE._serialized_end=1713
+  _QAENCODERRESPONSE_CANDIDATE._serialized_start=1543
+  _QAENCODERRESPONSE_CANDIDATE._serialized_end=1613
+  _QAENCODERRESPONSE_CANDIDATELIST._serialized_start=1615
+  _QAENCODERRESPONSE_CANDIDATELIST._serialized_end=1713
+  _SENTENCETRANSFORMERSERVICE._serialized_start=1769
+  _SENTENCETRANSFORMERSERVICE._serialized_end=1926
+  _CROSSENCODERSERVICE._serialized_start=1929
+  _CROSSENCODERSERVICE._serialized_end=2074
+  _CLIPENCODERSERVICE._serialized_start=2077
+  _CLIPENCODERSERVICE._serialized_end=2218
+  _QAENCODERSERVICE._serialized_start=2221
+  _QAENCODERSERVICE._serialized_end=2357
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.1/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.2/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica/sentence_transformer.py` & `cognica-0.1.2/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.1/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.2/src/cognica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for Cognica database
 Home-page: https://github.com/cognicadb/cognica-python
 Author: Cognica, Inc.
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cognica-0.1.1/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.2/src/cognica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

