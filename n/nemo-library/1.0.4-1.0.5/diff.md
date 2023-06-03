# Comparing `tmp/nemo_library-1.0.4.tar.gz` & `tmp/nemo_library-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.4.tar", last modified: Sat Jun  3 19:13:29 2023, max compression
+gzip compressed data, was "nemo_library-1.0.5.tar", last modified: Sat Jun  3 19:14:33 2023, max compression
```

## Comparing `nemo_library-1.0.4.tar` & `nemo_library-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:13:29.241520 nemo_library-1.0.4/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2169 2023-06-03 19:13:29.241255 nemo_library-1.0.4/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     1793 2023-06-03 06:16:17.000000 nemo_library-1.0.4/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     1875 2023-06-03 19:13:29.000000 nemo_library-1.0.4/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:13:29.238519 nemo_library-1.0.4/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.4/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    10969 2023-06-03 18:44:16.000000 nemo_library-1.0.4/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.4/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:13:29.240839 nemo_library-1.0.4/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2169 2023-06-03 19:13:29.000000 nemo_library-1.0.4/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:13:29.000000 nemo_library-1.0.4/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:13:29.000000 nemo_library-1.0.4/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:13:29.000000 nemo_library-1.0.4/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:13:29.000000 nemo_library-1.0.4/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:13:29.241577 nemo_library-1.0.4/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 19:13:09.000000 nemo_library-1.0.4/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.745807 nemo_library-1.0.5/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:14:33.745520 nemo_library-1.0.5/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.5/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-03 19:14:33.000000 nemo_library-1.0.5/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.743187 nemo_library-1.0.5/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.5/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    10969 2023-06-03 18:44:16.000000 nemo_library-1.0.5/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.5/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:14:33.745132 nemo_library-1.0.5/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:14:33.000000 nemo_library-1.0.5/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:14:33.745861 nemo_library-1.0.5/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 19:14:29.000000 nemo_library-1.0.5/setup.py
```

### Comparing `nemo_library-1.0.4/PKG-INFO` & `nemo_library-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_library
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
@@ -13,14 +13,20 @@
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
 pip install nemo_library
 
+Sources
+=======
+
+please find all sources on github:
+https://github.com/H3rm1nat0r/nemo_library
+
 configuration
 =============
 
 please create a file “config.ini”. This is an example for the content:
 
 ::
```

### Comparing `nemo_library-1.0.4/README.md` & `nemo_library-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 This library helps you with access to NEMO APIs
 
 # Installation
 
 pip install nemo_library
 
+# Sources
+
+please find all sources on github: https://github.com/H3rm1nat0r/nemo_library
+
 # configuration
 
 please create a file "config.ini". This is an example for the content:
 ```
 [nemo_library]
 nemo_url = https://enter.nemo-ai.com
 userid = <your userid>
```

### Comparing `nemo_library-1.0.4/README.rst` & `nemo_library-1.0.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
 pip install nemo_library
 
+Sources
+=======
+
+please find all sources on github:
+https://github.com/H3rm1nat0r/nemo_library
+
 configuration
 =============
 
 please create a file “config.ini”. This is an example for the content:
 
 ::
```

### Comparing `nemo_library-1.0.4/nemo_library/nemo_library.py` & `nemo_library-1.0.5/nemo_library/nemo_library.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.4/nemo_library/symbols.py` & `nemo_library-1.0.5/nemo_library/symbols.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.4/nemo_library.egg-info/PKG-INFO` & `nemo_library-1.0.5/nemo_library.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-library
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
@@ -13,14 +13,20 @@
 This library helps you with access to NEMO APIs
 
 Installation
 ============
 
 pip install nemo_library
 
+Sources
+=======
+
+please find all sources on github:
+https://github.com/H3rm1nat0r/nemo_library
+
 configuration
 =============
 
 please create a file “config.ini”. This is an example for the content:
 
 ::
```

### Comparing `nemo_library-1.0.4/setup.py` & `nemo_library-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nemo_library',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     install_requires=[
         'requests','pandas'
     ],
     author='Gunnar Schug',
     author_email='GunnarSchug81@gmail.com',
     description='A library for uploading data to and downloading reports from NEMO cloud solution',
```

