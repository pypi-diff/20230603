# Comparing `tmp/pydantic_tools-0.3.2.tar.gz` & `tmp/pydantic_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_tools-0.3.2.tar", last modified: Sat Jun  3 04:59:28 2023, max compression
+gzip compressed data, was "pydantic_tools-0.3.3.tar", last modified: Sat Jun  3 05:14:57 2023, max compression
```

## Comparing `pydantic_tools-0.3.2.tar` & `pydantic_tools-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1533 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/alias/__init__.py
--rw-r--r--   0        0        0      181 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/__main__.py
--rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/locales/__init__.py
--rw-r--r--   0        0        0     6932 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/locales/zh_cn.py
--rw-r--r--   0        0        0      897 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/model.py
--rw-r--r--   0        0        0     1267 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/templates.py
--rw-r--r--   0        0        0     1676 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/translate.py
--rw-r--r--   0        0        0      796 2023-06-03 04:59:28.657751 pydantic_tools-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2630 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/tests/test_i18n.py
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 pydantic_tools-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1975 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/alias/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/i18n/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/i18n/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/i18n/locales/__init__.py
+-rw-r--r--   0        0        0     6932 2023-06-03 05:14:16.067371 pydantic_tools-0.3.3/pydantic_tools/i18n/locales/zh_cn.py
+-rw-r--r--   0        0        0      897 2023-06-03 05:14:16.071372 pydantic_tools-0.3.3/pydantic_tools/i18n/model.py
+-rw-r--r--   0        0        0     1267 2023-06-03 05:14:16.071372 pydantic_tools-0.3.3/pydantic_tools/i18n/templates.py
+-rw-r--r--   0        0        0     1676 2023-06-03 05:14:16.071372 pydantic_tools-0.3.3/pydantic_tools/i18n/translate.py
+-rw-r--r--   0        0        0      796 2023-06-03 05:14:57.846629 pydantic_tools-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2630 2023-06-03 05:14:16.071372 pydantic_tools-0.3.3/tests/test_i18n.py
+-rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 pydantic_tools-0.3.3/PKG-INFO
```

### Comparing `pydantic_tools-0.3.2/pydantic_tools/i18n/__main__.py` & `pydantic_tools-0.3.3/pydantic_tools/i18n/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/pydantic_tools/i18n/locales/zh_cn.py` & `pydantic_tools-0.3.3/pydantic_tools/i18n/locales/zh_cn.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/pydantic_tools/i18n/model.py` & `pydantic_tools-0.3.3/pydantic_tools/i18n/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/pydantic_tools/i18n/templates.py` & `pydantic_tools-0.3.3/pydantic_tools/i18n/templates.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/pydantic_tools/i18n/translate.py` & `pydantic_tools-0.3.3/pydantic_tools/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/pyproject.toml` & `pydantic_tools-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydantic_tools"
-version = "0.3.2"
+version = "0.3.3"
 description = "Useful tools for pydantic"
 authors = [
     { name = "icebear", email = "iiiicebeaaaar@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
     "pytest>=7.3.1",
```

### Comparing `pydantic_tools-0.3.2/tests/test_i18n.py` & `pydantic_tools-0.3.3/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.2/PKG-INFO` & `pydantic_tools-0.3.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pydantic-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Useful tools for pydantic
 Author-Email: icebear <iiiicebeaaaar@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: rich>=13.3.5
 Requires-Dist: bullet>=2.2.0
 Requires-Dist: click>=8.1.3
 Description-Content-Type: text/markdown
 
 # pydantic-tools
 
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![codecov](https://codecov.io/gh/iiicebearrr/pydantic-tools/branch/main/graph/badge.svg?token=SBVE7WNDO9)](https://codecov.io/gh/iiicebearrr/pydantic-tools)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![codecov](https://codecov.io/gh/iiicebearrr/pydantic-tools/branch/main/graph/badge.svg?token=SBVE7WNDO9)](https://codecov.io/gh/iiicebearrr/pydantic-tools) 
 
+![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 
-A set of tools for pydantic(i18n, alias, etc.)
+
+A set of tools for pydantic(i18n, alias(comming soon), etc.)
 
 ## Installation
 
 `pip install pydantic-tools`
 
 ## i18n
 
@@ -53,7 +55,24 @@
 - `locale`: The locale of the model, default is `None`, which means no translation enabled, and the default error message will be used. Use `python -m pydantic_tools.i18n -l` to show all available locales.
 
 - `locale_strict`: Whether to raise an error when the locale is not found, default is `False`.
 
 - `translations`: If specified, the error messages will be translated according to the given dict instead of the locale config. The dict should be like `{"value_error.missing": "Missing"}`. One of `locale` and `translations` should be specified, do not set both of them.
 
 - `extra_translations`: If specified, an extra dict will be merged into the default translations. The dict should be like `{"value_error.missing": "some msg"}`.
+
+
+### Show all available locales
+
+```shell
+python -m pydantic_tools.i18n -l
+```
+
+### Show all available translations
+
+```shell  
+python -m pydantic_tools.i18n -t
+```
+
+## alias
+
+Comming soon
```

