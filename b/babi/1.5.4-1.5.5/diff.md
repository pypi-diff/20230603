# Comparing `tmp/babi-1.5.4.tar.gz` & `tmp/babi-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babi-1.5.4.tar", last modified: Sat May  6 20:19:47 2023, max compression
+gzip compressed data, was "babi-1.5.5.tar", last modified: Sat Jun  3 18:54:46 2023, max compression
```

## Comparing `babi-1.5.4.tar` & `babi-1.5.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:38.000000 babi-1.5.4/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-05-06 20:19:47.635421 babi-1.5.4/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5486 2022-12-29 22:23:55.000000 babi-1.5.4/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.627421 babi-1.5.4/babi/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      120 2022-04-30 16:59:38.000000 babi-1.5.4/babi/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      162 2022-04-30 16:59:38.000000 babi-1.5.4/babi/_types.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    10869 2022-04-30 16:59:38.000000 babi-1.5.4/babi/buf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      766 2022-04-30 16:59:38.000000 babi-1.5.4/babi/cached_property.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      600 2022-04-30 16:59:38.000000 babi-1.5.4/babi/color.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1825 2022-10-29 23:19:26.000000 babi-1.5.4/babi/color_kd.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2022-04-30 16:59:38.000000 babi-1.5.4/babi/color_manager.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2022-04-30 16:59:38.000000 babi-1.5.4/babi/dim.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2022-04-30 16:59:38.000000 babi-1.5.4/babi/fdict.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    35102 2022-10-29 23:19:26.000000 babi-1.5.4/babi/file.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    24091 2022-10-29 23:19:26.000000 babi-1.5.4/babi/highlight.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1249 2022-04-30 16:59:38.000000 babi-1.5.4/babi/history.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.631421 babi-1.5.4/babi/hl/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      577 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/interface.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8630 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/lint_errors.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/replace.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1914 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/selection.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5055 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/syntax.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1615 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/trailing_whitespace.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1051 2022-04-30 16:59:38.000000 babi-1.5.4/babi/horizontal_scrolling.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/babi/linters/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      537 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/flake8.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2345 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/pre_commit.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1349 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linting.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5811 2022-04-30 16:59:38.000000 babi-1.5.4/babi/main.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1622 2022-04-30 16:59:38.000000 babi-1.5.4/babi/perf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      311 2022-04-30 16:59:38.000000 babi-1.5.4/babi/proc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5759 2022-04-30 16:59:38.000000 babi-1.5.4/babi/prompt.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2295 2022-04-30 16:59:38.000000 babi-1.5.4/babi/reg.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/babi/resources/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/resources/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13089 2022-04-30 16:59:38.000000 babi-1.5.4/babi/resources/default-theme.json
--rw-r--r--   0 asottile  (1000) asottile  (1000)    29300 2022-10-29 23:19:26.000000 babi-1.5.4/babi/screen.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1225 2022-04-30 16:59:38.000000 babi-1.5.4/babi/status.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2217 2022-04-30 16:59:38.000000 babi-1.5.4/babi/textmate_demo.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4870 2022-10-29 23:19:26.000000 babi-1.5.4/babi/theme.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      535 2022-04-30 16:59:38.000000 babi-1.5.4/babi/user_data.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.631421 babi-1.5.4/babi.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      939 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       85 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/top_level.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/licenses/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1191 2022-04-30 16:59:38.000000 babi-1.5.4/licenses/microsoft_vscode_LICENSE.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1450 2023-05-06 20:19:47.635421 babi-1.5.4/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:38.000000 babi-1.5.4/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:38.000000 babi-1.5.5/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-06-03 18:54:46.271188 babi-1.5.5/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5486 2022-12-29 22:23:55.000000 babi-1.5.5/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/babi/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.5/babi/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      120 2022-04-30 16:59:38.000000 babi-1.5.5/babi/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      162 2022-04-30 16:59:38.000000 babi-1.5.5/babi/_types.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    10869 2022-04-30 16:59:38.000000 babi-1.5.5/babi/buf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      766 2022-04-30 16:59:38.000000 babi-1.5.5/babi/cached_property.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      600 2022-04-30 16:59:38.000000 babi-1.5.5/babi/color.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1825 2022-10-29 23:19:26.000000 babi-1.5.5/babi/color_kd.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2022-04-30 16:59:38.000000 babi-1.5.5/babi/color_manager.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2022-04-30 16:59:38.000000 babi-1.5.5/babi/dim.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2022-04-30 16:59:38.000000 babi-1.5.5/babi/fdict.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    35102 2022-10-29 23:19:26.000000 babi-1.5.5/babi/file.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    24091 2022-10-29 23:19:26.000000 babi-1.5.5/babi/highlight.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1249 2022-04-30 16:59:38.000000 babi-1.5.5/babi/history.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/babi/hl/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      577 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/interface.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8630 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/lint_errors.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/replace.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1914 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/selection.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5055 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/syntax.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1615 2022-04-30 16:59:38.000000 babi-1.5.5/babi/hl/trailing_whitespace.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1051 2022-04-30 16:59:38.000000 babi-1.5.5/babi/horizontal_scrolling.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/babi/linters/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.5/babi/linters/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      537 2022-04-30 16:59:38.000000 babi-1.5.5/babi/linters/flake8.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2345 2022-04-30 16:59:38.000000 babi-1.5.5/babi/linters/pre_commit.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1349 2022-04-30 16:59:38.000000 babi-1.5.5/babi/linting.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5811 2022-04-30 16:59:38.000000 babi-1.5.5/babi/main.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1622 2022-04-30 16:59:38.000000 babi-1.5.5/babi/perf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      311 2022-04-30 16:59:38.000000 babi-1.5.5/babi/proc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5759 2022-04-30 16:59:38.000000 babi-1.5.5/babi/prompt.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2295 2022-04-30 16:59:38.000000 babi-1.5.5/babi/reg.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/babi/resources/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.5/babi/resources/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13089 2022-04-30 16:59:38.000000 babi-1.5.5/babi/resources/default-theme.json
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    29352 2023-06-03 18:54:31.000000 babi-1.5.5/babi/screen.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1225 2022-04-30 16:59:38.000000 babi-1.5.5/babi/status.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2217 2022-04-30 16:59:38.000000 babi-1.5.5/babi/textmate_demo.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4870 2022-10-29 23:19:26.000000 babi-1.5.5/babi/theme.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      535 2022-04-30 16:59:38.000000 babi-1.5.5/babi/user_data.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/babi.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      939 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       85 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-06-03 18:54:46.000000 babi-1.5.5/babi.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-03 18:54:46.271188 babi-1.5.5/licenses/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1191 2022-04-30 16:59:38.000000 babi-1.5.5/licenses/microsoft_vscode_LICENSE.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1450 2023-06-03 18:54:46.275188 babi-1.5.5/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:38.000000 babi-1.5.5/setup.py
```

### Comparing `babi-1.5.4/LICENSE` & `babi-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/PKG-INFO` & `babi-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babi
-Version: 1.5.4
+Version: 1.5.5
 Summary: a text editor
 Home-page: https://github.com/asottile/babi
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `babi-1.5.4/README.md` & `babi-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/buf.py` & `babi-1.5.5/babi/buf.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/cached_property.py` & `babi-1.5.5/babi/cached_property.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/color.py` & `babi-1.5.5/babi/color.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/color_kd.py` & `babi-1.5.5/babi/color_kd.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/color_manager.py` & `babi-1.5.5/babi/color_manager.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/fdict.py` & `babi-1.5.5/babi/fdict.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/file.py` & `babi-1.5.5/babi/file.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/highlight.py` & `babi-1.5.5/babi/highlight.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/history.py` & `babi-1.5.5/babi/history.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/interface.py` & `babi-1.5.5/babi/hl/interface.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/lint_errors.py` & `babi-1.5.5/babi/hl/lint_errors.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/replace.py` & `babi-1.5.5/babi/hl/replace.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/selection.py` & `babi-1.5.5/babi/hl/selection.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/syntax.py` & `babi-1.5.5/babi/hl/syntax.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/hl/trailing_whitespace.py` & `babi-1.5.5/babi/hl/trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/horizontal_scrolling.py` & `babi-1.5.5/babi/horizontal_scrolling.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/linters/flake8.py` & `babi-1.5.5/babi/linters/flake8.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/linters/pre_commit.py` & `babi-1.5.5/babi/linters/pre_commit.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/linting.py` & `babi-1.5.5/babi/linting.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/main.py` & `babi-1.5.5/babi/main.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/perf.py` & `babi-1.5.5/babi/perf.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/prompt.py` & `babi-1.5.5/babi/prompt.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/reg.py` & `babi-1.5.5/babi/reg.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/resources/default-theme.json` & `babi-1.5.5/babi/resources/default-theme.json`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/screen.py` & `babi-1.5.5/babi/screen.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     b'KEY_SDOWN': b'KEY_SF',
     # macos: (sends this for backspace key, others interpret this as well)
     b'^?': b'KEY_BACKSPACE',
     # linux, perhaps others
     b'^H': b'KEY_BACKSPACE',  # ^Backspace on my keyboard
     b'^D': b'KEY_DC',
     b'PADENTER': b'^M',  # Enter on numpad
+    b'KEY_ENTER': b'^M',  # Enter, but in `fn` mode
 }
 
 LINTER_TYPES: tuple[type[linting.Linter], ...] = (PreCommit, Flake8)
 
 
 def _get_wch_with_retry(stdscr: curses._CursesWindow) -> str | int:
     while True:
```

### Comparing `babi-1.5.4/babi/status.py` & `babi-1.5.5/babi/status.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/textmate_demo.py` & `babi-1.5.5/babi/textmate_demo.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/theme.py` & `babi-1.5.5/babi/theme.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi/user_data.py` & `babi-1.5.5/babi/user_data.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/babi.egg-info/PKG-INFO` & `babi-1.5.5/babi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babi
-Version: 1.5.4
+Version: 1.5.5
 Summary: a text editor
 Home-page: https://github.com/asottile/babi
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `babi-1.5.4/babi.egg-info/SOURCES.txt` & `babi-1.5.5/babi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/licenses/microsoft_vscode_LICENSE.txt` & `babi-1.5.5/licenses/microsoft_vscode_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `babi-1.5.4/setup.cfg` & `babi-1.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = babi
-version = 1.5.4
+version = 1.5.5
 description = a text editor
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/babi
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

