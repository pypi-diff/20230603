# Comparing `tmp/dsmltf-0.0.5.tar.gz` & `tmp/dsmltf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmltf-0.0.5.tar", last modified: Thu May 25 13:14:05 2023, max compression
+gzip compressed data, was "dsmltf-0.0.6.tar", last modified: Sat Jun  3 06:19:01 2023, max compression
```

## Comparing `dsmltf-0.0.5.tar` & `dsmltf-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.897046 dsmltf-0.0.5/
--rw-r--r--   0 sergejzuev   (501) staff       (20)    35201 2023-05-14 06:35:21.000000 dsmltf-0.0.5/LICENSE
--rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-05-25 13:14:05.897321 dsmltf-0.0.5/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 dsmltf-0.0.5/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.893300 dsmltf-0.0.5/dsmltf/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 dsmltf-0.0.5/dsmltf/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    30600 2023-05-25 12:55:41.000000 dsmltf-0.0.5/dsmltf/main.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.896027 dsmltf-0.0.5/dsmltf.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      190 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-25 13:14:05.898828 dsmltf-0.0.5/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      623 2023-05-25 13:13:45.000000 dsmltf-0.0.5/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-06-03 06:19:01.915974 dsmltf-0.0.6/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35201 2023-05-14 06:35:21.000000 dsmltf-0.0.6/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-06-03 06:19:01.916269 dsmltf-0.0.6/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 dsmltf-0.0.6/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-06-03 06:19:01.909930 dsmltf-0.0.6/dsmltf/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 dsmltf-0.0.6/dsmltf/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    57134 2023-06-03 06:14:47.000000 dsmltf-0.0.6/dsmltf/main.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-06-03 06:19:01.914983 dsmltf-0.0.6/dsmltf.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-06-03 06:19:01.000000 dsmltf-0.0.6/dsmltf.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      190 2023-06-03 06:19:01.000000 dsmltf-0.0.6/dsmltf.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-06-03 06:19:01.000000 dsmltf-0.0.6/dsmltf.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-06-03 06:19:01.000000 dsmltf-0.0.6/dsmltf.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-06-03 06:19:01.917746 dsmltf-0.0.6/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      623 2023-06-03 06:17:48.000000 dsmltf-0.0.6/setup.py
```

### Comparing `dsmltf-0.0.5/LICENSE` & `dsmltf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmltf-0.0.5/PKG-INFO` & `dsmltf-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmltf
-Version: 0.0.5
+Version: 0.0.6
 Summary: A set of functions to study Data Science
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dsmltf-0.0.5/dsmltf.egg-info/PKG-INFO` & `dsmltf-0.0.6/dsmltf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmltf
-Version: 0.0.5
+Version: 0.0.6
 Summary: A set of functions to study Data Science
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dsmltf-0.0.5/setup.py` & `dsmltf-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 #requirements = ["requests<=2.21.0"]
 
 setuptools.setup(name="dsmltf",
-	version="0.0.5",
+	version="0.0.6",
 	author="Sergei Zuev",
 	author_email="shoukhov@mail.ru",
 	description="A set of functions to study Data Science",
 	packages=setuptools.find_packages(),
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
```

