# Comparing `tmp/gui_args_framework-1.2.1.tar.gz` & `tmp/gui_args_framework-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gui_args_framework-1.2.1.tar", last modified: Sat Jun  3 08:34:13 2023, max compression
+gzip compressed data, was "dist/gui_args_framework-1.2.2.tar", last modified: Sat Jun  3 08:47:44 2023, max compression
```

## Comparing `gui_args_framework-1.2.1.tar` & `gui_args_framework-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 08:34:13.512989 gui_args_framework-1.2.1/
--rw-rw-rw-   0        0        0        0 2023-05-30 19:08:14.000000 gui_args_framework-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2002 2023-06-03 08:34:13.512989 gui_args_framework-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-05-30 19:41:43.000000 gui_args_framework-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 08:34:13.507989 gui_args_framework-1.2.1/gui_args_framework/
--rw-rw-rw-   0        0        0        0 2023-05-30 19:19:44.000000 gui_args_framework-1.2.1/gui_args_framework/__init__.py
--rw-rw-rw-   0        0        0     6778 2023-05-30 19:08:14.000000 gui_args_framework-1.2.1/gui_args_framework/args_window.py
--rw-rw-rw-   0        0        0     3297 2023-06-03 08:29:15.000000 gui_args_framework-1.2.1/gui_args_framework/fields.py
--rw-rw-rw-   0        0        0     1068 2023-05-30 19:08:14.000000 gui_args_framework-1.2.1/gui_args_framework/main_thread.py
--rw-rw-rw-   0        0        0      615 2023-05-30 19:08:14.000000 gui_args_framework-1.2.1/gui_args_framework/rpc_call.py
--rw-rw-rw-   0        0        0       22 2023-06-03 08:19:12.000000 gui_args_framework-1.2.1/gui_args_framework/version.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:34:13.511989 gui_args_framework-1.2.1/gui_args_framework.egg-info/
--rw-rw-rw-   0        0        0     2002 2023-06-03 08:34:13.000000 gui_args_framework-1.2.1/gui_args_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-03 08:34:13.000000 gui_args_framework-1.2.1/gui_args_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 08:34:13.000000 gui_args_framework-1.2.1/gui_args_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-03 08:34:13.000000 gui_args_framework-1.2.1/gui_args_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-03 08:34:13.000000 gui_args_framework-1.2.1/gui_args_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 08:34:13.513990 gui_args_framework-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-06-03 08:17:35.000000 gui_args_framework-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/args_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/main_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/rpc_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/gui_args_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/gui_args_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:47:44.000000 gui_args_framework-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-03 08:47:38.000000 gui_args_framework-1.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gui_args_framework-1.2.1/PKG-INFO` & `gui_args_framework-1.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: gui_args_framework
-Version: 1.2.1
-Summary: A framework to create a GUI for a Python console application
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # gui-args-framework
 
 **gui-args-framework** provides a user-friendly way to implement your Python script with GUI easily and quickly, instead of dark ugly terminal window that scares people who are far from programming.
 
 Supposing, you have developed a program that takes arguments, does something and provides a result as text lines. Usually you develop such things as console applications that can be not so convenient to users. With gui-args-framework it can be easily done through GUI.
 
 The example below is simple to understand how it works. There is a program to calculate sum of two integers:
@@ -36,15 +26,15 @@
 
 
 TestWindow.run()
 ```
 
 ## Installation
 
-    pip install git+https://github.com/fomalhaut88/gui-args-framework.git
+    pip install gui-args-framework
 
 ## Window parameters
 
 ```
     title = None
     args = []
     description = ""
@@ -74,9 +64,7 @@
 - IntegerField
 - FloatField
 - BooleanField
 - EnumField
 - FileOpenField
 - DirectoryField
 - FileSaveField
-
-
```

### Comparing `gui_args_framework-1.2.1/gui_args_framework/args_window.py` & `gui_args_framework-1.2.2/gui_args_framework/args_window.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.1/gui_args_framework/fields.py` & `gui_args_framework-1.2.2/gui_args_framework/fields.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.1/gui_args_framework/main_thread.py` & `gui_args_framework-1.2.2/gui_args_framework/main_thread.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.1/gui_args_framework/rpc_call.py` & `gui_args_framework-1.2.2/gui_args_framework/rpc_call.py`

 * *Files identical despite different names*

### Comparing `gui_args_framework-1.2.1/setup.py` & `gui_args_framework-1.2.2/setup.py`

 * *Files identical despite different names*

