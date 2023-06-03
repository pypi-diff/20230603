# Comparing `tmp/nemo_library-1.0.5.tar.gz` & `tmp/nemo_library-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.5.tar", last modified: Sat Jun  3 19:14:33 2023, max compression
+gzip compressed data, was "nemo_library-1.0.6.tar", last modified: Sat Jun  3 19:49:11 2023, max compression
```

## Comparing `nemo_library-1.0.5.tar` & `nemo_library-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.745807 nemo_library-1.0.5/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:14:33.745520 nemo_library-1.0.5/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.5/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-03 19:14:33.000000 nemo_library-1.0.5/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.743187 nemo_library-1.0.5/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.5/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    10969 2023-06-03 18:44:16.000000 nemo_library-1.0.5/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.5/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.745132 nemo_library-1.0.5/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:14:33.745861 nemo_library-1.0.5/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 19:14:29.000000 nemo_library-1.0.5/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.795197 nemo_library-1.0.6/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:49:11.794929 nemo_library-1.0.6/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.6/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-03 19:49:11.000000 nemo_library-1.0.6/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.792436 nemo_library-1.0.6/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.6/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    10897 2023-06-03 19:48:41.000000 nemo_library-1.0.6/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.6/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.794512 nemo_library-1.0.6/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:49:11.795255 nemo_library-1.0.6/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 19:49:03.000000 nemo_library-1.0.6/setup.py
```

### Comparing `nemo_library-1.0.5/PKG-INFO` & `nemo_library-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_library
-Version: 1.0.5
+Version: 1.0.6
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
```

### Comparing `nemo_library-1.0.5/README.md` & `nemo_library-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.5/README.rst` & `nemo_library-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.5/nemo_library/nemo_library.py` & `nemo_library-1.0.6/nemo_library/nemo_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
                 if not data:
                     break
                 yield data
 
     #################################################################################################################################################################
 
     def UploadFile(self, projectname, filename):
-        print(f"Uploading file: {filename} into project {projectname}")
 
         # define some variables
         token = None
         upload_id = None
         project_id = None
         headers = None
```

### Comparing `nemo_library-1.0.5/nemo_library/symbols.py` & `nemo_library-1.0.6/nemo_library/symbols.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.5/nemo_library.egg-info/PKG-INFO` & `nemo_library-1.0.6/nemo_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-library
-Version: 1.0.5
+Version: 1.0.6
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
```

### Comparing `nemo_library-1.0.5/setup.py` & `nemo_library-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nemo_library',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     install_requires=[
         'requests','pandas'
     ],
     author='Gunnar Schug',
     author_email='GunnarSchug81@gmail.com',
     description='A library for uploading data to and downloading reports from NEMO cloud solution',
```

