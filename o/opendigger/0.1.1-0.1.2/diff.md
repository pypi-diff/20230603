# Comparing `tmp/opendigger-0.1.1.tar.gz` & `tmp/opendigger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendigger-0.1.1.tar", last modified: Sat Jun  3 11:02:22 2023, max compression
+gzip compressed data, was "opendigger-0.1.2.tar", last modified: Sat Jun  3 11:11:06 2023, max compression
```

## Comparing `opendigger-0.1.1.tar` & `opendigger-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:02:22.623662 opendigger-0.1.1/
--rw-r--r--   0 tangyue    (501) staff       (20)     1068 2023-06-02 11:20:46.000000 opendigger-0.1.1/LICENSE
--rw-r--r--   0 tangyue    (501) staff       (20)       33 2023-06-02 11:15:07.000000 opendigger-0.1.1/MANIFEST.in
--rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:02:22.623309 opendigger-0.1.1/PKG-INFO
--rw-r--r--   0 tangyue    (501) staff       (20)        0 2023-06-02 11:19:50.000000 opendigger-0.1.1/README.md
-drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:02:22.623089 opendigger-0.1.1/opendigger.egg-info/
--rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/PKG-INFO
--rw-r--r--   0 tangyue    (501) staff       (20)      244 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/SOURCES.txt
--rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/dependency_links.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       47 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/entry_points.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       25 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/requires.txt
--rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:02:22.000000 opendigger-0.1.1/opendigger.egg-info/top_level.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       38 2023-06-03 11:02:22.623719 opendigger-0.1.1/setup.cfg
--rw-r--r--   0 tangyue    (501) staff       (20)      905 2023-06-03 11:01:11.000000 opendigger-0.1.1/setup.py
+drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:11:06.555234 opendigger-0.1.2/
+-rw-r--r--   0 tangyue    (501) staff       (20)     1068 2023-06-02 11:20:46.000000 opendigger-0.1.2/LICENSE
+-rw-r--r--   0 tangyue    (501) staff       (20)       33 2023-06-02 11:15:07.000000 opendigger-0.1.2/MANIFEST.in
+-rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:11:06.554875 opendigger-0.1.2/PKG-INFO
+-rw-r--r--   0 tangyue    (501) staff       (20)        0 2023-06-02 11:19:50.000000 opendigger-0.1.2/README.md
+drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:11:06.554647 opendigger-0.1.2/opendigger.egg-info/
+-rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/PKG-INFO
+-rw-r--r--   0 tangyue    (501) staff       (20)      244 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/SOURCES.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/dependency_links.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       47 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/entry_points.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       25 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/requires.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:11:06.000000 opendigger-0.1.2/opendigger.egg-info/top_level.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       38 2023-06-03 11:11:06.555292 opendigger-0.1.2/setup.cfg
+-rw-r--r--   0 tangyue    (501) staff       (20)      905 2023-06-03 11:11:01.000000 opendigger-0.1.2/setup.py
```

### Comparing `opendigger-0.1.1/LICENSE` & `opendigger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opendigger-0.1.1/PKG-INFO` & `opendigger-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendigger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool for fetching OpenDigger metrics
 Home-page: https://github.com/TOMYUE/opendigger-cli
 Author: TOMYUE
 Author-email: tomyue2002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opendigger-0.1.1/opendigger.egg-info/PKG-INFO` & `opendigger-0.1.2/opendigger.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendigger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool for fetching OpenDigger metrics
 Home-page: https://github.com/TOMYUE/opendigger-cli
 Author: TOMYUE
 Author-email: tomyue2002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opendigger-0.1.1/setup.py` & `opendigger-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opendigger",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "plotext",
         "matplotlib",
     ],
     entry_points={
```

