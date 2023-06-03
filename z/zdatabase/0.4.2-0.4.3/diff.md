# Comparing `tmp/zdatabase-0.4.2.tar.gz` & `tmp/zdatabase-0.4.3.tar.gz`

## Comparing `zdatabase-0.4.2.tar` & `zdatabase-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/model.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 zdatabase-0.4.2/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.2/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.3/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.3/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.4.3/PKG-INFO
```

### Comparing `zdatabase-0.4.2/src/zdatabase/__init__.py` & `zdatabase-0.4.3/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.2/src/zdatabase/model.py` & `zdatabase-0.4.3/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.2/src/zdatabase/utility.py` & `zdatabase-0.4.3/src/zdatabase/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,9 +202,9 @@
         for item in cls.get_attrs_(attr_names):
             a, b = item
             rst_map[a] = b
         return rst_map
 
     @classmethod
     def delete_list_(cls, **kwargs):
-        cls.make_query(**kwargs).delete(synchronize_db.session=False)
+        cls.make_query(**kwargs).delete(synchronize_session=False)
         cls.commit()
```

### Comparing `zdatabase-0.4.2/LICENSE` & `zdatabase-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.2/pyproject.toml` & `zdatabase-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.4.2/PKG-INFO` & `zdatabase-0.4.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.4.2
+Version: 0.4.3
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

