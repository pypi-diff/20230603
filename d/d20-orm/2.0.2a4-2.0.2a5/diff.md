# Comparing `tmp/d20-orm-2.0.2a4.tar.gz` & `tmp/d20-orm-2.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-emxb7894\d20-orm-2.0.2a4.tar", last modified: Sat Jun  3 00:12:06 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-g7d_9fpg\d20-orm-2.0.2a5.tar", last modified: Sat Jun  3 00:25:00 2023, max compression
```

## Comparing `d20-orm-2.0.2a4.tar` & `d20-orm-2.0.2a5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.421131 d20-orm-2.0.2a4/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a4/LICENSE
--rw-rw-rw-   0        0        0      895 2023-06-03 00:12:06.422109 d20-orm-2.0.2a4/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a4/pyproject.toml
--rw-rw-rw-   0        0        0       72 2023-06-03 00:12:06.428109 d20-orm-2.0.2a4/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-03 00:11:38.000000 d20-orm-2.0.2a4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:12:05.954481 d20-orm-2.0.2a4/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.081567 d20-orm-2.0.2a4/src/d20_orm.egg-info/
--rw-rw-rw-   0        0        0      895 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 00:12:05.000000 d20-orm-2.0.2a4/src/d20_orm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.318710 d20-orm-2.0.2a4/src/dtwentyORM/
--rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.2a4/src/dtwentyORM/BasicElement.py
--rw-rw-rw-   0        0        0     7352 2023-06-02 00:08:14.000000 d20-orm-2.0.2a4/src/dtwentyORM/DBConnector.py
--rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a4/src/dtwentyORM/Element.py
--rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a4/src/dtwentyORM/Error.py
--rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a4/src/dtwentyORM/GraphClassFactory.py
--rw-rw-rw-   0        0        0     8120 2023-06-03 00:11:29.000000 d20-orm-2.0.2a4/src/dtwentyORM/Metadata.py
--rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a4/src/dtwentyORM/__init__.py
--rw-rw-rw-   0        0        0      161 2023-06-03 00:11:42.000000 d20-orm-2.0.2a4/src/dtwentyORM/__version__.py
--rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a4/src/dtwentyORM/support.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:12:06.420126 d20-orm-2.0.2a4/test/
--rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_basic_element_test.py
--rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_build_db.py
--rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_crud_collection.py
--rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a4/test/test_metadata.py
--rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a4/test/test_params.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:25:00.612048 d20-orm-2.0.2a5/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a5/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:25:00.613058 d20-orm-2.0.2a5/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a5/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a5/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-06-03 00:25:00.620043 d20-orm-2.0.2a5/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-06-03 00:24:42.000000 d20-orm-2.0.2a5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:25:00.486192 d20-orm-2.0.2a5/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 00:25:00.521733 d20-orm-2.0.2a5/src/d20_orm.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:25:00.000000 d20-orm-2.0.2a5/src/d20_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-06-03 00:25:00.000000 d20-orm-2.0.2a5/src/d20_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 00:25:00.000000 d20-orm-2.0.2a5/src/d20_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-03 00:25:00.000000 d20-orm-2.0.2a5/src/d20_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 00:25:00.000000 d20-orm-2.0.2a5/src/d20_orm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 00:25:00.604965 d20-orm-2.0.2a5/src/dtwentyORM/
+-rw-rw-rw-   0        0        0     8913 2023-06-03 00:24:29.000000 d20-orm-2.0.2a5/src/dtwentyORM/BasicElement.py
+-rw-rw-rw-   0        0        0     7352 2023-06-02 00:08:14.000000 d20-orm-2.0.2a5/src/dtwentyORM/DBConnector.py
+-rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a5/src/dtwentyORM/Element.py
+-rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a5/src/dtwentyORM/Error.py
+-rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a5/src/dtwentyORM/GraphClassFactory.py
+-rw-rw-rw-   0        0        0     8120 2023-06-03 00:11:29.000000 d20-orm-2.0.2a5/src/dtwentyORM/Metadata.py
+-rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a5/src/dtwentyORM/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-06-03 00:24:38.000000 d20-orm-2.0.2a5/src/dtwentyORM/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a5/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:25:00.611043 d20-orm-2.0.2a5/test/
+-rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a5/test/test_basic_element_test.py
+-rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a5/test/test_build_db.py
+-rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a5/test/test_crud_collection.py
+-rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a5/test/test_metadata.py
+-rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a5/test/test_params.py
```

### Comparing `d20-orm-2.0.2a4/LICENSE` & `d20-orm-2.0.2a5/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/PKG-INFO` & `d20-orm-2.0.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a4
+Version: 2.0.2a5
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a4/setup.py` & `d20-orm-2.0.2a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-orm",
-    version="2.0.2a4",
+    version="2.0.2a5",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/arangodb_python_orm",
     project_urls={
```

### Comparing `d20-orm-2.0.2a4/src/d20_orm.egg-info/PKG-INFO` & `d20-orm-2.0.2a5/src/d20_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a4
+Version: 2.0.2a5
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a4/src/d20_orm.egg-info/SOURCES.txt` & `d20-orm-2.0.2a5/src/d20_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/BasicElement.py` & `d20-orm-2.0.2a5/src/dtwentyORM/BasicElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,18 @@
             self.set_from_dict(data)
         self.set_edges()
         self.id = id
 
     # V2
     def load(self, id, get_if_deleted=False):
         self.id= id
-        self.load(get_if_deleted=get_if_deleted)
+        self._load(get_if_deleted=get_if_deleted)
 
     # V2
-    def load(self, get_if_deleted=False):
+    def _load(self, get_if_deleted=False):
         record = self.get_one(self.id, return_deleted=get_if_deleted)
         if record['deleted'] == True and get_if_deleted==False:
             raise ObjectNotFoundException
         self.set(record)
 
     # V2
     def set_edges(self, data=None):
```

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/DBConnector.py` & `d20-orm-2.0.2a5/src/dtwentyORM/DBConnector.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/Element.py` & `d20-orm-2.0.2a5/src/dtwentyORM/Element.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/Error.py` & `d20-orm-2.0.2a5/src/dtwentyORM/Error.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/GraphClassFactory.py` & `d20-orm-2.0.2a5/src/dtwentyORM/GraphClassFactory.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/Metadata.py` & `d20-orm-2.0.2a5/src/dtwentyORM/Metadata.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/src/dtwentyORM/support.py` & `d20-orm-2.0.2a5/src/dtwentyORM/support.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a4/test/test_build_db.py` & `d20-orm-2.0.2a5/test/test_build_db.py`

 * *Files identical despite different names*

