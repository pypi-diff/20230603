# Comparing `tmp/ironbot-0.0.2.tar.gz` & `tmp/ironbot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironbot-0.0.2.tar", max compression
+gzip compressed data, was "ironbot-0.0.3.tar", max compression
```

## Comparing `ironbot-0.0.2.tar` & `ironbot-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.2/LICENSE
--rw-r--r--   0        0        0     1823 2023-06-02 23:33:11.660579 ironbot-0.0.2/README.md
--rw-r--r--   0        0        0     4016 2023-06-02 23:38:38.857517 ironbot-0.0.2/ironbot/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-02 23:30:58.279636 ironbot-0.0.2/ironbot/__main__.py
--rw-r--r--   0        0        0     1131 2023-06-02 23:51:37.296030 ironbot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 ironbot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1823 2023-06-02 23:33:11.660579 ironbot-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.3/ironbot/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.3/ironbot/__main__.py
+-rw-r--r--   0        0        0     2103 2023-06-03 00:15:21.796445 ironbot-0.0.3/ironbot/models.py
+-rw-r--r--   0        0        0     2083 2023-06-03 00:01:27.405671 ironbot-0.0.3/ironbot/scrappers.py
+-rw-r--r--   0        0        0     1131 2023-06-03 00:15:50.438183 ironbot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 ironbot-0.0.3/PKG-INFO
```

### Comparing `ironbot-0.0.2/LICENSE` & `ironbot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.2/README.md` & `ironbot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.2/pyproject.toml` & `ironbot-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ironbot"
-version = "0.0.2"
+version = "0.0.3"
 description = "CLI to get information about Ironman professional races"
 authors = ["Eduardo Cuducos <4732915+cuducos@users.noreply.github.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/cuducos/ironbot/"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `ironbot-0.0.2/PKG-INFO` & `ironbot-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironbot
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI to get information about Ironman professional races
 Home-page: https://github.com/cuducos/ironbot/
 License: GPLv3
 Keywords: triathlon,Ironamn,Professional triathletes,Professional triathlon races
 Author: Eduardo Cuducos
 Author-email: 4732915+cuducos@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

