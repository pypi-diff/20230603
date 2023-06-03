# Comparing `tmp/e6data-python-connector-1.0.7.tar.gz` & `tmp/e6data-python-connector-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-1.0.7.tar", last modified: Tue May 30 07:52:31 2023, max compression
+gzip compressed data, was "e6data-python-connector-1.0.8.tar", last modified: Sat Jun  3 06:39:52 2023, max compression
```

## Comparing `e6data-python-connector-1.0.7.tar` & `e6data-python-connector-1.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.152654 e6data-python-connector-1.0.7/
--rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/LICENSE
--rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/MANIFEST.in
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-30 07:52:31.153050 e6data-python-connector-1.0.7/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-05-30 06:22:51.000000 e6data-python-connector-1.0.7/README.md
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.098571 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/top_level.txt
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.118765 e6data-python-connector-1.0.7/e6xdb/
--rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/common.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/datainputstream.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/date_time_utils.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    18483 2023-05-30 07:49:42.000000 e6data-python-connector-1.0.7/e6xdb/e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/exceptions.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.150871 e6data-python-connector-1.0.7/e6xdb/server/
--rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.7/e6xdb/server/QueryEngineService.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/server/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/server/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.7/e6xdb/server/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/sqlalchemy_e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/typeId.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/pyproject.toml
--rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-05-30 07:52:31.156686 e6data-python-connector-1.0.7/setup.cfg
--rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-05-30 06:22:52.000000 e6data-python-connector-1.0.7/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.539787 e6data-python-connector-1.0.8/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-06-03 06:39:52.540313 e6data-python-connector-1.0.8/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-06-03 05:39:57.000000 e6data-python-connector-1.0.8/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.419907 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/top_level.txt
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.519562 e6data-python-connector-1.0.8/e6xdb/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    17377 2023-06-03 05:40:26.000000 e6data-python-connector-1.0.8/e6xdb/e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/exceptions.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.538623 e6data-python-connector-1.0.8/e6xdb/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.8/e6xdb/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.8/e6xdb/server/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/sqlalchemy_e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/typeId.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-06-03 06:39:52.544712 e6data-python-connector-1.0.8/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-06-03 05:39:57.000000 e6data-python-connector-1.0.8/setup.py
```

### Comparing `e6data-python-connector-1.0.7/LICENSE` & `e6data-python-connector-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/PKG-INFO` & `e6data-python-connector-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.7
+Version: 1.0.8
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
```

### Comparing `e6data-python-connector-1.0.7/README.md` & `e6data-python-connector-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 To install the Python package, use the command below:
 ```shell
```

### Comparing `e6data-python-connector-1.0.7/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-1.0.8/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.7
+Version: 1.0.8
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
```

### Comparing `e6data-python-connector-1.0.7/e6data_python_connector.egg-info/SOURCES.txt` & `e6data-python-connector-1.0.8/e6data_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/common.py` & `e6data-python-connector-1.0.8/e6xdb/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/constants.py` & `e6data-python-connector-1.0.8/e6xdb/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/datainputstream.py` & `e6data-python-connector-1.0.8/e6xdb/datainputstream.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/date_time_utils.py` & `e6data-python-connector-1.0.8/e6xdb/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/e6x.py` & `e6data-python-connector-1.0.8/e6xdb/e6x.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,14 +361,15 @@
     def execute(self, operation, parameters=None, **kwargs):
         """Prepare and execute a database operation (query or command).
         Return values are not defined.
         """
         """
         Semicolon is now not supported. So removing it from query end.
         """
+        operation = operation.strip()
         if operation.endswith(';'):
             operation = operation[:-1]
 
         # Prepare statement
         if parameters is None:
             sql = operation
         else:
@@ -512,49 +513,7 @@
 #
 # Type Objects and Constructors
 #
 
 for type_id in PRIMITIVE_TYPES:
     name = TypeId._VALUES_TO_NAMES[type_id]
     setattr(sys.modules[__name__], name, DBAPITypeObject([name]))
-
-
-if __name__ == '__main__':
-    ip = '54.205.255.188'
-    conn = Connection(
-        host=ip,
-        username='admin',
-        password='admin',
-        port=9000
-    )
-    catalogs = {'catalogs': [{
-        "type": 'HIVE',
-        "name": 'hive',
-        "hive_ip": '18.233.112.169',
-        "hive_port": 9084,
-        "included_schemas": [],
-        "excluded_schemas": [],
-        "included_tables": [],
-        "excluded_tables": [],
-        "included_columns": [],
-        "excluded_columns": [],
-        "is_assumed_role": False,
-        "assumed_role_arn": '',
-        "default": True
-    }]}
-    import json
-    import time
-    start = time.time()
-    # print(conn.add_catalogs(json.dumps(catalogs)))
-    add_cat_time = time.time()
-    print('Add catalog time', add_cat_time - start)
-    status = 'in_progress'
-    res = conn.get_add_catalog_response()
-    print(res)
-    print(res.failures[0].reason)
-    # while status == 'in_progress':
-    #     res = conn.get_add_catalog_response()
-    #     status = res.status
-    #     print(res)
-    #     time.sleep(5)
-    print('get_add_catalog_response time', time.time() - add_cat_time)
-
```

### Comparing `e6data-python-connector-1.0.7/e6xdb/server/QueryEngineService.py` & `e6data-python-connector-1.0.8/e6xdb/server/QueryEngineService.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/server/ttypes.py` & `e6data-python-connector-1.0.8/e6xdb/server/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/sqlalchemy_e6x.py` & `e6data-python-connector-1.0.8/e6xdb/sqlalchemy_e6x.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/e6xdb/typeId.py` & `e6data-python-connector-1.0.8/e6xdb/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.7/setup.py` & `e6data-python-connector-1.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import os
 
 import setuptools
 
 envstring = lambda var: os.environ.get(var) or ""
 
-VERSION = [1, 0, 7]
+VERSION = [1, 0, 8]
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
```

