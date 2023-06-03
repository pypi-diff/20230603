# Comparing `tmp/iamlistening-0.1.4.tar.gz` & `tmp/iamlistening-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.4.tar", max compression
+gzip compressed data, was "iamlistening-0.1.5.tar", max compression
```

## Comparing `iamlistening-0.1.4.tar` & `iamlistening-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-02 20:19:16.824405 iamlistening-0.1.4/LICENSE
--rw-r--r--   0        0        0     1504 2023-06-02 20:19:16.824405 iamlistening-0.1.4/README.md
--rw-r--r--   0        0        0       99 2023-06-02 20:19:17.564414 iamlistening-0.1.4/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4292 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-02 20:19:17.564414 iamlistening-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 iamlistening-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-03 16:37:52.170408 iamlistening-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1504 2023-06-03 16:37:52.170408 iamlistening-0.1.5/README.md
+-rw-r--r--   0        0        0       99 2023-06-03 16:37:52.866416 iamlistening-0.1.5/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3661 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-03 16:37:52.866416 iamlistening-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 iamlistening-0.1.5/PKG-INFO
```

### Comparing `iamlistening-0.1.4/LICENSE` & `iamlistening-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.4/README.md` & `iamlistening-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.4/iamlistening/config.py` & `iamlistening-0.1.5/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.4/pyproject.toml` & `iamlistening-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.4"
+version = "0.1.5"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.4/PKG-INFO` & `iamlistening-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

