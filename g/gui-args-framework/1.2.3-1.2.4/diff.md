# Comparing `tmp/gui_args_framework-1.2.3.tar.gz` & `tmp/gui_args_framework-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gui_args_framework-1.2.3.tar", last modified: Sat Jun  3 08:53:58 2023, max compression
+gzip compressed data, was "dist/gui_args_framework-1.2.4.tar", last modified: Sat Jun  3 09:22:15 2023, max compression
```

## Comparing `gui_args_framework-1.2.3.tar` & `gui_args_framework-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/args_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/main_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/rpc_call.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/gui_args_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/args_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/main_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/rpc_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/gui_args_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-03 09:22:14.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:22:14.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 09:22:14.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 09:22:14.000000 gui_args_framework-1.2.4/gui_args_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:22:15.000000 gui_args_framework-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-03 09:22:11.000000 gui_args_framework-1.2.4/setup.py
```

### Comparing `gui_args_framework-1.2.3/gui_args_framework/args_window.py` & `gui_args_framework-1.2.4/gui_args_framework/args_window.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.3/gui_args_framework/fields.py` & `gui_args_framework-1.2.4/gui_args_framework/fields.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.3/gui_args_framework/main_thread.py` & `gui_args_framework-1.2.4/gui_args_framework/main_thread.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.3/gui_args_framework/rpc_call.py` & `gui_args_framework-1.2.4/gui_args_framework/rpc_call.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.3/setup.py` & `gui_args_framework-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 setup(
     name='gui_args_framework',
     version=__version__,
     packages=find_packages(),
     license="Free",
-    description="A framework to create a GUI for a Python console application",
+    description="A framework to create a GUI for a Python console application.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'PyQt5>=5.15',
         'PyQt5-Qt5>=5.15',
         'PyQt5-sip>=12.9',
     ],
```

