# Comparing `tmp/pydantic_tools-0.3.0.tar.gz` & `tmp/pydantic_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_tools-0.3.0.tar", last modified: Mon May 22 13:54:41 2023, max compression
+gzip compressed data, was "pydantic_tools-0.3.1.tar", last modified: Sat Jun  3 03:56:34 2023, max compression
```

## Comparing `pydantic_tools-0.3.0.tar` & `pydantic_tools-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1326 2023-05-21 14:02:10.710540 pydantic_tools-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-22 13:35:56.162801 pydantic_tools-0.3.0/pydantic_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:34:52.102521 pydantic_tools-0.3.0/pydantic_tools/alias/__init__.py
--rw-r--r--   0        0        0      181 2023-05-21 13:36:01.963863 pydantic_tools-0.3.0/pydantic_tools/i18n/__init__.py
--rw-r--r--   0        0        0     1881 2023-05-21 14:06:01.710783 pydantic_tools-0.3.0/pydantic_tools/i18n/__main__.py
--rw-r--r--   0        0        0        0 2023-05-20 03:41:40.806311 pydantic_tools-0.3.0/pydantic_tools/i18n/locales/__init__.py
--rw-r--r--   0        0        0     6932 2023-05-20 15:56:43.387030 pydantic_tools-0.3.0/pydantic_tools/i18n/locales/zh_cn.py
--rw-r--r--   0        0        0      897 2023-05-21 13:36:02.037013 pydantic_tools-0.3.0/pydantic_tools/i18n/model.py
--rw-r--r--   0        0        0     1267 2023-05-21 13:36:10.764355 pydantic_tools-0.3.0/pydantic_tools/i18n/templates.py
--rw-r--r--   0        0        0     1676 2023-05-21 07:26:37.197197 pydantic_tools-0.3.0/pydantic_tools/i18n/translate.py
--rw-r--r--   0        0        0      755 2023-05-22 13:54:41.828874 pydantic_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2597 2023-05-21 13:36:02.095934 pydantic_tools-0.3.0/tests/test_i18n.py
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 pydantic_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1373 2023-05-22 14:02:24.136380 pydantic_tools-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 13:35:56.162801 pydantic_tools-0.3.1/pydantic_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:34:52.102521 pydantic_tools-0.3.1/pydantic_tools/alias/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-21 13:36:01.963863 pydantic_tools-0.3.1/pydantic_tools/i18n/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-21 14:06:01.710783 pydantic_tools-0.3.1/pydantic_tools/i18n/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-20 03:41:40.806311 pydantic_tools-0.3.1/pydantic_tools/i18n/locales/__init__.py
+-rw-r--r--   0        0        0     6932 2023-05-20 15:56:43.387030 pydantic_tools-0.3.1/pydantic_tools/i18n/locales/zh_cn.py
+-rw-r--r--   0        0        0      897 2023-06-03 03:50:14.782276 pydantic_tools-0.3.1/pydantic_tools/i18n/model.py
+-rw-r--r--   0        0        0     1267 2023-05-21 13:36:10.764355 pydantic_tools-0.3.1/pydantic_tools/i18n/templates.py
+-rw-r--r--   0        0        0     1676 2023-05-21 07:26:37.197197 pydantic_tools-0.3.1/pydantic_tools/i18n/translate.py
+-rw-r--r--   0        0        0      796 2023-06-03 03:56:34.785452 pydantic_tools-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2630 2023-06-03 03:53:28.626074 pydantic_tools-0.3.1/tests/test_i18n.py
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 pydantic_tools-0.3.1/PKG-INFO
```

### Comparing `pydantic_tools-0.3.0/README.md` & `pydantic_tools-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # pydantic-tools
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 A set of tools for pydantic(i18n, alias, etc.)
 
+## Installation
+
+`pip install pydantic-tools`
+
 ## i18n
 
 ### A simple example
 
 ```python
 from pydantic_tools import i18n
 class TestModel(i18n.BaseModel_i18n):
```

### Comparing `pydantic_tools-0.3.0/pydantic_tools/i18n/__main__.py` & `pydantic_tools-0.3.1/pydantic_tools/i18n/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.0/pydantic_tools/i18n/locales/zh_cn.py` & `pydantic_tools-0.3.1/pydantic_tools/i18n/locales/zh_cn.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.0/pydantic_tools/i18n/model.py` & `pydantic_tools-0.3.1/pydantic_tools/i18n/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.0/pydantic_tools/i18n/templates.py` & `pydantic_tools-0.3.1/pydantic_tools/i18n/templates.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.0/pydantic_tools/i18n/translate.py` & `pydantic_tools-0.3.1/pydantic_tools/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `pydantic_tools-0.3.0/pyproject.toml` & `pydantic_tools-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydantic_tools"
-version = "0.3.0"
+version = "0.3.1"
 description = "Useful tools for pydantic"
 authors = [
     { name = "icebear", email = "iiiicebeaaaar@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
     "pytest>=7.3.1",
@@ -34,9 +34,10 @@
     "pytest-cov>=4.0.0",
     "pre-commit>=3.3.2",
     "tox-pdm>=0.6.1",
 ]
 
 [tool.coverage.run]
 omit = [
-    "src/i18n/__main__.py",
+    "pydantic_tools/i18n/__main__.py",
+    "pydantic_tools/alias/*",
 ]
```

### Comparing `pydantic_tools-0.3.0/tests/test_i18n.py` & `pydantic_tools-0.3.1/tests/test_i18n.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pydantic
 import pytest
 
-from src import i18n
-from src.i18n.locales.zh_cn import translations as translations_zh_cn
+from pydantic_tools import i18n
+from pydantic_tools.i18n.locales.zh_cn import translations as translations_zh_cn
 
 _TEST_TRANSLATIONS = translations_zh_cn
 
 _VE = pydantic.ValidationError
 
 
 def test_missing():
@@ -47,15 +47,15 @@
             }
 
     with pytest.raises(_VE, match="Missing value Extra"):
         TestMissing()
 
 
 def test_templates():
-    from src.i18n.templates import show_templates
+    from pydantic_tools.i18n.templates import show_templates
 
     show_templates()
 
 
 def test_strict():
     class TestMissing(i18n.BaseModel_i18n):
         name: str
```

### Comparing `pydantic_tools-0.3.0/PKG-INFO` & `pydantic_tools-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Useful tools for pydantic
 Author-Email: icebear <iiiicebeaaaar@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: rich>=13.3.5
@@ -14,14 +14,18 @@
 
 # pydantic-tools
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 A set of tools for pydantic(i18n, alias, etc.)
 
+## Installation
+
+`pip install pydantic-tools`
+
 ## i18n
 
 ### A simple example
 
 ```python
 from pydantic_tools import i18n
 class TestModel(i18n.BaseModel_i18n):
```

