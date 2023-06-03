# Comparing `tmp/bettertest-0.1.96.tar.gz` & `tmp/bettertest-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.96.tar", max compression
+gzip compressed data, was "bettertest-0.1.97.tar", max compression
```

## Comparing `bettertest-0.1.96.tar` & `bettertest-0.1.97.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.96/README.md
--rw-r--r--   0        0        0     8413 2023-06-03 20:00:16.980530 bettertest-0.1.96/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.96/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    26031 2023-06-03 19:48:49.262447 bettertest-0.1.96/bettertest/test.py
--rw-r--r--   0        0        0      336 2023-06-03 20:00:25.188351 bettertest-0.1.96/pyproject.toml
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.96/PKG-INFO
+-rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.97/README.md
+-rw-r--r--   0        0        0     8413 2023-06-03 21:12:49.884010 bettertest-0.1.97/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.97/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    26031 2023-06-03 19:48:49.262447 bettertest-0.1.97/bettertest/test.py
+-rw-r--r--   0        0        0      336 2023-06-03 21:12:51.965358 bettertest-0.1.97/pyproject.toml
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.97/PKG-INFO
```

### Comparing `bettertest-0.1.96/README.md` & `bettertest-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.96/bettertest/__init__.py` & `bettertest-0.1.97/bettertest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__version__ = '0.1.96'
+__version__ = '0.1.97'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
 import os 
 from collections import Counter
-# from bettertest.promptTemplate import promptTemplate
-from promptTemplate import promptTemplate
+from bettertest.promptTemplate import promptTemplate
+# from promptTemplate import promptTemplate
 import concurrent.futures
 import threading
 import uuid
 import builtins
 import inspect
 import webbrowser
```

### Comparing `bettertest-0.1.96/bettertest/promptTemplate.py` & `bettertest-0.1.97/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.96/bettertest/test.py` & `bettertest-0.1.97/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.96/PKG-INFO` & `bettertest-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.96
+Version: 0.1.97
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

