# Comparing `tmp/headless-ida-0.4.0.tar.gz` & `tmp/headless-ida-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headless-ida-0.4.0.tar", last modified: Sat Jun  3 04:12:03 2023, max compression
+gzip compressed data, was "headless-ida-0.4.1.tar", last modified: Sat Jun  3 04:25:30 2023, max compression
```

## Comparing `headless-ida-0.4.0.tar` & `headless-ida-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 04:11:53.000000 headless-ida-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:12:03.869734 headless-ida-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-03 04:11:53.000000 headless-ida-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/headless_ida/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/ida_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/ida_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/headless_ida.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-03 04:11:56.000000 headless-ida-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:12:03.869734 headless-ida-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:25:30.053297 headless-ida-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 04:25:18.000000 headless-ida-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:25:30.053297 headless-ida-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-03 04:25:18.000000 headless-ida-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:25:30.049297 headless-ida-0.4.1/headless_ida/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-03 04:25:18.000000 headless-ida-0.4.1/headless_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-03 04:25:19.000000 headless-ida-0.4.1/headless_ida/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-03 04:25:19.000000 headless-ida-0.4.1/headless_ida/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-03 04:25:19.000000 headless-ida-0.4.1/headless_ida/ida_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 04:25:19.000000 headless-ida-0.4.1/headless_ida/ida_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 04:25:19.000000 headless-ida-0.4.1/headless_ida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:25:30.053297 headless-ida-0.4.1/headless_ida.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 04:25:30.000000 headless-ida-0.4.1/headless_ida.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-03 04:25:21.000000 headless-ida-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:25:30.053297 headless-ida-0.4.1/setup.cfg
```

### Comparing `headless-ida-0.4.0/LICENSE` & `headless-ida-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/PKG-INFO` & `headless-ida-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.4.0
+Version: 0.4.1
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `headless-ida-0.4.0/README.md` & `headless-ida-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida/cli.py` & `headless-ida-0.4.1/headless_ida/cli.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida/client.py` & `headless-ida-0.4.1/headless_ida/client.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida/ida_headers.py` & `headless-ida-0.4.1/headless_ida/ida_headers.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida/ida_script.py` & `headless-ida-0.4.1/headless_ida/ida_script.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida/server.py` & `headless-ida-0.4.1/headless_ida/server.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.4.0/headless_ida.egg-info/PKG-INFO` & `headless-ida-0.4.1/headless_ida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.4.0
+Version: 0.4.1
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `headless-ida-0.4.0/pyproject.toml` & `headless-ida-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "headless-ida"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
     "rpyc",
 ]
 readme = "README.md"
 description = "Headless IDA"
 authors = [
     {name = "Han Dai", email = "pypi@han.do"},
```

