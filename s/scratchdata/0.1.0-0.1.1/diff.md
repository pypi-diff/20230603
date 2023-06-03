# Comparing `tmp/scratchdata-0.1.0.tar.gz` & `tmp/scratchdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchdata-0.1.0.tar", last modified: Sat Jun  3 12:29:24 2023, max compression
+gzip compressed data, was "scratchdata-0.1.1.tar", last modified: Sat Jun  3 13:26:26 2023, max compression
```

## Comparing `scratchdata-0.1.0.tar` & `scratchdata-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 vyacheslavc.   (501) staff       (20)        0 2023-06-03 12:29:24.388282 scratchdata-0.1.0/
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)      535 2023-06-03 12:29:24.388178 scratchdata-0.1.0/PKG-INFO
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)       22 2023-06-02 15:39:27.000000 scratchdata-0.1.0/README.md
-drwxr-xr-x   0 vyacheslavc.   (501) staff       (20)        0 2023-06-03 12:29:24.388026 scratchdata-0.1.0/scratchdata.egg-info/
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)      535 2023-06-03 12:29:24.000000 scratchdata-0.1.0/scratchdata.egg-info/PKG-INFO
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)      192 2023-06-03 12:29:24.000000 scratchdata-0.1.0/scratchdata.egg-info/SOURCES.txt
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)        1 2023-06-03 12:29:24.000000 scratchdata-0.1.0/scratchdata.egg-info/dependency_links.txt
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)       14 2023-06-03 12:29:24.000000 scratchdata-0.1.0/scratchdata.egg-info/requires.txt
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)        1 2023-06-03 12:29:24.000000 scratchdata-0.1.0/scratchdata.egg-info/top_level.txt
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)       38 2023-06-03 12:29:24.388316 scratchdata-0.1.0/setup.cfg
--rw-r--r--   0 vyacheslavc.   (501) staff       (20)      713 2023-06-03 12:25:35.000000 scratchdata-0.1.0/setup.py
+drwxr-xr-x   0 vyacheslavc.   (501) staff       (20)        0 2023-06-03 13:26:26.420633 scratchdata-0.1.1/
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)      535 2023-06-03 13:26:26.420528 scratchdata-0.1.1/PKG-INFO
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)       22 2023-06-02 15:39:27.000000 scratchdata-0.1.1/README.md
+drwxr-xr-x   0 vyacheslavc.   (501) staff       (20)        0 2023-06-03 13:26:26.420381 scratchdata-0.1.1/scratchdata.egg-info/
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)      535 2023-06-03 13:26:26.000000 scratchdata-0.1.1/scratchdata.egg-info/PKG-INFO
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)      192 2023-06-03 13:26:26.000000 scratchdata-0.1.1/scratchdata.egg-info/SOURCES.txt
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)        1 2023-06-03 13:26:26.000000 scratchdata-0.1.1/scratchdata.egg-info/dependency_links.txt
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)        9 2023-06-03 13:26:26.000000 scratchdata-0.1.1/scratchdata.egg-info/requires.txt
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)        1 2023-06-03 13:26:26.000000 scratchdata-0.1.1/scratchdata.egg-info/top_level.txt
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)       38 2023-06-03 13:26:26.420674 scratchdata-0.1.1/setup.cfg
+-rw-r--r--   0 vyacheslavc.   (501) staff       (20)      705 2023-06-03 13:25:56.000000 scratchdata-0.1.1/setup.py
```

### Comparing `scratchdata-0.1.0/PKG-INFO` & `scratchdata-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for data from scratch
 Home-page: UNKNOWN
 Author: Vyacheslav C.
 Author-email: <vyacheslav_h@icloud.com>
 License: UNKNOWN
 Keywords: python,scratch,data,scraper
 Platform: UNKNOWN
```

### Comparing `scratchdata-0.1.0/scratchdata.egg-info/PKG-INFO` & `scratchdata-0.1.1/scratchdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for data from scratch
 Home-page: UNKNOWN
 Author: Vyacheslav C.
 Author-email: <vyacheslav_h@icloud.com>
 License: UNKNOWN
 Keywords: python,scratch,data,scraper
 Platform: UNKNOWN
```

### Comparing `scratchdata-0.1.0/setup.py` & `scratchdata-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Module for data from scratch'
 
 setup(
     name="scratchdata",
     version=VERSION,
     author="Vyacheslav C.",
     author_email="<vyacheslav_h@icloud.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'json'],
+    install_requires=['requests'],
     keywords=['python', 'scratch', 'data', 'scraper'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

