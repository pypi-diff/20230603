# Comparing `tmp/cncd_package-0.3.2.tar.gz` & `tmp/cncd_package-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cncd_package-0.3.2.tar", last modified: Sat Jun  3 07:48:24 2023, max compression
+gzip compressed data, was "cncd_package-0.3.3.tar", last modified: Sat Jun  3 07:59:14 2023, max compression
```

## Comparing `cncd_package-0.3.2.tar` & `cncd_package-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.291514 cncd_package-0.3.2/
--rw-rw-rw-   0        0        0      996 2023-06-03 07:48:24.291514 cncd_package-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.275892 cncd_package-0.3.2/cncd_package/
--rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.2/cncd_package/QC.py
--rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.2/cncd_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:48:24.291514 cncd_package-0.3.2/cncd_package.egg-info/
--rw-rw-rw-   0        0        0      996 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 07:48:24.000000 cncd_package-0.3.2/cncd_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 07:48:24.291514 cncd_package-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-03 07:47:48.000000 cncd_package-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.572418 cncd_package-0.3.3/
+-rw-rw-rw-   0        0        0    10336 2023-06-03 07:59:14.572418 cncd_package-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.556794 cncd_package-0.3.3/cncd_package/
+-rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.3/cncd_package/QC.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.3/cncd_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.572418 cncd_package-0.3.3/cncd_package.egg-info/
+-rw-rw-rw-   0        0        0    10336 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 07:59:14.572418 cncd_package-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-06-03 07:58:09.000000 cncd_package-0.3.3/setup.py
```

### Comparing `cncd_package-0.3.2/cncd_package/QC.py` & `cncd_package-0.3.3/cncd_package/QC.py`

 * *Files identical despite different names*

### Comparing `cncd_package-0.3.2/setup.py` & `cncd_package-0.3.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from setuptools import setup
+from pathlib import Path
+
+this_directory = Path("README.md").parent
+long_desc = (this_directory / "README.md").read_text()
 
 setup(
     name='cncd_package',
-    version='0.3.2',    
-    description='An example Python package for CNCD',
+    version='0.3.3',    
+    description='A Python package for CNCD',
+    long_description=long_desc,
+    long_description_content_type='text/markdown',
     url='https://github.com/shahzaib-raza/cncd',
     author='Shahzaib Raza',
     author_email='shahzaib.raza@cncd.org',
     license='BSD 2-clause',
     packages=['cncd_package'],
     install_requires=['mpi4py>=2.0', 'numpy>=1.24.1', 'pandas>=1.5.3'],
     classifiers=[
```

