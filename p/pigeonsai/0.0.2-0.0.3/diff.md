# Comparing `tmp/pigeonsai-0.0.2.tar.gz` & `tmp/pigeonsai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.2.tar", last modified: Sat Jun  3 00:04:32 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.3.tar", last modified: Sat Jun  3 00:16:04 2023, max compression
```

## Comparing `pigeonsai-0.0.2.tar` & `pigeonsai-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:04:32.678544 pigeonsai-0.0.2/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:04:32.678409 pigeonsai-0.0.2/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:01:12.000000 pigeonsai-0.0.2/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-03 00:04:32.678588 pigeonsai-0.0.2/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-03 00:00:44.000000 pigeonsai-0.0.2/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:04:32.676293 pigeonsai-0.0.2/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:04:32.677138 pigeonsai-0.0.2/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.2/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     2502 2023-06-03 00:01:21.000000 pigeonsai-0.0.2/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:04:32.678033 pigeonsai-0.0.2/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:04:32.000000 pigeonsai-0.0.2/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-03 00:04:32.000000 pigeonsai-0.0.2/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-03 00:04:32.000000 pigeonsai-0.0.2/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-03 00:04:32.000000 pigeonsai-0.0.2/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-03 00:04:32.000000 pigeonsai-0.0.2/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:04:32.678151 pigeonsai-0.0.2/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.2/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799834 pigeonsai-0.0.3/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:16:04.799669 pigeonsai-0.0.3/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.3/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-03 00:16:04.799885 pigeonsai-0.0.3/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-03 00:15:54.000000 pigeonsai-0.0.3/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.797424 pigeonsai-0.0.3/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.798289 pigeonsai-0.0.3/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.3/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2465 2023-06-03 00:15:50.000000 pigeonsai-0.0.3/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799105 pigeonsai-0.0.3/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799273 pigeonsai-0.0.3/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.3/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.2/PKG-INFO` & `pigeonsai-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.2
+Version: 0.0.3
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.2/README.md` & `pigeonsai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.2/setup.py` & `pigeonsai-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.2",
+    version="0.0.3",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.2/src/pigeonsai/pigeonsdb.py` & `pigeonsai-0.0.3/src/pigeonsai/pigeonsdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,80 +2,79 @@
 import json
 
 
 
 class PigeonsDB:
 
     __connection = None
-    __index_path = None
+    __index_p = None
 
     @staticmethod
     def search(query_text, k, metadata_filters=None, keywords=None):
         if PigeonsDB.__connection is None:
             print("Error: Connection not initialized.")
             return
 
         url = "http://test-search-1248249294.us-east-2.elb.amazonaws.com:8080/search"
         headers = {"Content-Type": "application/json"}
         data = {
             "connection": PigeonsDB.__connection,
-            "index_path": PigeonsDB.__index_path,
+            "index_path": PigeonsDB.__index_p,
             "query_text": query_text,
             "k": k,
             "metadata_filters": metadata_filters,
             "keywords": keywords
         }
 
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # print the response
         print(response.text)
 
     @staticmethod
     def init(API, DB_Name):
-        index_path, connection = PigeonsDB.get_db_info(API, DB_Name)
-        if connection:
-            PigeonsDB.__connection = connection
-            PigeonsDB.__index_path = index_path
+        index_p, connect = PigeonsDB.get_db_info(API, DB_Name)
+        if connect:
+            PigeonsDB.__connection = connect
+            PigeonsDB.__index_p = index_p
         else:
             print("API key or DB name not found")
 
     @staticmethod
     def get_db_info(api_key, db_name):
         url = "http://ec2-52-14-162-65.us-east-2.compute.amazonaws.com/api/v1/sdk/get-db-info"
         headers = {"Content-Type": "application/json"}
         data = {"api_key": api_key, "dbname": db_name}
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # Extract data from the response
         db_info = response.json().get('DB info', {})
-        index_path = db_info.get('index_path')
+        index_p = db_info.get('s3_identifier')
 
         # Create db object with specific keys
         keys = ['dbname', 'user', 'password', 'host']
-        connection = {key: db_info.get(key) for key in keys}
+        connect = {key: db_info.get(key) for key in keys}
 
-        return index_path, connection
+        return index_p, connect
 
 
     @staticmethod
     def add(documents, metadata_list):
         if PigeonsDB.__connection is None:
             print("Error: Connection not initialized.")
             return
 
         url = "http://add-dev-177401989.us-east-2.elb.amazonaws.com:8080/add_documents"
         headers = {"Content-Type": "application/json"}
         data = {
             "connection": PigeonsDB.__connection,
-            "index_path": PigeonsDB.__index_path,
+            "index_path": PigeonsDB.__index_p,
             "documents": documents,
             "metadata_list": metadata_list
         }
 
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # print the response
         print(response.text)
 
 
-
```

### Comparing `pigeonsai-0.0.2/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.3/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.2
+Version: 0.0.3
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.2/tests/test_pigeonsdb.py` & `pigeonsai-0.0.3/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

