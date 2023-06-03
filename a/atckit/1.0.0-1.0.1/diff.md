# Comparing `tmp/atckit-1.0.0.tar.gz` & `tmp/atckit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atckit-1.0.0.tar", last modified: Sat Jun  3 09:28:33 2023, max compression
+gzip compressed data, was "atckit-1.0.1.tar", last modified: Sat Jun  3 10:31:59 2023, max compression
```

## Comparing `atckit-1.0.0.tar` & `atckit-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 09:28:33.892273 atckit-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-03 09:08:12.000000 atckit-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.0/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-03 09:08:12.000000 atckit-1.0.0/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 09:28:33.892273 atckit-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-06-03 09:08:12.000000 atckit-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.0/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.0/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.0/icon.png
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-03 09:28:27.000000 atckit-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 09:28:33.892273 atckit-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 09:28:33.892273 atckit-1.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 09:26:52.000000 atckit-1.0.0/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 09:28:33.892273 atckit-1.0.0/src/atckit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 09:28:33.000000 atckit-1.0.0/src/atckit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-03 09:28:33.000000 atckit-1.0.0/src/atckit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 09:28:33.000000 atckit-1.0.0/src/atckit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 09:28:33.000000 atckit-1.0.0/src/atckit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-06-03 09:16:59.000000 atckit-1.0.0/src/subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-03 09:16:59.000000 atckit-1.0.0/src/utilfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.596177 atckit-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-03 09:08:12.000000 atckit-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.1/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.1/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-03 09:48:35.000000 atckit-1.0.1/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 10:31:59.592177 atckit-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-06-03 09:08:12.000000 atckit-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.1/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.1/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.1/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-03 10:31:52.000000 atckit-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 10:31:59.596177 atckit-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.548178 atckit-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.580178 atckit-1.0.1/src/atckit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 10:20:40.000000 atckit-1.0.1/src/atckit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-06-03 09:44:24.000000 atckit-1.0.1/src/atckit/subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-03 09:44:24.000000 atckit-1.0.1/src/atckit/utilfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.592177 atckit-1.0.1/src/atckit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/top_level.txt
```

### Comparing `atckit-1.0.0/.gitlab-ci.yml` & `atckit-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/.pylintrc` & `atckit-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/Doxyfile` & `atckit-1.0.1/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "AccidentallyTheCable's Utility Kit"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.0.0"
+PROJECT_NUMBER = "1.0.1"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `atckit-1.0.0/LICENSE.md` & `atckit-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/Makefile` & `atckit-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/PKG-INFO` & `atckit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.0.0
+Version: 1.0.1
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atckit-1.0.0/README.md` & `atckit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/git-tags.sh` & `atckit-1.0.1/git-tags.sh`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/icon.png` & `atckit-1.0.1/icon.png`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/pyproject.toml` & `atckit-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atckit"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "AccidentallyTheCable's Utility Kit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `atckit-1.0.0/src/atckit.egg-info/PKG-INFO` & `atckit-1.0.1/src/atckit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.0.0
+Version: 1.0.1
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atckit-1.0.0/src/subscriber.py` & `atckit-1.0.1/src/atckit/subscriber.py`

 * *Files identical despite different names*

### Comparing `atckit-1.0.0/src/utilfuncs.py` & `atckit-1.0.1/src/atckit/utilfuncs.py`

 * *Files identical despite different names*

