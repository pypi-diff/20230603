# Comparing `tmp/BatchParse-0.0.3.tar.gz` & `tmp/BatchParse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.3.tar", last modified: Wed May 31 00:06:23 2023, max compression
+gzip compressed data, was "BatchParse-0.0.4.tar", last modified: Sat Jun  3 01:59:30 2023, max compression
```

## Comparing `BatchParse-0.0.3.tar` & `BatchParse-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.729117 BatchParse-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 00:06:09.000000 BatchParse-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 00:06:23.729117 BatchParse-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 00:06:09.000000 BatchParse-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:06:23.729117 BatchParse-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 00:06:09.000000 BatchParse-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 00:06:09.000000 BatchParse-0.0.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-03 01:59:21.000000 BatchParse-0.0.4/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 01:59:30.000000 BatchParse-0.0.4/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 01:59:21.000000 BatchParse-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 01:59:30.957388 BatchParse-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 01:59:21.000000 BatchParse-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:59:30.957388 BatchParse-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-03 01:59:21.000000 BatchParse-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:59:30.957388 BatchParse-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-03 01:59:21.000000 BatchParse-0.0.4/test/test.py
```

### Comparing `BatchParse-0.0.3/BatchParse/main.py` & `BatchParse-0.0.4/BatchParse/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,39 +22,45 @@
     logging.basicConfig(
         level=logging.INFO, format="%(message)s", datefmt="[%X]", handlers=[handler]
     )
 logger = logging.getLogger("rich")
 
 
 def parse(
-    code: str,
+    code,
     bsplit_and: bool = True,
     bsplit_carrot: bool = True,
     bsplit_script_block: bool = True,
 ) -> list:
     """Parse initial Batch Code
 
     Args:
         code (str): Inital Batch Code to Parse
 
     Returns:
         list: Returns Parsed Batch Code as an Array
     """
-    code_to_array = code.split("\n")
+
+    if isinstance(code, str):
+        code_to_array = code.split("\n")
+    elif isinstance(code, list):
+        code_to_array = code
+    else:
+        raise TypeError("code must be a string or list")
 
     functions = [
         parse_and,
         parse_carrot,
-        parse_script_block,
+        # parse_script_block,
     ]
 
     bool_parse = [
         bsplit_and,
         bsplit_carrot,
-        bsplit_script_block,
+        # bsplit_script_block,
     ]
 
     for function in track(functions, description="Splitting Batch Code..."):
         if bool_parse[functions.index(function)]:
             code_to_array = function(code_to_array)
 
     parsed_code = []
```

### Comparing `BatchParse-0.0.3/BatchParse/util/info.py` & `BatchParse-0.0.4/BatchParse/util/info.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.3/BatchParse/util/splitting.py` & `BatchParse-0.0.4/BatchParse/util/splitting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import List, Union
 
 
 def parse_and(code: list) -> list:
     """
     Parse the Batch Code for the AND Operator
 
     Args:
@@ -40,24 +41,29 @@
             index = code.index(line)
             code[index] = code[index] + " " + code[index + 1]
             code.pop(index + 1)
 
     return code
 
 
-def parse_script_block(code: list, ignore_indents: bool = False) -> list:
+def parse_script_block(
+    code: Union[List[str], str], ignore_indents: bool = False
+) -> list:
     """Parses the Batch Code for Script Blocks
 
     Args:
         code (list): Batch Code as an Array
 
     Returns:
         list: Returns Parsed Batch Code as an Array
     """
 
+    if isinstance(code, list):
+        code = "".join(code)
+
     if ignore_indents:
         for line in code:
             ammount_of_indents = len(re.findall("^ *", line)[0])
             if ammount_of_indents >= 12:
                 raise Exception(
                     "You have more than 12 spaces for 1 indent. Please don't use more than 4 and chain your indents into 1 line."
                 )
```

### Comparing `BatchParse-0.0.3/LICENSE` & `BatchParse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.3/setup.py` & `BatchParse-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

