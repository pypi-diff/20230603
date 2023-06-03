# Comparing `tmp/metabolabpytools-0.8.13.tar.gz` & `tmp/metabolabpytools-0.8.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolabpytools-0.8.13.tar", last modified: Sat Jun  3 18:22:37 2023, max compression
+gzip compressed data, was "metabolabpytools-0.8.14.tar", last modified: Sat Jun  3 18:27:04 2023, max compression
```

## Comparing `metabolabpytools-0.8.13.tar` & `metabolabpytools-0.8.14.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:22:37.364024 metabolabpytools-0.8.13/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-05-22 20:46:08.000000 metabolabpytools-0.8.13/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:22:37.363884 metabolabpytools-0.8.13/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-05-28 14:07:17.000000 metabolabpytools-0.8.13/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:22:37.362585 metabolabpytools-0.8.13/metabolabpytools/
--rw-r--r--   0 ludwigc    (501) staff       (20)      154 2023-06-03 18:22:31.000000 metabolabpytools-0.8.13/metabolabpytools/__init__.py
--rw-r--r--   0 ludwigc    (501) staff       (20)     1893 2023-05-22 20:47:01.000000 metabolabpytools-0.8.13/metabolabpytools/analysis.py
--rw-r--r--   0 ludwigc    (501) staff       (20)     2568 2023-05-22 20:48:43.000000 metabolabpytools-0.8.13/metabolabpytools/isotopomerAnalysis.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:22:37.363671 metabolabpytools-0.8.13/metabolabpytools.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:22:37.000000 metabolabpytools-0.8.13/metabolabpytools.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      323 2023-06-03 18:22:37.000000 metabolabpytools-0.8.13/metabolabpytools.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-06-03 18:22:37.000000 metabolabpytools-0.8.13/metabolabpytools.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        7 2023-06-03 18:22:37.000000 metabolabpytools-0.8.13/metabolabpytools.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       17 2023-06-03 18:22:37.000000 metabolabpytools-0.8.13/metabolabpytools.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-06-03 18:22:37.364057 metabolabpytools-0.8.13/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     1507 2023-05-28 14:15:23.000000 metabolabpytools-0.8.13/setup.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.238984 metabolabpytools-0.8.14/
+-rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-05-22 20:46:08.000000 metabolabpytools-0.8.14/LICENSE
+-rw-r--r--   0 ludwigc    (501) staff       (20)       78 2023-06-03 18:26:27.000000 metabolabpytools-0.8.14/MANIFEST.in
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:27:04.238855 metabolabpytools-0.8.14/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)       67 2023-05-22 20:46:08.000000 metabolabpytools-0.8.14/README.md
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-05-28 14:07:17.000000 metabolabpytools-0.8.14/README.rst
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.237864 metabolabpytools-0.8.14/metabolabpytools/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      154 2023-06-03 18:26:47.000000 metabolabpytools-0.8.14/metabolabpytools/__init__.py
+-rw-r--r--   0 ludwigc    (501) staff       (20)     1893 2023-05-22 20:47:01.000000 metabolabpytools-0.8.14/metabolabpytools/analysis.py
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2568 2023-05-22 20:48:43.000000 metabolabpytools-0.8.14/metabolabpytools/isotopomerAnalysis.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.238666 metabolabpytools-0.8.14/metabolabpytools.egg-info/
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)      362 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/requires.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       17 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-06-03 18:26:57.000000 metabolabpytools-0.8.14/requirements.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-06-03 18:27:04.239017 metabolabpytools-0.8.14/setup.cfg
+-rw-r--r--   0 ludwigc    (501) staff       (20)     1507 2023-05-28 14:15:23.000000 metabolabpytools-0.8.14/setup.py
```

### Comparing `metabolabpytools-0.8.13/LICENSE` & `metabolabpytools-0.8.14/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.13/PKG-INFO` & `metabolabpytools-0.8.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.8.13
+Version: 0.8.14
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.8.13/README.rst` & `metabolabpytools-0.8.14/README.rst`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.13/metabolabpytools/analysis.py` & `metabolabpytools-0.8.14/metabolabpytools/analysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.13/metabolabpytools/isotopomerAnalysis.py` & `metabolabpytools-0.8.14/metabolabpytools/isotopomerAnalysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.13/metabolabpytools.egg-info/PKG-INFO` & `metabolabpytools-0.8.14/metabolabpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.8.13
+Version: 0.8.14
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.8.13/setup.py` & `metabolabpytools-0.8.14/setup.py`

 * *Files identical despite different names*

