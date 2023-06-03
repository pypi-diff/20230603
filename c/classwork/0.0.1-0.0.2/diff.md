# Comparing `tmp/classwork-0.0.1.tar.gz` & `tmp/classwork-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.1.tar", last modified: Sat Jun  3 17:12:22 2023, max compression
+gzip compressed data, was "classwork-0.0.2.tar", last modified: Sat Jun  3 18:53:04 2023, max compression
```

## Comparing `classwork-0.0.1.tar` & `classwork-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 17:12:22.040079 classwork-0.0.1/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     1072 2023-06-03 17:09:04.000000 classwork-0.0.1/LICENSE.md
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 17:12:22.040079 classwork-0.0.1/PKG-INFO
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4193 2023-06-03 16:54:31.000000 classwork-0.0.1/README.md
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 17:12:22.040079 classwork-0.0.1/classwork/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      161 2023-06-03 15:43:24.000000 classwork-0.0.1/classwork/__init__.py
--rw-rw-r--   0 mugz      (1000) mugz      (1000)    11866 2023-06-03 16:13:53.000000 classwork-0.0.1/classwork/main.py
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     3086 2023-06-03 15:08:39.000000 classwork-0.0.1/classwork/utils.py
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 17:12:22.040079 classwork-0.0.1/classwork.egg-info/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 17:12:22.000000 classwork-0.0.1/classwork.egg-info/PKG-INFO
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      226 2023-06-03 17:12:22.000000 classwork-0.0.1/classwork.egg-info/SOURCES.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)        1 2023-06-03 17:12:22.000000 classwork-0.0.1/classwork.egg-info/dependency_links.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)       10 2023-06-03 17:12:22.000000 classwork-0.0.1/classwork.egg-info/top_level.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      642 2023-06-03 17:10:48.000000 classwork-0.0.1/pyproject.toml
--rw-rw-r--   0 mugz      (1000) mugz      (1000)       38 2023-06-03 17:12:22.040079 classwork-0.0.1/setup.cfg
+drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.188561 classwork-0.0.2/
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)     1072 2023-06-03 17:09:04.000000 classwork-0.0.2/LICENSE.md
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 18:53:04.188561 classwork-0.0.2/PKG-INFO
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)     4193 2023-06-03 16:54:31.000000 classwork-0.0.2/README.md
+drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.184561 classwork-0.0.2/classwork/
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)      161 2023-06-03 15:43:24.000000 classwork-0.0.2/classwork/__init__.py
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)    11866 2023-06-03 16:13:53.000000 classwork-0.0.2/classwork/main.py
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)     3086 2023-06-03 15:08:39.000000 classwork-0.0.2/classwork/utils.py
+drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.188561 classwork-0.0.2/classwork.egg-info/
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/PKG-INFO
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)      258 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/SOURCES.txt
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)        1 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/dependency_links.txt
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)       75 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/requires.txt
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)       10 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/top_level.txt
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)      759 2023-06-03 18:08:27.000000 classwork-0.0.2/pyproject.toml
+-rw-rw-r--   0 mugz      (1000) mugz      (1000)       38 2023-06-03 18:53:04.188561 classwork-0.0.2/setup.cfg
```

### Comparing `classwork-0.0.1/LICENSE.md` & `classwork-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.1/PKG-INFO` & `classwork-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 Author-email: Anthony Mugendi <ngurumugz@gmail.com>
-Project-URL: Homepage, https://github.com/mugendi/classwork
 Project-URL: Bug Tracker, https://github.com/mugendi/classwork/issues
+Project-URL: Homepage, https://github.com/mugendi/classwork
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `classwork-0.0.1/README.md` & `classwork-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.1/classwork/main.py` & `classwork-0.0.2/classwork/main.py`

 * *Files identical despite different names*

### Comparing `classwork-0.0.1/classwork/utils.py` & `classwork-0.0.2/classwork/utils.py`

 * *Files identical despite different names*

### Comparing `classwork-0.0.1/classwork.egg-info/PKG-INFO` & `classwork-0.0.2/classwork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 Author-email: Anthony Mugendi <ngurumugz@gmail.com>
-Project-URL: Homepage, https://github.com/mugendi/classwork
 Project-URL: Bug Tracker, https://github.com/mugendi/classwork/issues
+Project-URL: Homepage, https://github.com/mugendi/classwork
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

