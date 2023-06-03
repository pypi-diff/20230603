# Comparing `tmp/firegs-0.6.tar.gz` & `tmp/firegs-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firegs-0.6.tar", last modified: Sat Jun  3 16:53:42 2023, max compression
+gzip compressed data, was "firegs-0.7.tar", last modified: Sat Jun  3 17:33:35 2023, max compression
```

## Comparing `firegs-0.6.tar` & `firegs-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.659941 firegs-0.6/
--rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.6/LICENSE
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:53:42.659803 firegs-0.6/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.6/README.md
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.658868 firegs-0.6/firegs/
--rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.6/firegs/__init__.py
--rw-r--r--   0 ask        (501) staff       (20)     5921 2023-06-03 16:53:08.000000 firegs-0.6/firegs/script.py
--rw-r--r--   0 ask        (501) staff       (20)       19 2023-06-03 16:53:36.000000 firegs-0.6/firegs/version.py
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.659612 firegs-0.6/firegs.egg-info/
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      262 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/SOURCES.txt
--rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/dependency_links.txt
--rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/entry_points.txt
--rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/requires.txt
--rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/top_level.txt
--rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:53:42.659982 firegs-0.6/setup.cfg
--rw-r--r--   0 ask        (501) staff       (20)      879 2023-06-03 16:53:08.000000 firegs-0.6/setup.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.653414 firegs-0.7/
+-rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.7/LICENSE
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:33:35.653265 firegs-0.7/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.7/README.md
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.651936 firegs-0.7/firegs/
+-rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.7/firegs/__init__.py
+-rw-r--r--   0 ask        (501) staff       (20)     5921 2023-06-03 16:53:08.000000 firegs-0.7/firegs/script.py
+-rw-r--r--   0 ask        (501) staff       (20)       19 2023-06-03 17:33:30.000000 firegs-0.7/firegs/version.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.652848 firegs-0.7/firegs.egg-info/
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      262 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/SOURCES.txt
+-rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/dependency_links.txt
+-rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/entry_points.txt
+-rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/requires.txt
+-rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/top_level.txt
+-rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 17:33:35.653468 firegs-0.7/setup.cfg
+-rw-r--r--   0 ask        (501) staff       (20)      879 2023-06-03 16:53:08.000000 firegs-0.7/setup.py
```

### Comparing `firegs-0.6/LICENSE` & `firegs-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `firegs-0.6/PKG-INFO` & `firegs-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.6
+Version: 0.7
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.6/README.md` & `firegs-0.7/README.md`

 * *Files identical despite different names*

### Comparing `firegs-0.6/firegs/script.py` & `firegs-0.7/firegs/script.py`

 * *Files identical despite different names*

### Comparing `firegs-0.6/firegs.egg-info/PKG-INFO` & `firegs-0.7/firegs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.6
+Version: 0.7
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.6/setup.py` & `firegs-0.7/setup.py`

 * *Files identical despite different names*

