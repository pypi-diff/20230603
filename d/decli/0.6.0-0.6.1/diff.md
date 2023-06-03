# Comparing `tmp/decli-0.6.0.tar.gz` & `tmp/decli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decli-0.6.0.tar", max compression
+gzip compressed data, was "decli-0.6.1.tar", max compression
```

## Comparing `decli-0.6.0.tar` & `decli-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-28 09:49:27.803266 decli-0.6.0/LICENSE
--rw-r--r--   0        0        0    17159 2023-04-28 09:49:27.803266 decli-0.6.0/README.rst
--rw-r--r--   0        0        0       72 2023-04-28 09:49:27.803266 decli-0.6.0/decli/__init__.py
--rw-r--r--   0        0        0     4607 2023-04-28 09:49:27.803266 decli-0.6.0/decli/application.py
--rw-r--r--   0        0        0        0 2023-04-28 09:49:27.803266 decli-0.6.0/decli/py.typed
--rw-r--r--   0        0        0      750 2023-04-28 09:49:27.803266 decli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 decli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-03 08:50:02.464636 decli-0.6.1/LICENSE
+-rw-r--r--   0        0        0    17159 2023-06-03 08:50:02.464636 decli-0.6.1/README.rst
+-rw-r--r--   0        0        0       72 2023-06-03 08:50:02.464636 decli-0.6.1/decli/__init__.py
+-rw-r--r--   0        0        0     4607 2023-06-03 08:50:02.464636 decli-0.6.1/decli/application.py
+-rw-r--r--   0        0        0        0 2023-06-03 08:50:02.464636 decli-0.6.1/decli/py.typed
+-rw-r--r--   0        0        0      807 2023-06-03 08:50:02.464636 decli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 decli-0.6.1/PKG-INFO
```

### Comparing `decli-0.6.0/LICENSE` & `decli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decli-0.6.0/README.rst` & `decli-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `decli-0.6.0/decli/application.py` & `decli-0.6.1/decli/application.py`

 * *Files identical despite different names*

### Comparing `decli-0.6.0/pyproject.toml` & `decli-0.6.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decli"
-version = "0.6.0"
+version = "0.6.1"
 description = "Minimal, easy-to-use, declarative cli tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 readme = 'README.rst'
 
 [tool.poetry.dependencies]
 python = ">=3.7"
@@ -33,7 +33,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 version_type = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
+version_files = [
+    "decli/__init__.py:__version__",
+]
```

### Comparing `decli-0.6.0/PKG-INFO` & `decli-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Minimal, easy-to-use, declarative cli tool
 License: MIT
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

