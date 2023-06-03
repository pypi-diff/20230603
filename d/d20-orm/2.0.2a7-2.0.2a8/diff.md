# Comparing `tmp/d20-orm-2.0.2a7.tar.gz` & `tmp/d20-orm-2.0.2a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-d98xytdp\d20-orm-2.0.2a7.tar", last modified: Sat Jun  3 00:31:35 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-gnztg8tw\d20-orm-2.0.2a8.tar", last modified: Sat Jun  3 00:34:16 2023, max compression
```

## Comparing `d20-orm-2.0.2a7.tar` & `d20-orm-2.0.2a8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 00:31:35.816868 d20-orm-2.0.2a7/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a7/LICENSE
--rw-rw-rw-   0        0        0      895 2023-06-03 00:31:35.817902 d20-orm-2.0.2a7/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a7/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a7/pyproject.toml
--rw-rw-rw-   0        0        0       72 2023-06-03 00:31:35.824853 d20-orm-2.0.2a7/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-03 00:31:22.000000 d20-orm-2.0.2a7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:31:35.720342 d20-orm-2.0.2a7/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 00:31:35.746650 d20-orm-2.0.2a7/src/d20_orm.egg-info/
--rw-rw-rw-   0        0        0      895 2023-06-03 00:31:35.000000 d20-orm-2.0.2a7/src/d20_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-06-03 00:31:35.000000 d20-orm-2.0.2a7/src/d20_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 00:31:35.000000 d20-orm-2.0.2a7/src/d20_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-03 00:31:35.000000 d20-orm-2.0.2a7/src/d20_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 00:31:35.000000 d20-orm-2.0.2a7/src/d20_orm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 00:31:35.810857 d20-orm-2.0.2a7/src/dtwentyORM/
--rw-rw-rw-   0        0        0     8882 2023-06-03 00:28:27.000000 d20-orm-2.0.2a7/src/dtwentyORM/BasicElement.py
--rw-rw-rw-   0        0        0     7352 2023-06-02 00:08:14.000000 d20-orm-2.0.2a7/src/dtwentyORM/DBConnector.py
--rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a7/src/dtwentyORM/Element.py
--rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a7/src/dtwentyORM/Error.py
--rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a7/src/dtwentyORM/GraphClassFactory.py
--rw-rw-rw-   0        0        0     8172 2023-06-03 00:31:12.000000 d20-orm-2.0.2a7/src/dtwentyORM/Metadata.py
--rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a7/src/dtwentyORM/__init__.py
--rw-rw-rw-   0        0        0      161 2023-06-03 00:31:19.000000 d20-orm-2.0.2a7/src/dtwentyORM/__version__.py
--rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a7/src/dtwentyORM/support.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:31:35.815885 d20-orm-2.0.2a7/test/
--rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a7/test/test_basic_element_test.py
--rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a7/test/test_build_db.py
--rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a7/test/test_crud_collection.py
--rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a7/test/test_metadata.py
--rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a7/test/test_params.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:34:16.906448 d20-orm-2.0.2a8/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.2a8/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:34:16.906448 d20-orm-2.0.2a8/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.2a8/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.2a8/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-06-03 00:34:16.917864 d20-orm-2.0.2a8/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-06-03 00:34:03.000000 d20-orm-2.0.2a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:34:16.837923 d20-orm-2.0.2a8/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 00:34:16.868448 d20-orm-2.0.2a8/src/d20_orm.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-06-03 00:34:16.000000 d20-orm-2.0.2a8/src/d20_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-06-03 00:34:16.000000 d20-orm-2.0.2a8/src/d20_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 00:34:16.000000 d20-orm-2.0.2a8/src/d20_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-03 00:34:16.000000 d20-orm-2.0.2a8/src/d20_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 00:34:16.000000 d20-orm-2.0.2a8/src/d20_orm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 00:34:16.897451 d20-orm-2.0.2a8/src/dtwentyORM/
+-rw-rw-rw-   0        0        0     8882 2023-06-03 00:28:27.000000 d20-orm-2.0.2a8/src/dtwentyORM/BasicElement.py
+-rw-rw-rw-   0        0        0     7352 2023-06-02 00:08:14.000000 d20-orm-2.0.2a8/src/dtwentyORM/DBConnector.py
+-rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.2a8/src/dtwentyORM/Element.py
+-rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.2a8/src/dtwentyORM/Error.py
+-rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.2a8/src/dtwentyORM/GraphClassFactory.py
+-rw-rw-rw-   0        0        0     8166 2023-06-03 00:33:55.000000 d20-orm-2.0.2a8/src/dtwentyORM/Metadata.py
+-rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.2a8/src/dtwentyORM/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-06-03 00:34:00.000000 d20-orm-2.0.2a8/src/dtwentyORM/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.2a8/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:34:16.905459 d20-orm-2.0.2a8/test/
+-rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.2a8/test/test_basic_element_test.py
+-rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.2a8/test/test_build_db.py
+-rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.2a8/test/test_crud_collection.py
+-rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.2a8/test/test_metadata.py
+-rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.2a8/test/test_params.py
```

### Comparing `d20-orm-2.0.2a7/LICENSE` & `d20-orm-2.0.2a8/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/PKG-INFO` & `d20-orm-2.0.2a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a7
+Version: 2.0.2a8
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a7/setup.py` & `d20-orm-2.0.2a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-orm",
-    version="2.0.2a7",
+    version="2.0.2a8",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/arangodb_python_orm",
     project_urls={
```

### Comparing `d20-orm-2.0.2a7/src/d20_orm.egg-info/PKG-INFO` & `d20-orm-2.0.2a8/src/d20_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.2a7
+Version: 2.0.2a8
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.2a7/src/d20_orm.egg-info/SOURCES.txt` & `d20-orm-2.0.2a8/src/d20_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/BasicElement.py` & `d20-orm-2.0.2a8/src/dtwentyORM/BasicElement.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/DBConnector.py` & `d20-orm-2.0.2a8/src/dtwentyORM/DBConnector.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/Element.py` & `d20-orm-2.0.2a8/src/dtwentyORM/Element.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/Error.py` & `d20-orm-2.0.2a8/src/dtwentyORM/Error.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/GraphClassFactory.py` & `d20-orm-2.0.2a8/src/dtwentyORM/GraphClassFactory.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/Metadata.py` & `d20-orm-2.0.2a8/src/dtwentyORM/Metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 setattr(self, key, None)
 
 
         def install(self):
             self.get_all()
             for res in self.found:
                 res.wipe()
-            with open(os.path.join("./datafield.json"), mode='r', encoding='utf-8') as infile:
+            with open(os.path.join("datafield.json"), mode='r', encoding='utf-8') as infile:
                 cts = infile.read()
                 dfs = json.loads(cts)
                 for df in dfs:
                     to_insert = {}
                     to_insert['date_created']= datetime.datetime.utcnow()
                     to_insert['date_updated'] = datetime.datetime.utcnow()
                     to_insert['deleted'] = False
@@ -134,15 +134,15 @@
                 setattr(self, key, None)
 
 
         def install(self):
             self.get_all()
             for res in self.found:
                 res.wipe()
-            with open(os.path.join("./parameters.json"), mode='r', encoding='utf-8') as infile:
+            with open(os.path.join("parameters.json"), mode='r', encoding='utf-8') as infile:
                 cts = infile.read()
                 dfs = json.loads(cts)
                 for df in dfs:
                     to_insert = {}
                     to_insert['date_created']= datetime.datetime.utcnow()
                     to_insert['date_updated'] = datetime.datetime.utcnow()
                     to_insert['deleted'] = False
@@ -196,15 +196,15 @@
                 setattr(self, key, None)
 
 
         def install(self):
             self.get_all()
             for res in self.found:
                 res.wipe()
-            with open(os.path.join("./ountries.json"), mode='r', encoding='utf-8') as infile:
+            with open(os.path.join("ountries.json"), mode='r', encoding='utf-8') as infile:
                 cts = infile.read()
                 dfs = json.loads(cts)
                 for df in dfs:
                     to_insert = {}
                     to_insert['date_created']= datetime.datetime.utcnow()
                     to_insert['date_updated'] = datetime.datetime.utcnow()
                     to_insert['deleted'] = False
```

### Comparing `d20-orm-2.0.2a7/src/dtwentyORM/support.py` & `d20-orm-2.0.2a8/src/dtwentyORM/support.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.2a7/test/test_build_db.py` & `d20-orm-2.0.2a8/test/test_build_db.py`

 * *Files identical despite different names*

