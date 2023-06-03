# Comparing `tmp/BatchParse-0.0.4.tar.gz` & `tmp/BatchParse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.4.tar", last modified: Sat Jun  3 01:59:30 2023, max compression
+gzip compressed data, was "BatchParse-0.0.5.tar", last modified: Sat Jun  3 02:43:10 2023, max compression
```

## Comparing `BatchParse-0.0.4.tar` & `BatchParse-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 01:59:21.000000 BatchParse-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 01:59:30.957388 BatchParse-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 01:59:21.000000 BatchParse-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:59:30.957388 BatchParse-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-03 01:59:21.000000 BatchParse-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-03 01:59:21.000000 BatchParse-0.0.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.360257 BatchParse-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 02:42:55.000000 BatchParse-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 02:43:10.360257 BatchParse-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 02:42:55.000000 BatchParse-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 02:43:10.360257 BatchParse-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-03 02:42:55.000000 BatchParse-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-03 02:42:55.000000 BatchParse-0.0.5/test/test.py
```

### Comparing `BatchParse-0.0.4/BatchParse/main.py` & `BatchParse-0.0.5/BatchParse/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 from .util.info import *
 from .util.splitting import *
 from .util.settings import Settings
 
 from rich.logging import RichHandler
-from rich.progress import track
 from rich.traceback import install
 
 install(show_locals=True)
 
 debug = False
 
 handler = RichHandler(rich_tracebacks=True, tracebacks_show_locals=True)
@@ -55,15 +54,15 @@
 
     bool_parse = [
         bsplit_and,
         bsplit_carrot,
         # bsplit_script_block,
     ]
 
-    for function in track(functions, description="Splitting Batch Code..."):
+    for function in functions:
         if bool_parse[functions.index(function)]:
             code_to_array = function(code_to_array)
 
     parsed_code = []
 
     allowed_methods = Settings.allowed_methods
 
@@ -72,15 +71,15 @@
     # if line doesn't start with a letter then we just ignore everything up until the first letter
 
     # remove all lines that start with ignorable_lines
     for line in code_to_array:
         if line in ignorable_lines:
             code_to_array.remove(line)
 
-    for line in track(code_to_array, description="Parsing Batch Code LIGHT..."):
+    for line in code_to_array:
         if not line[0].isalpha() and not line[0] in allowed_methods:
             for char in line:
                 if char.isalpha():
                     parsed_code.append(line[line.index(char) :])
                     break
         else:
             parsed_code.append(line)
@@ -98,14 +97,14 @@
         list: Parsed code as a list with [[code, dict], [code, dict], [code, dict]] (EXAMPLE)
     """
 
     final_arr = []
 
     initial_parse = parse(code, bsplit_and=bsplit_and)
     logger.debug(f"Initial Parse: {initial_parse}")
-    for array in track(initial_parse, description="Parsing Batch Code HEAVY..."):
+    for array in initial_parse:
         logger.debug(f"Array: {array}")
         dict_parse = info_gather(array)
         logger.debug(f"Dict Parse: {dict_parse}")
         final_arr.append([array, dict_parse])
 
     return final_arr
```

### Comparing `BatchParse-0.0.4/BatchParse/util/info.py` & `BatchParse-0.0.5/BatchParse/util/info.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.4/BatchParse/util/splitting.py` & `BatchParse-0.0.5/BatchParse/util/splitting.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.4/LICENSE` & `BatchParse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.4/setup.py` & `BatchParse-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

