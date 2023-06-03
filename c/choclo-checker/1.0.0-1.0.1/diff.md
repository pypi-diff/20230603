# Comparing `tmp/choclo-checker-1.0.0.tar.gz` & `tmp/choclo-checker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\choclo-checker-1.0.0.tar", last modified: Sat Jun  3 03:45:37 2023, max compression
+gzip compressed data, was "dist\choclo-checker-1.0.1.tar", last modified: Sat Jun  3 05:53:36 2023, max compression
```

## Comparing `choclo-checker-1.0.0.tar` & `choclo-checker-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.951630 choclo-checker-1.0.0/
--rw-rw-rw-   0        0        0      260 2023-06-03 03:45:37.947645 choclo-checker-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-06-02 02:21:48.000000 choclo-checker-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.194690 choclo-checker-1.0.0/choclo_checker/
--rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.0/choclo_checker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.399110 choclo-checker-1.0.0/choclo_checker/api/
--rw-rw-rw-   0        0        0        0 2023-06-02 02:21:47.000000 choclo-checker-1.0.0/choclo_checker/api/__init__.py
--rw-rw-rw-   0        0        0     1278 2023-06-02 03:22:51.000000 choclo-checker-1.0.0/choclo_checker/api/choclocheck_graphql.py
--rw-rw-rw-   0        0        0     1265 2023-06-02 03:22:21.000000 choclo-checker-1.0.0/choclo_checker/api/choclocheck_rest.py
--rw-rw-rw-   0        0        0     1486 2023-06-02 03:22:27.000000 choclo-checker-1.0.0/choclo_checker/api/choclocheck_soap.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.846909 choclo-checker-1.0.0/choclo_checker/db/
--rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.0/choclo_checker/db/__init__.py
--rw-rw-rw-   0        0        0     2103 2023-06-02 03:17:15.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_dynamodb.py
--rw-rw-rw-   0        0        0     2396 2023-06-02 03:18:12.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_elasticsearch.py
--rw-rw-rw-   0        0        0     4022 2023-06-02 03:12:46.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_influx.py
--rw-rw-rw-   0        0        0     6497 2023-06-02 03:09:47.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_mongodb.py
--rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_mysql.py
--rw-rw-rw-   0        0        0     4561 2023-06-02 03:13:38.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_oracle.py
--rw-rw-rw-   0        0        0     4245 2023-06-02 03:15:56.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_postgres.py
--rw-rw-rw-   0        0        0     4925 2023-06-02 03:11:35.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_redis.py
--rw-rw-rw-   0        0        0     3149 2023-06-02 03:17:01.000000 choclo-checker-1.0.0/choclo_checker/db/choclocheck_sql.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.936679 choclo-checker-1.0.0/choclo_checker/networking/
--rw-rw-rw-   0        0        0        0 2023-06-02 02:21:47.000000 choclo-checker-1.0.0/choclo_checker/networking/__init__.py
--rw-rw-rw-   0        0        0     1812 2023-06-02 03:24:22.000000 choclo-checker-1.0.0/choclo_checker/networking/choclocheck_ping.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:45:37.247518 choclo-checker-1.0.0/choclo_checker.egg-info/
--rw-rw-rw-   0        0        0      260 2023-06-03 03:45:36.000000 choclo-checker-1.0.0/choclo_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-06-03 03:45:36.000000 choclo-checker-1.0.0/choclo_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 03:45:36.000000 choclo-checker-1.0.0/choclo_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-03 03:45:36.000000 choclo-checker-1.0.0/choclo_checker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-03 03:45:36.000000 choclo-checker-1.0.0/choclo_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 03:45:37.953625 choclo-checker-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-06-03 03:45:13.000000 choclo-checker-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.573866 choclo-checker-1.0.1/
+-rw-rw-rw-   0        0        0      260 2023-06-03 05:53:36.549935 choclo-checker-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-06-02 02:21:48.000000 choclo-checker-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.195880 choclo-checker-1.0.1/choclo_checker/
+-rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.1/choclo_checker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.301594 choclo-checker-1.0.1/choclo_checker/api/
+-rw-rw-rw-   0        0        0        0 2023-06-02 02:21:47.000000 choclo-checker-1.0.1/choclo_checker/api/__init__.py
+-rw-rw-rw-   0        0        0     1278 2023-06-02 03:22:51.000000 choclo-checker-1.0.1/choclo_checker/api/choclocheck_graphql.py
+-rw-rw-rw-   0        0        0     1265 2023-06-02 03:22:21.000000 choclo-checker-1.0.1/choclo_checker/api/choclocheck_rest.py
+-rw-rw-rw-   0        0        0     1486 2023-06-02 03:22:27.000000 choclo-checker-1.0.1/choclo_checker/api/choclocheck_soap.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.447203 choclo-checker-1.0.1/choclo_checker/db/
+-rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.1/choclo_checker/db/__init__.py
+-rw-rw-rw-   0        0        0     2103 2023-06-02 03:17:15.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_dynamodb.py
+-rw-rw-rw-   0        0        0     2396 2023-06-02 03:18:12.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_elasticsearch.py
+-rw-rw-rw-   0        0        0     4022 2023-06-02 03:12:46.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_influx.py
+-rw-rw-rw-   0        0        0     6528 2023-06-03 05:48:48.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_mongodb.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 02:21:45.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_mysql.py
+-rw-rw-rw-   0        0        0     4561 2023-06-02 03:13:38.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_oracle.py
+-rw-rw-rw-   0        0        0     4245 2023-06-02 03:15:56.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_postgres.py
+-rw-rw-rw-   0        0        0     4925 2023-06-02 03:11:35.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_redis.py
+-rw-rw-rw-   0        0        0     3149 2023-06-02 03:17:01.000000 choclo-checker-1.0.1/choclo_checker/db/choclocheck_sql.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.519010 choclo-checker-1.0.1/choclo_checker/networking/
+-rw-rw-rw-   0        0        0        0 2023-06-02 02:21:47.000000 choclo-checker-1.0.1/choclo_checker/networking/__init__.py
+-rw-rw-rw-   0        0        0     1812 2023-06-02 03:24:22.000000 choclo-checker-1.0.1/choclo_checker/networking/choclocheck_ping.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:53:36.257719 choclo-checker-1.0.1/choclo_checker.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-06-03 05:53:35.000000 choclo-checker-1.0.1/choclo_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-06-03 05:53:36.000000 choclo-checker-1.0.1/choclo_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:53:35.000000 choclo-checker-1.0.1/choclo_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-03 05:53:35.000000 choclo-checker-1.0.1/choclo_checker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-03 05:53:35.000000 choclo-checker-1.0.1/choclo_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:53:36.574863 choclo-checker-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-03 05:52:54.000000 choclo-checker-1.0.1/setup.py
```

### Comparing `choclo-checker-1.0.0/README.md` & `choclo-checker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/api/choclocheck_graphql.py` & `choclo-checker-1.0.1/choclo_checker/api/choclocheck_graphql.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/api/choclocheck_rest.py` & `choclo-checker-1.0.1/choclo_checker/api/choclocheck_rest.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/api/choclocheck_soap.py` & `choclo-checker-1.0.1/choclo_checker/api/choclocheck_soap.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_dynamodb.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_dynamodb.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_elasticsearch.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_influx.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_influx.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_mongodb.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 ChocloChecker MongoDB Module
 
 This module contains the functions for monitoring the status of MongoDB databases.
 """
 
 import pymongo
-
+from pymongo.errors import ConnectionFailure
 def check_connection(host, port):
     """
     Check the connection to the MongoDB server.
 
     Args:
         host (str): The host address of the MongoDB server.
         port (int): The port number of the MongoDB server.
@@ -17,15 +17,15 @@
     Returns:
         bool: True if the connection is successful, False otherwise.
     """
     try:
         client = pymongo.MongoClient(host, port)
         client.admin.command('ping')
         return True
-    except pymongo.errors.ConnectionError:
+    except ConnectionFailure:
         return False
 
 def check_status(host, port):
     """
     Check the status of the MongoDB database.
 
     Args:
```

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_oracle.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_oracle.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_postgres.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_postgres.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_redis.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_redis.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/db/choclocheck_sql.py` & `choclo-checker-1.0.1/choclo_checker/db/choclocheck_sql.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker/networking/choclocheck_ping.py` & `choclo-checker-1.0.1/choclo_checker/networking/choclocheck_ping.py`

 * *Files identical despite different names*

### Comparing `choclo-checker-1.0.0/choclo_checker.egg-info/SOURCES.txt` & `choclo-checker-1.0.1/choclo_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

