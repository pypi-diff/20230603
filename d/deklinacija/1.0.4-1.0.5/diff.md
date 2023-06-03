# Comparing `tmp/deklinacija-1.0.4.tar.gz` & `tmp/deklinacija-1.0.5.tar.gz`

## Comparing `deklinacija-1.0.4.tar` & `deklinacija-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/__init__.py
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/module.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.4/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 deklinacija-1.0.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.4/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 deklinacija-1.0.4/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 deklinacija-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/__init__.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/module.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.5/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 deklinacija-1.0.5/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 deklinacija-1.0.5/PKG-INFO
```

### Comparing `deklinacija-1.0.4/.github/workflows/python-package.yml` & `deklinacija-1.0.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/deklinacija/module.py` & `deklinacija-1.0.5/deklinacija/module.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/deklinacija/utils.py` & `deklinacija-1.0.5/deklinacija/utils.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/deklinacija/vokativ_database.csv` & `deklinacija-1.0.5/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/.gitignore` & `deklinacija-1.0.5/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `deklinacija-1.0.4/LICENSE` & `deklinacija-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/README.md` & `deklinacija-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.4/pyproject.toml` & `deklinacija-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.0.4/PKG-INFO` & `deklinacija-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

