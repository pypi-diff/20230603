# Comparing `tmp/findu-0.0.1.tar.gz` & `tmp/findu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.1.tar", max compression
+gzip compressed data, was "findu-0.0.2.tar", max compression
```

## Comparing `findu-0.0.1.tar` & `findu-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2023-06-03 07:46:58.537797 findu-0.0.1/findu/__init__.py
--rw-r--r--   0        0        0       41 2023-06-03 08:24:31.306646 findu-0.0.1/findu/findu.py
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.1/LICENSE
--rw-r--r--   0        0        0     1311 2023-06-03 07:49:40.854608 findu-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      609 2023-06-03 07:50:38.419853 findu-0.0.1/README.md
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 findu-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-06-03 08:30:24.870103 findu-0.0.2/findu/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-03 08:24:31.306646 findu-0.0.2/findu/findu.py
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1311 2023-06-03 08:30:35.960087 findu-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      609 2023-06-03 07:50:38.419853 findu-0.0.2/README.md
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 findu-0.0.2/PKG-INFO
```

### Comparing `findu-0.0.1/LICENSE` & `findu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.1/pyproject.toml` & `findu-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.1"
+version = "0.0.2"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.1/README.md` & `findu-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.1/PKG-INFO` & `findu-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

