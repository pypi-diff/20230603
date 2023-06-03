# Comparing `tmp/pycln-2.1.4.tar.gz` & `tmp/pycln-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycln-2.1.4.tar", max compression
+gzip compressed data, was "pycln-2.1.5.tar", max compression
```

## Comparing `pycln-2.1.4.tar` & `pycln-2.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1099 2023-05-31 14:52:37.059019 pycln-2.1.4/LICENSE
--rw-r--r--   0        0        0     7370 2023-05-31 14:52:37.059019 pycln-2.1.4/README.md
--rw-r--r--   0        0        0     1160 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/__init__.py
--rw-r--r--   0        0        0      113 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/__main__.py
--rw-r--r--   0        0        0     6828 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/cli.py
--rw-r--r--   0        0        0       26 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/__init__.py
--rw-r--r--   0        0        0     3192 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/_exceptions.py
--rw-r--r--   0        0        0     1813 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/_nodes.py
--rw-r--r--   0        0        0     7477 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/config.py
--rw-r--r--   0        0        0     3908 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/iou.py
--rw-r--r--   0        0        0    12640 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/pathu.py
--rw-r--r--   0        0        0    20961 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/refactor.py
--rw-r--r--   0        0        0     4138 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/regexu.py
--rw-r--r--   0        0        0    18739 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/report.py
--rw-r--r--   0        0        0    34842 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/scan.py
--rw-r--r--   0        0        0     8055 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/transform.py
--rw-r--r--   0        0        0     1796 2023-05-31 14:52:37.063019 pycln-2.1.4/pyproject.toml
--rw-r--r--   0        0        0       66 2023-05-31 14:52:37.067020 pycln-2.1.4/vendor/custom/__init__.py
--rw-r--r--   0        0        0     2018 2023-05-31 14:52:37.067020 pycln-2.1.4/vendor/custom/_site.py
--rw-r--r--   0        0        0     8637 1970-01-01 00:00:00.000000 pycln-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-06-03 11:10:17.232623 pycln-2.1.5/LICENSE
+-rw-r--r--   0        0        0     7370 2023-06-03 11:10:17.232623 pycln-2.1.5/README.md
+-rw-r--r--   0        0        0     1160 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/__main__.py
+-rw-r--r--   0        0        0     6828 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/cli.py
+-rw-r--r--   0        0        0       26 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/_exceptions.py
+-rw-r--r--   0        0        0     1813 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/_nodes.py
+-rw-r--r--   0        0        0     7477 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/config.py
+-rw-r--r--   0        0        0     3908 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/iou.py
+-rw-r--r--   0        0        0    12640 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/pathu.py
+-rw-r--r--   0        0        0    20961 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/refactor.py
+-rw-r--r--   0        0        0     4138 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/regexu.py
+-rw-r--r--   0        0        0    18739 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/report.py
+-rw-r--r--   0        0        0    34842 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/scan.py
+-rw-r--r--   0        0        0     8055 2023-06-03 11:10:17.236623 pycln-2.1.5/pycln/utils/transform.py
+-rw-r--r--   0        0        0     1805 2023-06-03 11:10:17.236623 pycln-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-06-03 11:10:17.240623 pycln-2.1.5/vendor/custom/__init__.py
+-rw-r--r--   0        0        0     2018 2023-06-03 11:10:17.240623 pycln-2.1.5/vendor/custom/_site.py
+-rw-r--r--   0        0        0     8637 1970-01-01 00:00:00.000000 pycln-2.1.5/PKG-INFO
```

### Comparing `pycln-2.1.4/LICENSE` & `pycln-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/README.md` & `pycln-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/__init__.py` & `pycln-2.1.5/pycln/__init__.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/cli.py` & `pycln-2.1.5/pycln/cli.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/_exceptions.py` & `pycln-2.1.5/pycln/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/_nodes.py` & `pycln-2.1.5/pycln/utils/_nodes.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/config.py` & `pycln-2.1.5/pycln/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/iou.py` & `pycln-2.1.5/pycln/utils/iou.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/pathu.py` & `pycln-2.1.5/pycln/utils/pathu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/refactor.py` & `pycln-2.1.5/pycln/utils/refactor.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/regexu.py` & `pycln-2.1.5/pycln/utils/regexu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/report.py` & `pycln-2.1.5/pycln/utils/report.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/scan.py` & `pycln-2.1.5/pycln/utils/scan.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pycln/utils/transform.py` & `pycln-2.1.5/pycln/utils/transform.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/pyproject.toml` & `pycln-2.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycln"
-version = "2.1.4"
+version = "2.1.5"
 description = "A formatter for finding and removing unused import statements."
 authors = ["Hadi Alqattan <alqattanhadizaki@gmail.com>"]
 homepage = "https://hadialqattan.github.io/pycln"
 repository = "https://github.com/hadialqattan/pycln"
 keywords = ["formatter", "linter", "quality-assurance", "tools", "cli"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -24,15 +24,15 @@
 pycln = "pycln.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.6.2, <4"
 typer = ">=0.4.1,<0.10.0"
 dataclasses = {version = "^0.7", python = "3.6"}
 pyyaml = ">=5.3.1,<7.0.0"
-pathspec = "^0.9.0"
+pathspec = ">=0.9.0,<0.12.0"
 tomlkit = "^0.11.1"
 libcst = [{version = ">=0.3.10,<0.5.0", python = ">=3.7"}, {version = ">=0.3.10,<0.4.0", python = "<3.7"}]
 
 [tool.poetry.dev-dependencies]
 requests = "^2.24.0"
 semver = "^2.10.2"
 pytest = "^7.0"
```

### Comparing `pycln-2.1.4/vendor/custom/_site.py` & `pycln-2.1.5/vendor/custom/_site.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.4/PKG-INFO` & `pycln-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycln
-Version: 2.1.4
+Version: 2.1.5
 Summary: A formatter for finding and removing unused import statements.
 Home-page: https://hadialqattan.github.io/pycln
 License: MIT
 Keywords: formatter,linter,quality-assurance,tools,cli
 Author: Hadi Alqattan
 Author-email: alqattanhadizaki@gmail.com
 Requires-Python: >=3.6.2,<4
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
 Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7"
 Requires-Dist: libcst (>=0.3.10,<0.5.0) ; python_version >= "3.7"
-Requires-Dist: pathspec (>=0.9.0,<0.10.0)
+Requires-Dist: pathspec (>=0.9.0,<0.12.0)
 Requires-Dist: pyyaml (>=5.3.1,<7.0.0)
 Requires-Dist: tomlkit (>=0.11.1,<0.12.0)
 Requires-Dist: typer (>=0.4.1,<0.10.0)
 Project-URL: Repository, https://github.com/hadialqattan/pycln
 Description-Content-Type: text/markdown
 
 <img src="https://raw.githubusercontent.com/hadialqattan/pycln/master/docs/_media/logo-background.png" width="100%" alt="Logo">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pycln Version: 2.1.4 Summary: A formatter for
+Metadata-Version: 2.1 Name: pycln Version: 2.1.5 Summary: A formatter for
 finding and removing unused import statements. Home-page: https://
 hadialqattan.github.io/pycln License: MIT Keywords: formatter,linter,quality-
 assurance,tools,cli Author: Hadi Alqattan Author-email:
 alqattanhadizaki@gmail.com Requires-Python: >=3.6.2,<4 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Utilities Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
 Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7" Requires-Dist:
 libcst (>=0.3.10,<0.5.0) ; python_version >= "3.7" Requires-Dist: pathspec
-(>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=5.3.1,<7.0.0) Requires-Dist: tomlkit
+(>=0.9.0,<0.12.0) Requires-Dist: pyyaml (>=5.3.1,<7.0.0) Requires-Dist: tomlkit
 (>=0.11.1,<0.12.0) Requires-Dist: typer (>=0.4.1,<0.10.0) Project-URL:
 Repository, https://github.com/hadialqattan/pycln Description-Content-Type:
 text/markdown [Logo]
   ***** A formatter for finding and removing unused import statements. *****
    [Pycln_Docs] [CI] [CD] [FUZZ] [Codacy_Badge] [Codecov] [Maintainability]
  [PYPI - Python Version] [PYPI_-_Pycln_Version] [Total_Downloads] [Downloads]
 [Forks] [Stars] [Issues] [Pull_Requests] [Contributors] [Last_Commit] [License]
```

