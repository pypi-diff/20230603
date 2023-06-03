# Comparing `tmp/pydantic_tools-0.3.1.tar.gz` & `tmp/pydantic_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_tools-0.3.1.tar", last modified: Sat Jun  3 03:56:34 2023, max compression
+gzip compressed data, was "pydantic_tools-0.3.2.tar", last modified: Sat Jun  3 04:59:28 2023, max compression
```

## Comparing `pydantic_tools-0.3.1.tar` & `pydantic_tools-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1373 2023-05-22 14:02:24.136380 pydantic_tools-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-22 13:35:56.162801 pydantic_tools-0.3.1/pydantic_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:34:52.102521 pydantic_tools-0.3.1/pydantic_tools/alias/__init__.py
--rw-r--r--   0        0        0      181 2023-05-21 13:36:01.963863 pydantic_tools-0.3.1/pydantic_tools/i18n/__init__.py
--rw-r--r--   0        0        0     1881 2023-05-21 14:06:01.710783 pydantic_tools-0.3.1/pydantic_tools/i18n/__main__.py
--rw-r--r--   0        0        0        0 2023-05-20 03:41:40.806311 pydantic_tools-0.3.1/pydantic_tools/i18n/locales/__init__.py
--rw-r--r--   0        0        0     6932 2023-05-20 15:56:43.387030 pydantic_tools-0.3.1/pydantic_tools/i18n/locales/zh_cn.py
--rw-r--r--   0        0        0      897 2023-06-03 03:50:14.782276 pydantic_tools-0.3.1/pydantic_tools/i18n/model.py
--rw-r--r--   0        0        0     1267 2023-05-21 13:36:10.764355 pydantic_tools-0.3.1/pydantic_tools/i18n/templates.py
--rw-r--r--   0        0        0     1676 2023-05-21 07:26:37.197197 pydantic_tools-0.3.1/pydantic_tools/i18n/translate.py
--rw-r--r--   0        0        0      796 2023-06-03 03:56:34.785452 pydantic_tools-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2630 2023-06-03 03:53:28.626074 pydantic_tools-0.3.1/tests/test_i18n.py
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 pydantic_tools-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/alias/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/locales/__init__.py
+-rw-r--r--   0        0        0     6932 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/locales/zh_cn.py
+-rw-r--r--   0        0        0      897 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/model.py
+-rw-r--r--   0        0        0     1267 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/templates.py
+-rw-r--r--   0        0        0     1676 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/pydantic_tools/i18n/translate.py
+-rw-r--r--   0        0        0      796 2023-06-03 04:59:28.657751 pydantic_tools-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2630 2023-06-03 04:58:55.873790 pydantic_tools-0.3.2/tests/test_i18n.py
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 pydantic_tools-0.3.2/PKG-INFO
```

### Comparing `pydantic_tools-0.3.1/README.md` & `pydantic_tools-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # pydantic-tools
 
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![codecov](https://codecov.io/gh/iiicebearrr/pydantic-tools/branch/main/graph/badge.svg?token=SBVE7WNDO9)](https://codecov.io/gh/iiicebearrr/pydantic-tools)
+
+
 
 A set of tools for pydantic(i18n, alias, etc.)
 
 ## Installation
 
 `pip install pydantic-tools`
```

### Comparing `pydantic_tools-0.3.1/pydantic_tools/i18n/__main__.py` & `pydantic_tools-0.3.2/pydantic_tools/i18n/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/pydantic_tools/i18n/locales/zh_cn.py` & `pydantic_tools-0.3.2/pydantic_tools/i18n/locales/zh_cn.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/pydantic_tools/i18n/model.py` & `pydantic_tools-0.3.2/pydantic_tools/i18n/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/pydantic_tools/i18n/templates.py` & `pydantic_tools-0.3.2/pydantic_tools/i18n/templates.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/pydantic_tools/i18n/translate.py` & `pydantic_tools-0.3.2/pydantic_tools/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/pyproject.toml` & `pydantic_tools-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydantic_tools"
-version = "0.3.1"
+version = "0.3.2"
 description = "Useful tools for pydantic"
 authors = [
     { name = "icebear", email = "iiiicebeaaaar@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
     "pytest>=7.3.1",
```

### Comparing `pydantic_tools-0.3.1/tests/test_i18n.py` & `pydantic_tools-0.3.2/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.1/PKG-INFO` & `pydantic_tools-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pydantic-tools
-Version: 0.3.1
+Version: 0.3.2
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
 
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![codecov](https://codecov.io/gh/iiicebearrr/pydantic-tools/branch/main/graph/badge.svg?token=SBVE7WNDO9)](https://codecov.io/gh/iiicebearrr/pydantic-tools)
+
+
 
 A set of tools for pydantic(i18n, alias, etc.)
 
 ## Installation
 
 `pip install pydantic-tools`
```

