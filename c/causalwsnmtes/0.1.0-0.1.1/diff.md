# Comparing `tmp/causalwsnmtes-0.1.0.tar.gz` & `tmp/causalwsnmtes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalwsnmtes-0.1.0.tar", last modified: Sat Jun  3 04:15:57 2023, max compression
+gzip compressed data, was "causalwsnmtes-0.1.1.tar", last modified: Sat Jun  3 04:44:57 2023, max compression
```

## Comparing `causalwsnmtes-0.1.0.tar` & `causalwsnmtes-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.465196 causalwsnmtes-0.1.0/
--rw-r--r--   0 macbook    (501) staff       (20)     6148 2023-06-03 04:07:08.000000 causalwsnmtes-0.1.0/.DS_Store
--rw-r--r--   0 macbook    (501) staff       (20)      292 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/.editorconfig
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.312726 causalwsnmtes-0.1.0/.github/
--rw-r--r--   0 macbook    (501) staff       (20)      324 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 macbook    (501) staff       (20)     1204 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/.gitignore
--rw-r--r--   0 macbook    (501) staff       (20)      681 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/.travis.yml
--rw-r--r--   0 macbook    (501) staff       (20)      150 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/AUTHORS.rst
--rw-r--r--   0 macbook    (501) staff       (20)     3480 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 macbook    (501) staff       (20)       89 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/HISTORY.rst
--rw-r--r--   0 macbook    (501) staff       (20)     1065 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)      262 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)     2346 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/Makefile
--rw-r--r--   0 macbook    (501) staff       (20)     1754 2023-06-03 04:15:57.465474 causalwsnmtes-0.1.0/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      973 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/README.rst
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.317288 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     1754 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      893 2023-06-03 04:15:57.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       57 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/not-zip-safe
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.0/causalwsnmtes.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.386064 causalwsnmtes-0.1.0/docs/
--rw-r--r--   0 macbook    (501) staff       (20)      604 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/Makefile
--rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/authors.rst
--rwxr-xr-x   0 macbook    (501) staff       (20)     4755 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/conf.py
--rw-r--r--   0 macbook    (501) staff       (20)       33 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/contributing.rst
--rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/history.rst
--rw-r--r--   0 macbook    (501) staff       (20)      310 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/index.rst
--rw-r--r--   0 macbook    (501) staff       (20)     1112 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/installation.rst
--rw-r--r--   0 macbook    (501) staff       (20)      765 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/make.bat
--rw-r--r--   0 macbook    (501) staff       (20)       27 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/readme.rst
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/docs/usage.rst
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/make.bat
--rw-r--r--   0 macbook    (501) staff       (20)      174 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/requirements_dev.txt
--rw-r--r--   0 macbook    (501) staff       (20)      420 2023-06-03 04:15:57.470585 causalwsnmtes-0.1.0/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1407 2023-06-03 04:15:31.000000 causalwsnmtes-0.1.0/setup.py
--rw-r--r--   0 macbook    (501) staff       (20)      144 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/shorts.sh
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.396963 causalwsnmtes-0.1.0/source/
--rw-r--r--   0 macbook    (501) staff       (20)     2149 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/source/conf.py
--rw-r--r--   0 macbook    (501) staff       (20)      425 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/source/index.rst
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.428340 causalwsnmtes-0.1.0/tests/
--rw-r--r--   0 macbook    (501) staff       (20)       33 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      943 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/tests/test_CPE.py
--rw-r--r--   0 macbook    (501) staff       (20)      534 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/tox.ini
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:15:57.455349 causalwsnmtes-0.1.0/transformersapp/
--rw-r--r--   0 macbook    (501) staff       (20)      125 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      373 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/cli.py
--rw-r--r--   0 macbook    (501) staff       (20)     1217 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/huggingface.py
--rw-r--r--   0 macbook    (501) staff       (20)     1912 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/main.py
--rw-r--r--   0 macbook    (501) staff       (20)     1738 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/timeseriesforecastor
--rw-r--r--   0 macbook    (501) staff       (20)     1999 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.0/transformersapp/woringtransfoemer.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.730626 causalwsnmtes-0.1.1/
+-rw-r--r--   0 macbook    (501) staff       (20)     6148 2023-06-03 04:07:08.000000 causalwsnmtes-0.1.1/.DS_Store
+-rw-r--r--   0 macbook    (501) staff       (20)      292 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/.editorconfig
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.647037 causalwsnmtes-0.1.1/.github/
+-rw-r--r--   0 macbook    (501) staff       (20)      324 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 macbook    (501) staff       (20)     1204 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/.gitignore
+-rw-r--r--   0 macbook    (501) staff       (20)      681 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/.travis.yml
+-rw-r--r--   0 macbook    (501) staff       (20)      150 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/AUTHORS.rst
+-rw-r--r--   0 macbook    (501) staff       (20)     3480 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 macbook    (501) staff       (20)       89 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/HISTORY.rst
+-rw-r--r--   0 macbook    (501) staff       (20)     1065 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)      262 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)     2346 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/Makefile
+-rw-r--r--   0 macbook    (501) staff       (20)     1754 2023-06-03 04:44:57.730839 causalwsnmtes-0.1.1/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      973 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/README.rst
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.667111 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     1754 2023-06-03 04:44:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      893 2023-06-03 04:44:57.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:44:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       57 2023-06-03 04:44:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:15:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/not-zip-safe
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-03 04:44:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-03 04:44:56.000000 causalwsnmtes-0.1.1/causalwsnmtes.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.702925 causalwsnmtes-0.1.1/docs/
+-rw-r--r--   0 macbook    (501) staff       (20)      604 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/Makefile
+-rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 macbook    (501) staff       (20)     4755 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/conf.py
+-rw-r--r--   0 macbook    (501) staff       (20)       33 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/contributing.rst
+-rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/history.rst
+-rw-r--r--   0 macbook    (501) staff       (20)      310 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/index.rst
+-rw-r--r--   0 macbook    (501) staff       (20)     1112 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/installation.rst
+-rw-r--r--   0 macbook    (501) staff       (20)      765 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/make.bat
+-rw-r--r--   0 macbook    (501) staff       (20)       27 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/readme.rst
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/docs/usage.rst
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/make.bat
+-rw-r--r--   0 macbook    (501) staff       (20)      174 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/requirements_dev.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      420 2023-06-03 04:44:57.731778 causalwsnmtes-0.1.1/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1407 2023-06-03 04:44:40.000000 causalwsnmtes-0.1.1/setup.py
+-rw-r--r--   0 macbook    (501) staff       (20)      144 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/shorts.sh
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.713655 causalwsnmtes-0.1.1/source/
+-rw-r--r--   0 macbook    (501) staff       (20)     2149 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/source/conf.py
+-rw-r--r--   0 macbook    (501) staff       (20)      425 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/source/index.rst
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.720256 causalwsnmtes-0.1.1/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)       33 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      943 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/tests/test_CPE.py
+-rw-r--r--   0 macbook    (501) staff       (20)      534 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/tox.ini
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-03 04:44:57.729614 causalwsnmtes-0.1.1/transformersapp/
+-rw-r--r--   0 macbook    (501) staff       (20)      125 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      373 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/cli.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1217 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/huggingface.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1912 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/main.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1738 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/timeseriesforecastor
+-rw-r--r--   0 macbook    (501) staff       (20)     1999 2023-06-03 04:03:31.000000 causalwsnmtes-0.1.1/transformersapp/woringtransfoemer.py
```

### Comparing `causalwsnmtes-0.1.0/.DS_Store` & `causalwsnmtes-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/.gitignore` & `causalwsnmtes-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/.travis.yml` & `causalwsnmtes-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/CONTRIBUTING.rst` & `causalwsnmtes-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/LICENSE` & `causalwsnmtes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/Makefile` & `causalwsnmtes-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/PKG-INFO` & `causalwsnmtes-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalwsnmtes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Testing the Cookiecutter
 Home-page: https://github.com/apargc61/causalwsnmtes
 Author: Apar C
 Author-email: apargc61@gmail.com
 License: MIT license
 Keywords: causalwsnmtes
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `causalwsnmtes-0.1.0/README.rst` & `causalwsnmtes-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/causalwsnmtes.egg-info/PKG-INFO` & `causalwsnmtes-0.1.1/causalwsnmtes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalwsnmtes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Testing the Cookiecutter
 Home-page: https://github.com/apargc61/causalwsnmtes
 Author: Apar C
 Author-email: apargc61@gmail.com
 License: MIT license
 Keywords: causalwsnmtes
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `causalwsnmtes-0.1.0/causalwsnmtes.egg-info/SOURCES.txt` & `causalwsnmtes-0.1.1/causalwsnmtes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/docs/Makefile` & `causalwsnmtes-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/docs/conf.py` & `causalwsnmtes-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/docs/installation.rst` & `causalwsnmtes-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/docs/make.bat` & `causalwsnmtes-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/make.bat` & `causalwsnmtes-0.1.1/make.bat`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/setup.py` & `causalwsnmtes-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="causalwsnmtes",
     name="causalwsnmtes",
     packages=find_packages(include=["causalwsnmtes", "causalwsnmtes.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/apargc61/causalwsnmtes",
-    version="0.1.0",
+    version="0.1.1",
     zip_safe=False,
 )
```

### Comparing `causalwsnmtes-0.1.0/source/conf.py` & `causalwsnmtes-0.1.1/source/conf.py`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/tests/test_CPE.py` & `causalwsnmtes-0.1.1/tests/test_CPE.py`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/tox.ini` & `causalwsnmtes-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/transformersapp/huggingface.py` & `causalwsnmtes-0.1.1/transformersapp/huggingface.py`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/transformersapp/main.py` & `causalwsnmtes-0.1.1/transformersapp/main.py`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/transformersapp/timeseriesforecastor` & `causalwsnmtes-0.1.1/transformersapp/timeseriesforecastor`

 * *Files identical despite different names*

### Comparing `causalwsnmtes-0.1.0/transformersapp/woringtransfoemer.py` & `causalwsnmtes-0.1.1/transformersapp/woringtransfoemer.py`

 * *Files identical despite different names*

