# Comparing `tmp/zdatabase-0.4.1.tar.gz` & `tmp/zdatabase-0.4.2.tar.gz`

## Comparing `zdatabase-0.4.1.tar` & `zdatabase-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 zdatabase-0.4.1/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 zdatabase-0.4.1/src/zdatabase/model.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 zdatabase-0.4.1/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.1/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.1/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.2/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.2/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.4.2/PKG-INFO
```

### Comparing `zdatabase-0.4.1/src/zdatabase/__init__.py` & `zdatabase-0.4.2/src/zdatabase/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         engine = create_engine(url)
         metadata = MetaData(bind=engine)
         Session = sessionmaker(autocommit=False, autoflush=False, bind=engine)
         self.session = Session()
         return engine, metadata
  
  
-Model = declarative_base()
+Base = declarative_base()
 db = Database()
```

### Comparing `zdatabase-0.4.1/src/zdatabase/model.py` & `zdatabase-0.4.2/src/zdatabase/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from zdatabase import Model, db
+from zdatabase import Base, db
 from zdatabase.utility import DatabaseUtility, QueryUtility, MapperUtility
 from inspirare import time
 
 
-class Model(Model, DatabaseUtility, QueryUtility, MapperUtility):
+class Model(Base, DatabaseUtility, QueryUtility, MapperUtility):
     __abstract__ = True
 
     @classmethod
     def filter(cls, *args, **kwargs):
         return cls.query.filter(*args, **kwargs)
 
     @classmethod
```

### Comparing `zdatabase-0.4.1/src/zdatabase/utility.py` & `zdatabase-0.4.2/src/zdatabase/utility.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.1/LICENSE` & `zdatabase-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.1/pyproject.toml` & `zdatabase-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.4.1/PKG-INFO` & `zdatabase-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.4.1
+Version: 0.4.2
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

