# Comparing `tmp/azurisorting-0.0.2.tar.gz` & `tmp/azurisorting-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurisorting-0.0.2.tar", last modified: Sat Jun  3 12:35:08 2023, max compression
+gzip compressed data, was "azurisorting-0.0.3.tar", last modified: Sat Jun  3 12:41:58 2023, max compression
```

## Comparing `azurisorting-0.0.2.tar` & `azurisorting-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.617834 azurisorting-0.0.2/
--rw-r--r--   0 azure     (1000) azure     (1000)      940 2023-06-03 12:35:08.615834 azurisorting-0.0.2/PKG-INFO
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.610834 azurisorting-0.0.2/azurisorting/
--rw-r--r--   0 azure     (1000) azure     (1000)     1013 2023-05-31 12:08:43.000000 azurisorting-0.0.2/azurisorting/ACS.py
--rw-r--r--   0 azure     (1000) azure     (1000)     1299 2023-06-03 12:31:42.000000 azurisorting-0.0.2/azurisorting/AFS.py
--rw-r--r--   0 azure     (1000) azure     (1000)     1785 2023-05-31 12:08:52.000000 azurisorting-0.0.2/azurisorting/AS.py
--rw-r--r--   0 azure     (1000) azure     (1000)       52 2023-06-03 12:32:15.000000 azurisorting-0.0.2/azurisorting/__init__.py
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.614834 azurisorting-0.0.2/azurisorting.egg-info/
--rw-r--r--   0 azure     (1000) azure     (1000)      940 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/PKG-INFO
--rw-r--r--   0 azure     (1000) azure     (1000)      236 2023-06-03 12:35:08.000000 azurisorting-0.0.2/azurisorting.egg-info/SOURCES.txt
--rw-r--r--   0 azure     (1000) azure     (1000)        1 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/dependency_links.txt
--rw-r--r--   0 azure     (1000) azure     (1000)       13 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/top_level.txt
--rw-r--r--   0 azure     (1000) azure     (1000)       38 2023-06-03 12:35:08.617834 azurisorting-0.0.2/setup.cfg
--rw-r--r--   0 azure     (1000) azure     (1000)     1405 2023-06-03 12:34:11.000000 azurisorting-0.0.2/setup.py
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:41:58.148821 azurisorting-0.0.3/
+-rw-r--r--   0 azure     (1000) azure     (1000)      960 2023-06-03 12:41:58.146821 azurisorting-0.0.3/PKG-INFO
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:41:58.141821 azurisorting-0.0.3/azurisorting/
+-rw-r--r--   0 azure     (1000) azure     (1000)      130 2023-06-03 12:39:10.000000 azurisorting-0.0.3/azurisorting/__init__.py
+-rw-r--r--   0 azure     (1000) azure     (1000)     1013 2023-05-31 12:08:43.000000 azurisorting-0.0.3/azurisorting/azuricorrectivesorter.py
+-rw-r--r--   0 azure     (1000) azure     (1000)     1299 2023-06-03 12:31:42.000000 azurisorting-0.0.3/azurisorting/azurifastsorter.py
+-rw-r--r--   0 azure     (1000) azure     (1000)     1785 2023-05-31 12:08:52.000000 azurisorting-0.0.3/azurisorting/azurisorter.py
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:41:58.144822 azurisorting-0.0.3/azurisorting.egg-info/
+-rw-r--r--   0 azure     (1000) azure     (1000)      960 2023-06-03 12:41:57.000000 azurisorting-0.0.3/azurisorting.egg-info/PKG-INFO
+-rw-r--r--   0 azure     (1000) azure     (1000)      275 2023-06-03 12:41:57.000000 azurisorting-0.0.3/azurisorting.egg-info/SOURCES.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)        1 2023-06-03 12:41:57.000000 azurisorting-0.0.3/azurisorting.egg-info/dependency_links.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)       13 2023-06-03 12:41:57.000000 azurisorting-0.0.3/azurisorting.egg-info/top_level.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)       38 2023-06-03 12:41:58.148821 azurisorting-0.0.3/setup.cfg
+-rw-r--r--   0 azure     (1000) azure     (1000)     1425 2023-06-03 12:41:31.000000 azurisorting-0.0.3/setup.py
```

### Comparing `azurisorting-0.0.2/PKG-INFO` & `azurisorting-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: azurisorting
-Version: 0.0.2
+Version: 0.0.3
 Summary: This sorter is used to sort datasets based on their ASCII Position.
 Home-page: UNKNOWN
 Author: Nathan Hornby
 Author-email: alexmybestcat@gmail.com
 License: UNKNOWN
 Description: These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy.
-        Fixes: Fixed Major error in which causes the package to be unusable.
+        Fixes: Fixed Major error in which causes the package to be unusable. Attempts to fix: #2
 Keywords: python,sorter,quick sorter,sort,fast sort,fast,corrective sorter,corrective,auto sorter,auto,easy sorter,easy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `azurisorting-0.0.2/azurisorting/ACS.py` & `azurisorting-0.0.3/azurisorting/azuricorrectivesorter.py`

 * *Files identical despite different names*

### Comparing `azurisorting-0.0.2/azurisorting/AFS.py` & `azurisorting-0.0.3/azurisorting/azurifastsorter.py`

 * *Files identical despite different names*

### Comparing `azurisorting-0.0.2/azurisorting/AS.py` & `azurisorting-0.0.3/azurisorting/azurisorter.py`

 * *Files identical despite different names*

### Comparing `azurisorting-0.0.2/azurisorting.egg-info/PKG-INFO` & `azurisorting-0.0.3/azurisorting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: azurisorting
-Version: 0.0.2
+Version: 0.0.3
 Summary: This sorter is used to sort datasets based on their ASCII Position.
 Home-page: UNKNOWN
 Author: Nathan Hornby
 Author-email: alexmybestcat@gmail.com
 License: UNKNOWN
 Description: These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy.
-        Fixes: Fixed Major error in which causes the package to be unusable.
+        Fixes: Fixed Major error in which causes the package to be unusable. Attempts to fix: #2
 Keywords: python,sorter,quick sorter,sort,fast sort,fast,corrective sorter,corrective,auto sorter,auto,easy sorter,easy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `azurisorting-0.0.2/setup.py` & `azurisorting-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'This sorter is used to sort datasets based on their ASCII Position.'
-LONG_DESCRIPTION = "These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy.\nFixes: Fixed Major error in which causes the package to be unusable."
+LONG_DESCRIPTION = "These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy.\nFixes: Fixed Major error in which causes the package to be unusable. Attempts to fix: #2"
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="azurisorting", 
         version=VERSION,
         author="Nathan Hornby",
```

