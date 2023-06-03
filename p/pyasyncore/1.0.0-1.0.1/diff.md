# Comparing `tmp/pyasyncore-1.0.0.tar.gz` & `tmp/pyasyncore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyasyncore-1.0.0.tar", last modified: Wed Jun 29 19:52:44 2022, max compression
+gzip compressed data, was "pyasyncore-1.0.1.tar", last modified: Sat Jun  3 19:31:39 2023, max compression
```

## Comparing `pyasyncore-1.0.0.tar` & `pyasyncore-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/
--rwxr-xr-x   0 simon      (501) staff       (20)     2490 2022-06-29 19:12:29.000000 pyasyncore-1.0.0/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     2494 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/PKG-INFO
--rwxr-xr-x   0 simon      (501) staff       (20)     1964 2022-06-29 19:44:47.000000 pyasyncore-1.0.0/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/pyasyncore.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/pyasyncore.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      162 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/pyasyncore.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/pyasyncore.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/pyasyncore.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2022-06-29 19:52:44.000000 pyasyncore-1.0.0/setup.cfg
--rwxr-xr-x   0 simon      (501) staff       (20)     1209 2022-06-29 19:51:57.000000 pyasyncore-1.0.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:31:39.213824 pyasyncore-1.0.1/
+-rwxr-xr-x   0 simon      (501) staff       (20)     2490 2022-06-29 19:54:16.000000 pyasyncore-1.0.1/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     2492 2023-06-03 19:31:39.213741 pyasyncore-1.0.1/PKG-INFO
+-rwxr-xr-x   0 simon      (501) staff       (20)     1964 2022-06-29 19:54:16.000000 pyasyncore-1.0.1/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:31:39.213176 pyasyncore-1.0.1/asyncore/
+-rw-rw-r--   0 simon      (501) staff       (20)       24 2022-06-29 19:54:16.000000 pyasyncore-1.0.1/asyncore/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    20086 2022-06-29 19:54:16.000000 pyasyncore-1.0.1/asyncore/asyncore.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:31:39.213588 pyasyncore-1.0.1/pyasyncore.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2492 2023-06-03 19:31:39.000000 pyasyncore-1.0.1/pyasyncore.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      204 2023-06-03 19:31:39.000000 pyasyncore-1.0.1/pyasyncore.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-03 19:31:39.000000 pyasyncore-1.0.1/pyasyncore.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-03 19:31:39.000000 pyasyncore-1.0.1/pyasyncore.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-03 19:31:39.213853 pyasyncore-1.0.1/setup.cfg
+-rwxr-xr-x   0 simon      (501) staff       (20)     1209 2023-06-03 19:30:30.000000 pyasyncore-1.0.1/setup.py
```

### Comparing `pyasyncore-1.0.0/LICENSE` & `pyasyncore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasyncore-1.0.0/PKG-INFO` & `pyasyncore-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyasyncore
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make asyncore available for Python 3.12 onwards
 Home-page: https://github.com/simonrob/pyasyncore
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Python Software Foundation License Version 2
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,9 +43,7 @@
 ## Maintenance
 Due to the fact that this module is [no-longer supported](https://peps.python.org/pep-0594/), no further maintenance of the code in [`asyncore.py`](asyncore/asyncore.py) is intended.
 This project is only intended to be updated to make changes or improvements to the module packaging.
 
 
 ## License
 [Python Software Foundation License Version 2](LICENSE)
-
-
```

### Comparing `pyasyncore-1.0.0/README.md` & `pyasyncore-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyasyncore-1.0.0/pyasyncore.egg-info/PKG-INFO` & `pyasyncore-1.0.1/pyasyncore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyasyncore
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make asyncore available for Python 3.12 onwards
 Home-page: https://github.com/simonrob/pyasyncore
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Python Software Foundation License Version 2
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,9 +43,7 @@
 ## Maintenance
 Due to the fact that this module is [no-longer supported](https://peps.python.org/pep-0594/), no further maintenance of the code in [`asyncore.py`](asyncore/asyncore.py) is intended.
 This project is only intended to be updated to make changes or improvements to the module packaging.
 
 
 ## License
 [Python Software Foundation License Version 2](LICENSE)
-
-
```

### Comparing `pyasyncore-1.0.0/setup.py` & `pyasyncore-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 python_classifiers = ['Programming Language :: Python :: %s' % version for version in ['3.12']]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyasyncore',
-    version='1.0.0',
+    version='1.0.1',
     description='Make asyncore available for Python 3.12 onwards',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Simon Robinson',
     author_email='simon@robinson.ac',
     url='https://github.com/simonrob/pyasyncore',
```

