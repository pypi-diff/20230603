# Comparing `tmp/automateeda-0.0.1.tar.gz` & `tmp/automateeda-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automateeda-0.0.1.tar", last modified: Sat Jun  3 03:46:02 2023, max compression
+gzip compressed data, was "automateeda-0.0.2.tar", last modified: Sat Jun  3 04:39:22 2023, max compression
```

## Comparing `automateeda-0.0.1.tar` & `automateeda-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 03:46:02.792698 automateeda-0.0.1/
--rw-rw-rw-   0        0        0      800 2023-06-03 03:46:02.791700 automateeda-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 03:46:02.765852 automateeda-0.0.1/automateeda/
--rw-rw-rw-   0        0        0      219 2023-05-29 18:00:56.000000 automateeda-0.0.1/automateeda/__init__.py
--rw-rw-rw-   0        0        0     5595 2023-05-29 18:00:59.000000 automateeda-0.0.1/automateeda/automateeda.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:46:02.790698 automateeda-0.0.1/automateeda.egg-info/
--rw-rw-rw-   0        0        0      800 2023-06-03 03:46:02.000000 automateeda-0.0.1/automateeda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-03 03:46:02.000000 automateeda-0.0.1/automateeda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 03:46:02.000000 automateeda-0.0.1/automateeda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-03 03:46:02.000000 automateeda-0.0.1/automateeda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 03:46:02.000000 automateeda-0.0.1/automateeda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 03:46:02.792698 automateeda-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-05-29 18:39:21.000000 automateeda-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:39:21.998648 automateeda-0.0.2/
+-rw-rw-rw-   0        0        0      800 2023-06-03 04:39:21.997649 automateeda-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 04:39:21.979462 automateeda-0.0.2/automateeda/
+-rw-rw-rw-   0        0        0      219 2023-05-29 18:00:56.000000 automateeda-0.0.2/automateeda/__init__.py
+-rw-rw-rw-   0        0        0     5595 2023-05-29 18:00:59.000000 automateeda-0.0.2/automateeda/automateeda.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:39:21.996641 automateeda-0.0.2/automateeda.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-06-03 04:39:21.000000 automateeda-0.0.2/automateeda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-03 04:39:21.000000 automateeda-0.0.2/automateeda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 04:39:21.000000 automateeda-0.0.2/automateeda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-03 04:39:21.000000 automateeda-0.0.2/automateeda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 04:39:21.000000 automateeda-0.0.2/automateeda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 04:39:21.998648 automateeda-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2023-06-03 04:39:02.000000 automateeda-0.0.2/setup.py
```

### Comparing `automateeda-0.0.1/PKG-INFO` & `automateeda-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automateeda
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic insight generator - EDA
 Author: Hirshikesh karan Ahilan
 Author-email: hirshiahilan2003@gmail.com
 Keywords: python,automate,automate eda,eda,analysis,data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `automateeda-0.0.1/automateeda/automateeda.py` & `automateeda-0.0.2/automateeda/automateeda.py`

 * *Files identical despite different names*

### Comparing `automateeda-0.0.1/automateeda.egg-info/PKG-INFO` & `automateeda-0.0.2/automateeda.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automateeda
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic insight generator - EDA
 Author: Hirshikesh karan Ahilan
 Author-email: hirshiahilan2003@gmail.com
 Keywords: python,automate,automate eda,eda,analysis,data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `automateeda-0.0.1/setup.py` & `automateeda-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Basic insight generator - EDA'
 LONG_DESCRIPTION = 'This package automates and gives you basic visualization of the data, before using the package please install the required lib, the list of lib are mentioned in the __init__.py file in the git hub - https://github.com/Hirshikesh2003/Automate_EDA'
 
 # Setting up
 setup(
     name="automateeda",
     version=VERSION,
     author="Hirshikesh karan Ahilan",
     author_email="hirshiahilan2003@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pandas' , 'numpy', 'matplotlib.pyplot', 'seaborn', 'plotly.express' , 'ipywidgets'],
+    install_requires=['pandas' , 'numpy', 'matplotlib', 'seaborn', 'plotly.express' , 'ipywidgets'],
     keywords=['python', 'automate', 'automate eda', 'eda', 'analysis', 'data analysis'],
     
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Education',
         'Operating System :: Microsoft :: Windows :: Windows 10',
         'License :: OSI Approved :: MIT License',
```

