# Comparing `tmp/pollenflug-0.2.1.tar.gz` & `tmp/pollenflug-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollenflug-0.2.1.tar", max compression
+gzip compressed data, was "pollenflug-0.2.2.tar", max compression
```

## Comparing `pollenflug-0.2.1.tar` & `pollenflug-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2022-12-14 00:12:43.679194 pollenflug-0.2.1/LICENSE
--rw-r--r--   0        0        0     1279 2023-06-03 10:59:02.248456 pollenflug-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-03 12:22:51.970324 pollenflug-0.2.1/pollenflug/lib/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-03 12:22:47.882269 pollenflug-0.2.1/pollenflug/lib/color.py
--rw-r--r--   0        0        0      682 2023-06-03 12:22:45.020231 pollenflug-0.2.1/pollenflug/lib/consts.py
--rw-r--r--   0        0        0     3948 2023-06-03 12:22:41.695186 pollenflug-0.2.1/pollenflug/lib/functions.py
--rwxr-xr-x   0        0        0     2526 2023-06-03 12:22:34.607091 pollenflug-0.2.1/pollenflug/pollenflug.py
--rw-r--r--   0        0        0     1127 2023-06-03 13:36:37.904835 pollenflug-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pollenflug-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 15:05:18.704873 pollenflug-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1279 2023-06-03 15:05:18.704873 pollenflug-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/color.py
+-rw-r--r--   0        0        0      682 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/consts.py
+-rw-r--r--   0        0        0     3948 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/functions.py
+-rwxr-xr-x   0        0        0     2526 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/pollenflug.py
+-rw-r--r--   0        0        0     1127 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pollenflug-0.2.2/PKG-INFO
```

### Comparing `pollenflug-0.2.1/LICENSE` & `pollenflug-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/README.md` & `pollenflug-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/pollenflug/lib/color.py` & `pollenflug-0.2.2/pollenflug/lib/color.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/pollenflug/lib/consts.py` & `pollenflug-0.2.2/pollenflug/lib/consts.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/pollenflug/lib/functions.py` & `pollenflug-0.2.2/pollenflug/lib/functions.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/pollenflug/pollenflug.py` & `pollenflug-0.2.2/pollenflug/pollenflug.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.1/pyproject.toml` & `pollenflug-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pollenflug"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
 	"Bader Zaidan <python@zaidan.tech>"
 ]
 description = "CLI allergy forecast tool"
 readme = "README.md"
 homepage = "https://github.com/BaderSZ/pollenflug"
 repository = "https://github.com/BaderSZ/pollenflug"
```

### Comparing `pollenflug-0.2.1/PKG-INFO` & `pollenflug-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollenflug
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI allergy forecast tool
 Home-page: https://github.com/BaderSZ/pollenflug
 License: GGPL-3.0-or-later
 Author: Bader Zaidan
 Author-email: python@zaidan.tech
 Requires-Python: >=3.7,<4
 Classifier: Environment :: Console
```

