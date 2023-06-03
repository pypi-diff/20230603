# Comparing `tmp/pyasynchat-1.0.1.tar.gz` & `tmp/pyasynchat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyasynchat-1.0.1.tar", last modified: Thu Jun 30 06:04:27 2022, max compression
+gzip compressed data, was "pyasynchat-1.0.2.tar", last modified: Sat Jun  3 19:55:02 2023, max compression
```

## Comparing `pyasynchat-1.0.1.tar` & `pyasynchat-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/
--rwxr-xr-x   0 simon      (501) staff       (20)     2490 2022-06-29 19:12:29.000000 pyasynchat-1.0.1/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     2444 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/PKG-INFO
--rwxr-xr-x   0 simon      (501) staff       (20)     1914 2022-06-30 04:25:01.000000 pyasynchat-1.0.1/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/asynchat/
--rw-r--r--   0 simon      (501) staff       (20)       24 2022-06-29 20:00:59.000000 pyasynchat-1.0.1/asynchat/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    11321 2022-06-29 20:00:08.000000 pyasynchat-1.0.1/asynchat/asynchat.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2444 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      237 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       11 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/pyasynchat.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2022-06-30 06:04:27.000000 pyasynchat-1.0.1/setup.cfg
--rwxr-xr-x   0 simon      (501) staff       (20)     1477 2022-06-30 05:34:14.000000 pyasynchat-1.0.1/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:55:02.927803 pyasynchat-1.0.2/
+-rwxr-xr-x   0 simon      (501) staff       (20)     2490 2023-06-03 19:53:15.000000 pyasynchat-1.0.2/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     2442 2023-06-03 19:55:02.927716 pyasynchat-1.0.2/PKG-INFO
+-rwxr-xr-x   0 simon      (501) staff       (20)     1914 2023-06-03 19:53:15.000000 pyasynchat-1.0.2/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:55:02.927050 pyasynchat-1.0.2/asynchat/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-06-03 19:53:15.000000 pyasynchat-1.0.2/asynchat/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    11321 2023-06-03 19:53:15.000000 pyasynchat-1.0.2/asynchat/asynchat.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-03 19:55:02.927564 pyasynchat-1.0.2/pyasynchat.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2442 2023-06-03 19:55:02.000000 pyasynchat-1.0.2/pyasynchat.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      237 2023-06-03 19:55:02.000000 pyasynchat-1.0.2/pyasynchat.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-03 19:55:02.000000 pyasynchat-1.0.2/pyasynchat.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       11 2023-06-03 19:55:02.000000 pyasynchat-1.0.2/pyasynchat.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-03 19:55:02.000000 pyasynchat-1.0.2/pyasynchat.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-03 19:55:02.927838 pyasynchat-1.0.2/setup.cfg
+-rwxr-xr-x   0 simon      (501) staff       (20)     1246 2023-06-03 19:54:10.000000 pyasynchat-1.0.2/setup.py
```

### Comparing `pyasynchat-1.0.1/LICENSE` & `pyasynchat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasynchat-1.0.1/PKG-INFO` & `pyasynchat-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyasynchat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make asynchat available for Python 3.12 onwards
 Home-page: https://github.com/simonrob/pyasynchat
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Python Software Foundation License Version 2
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,9 +43,7 @@
 ## Maintenance
 Due to the fact that this module is [no-longer supported](https://peps.python.org/pep-0594/), no further maintenance of the code in [`asynchat.py`](asynchat/asynchat.py) is intended.
 This project is only intended to be updated to make changes or improvements to the module packaging.
 
 
 ## License
 [Python Software Foundation License Version 2](LICENSE)
-
-
```

### Comparing `pyasynchat-1.0.1/README.md` & `pyasynchat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyasynchat-1.0.1/asynchat/asynchat.py` & `pyasynchat-1.0.2/asynchat/asynchat.py`

 * *Files identical despite different names*

### Comparing `pyasynchat-1.0.1/pyasynchat.egg-info/PKG-INFO` & `pyasynchat-1.0.2/pyasynchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyasynchat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make asynchat available for Python 3.12 onwards
 Home-page: https://github.com/simonrob/pyasynchat
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Python Software Foundation License Version 2
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,9 +43,7 @@
 ## Maintenance
 Due to the fact that this module is [no-longer supported](https://peps.python.org/pep-0594/), no further maintenance of the code in [`asynchat.py`](asynchat/asynchat.py) is intended.
 This project is only intended to be updated to make changes or improvements to the module packaging.
 
 
 ## License
 [Python Software Foundation License Version 2](LICENSE)
-
-
```

### Comparing `pyasynchat-1.0.1/setup.py` & `pyasynchat-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from setuptools import setup
 import sys
 
-# TODO: test by `import asynchat` then removing/renaming the file at the location shown from `print(asynchat)`
-#  make sure to temporarily the version check below when testing; sys.modules shows currently loaded modules if needed
-
 # note: this check is not technically required as imports default to standard libraries where available, but it
 # ensures that we cannot cause any adverse effects where existing code is somehow reliant on behaviours of the
 # standard library asynchat module that are different to the one provided here
 packages = []
 if sys.version_info[0] == 3 and sys.version_info[1] >= 12:
     packages.append('asynchat')
 
 python_classifiers = ['Programming Language :: Python :: %s' % version for version in ['3.12']]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyasynchat',
-    version='1.0.1',
+    version='1.0.2',
     description='Make asynchat available for Python 3.12 onwards',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Simon Robinson',
     author_email='simon@robinson.ac',
     url='https://github.com/simonrob/pyasynchat',
```

