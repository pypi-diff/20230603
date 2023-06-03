# Comparing `tmp/LinSATNet-0.0.1.tar.gz` & `tmp/LinSATNet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.1.tar", last modified: Wed May 31 16:02:54 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.2.tar", last modified: Sat Jun  3 08:17:00 2023, max compression
```

## Comparing `LinSATNet-0.0.1.tar` & `LinSATNet-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:02:54.557037 LinSATNet-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 16:02:43.000000 LinSATNet-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:02:54.553038 LinSATNet-0.0.1/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 16:02:43.000000 LinSATNet-0.0.1/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-31 16:02:43.000000 LinSATNet-0.0.1/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:02:54.557037 LinSATNet-0.0.1/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 16:02:54.000000 LinSATNet-0.0.1/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 16:02:54.000000 LinSATNet-0.0.1/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:02:54.000000 LinSATNet-0.0.1/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 16:02:54.000000 LinSATNet-0.0.1/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 16:02:54.000000 LinSATNet-0.0.1/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 16:02:54.557037 LinSATNet-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 16:02:43.000000 LinSATNet-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:02:54.557037 LinSATNet-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-31 16:02:43.000000 LinSATNet-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:17:00.755010 LinSATNet-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 08:16:42.000000 LinSATNet-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:17:00.755010 LinSATNet-0.0.2/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 08:16:42.000000 LinSATNet-0.0.2/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-03 08:16:42.000000 LinSATNet-0.0.2/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:17:00.755010 LinSATNet-0.0.2/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-06-03 08:17:00.000000 LinSATNet-0.0.2/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-03 08:17:00.000000 LinSATNet-0.0.2/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:17:00.000000 LinSATNet-0.0.2/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 08:17:00.000000 LinSATNet-0.0.2/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 08:17:00.000000 LinSATNet-0.0.2/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-06-03 08:17:00.755010 LinSATNet-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-06-03 08:16:42.000000 LinSATNet-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:17:00.755010 LinSATNet-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-03 08:16:42.000000 LinSATNet-0.0.2/setup.py
```

### Comparing `LinSATNet-0.0.1/LICENSE` & `LinSATNet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.1/setup.py` & `LinSATNet-0.0.2/setup.py`

 * *Files identical despite different names*

