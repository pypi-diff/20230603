# Comparing `tmp/cuallee-0.4.3.tar.gz` & `tmp/cuallee-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.4.3.tar", last modified: Sat Jun  3 16:11:34 2023, max compression
+gzip compressed data, was "cuallee-0.4.4.tar", last modified: Sat Jun  3 16:14:56 2023, max compression
```

## Comparing `cuallee-0.4.3.tar` & `cuallee-0.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:11:34.739352 cuallee-0.4.3/
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.3/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:11:34.739352 cuallee-0.4.3/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.3/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:11:34.736019 cuallee-0.4.3/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:11:34.739352 cuallee-0.4.3/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/pandas_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)        0 2022-11-26 21:58:56.000000 cuallee-0.4.3/cuallee/polars.validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.3/cuallee/pyspark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.3/cuallee/snowpark_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.3/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:11:34.739352 cuallee-0.4.3/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:11:34.000000 cuallee-0.4.3/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-03 16:11:34.000000 cuallee-0.4.3/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-03 16:11:34.000000 cuallee-0.4.3/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      312 2023-06-03 16:11:34.000000 cuallee-0.4.3/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-03 16:11:34.000000 cuallee-0.4.3/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1211 2023-06-03 16:11:16.000000 cuallee-0.4.3/pyproject.toml
--rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-03 16:11:34.739352 cuallee-0.4.3/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.4/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:14:56.499344 cuallee-0.4.4/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.4/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/pandas_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)        0 2022-11-26 21:58:56.000000 cuallee-0.4.4/cuallee/polars.validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/pyspark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.4/cuallee/snowpark_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.4/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      312 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1211 2023-06-03 16:13:57.000000 cuallee-0.4.4/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-03 16:14:56.499344 cuallee-0.4.4/setup.cfg
```

### Comparing `cuallee-0.4.3/LICENSE` & `cuallee-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/PKG-INFO` & `cuallee-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuallee-0.4.3/README.md` & `cuallee-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/__init__.py` & `cuallee-0.4.4/cuallee/__init__.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/duckdb_validation.py` & `cuallee-0.4.4/cuallee/duckdb_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/iso/checks.py` & `cuallee-0.4.4/cuallee/iso/checks.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/pandas_validation.py` & `cuallee-0.4.4/cuallee/pandas_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/pyspark_validation.py` & `cuallee-0.4.4/cuallee/pyspark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/snowpark_validation.py` & `cuallee-0.4.4/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee/utils.py` & `cuallee-0.4.4/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.3/cuallee.egg-info/PKG-INFO` & `cuallee-0.4.4/cuallee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuallee-0.4.3/pyproject.toml` & `cuallee-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" },
   { name="Herminio Vazquez", email="canimus@gmail.com"}
 ]
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -19,15 +19,15 @@
 ]
 dependencies = [
     "colorama >= 0.4.6",
     "toolz >= 0.12.0",
     "pygments >= 2.15.1",
     "lxml >= 4.9.2",
     "requests >= 2.28.2",
-    "pandas>=2.0.1"
+    "pandas>=1.5.3"
 ]
 
 [project.optional-dependencies]
 pyspark = [
   "pyspark>=3.4.0"
 ]
 snowpark = [
```

