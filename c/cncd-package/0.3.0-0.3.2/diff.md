# Comparing `tmp/cncd_package-0.3.0.tar.gz` & `tmp/cncd_package-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cncd_package-0.3.0.tar", last modified: Sat Jun  3 07:23:58 2023, max compression
+gzip compressed data, was "cncd_package-0.3.2.tar", last modified: Sat Jun  3 07:48:24 2023, max compression
```

## Comparing `cncd_package-0.3.0.tar` & `cncd_package-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:23:58.897346 cncd_package-0.3.0/
--rw-rw-rw-   0        0        0      996 2023-06-03 07:23:58.897346 cncd_package-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 07:23:58.851987 cncd_package-0.3.0/cncd_package/
--rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.0/cncd_package/QC.py
--rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.0/cncd_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:23:58.868200 cncd_package-0.3.0/cncd_package.egg-info/
--rw-rw-rw-   0        0        0      996 2023-06-03 07:23:58.000000 cncd_package-0.3.0/cncd_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-03 07:23:58.000000 cncd_package-0.3.0/cncd_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:23:58.000000 cncd_package-0.3.0/cncd_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-03 07:23:58.000000 cncd_package-0.3.0/cncd_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 07:23:58.000000 cncd_package-0.3.0/cncd_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 07:23:58.898350 cncd_package-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-03 07:23:22.000000 cncd_package-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.291514 cncd_package-0.3.2/
+-rw-rw-rw-   0        0        0      996 2023-06-03 07:48:24.291514 cncd_package-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.275892 cncd_package-0.3.2/cncd_package/
+-rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.2/cncd_package/QC.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.2/cncd_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.291514 cncd_package-0.3.2/cncd_package.egg-info/
+-rw-rw-rw-   0        0        0      996 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 07:48:24.291514 cncd_package-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-03 07:47:48.000000 cncd_package-0.3.2/setup.py
```

### Comparing `cncd_package-0.3.0/PKG-INFO` & `cncd_package-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cncd_package
-Version: 0.3.0
+Version: 0.3.2
 Summary: An example Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cncd_package-0.3.0/cncd_package/QC.py` & `cncd_package-0.3.2/cncd_package/QC.py`

 * *Files identical despite different names*

### Comparing `cncd_package-0.3.0/cncd_package.egg-info/PKG-INFO` & `cncd_package-0.3.2/cncd_package.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cncd-package
-Version: 0.3.0
+Version: 0.3.2
 Summary: An example Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cncd_package-0.3.0/setup.py` & `cncd_package-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cncd_package',
-    version='0.3.0',    
+    version='0.3.2',    
     description='An example Python package for CNCD',
     url='https://github.com/shahzaib-raza/cncd',
     author='Shahzaib Raza',
     author_email='shahzaib.raza@cncd.org',
     license='BSD 2-clause',
     packages=['cncd_package'],
     install_requires=['mpi4py>=2.0', 'numpy>=1.24.1', 'pandas>=1.5.3'],
```

