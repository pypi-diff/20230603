# Comparing `tmp/navalmartin_mir_db_utils-0.0.35.tar.gz` & `tmp/navalmartin_mir_db_utils-0.0.9.tar.gz`

## Comparing `navalmartin_mir_db_utils-0.0.35.tar` & `navalmartin_mir_db_utils-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,23 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/requirements.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/setup.cfg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/setup.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/crud/__init__.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/crud/crud_utils.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/crud/mongodb_crud_ops.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/crud/mongodb_response_adaptors.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/crud/task_utils.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/dbs/__init__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/dbs/dbs_utils.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/dbs/mongodb_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/monitoring_tasks.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/simple_queries.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/simple_schemata.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/use_transaction.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/__init__.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/task_configuration_schema.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/task_performance_result_schema.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/task_result_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/data_views/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/data_views/indexed_item_data_view_base.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/schemata/data_views/user_data_view_base.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/transanctions/__init__.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/transanctions/decorators.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/transanctions/mongodb_transactions.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/utils/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/utils/db_enums.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/utils/exceptions.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/utils/transform_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/tests/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/LICENSE
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/pyproject.toml
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/crud/__init__.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/crud/mongodb_crud_utils.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/dbs/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/dbs/dbs_utils.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/dbs/mongodb_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/examples/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/examples/simple_queries.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/examples/use_transaction.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/transanctions/__init__.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/transanctions/decorators.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/transanctions/mongodb_transactions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/utils/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/utils/db_enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 navalmartin_mir_db_utils-0.0.9/PKG-INFO
```

### Comparing `navalmartin_mir_db_utils-0.0.35/setup.py` & `navalmartin_mir_db_utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/dbs/mongodb_session.py` & `navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/dbs/mongodb_session.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/simple_queries.py` & `navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/examples/simple_queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,47 @@
 import asyncio
 import bson
 from navalmartin_mir_db_utils.dbs.mongodb_session import MongoDBSession
-from navalmartin_mir_db_utils.crud.mongodb_crud_ops import ReadEntityCRUDAPI
-from navalmartin_mir_db_utils.utils.exceptions import ResourceNotFoundException
-from navalmartin_mir_db_utils.crud.crud_utils import get_one_result_or_raise
-
-COLLECTION_NAME = "YOUR_COLLECTION_NAME"
-MONGODB_URL = "YOUR_MONGODB_URL"
-MONGO_DB_NAME_FROM = "YOUR_MONGODB_NAME"
+from navalmartin_mir_db_utils.crud.mongodb_crud_utils import ReadEntityCRUDAPI
+
+IMAGES_COLLECTION_TO_READ = 'YOUR_COLLECTION_NAME'
 
 
 async def query_db(mongodb_session: MongoDBSession, criteria: dict,
                    projection: dict,
                    collection_name: str):
-    query_result = ReadEntityCRUDAPI.find(criteria=criteria, projection=projection,
-                                          db_session=mongodb_session,
-                                          collection_name=collection_name)
-    docs = [doc async for doc in query_result]
-    return docs
+    query_result = ReadEntityCRUDAPI.do_find(criteria=criteria, projection=projection,
+                                             db_session=mongodb_session,
+                                             collection_name=collection_name)
+    images = [img async for img in query_result]
+    return images
 
 
 async def count_docs(mongodb_session: MongoDBSession, criteria: dict,
                      collection_name: str):
     query_result = await ReadEntityCRUDAPI.count_documents(criteria=criteria,
                                                            db_session=mongodb_session,
                                                            collection_name=collection_name)
     return query_result
 
 
-async def query_db_or_raise(mongodb_session: MongoDBSession, criteria: dict,
-                            projection: dict,
-                            collection_name: str):
-    query_result = await get_one_result_or_raise(crud_handler=ReadEntityCRUDAPI(collection_name=collection_name),
-                                                 projection=projection,
-                                                 criteria=criteria,
-                                                 db_session=mongodb_session)
-
-    return query_result
-
-
-async def run_examples(mir_db_session_from: MongoDBSession):
-    result = await query_db(mongodb_session=mir_db_session_from,
-                            criteria={'_id': bson.ObjectId('63ebc9f94c092a48bd179ae7')},
-                            projection={},
-                            collection_name=COLLECTION_NAME)
-    print(result)
-    n_docs = await count_docs(mongodb_session=mir_db_session_from,
-                              criteria={},
-                              collection_name=COLLECTION_NAME)
-    print(n_docs)
-
-    try:
-        result = await query_db_or_raise(mongodb_session=mir_db_session_from,
-                                         criteria={'survey_idx': bson.ObjectId('63ad64252c853ee163fc6a63')},
-                                         projection={'original_filename': 1},
-                                         collection_name=COLLECTION_NAME)
-    except ResourceNotFoundException as e:
-        print(str(e))
-
-
 def main():
+    MONGODB_URL = "YOUR_MONGODB_URL"
+    MONGO_DB_NAME_FROM = "YOUR_MONGODB_NAME"
     mir_db_session_from = MongoDBSession(mongodb_url=MONGODB_URL,
                                          db_name=MONGO_DB_NAME_FROM)
 
-    asyncio.run(run_examples(mir_db_session_from=mir_db_session_from))
+    result = asyncio.run(query_db(mongodb_session=mir_db_session_from,
+                                  criteria={'survey_idx': bson.ObjectId('63ad64252c853ee163fc6a63')},
+                                  projection={'original_filename': 1},
+                                  collection_name=IMAGES_COLLECTION_TO_READ))
+    print(result)
+
+    # count how many images the survey has
+    n_docs = asyncio.run(count_docs(mongodb_session=mir_db_session_from,
+                                    criteria={'survey_idx': bson.ObjectId('63ad64252c853ee163fc6a63')},
+                                    collection_name=IMAGES_COLLECTION_TO_READ))
+    print(n_docs)
+
 
-    
 if __name__ == '__main__':
     main()
```

### Comparing `navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/examples/use_transaction.py` & `navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/examples/use_transaction.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/transanctions/decorators.py` & `navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/transanctions/decorators.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/src/navalmartin_mir_db_utils/transanctions/mongodb_transactions.py` & `navalmartin_mir_db_utils-0.0.9/src/navalmartin_mir_db_utils/transanctions/mongodb_transactions.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/.gitignore` & `navalmartin_mir_db_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/LICENSE` & `navalmartin_mir_db_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_db_utils-0.0.35/pyproject.toml` & `navalmartin_mir_db_utils-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["hatchling", "pymongo", "motor", "bcrypt", "httpx", "pydantic", "pydantic[email]", "hurry.filesize", "python-dotenv", "psutil"]
+requires = ["hatchling", "pymongo", "motor"]
 build-backend = "hatchling.build"
 [project]
 name = "navalmartin_mir_db_utils"
-version = "0.0.35"
+version = "0.0.9"
 authors = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" },
 ]
 maintainers = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" }
 ]
 description = "Persistence layer utilities for mir project"
```

