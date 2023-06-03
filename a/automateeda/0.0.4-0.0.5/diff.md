# Comparing `tmp/automateeda-0.0.4.tar.gz` & `tmp/automateeda-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automateeda-0.0.4.tar", last modified: Sat Jun  3 04:59:26 2023, max compression
+gzip compressed data, was "automateeda-0.0.5.tar", last modified: Sat Jun  3 05:05:50 2023, max compression
```

## Comparing `automateeda-0.0.4.tar` & `automateeda-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 04:59:26.984017 automateeda-0.0.4/
--rw-rw-rw-   0        0        0      800 2023-06-03 04:59:26.983024 automateeda-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 04:59:26.959449 automateeda-0.0.4/automateeda/
--rw-rw-rw-   0        0        0      255 2023-06-03 04:57:40.000000 automateeda-0.0.4/automateeda/__init__.py
--rw-rw-rw-   0        0        0     5595 2023-05-29 18:00:59.000000 automateeda-0.0.4/automateeda/automateeda.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:59:26.981017 automateeda-0.0.4/automateeda.egg-info/
--rw-rw-rw-   0        0        0      800 2023-06-03 04:59:26.000000 automateeda-0.0.4/automateeda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-03 04:59:26.000000 automateeda-0.0.4/automateeda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 04:59:26.000000 automateeda-0.0.4/automateeda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-03 04:59:26.000000 automateeda-0.0.4/automateeda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 04:59:26.000000 automateeda-0.0.4/automateeda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 04:59:26.984017 automateeda-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-06-03 04:57:54.000000 automateeda-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:50.231505 automateeda-0.0.5/
+-rw-rw-rw-   0        0        0      800 2023-06-03 05:05:50.230505 automateeda-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:50.199929 automateeda-0.0.5/automateeda/
+-rw-rw-rw-   0        0        0      260 2023-06-03 05:04:14.000000 automateeda-0.0.5/automateeda/__init__.py
+-rw-rw-rw-   0        0        0     5595 2023-05-29 18:00:59.000000 automateeda-0.0.5/automateeda/automateeda.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:50.229504 automateeda-0.0.5/automateeda.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-06-03 05:05:50.000000 automateeda-0.0.5/automateeda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-03 05:05:50.000000 automateeda-0.0.5/automateeda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:05:50.000000 automateeda-0.0.5/automateeda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-03 05:05:50.000000 automateeda-0.0.5/automateeda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 05:05:50.000000 automateeda-0.0.5/automateeda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:05:50.231505 automateeda-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-06-03 05:05:44.000000 automateeda-0.0.5/setup.py
```

### Comparing `automateeda-0.0.4/PKG-INFO` & `automateeda-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automateeda
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic insight generator - EDA
 Author: Hirshikesh karan Ahilan
 Author-email: hirshiahilan2003@gmail.com
 Keywords: python,automate,automate eda,eda,analysis,data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `automateeda-0.0.4/automateeda/automateeda.py` & `automateeda-0.0.5/automateeda/automateeda.py`

 * *Files identical despite different names*

### Comparing `automateeda-0.0.4/automateeda.egg-info/PKG-INFO` & `automateeda-0.0.5/automateeda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automateeda
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic insight generator - EDA
 Author: Hirshikesh karan Ahilan
 Author-email: hirshiahilan2003@gmail.com
 Keywords: python,automate,automate eda,eda,analysis,data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `automateeda-0.0.4/setup.py` & `automateeda-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Basic insight generator - EDA'
 LONG_DESCRIPTION = 'This package automates and gives you basic visualization of the data, before using the package please install the required lib, the list of lib are mentioned in the __init__.py file in the git hub - https://github.com/Hirshikesh2003/Automate_EDA'
 
 # Setting up
 setup(
     name="automateeda",
     version=VERSION,
```

