# Comparing `tmp/cncd_package-0.3.4.tar.gz` & `tmp/cncd_package-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cncd_package-0.3.4.tar", last modified: Sat Jun  3 09:06:01 2023, max compression
+gzip compressed data, was "cncd_package-0.3.5.tar", last modified: Sat Jun  3 09:38:42 2023, max compression
```

## Comparing `cncd_package-0.3.4.tar` & `cncd_package-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.532954 cncd_package-0.3.4/
--rw-rw-rw-   0        0        0     9376 2023-06-03 09:06:01.532954 cncd_package-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.517329 cncd_package-0.3.4/cncd_package/
--rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.4/cncd_package/QC.py
--rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.4/cncd_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.532954 cncd_package-0.3.4/cncd_package.egg-info/
--rw-rw-rw-   0        0        0     9376 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 09:06:01.532954 cncd_package-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1388 2023-06-03 09:05:27.000000 cncd_package-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:38:42.215386 cncd_package-0.3.5/
+-rw-rw-rw-   0        0        0     9377 2023-06-03 09:38:42.215386 cncd_package-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 09:38:42.199294 cncd_package-0.3.5/cncd_package/
+-rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.5/cncd_package/QC.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.5/cncd_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:38:42.214383 cncd_package-0.3.5/cncd_package.egg-info/
+-rw-rw-rw-   0        0        0     9377 2023-06-03 09:38:42.000000 cncd_package-0.3.5/cncd_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-03 09:38:42.000000 cncd_package-0.3.5/cncd_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:38:42.000000 cncd_package-0.3.5/cncd_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 09:38:42.000000 cncd_package-0.3.5/cncd_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 09:38:42.000000 cncd_package-0.3.5/cncd_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:38:42.215386 cncd_package-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-06-03 09:37:16.000000 cncd_package-0.3.5/setup.py
```

### Comparing `cncd_package-0.3.4/PKG-INFO` & `cncd_package-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cncd_package
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Download
-pip install cncd-module
+pip install cncd-package
 
 # Loading the QC checks class
 
 
 ```python
 from cncd_package.QC import QC_Check
 ```
```

### Comparing `cncd_package-0.3.4/cncd_package/QC.py` & `cncd_package-0.3.5/cncd_package/QC.py`

 * *Files identical despite different names*

### Comparing `cncd_package-0.3.4/cncd_package.egg-info/PKG-INFO` & `cncd_package-0.3.5/cncd_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cncd-package
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Download
-pip install cncd-module
+pip install cncd-package
 
 # Loading the QC checks class
 
 
 ```python
 from cncd_package.QC import QC_Check
 ```
```

### Comparing `cncd_package-0.3.4/setup.py` & `cncd_package-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path("README.md").parent
 long_desc = (this_directory / "README.md").read_text()
 
 setup(
     name='cncd_package',
-    version='0.3.4',    
+    version='0.3.5',    
     description='A Python package for CNCD',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://github.com/shahzaib-raza/cncd',
     author='Shahzaib Raza',
     author_email='shahzaib.raza@cncd.org',
     license='BSD 2-clause',
```

