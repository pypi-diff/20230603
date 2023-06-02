# Comparing `tmp/dcnum-0.0.1.tar.gz` & `tmp/dcnum-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.1.tar", last modified: Fri Jun  2 21:57:19 2023, max compression
+gzip compressed data, was "dcnum-0.0.2.tar", last modified: Fri Jun  2 22:10:39 2023, max compression
```

## Comparing `dcnum-0.0.1.tar` & `dcnum-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.207189 dcnum-0.0.1/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.203190 dcnum-0.0.1/.github/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.203190 dcnum-0.0.1/.github/workflows/
--rw-rw-r--   0 paul      (1000) paul      (1000)     1669 2023-06-02 21:28:09.000000 dcnum-0.0.1/.github/workflows/check.yml
--rw-rw-r--   0 paul      (1000) paul      (1000)     1096 2023-06-02 21:28:36.000000 dcnum-0.0.1/.github/workflows/deploy_pypi.yml
--rw-rw-r--   0 paul      (1000) paul      (1000)     3096 2023-06-02 21:18:57.000000 dcnum-0.0.1/.gitignore
--rw-rw-r--   0 paul      (1000) paul      (1000)      199 2023-06-02 21:33:14.000000 dcnum-0.0.1/.readthedocs.yml
--rw-rw-r--   0 paul      (1000) paul      (1000)       22 2023-06-02 21:56:14.000000 dcnum-0.0.1/CHANGELOG
--rw-rw-r--   0 paul      (1000) paul      (1000)     1089 2023-06-02 21:11:26.000000 dcnum-0.0.1/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)     2089 2023-06-02 21:57:19.207189 dcnum-0.0.1/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     1291 2023-06-02 21:25:37.000000 dcnum-0.0.1/README.rst
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.203190 dcnum-0.0.1/dcnum/
--rw-rw-r--   0 paul      (1000) paul      (1000)       75 2023-06-02 21:53:50.000000 dcnum-0.0.1/dcnum/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)      160 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum/_version.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.207189 dcnum-0.0.1/dcnum.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     2089 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      441 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       61 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       22 2023-06-02 21:57:19.000000 dcnum-0.0.1/dcnum.egg-info/top_level.txt
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.207189 dcnum-0.0.1/docs/
--rw-rw-r--   0 paul      (1000) paul      (1000)     3022 2023-06-02 21:52:56.000000 dcnum-0.0.1/docs/conf.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.207189 dcnum-0.0.1/docs/extensions/
--rw-r--r--   0 paul      (1000) paul      (1000)     2375 2023-06-02 21:52:01.000000 dcnum-0.0.1/docs/extensions/github_changelog.py
--rw-rw-r--   0 paul      (1000) paul      (1000)      431 2023-06-02 21:46:40.000000 dcnum-0.0.1/docs/index.rst
--rw-rw-r--   0 paul      (1000) paul      (1000)       87 2023-06-02 21:53:09.000000 dcnum-0.0.1/docs/requirements.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1445 2023-06-02 21:18:38.000000 dcnum-0.0.1/pyproject.toml
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-06-02 21:57:19.207189 dcnum-0.0.1/setup.cfg
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-02 21:57:19.207189 dcnum-0.0.1/tests/
--rw-rw-r--   0 paul      (1000) paul      (1000)        7 2023-06-02 21:32:07.000000 dcnum-0.0.1/tests/requirements.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       73 2023-06-02 21:31:46.000000 dcnum-0.0.1/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.263626 dcnum-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.267626 dcnum-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 22:10:27.000000 dcnum-0.0.2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-02 22:10:27.000000 dcnum-0.0.2/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-02 22:10:27.000000 dcnum-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-02 22:10:27.000000 dcnum-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 22:10:27.000000 dcnum-0.0.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-02 22:10:27.000000 dcnum-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-02 22:10:39.271626 dcnum-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-02 22:10:27.000000 dcnum-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.267626 dcnum-0.0.2/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 22:10:27.000000 dcnum-0.0.2/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-02 22:10:27.000000 dcnum-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:10:39.271626 dcnum-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 22:10:27.000000 dcnum-0.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 22:10:27.000000 dcnum-0.0.2/tests/test_init.py
```

### Comparing `dcnum-0.0.1/.github/workflows/check.yml` & `dcnum-0.0.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.2/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/.gitignore` & `dcnum-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/LICENSE` & `dcnum-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/PKG-INFO` & `dcnum-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.1
+Version: 0.0.2
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
@@ -20,17 +20,15 @@
 
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for the post-measurement analysis of
-real-time deformability cytometry (RT-DC) datasets; an essential part of
-`Shape-Out <https://github.com/ZELLMECHANIK-DRESDEN/ShapeOut2>`__.
+This is a Python library for postprocessing deformability cytometry data.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.1/README.rst` & `dcnum-0.0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for the post-measurement analysis of
-real-time deformability cytometry (RT-DC) datasets; an essential part of
-`Shape-Out <https://github.com/ZELLMECHANIK-DRESDEN/ShapeOut2>`__.
+This is a Python library for postprocessing deformability cytometry data.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.1/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.2/dcnum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.1
+Version: 0.0.2
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
@@ -20,17 +20,15 @@
 
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for the post-measurement analysis of
-real-time deformability cytometry (RT-DC) datasets; an essential part of
-`Shape-Out <https://github.com/ZELLMECHANIK-DRESDEN/ShapeOut2>`__.
+This is a Python library for postprocessing deformability cytometry data.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.1/docs/conf.py` & `dcnum-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/docs/extensions/github_changelog.py` & `dcnum-0.0.2/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.1/pyproject.toml` & `dcnum-0.0.2/pyproject.toml`

 * *Files identical despite different names*

