# Comparing `tmp/gui_args_framework-1.2.2.tar.gz` & `tmp/gui_args_framework-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gui_args_framework-1.2.2.tar", last modified: Sat Jun  3 08:47:44 2023, max compression
+gzip compressed data, was "dist/gui_args_framework-1.2.3.tar", last modified: Sat Jun  3 08:53:58 2023, max compression
```

## Comparing `gui_args_framework-1.2.2.tar` & `gui_args_framework-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/args_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/main_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/rpc_call.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/args_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/main_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/rpc_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/gui_args_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/gui_args_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:53:58.000000 gui_args_framework-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-03 08:53:52.000000 gui_args_framework-1.2.3/setup.py
```

### Comparing `gui_args_framework-1.2.2/PKG-INFO` & `gui_args_framework-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gui_args_framework
-Version: 1.2.2
+Version: 1.2.3
 Summary: A framework to create a GUI for a Python console application
 Home-page: UNKNOWN
-License: UNKNOWN
+License: Free
 Description: # gui-args-framework
         
         **gui-args-framework** provides a user-friendly way to implement your Python script with GUI easily and quickly, instead of dark ugly terminal window that scares people who are far from programming.
         
         Supposing, you have developed a program that takes arguments, does something and provides a result as text lines. Usually you develop such things as console applications that can be not so convenient to users. With gui-args-framework it can be easily done through GUI.
         
         The example below is simple to understand how it works. There is a program to calculate sum of two integers:
```

### Comparing `gui_args_framework-1.2.2/README.md` & `gui_args_framework-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.2/gui_args_framework/args_window.py` & `gui_args_framework-1.2.3/gui_args_framework/args_window.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.2/gui_args_framework/fields.py` & `gui_args_framework-1.2.3/gui_args_framework/fields.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.2/gui_args_framework/main_thread.py` & `gui_args_framework-1.2.3/gui_args_framework/main_thread.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.2/gui_args_framework/rpc_call.py` & `gui_args_framework-1.2.3/gui_args_framework/rpc_call.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.2/gui_args_framework.egg-info/PKG-INFO` & `gui_args_framework-1.2.3/gui_args_framework.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gui-args-framework
-Version: 1.2.2
+Version: 1.2.3
 Summary: A framework to create a GUI for a Python console application
 Home-page: UNKNOWN
-License: UNKNOWN
+License: Free
 Description: # gui-args-framework
         
         **gui-args-framework** provides a user-friendly way to implement your Python script with GUI easily and quickly, instead of dark ugly terminal window that scares people who are far from programming.
         
         Supposing, you have developed a program that takes arguments, does something and provides a result as text lines. Usually you develop such things as console applications that can be not so convenient to users. With gui-args-framework it can be easily done through GUI.
         
         The example below is simple to understand how it works. There is a program to calculate sum of two integers:
```

