# Comparing `tmp/d20-orm-2.0.2a2.tar.gz` & `tmp/d20-orm-2.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-0oy7kqys\d20-orm-2.0.2a2.tar", last modified: Thu Jun  1 03:03:43 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-emxb7894\d20-orm-2.0.2a4.tar", last modified: Sat Jun  3 00:12:06 2023, max compression
```

## Comparing `d20-orm-2.0.2a2.tar` & `d20-orm-2.0.2a4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:43.953889 d20-orm-2.0.2a2/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a2/LICENSE
--rw-rw-rw-   0        0        0      895 2023-06-01 03:03:43.953889 d20-orm-2.0.2a2/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a2/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a2/pyproject.toml
--rw-rw-rw-   0        0        0       72 2023-06-01 03:03:43.960401 d20-orm-2.0.2a2/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-01 03:03:01.000000 d20-orm-2.0.2a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:43.784908 d20-orm-2.0.2a2/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:43.922758 d20-orm-2.0.2a2/src/d20_orm.egg-info/
--rw-rw-rw-   0        0        0      895 2023-06-01 03:03:43.000000 d20-orm-2.0.2a2/src/d20_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-06-01 03:03:43.000000 d20-orm-2.0.2a2/src/d20_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:03:43.000000 d20-orm-2.0.2a2/src/d20_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 03:03:43.000000 d20-orm-2.0.2a2/src/d20_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 03:03:43.000000 d20-orm-2.0.2a2/src/d20_orm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:43.945666 d20-orm-2.0.2a2/src/dtwentyORM/
--rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.2a2/src/dtwentyORM/BasicElement.py
--rw-rw-rw-   0        0        0     7213 2023-05-27 00:02:43.000000 d20-orm-2.0.2a2/src/dtwentyORM/DBConnector.py
--rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a2/src/dtwentyORM/Element.py
--rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a2/src/dtwentyORM/Error.py
--rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a2/src/dtwentyORM/GraphClassFactory.py
--rw-rw-rw-   0        0        0     5156 2023-06-01 03:02:50.000000 d20-orm-2.0.2a2/src/dtwentyORM/Metadata.py
--rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a2/src/dtwentyORM/__init__.py
--rw-rw-rw-   0        0        0      161 2023-02-28 02:21:55.000000 d20-orm-2.0.2a2/src/dtwentyORM/__version__.py
--rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a2/src/dtwentyORM/support.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:43.952890 d20-orm-2.0.2a2/test/
--rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a2/test/test_basic_element_test.py
--rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a2/test/test_build_db.py
--rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a2/test/test_crud_collection.py
--rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a2/test/test_metadata.py
--rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a2/test/test_params.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.421131 d20-orm-2.0.2a4/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a4/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:12:06.422109 d20-orm-2.0.2a4/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a4/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-06-03 00:12:06.428109 d20-orm-2.0.2a4/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-06-03 00:11:38.000000 d20-orm-2.0.2a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:12:05.954481 d20-orm-2.0.2a4/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.081567 d20-orm-2.0.2a4/src/d20_orm.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.318710 d20-orm-2.0.2a4/src/dtwentyORM/
+-rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.2a4/src/dtwentyORM/BasicElement.py
+-rw-rw-rw-   0        0        0     7352 2023-06-02 00:08:14.000000 d20-orm-2.0.2a4/src/dtwentyORM/DBConnector.py
+-rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a4/src/dtwentyORM/Element.py
+-rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a4/src/dtwentyORM/Error.py
+-rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a4/src/dtwentyORM/GraphClassFactory.py
+-rw-rw-rw-   0        0        0     8120 2023-06-03 00:11:29.000000 d20-orm-2.0.2a4/src/dtwentyORM/Metadata.py
+-rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a4/src/dtwentyORM/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-06-03 00:11:42.000000 d20-orm-2.0.2a4/src/dtwentyORM/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a4/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.420126 d20-orm-2.0.2a4/test/
+-rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_basic_element_test.py
+-rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_build_db.py
+-rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_crud_collection.py
+-rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_metadata.py
+-rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a4/test/test_params.py
```

### Comparing `d20-orm-2.0.2a2/LICENSE` & `d20-orm-2.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/PKG-INFO` & `d20-orm-2.0.2a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a2
+Version: 2.0.2a4
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a2/setup.py` & `d20-orm-2.0.2a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-orm",
-    version="2.0.2a2",
+    version="2.0.2a4",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/arangodb_python_orm",
     project_urls={
```

### Comparing `d20-orm-2.0.2a2/src/d20_orm.egg-info/PKG-INFO` & `d20-orm-2.0.2a4/src/d20_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a2
+Version: 2.0.2a4
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a2/src/d20_orm.egg-info/SOURCES.txt` & `d20-orm-2.0.2a4/src/d20_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/BasicElement.py` & `d20-orm-2.0.2a4/src/dtwentyORM/BasicElement.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/DBConnector.py` & `d20-orm-2.0.2a4/src/dtwentyORM/DBConnector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyArango.connection import *
+from pyArango.theExceptions import *
 from .Error import *
 import os
 import json
 import re
 
 class DBConnector():
 
@@ -117,15 +118,18 @@
         re_string = re.sub("[ýÿ]", 'y', re_string)
         if line_end == True:
             re_string = re_string + '$'
         return re_string
 
 
     def get_one(self, id, rawResults = True):
-        found = self.collection.fetchDocument(id, rawResults = rawResults)
+        try:
+            found = self.collection.fetchDocument(id, rawResults = rawResults)
+        except DocumentNotFoundError as e:
+            raise ObjectNotFoundException
         return found
 
     def update_one(self, id, data):
         # Document Object from PyArango
         document = self.get_one(id, rawResults = False)
         before_rev = document['_rev']
         data.pop('_key', None)
```

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/Element.py` & `d20-orm-2.0.2a4/src/dtwentyORM/Element.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/Error.py` & `d20-orm-2.0.2a4/src/dtwentyORM/Error.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/GraphClassFactory.py` & `d20-orm-2.0.2a4/src/dtwentyORM/GraphClassFactory.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/src/dtwentyORM/support.py` & `d20-orm-2.0.2a4/src/dtwentyORM/support.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a2/test/test_build_db.py` & `d20-orm-2.0.2a4/test/test_build_db.py`

 * *Files identical despite different names*

