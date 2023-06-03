# Comparing `tmp/bettertest-0.1.2.tar.gz` & `tmp/bettertest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.2.tar", max compression
+gzip compressed data, was "bettertest-0.1.3.tar", max compression
```

## Comparing `bettertest-0.1.2.tar` & `bettertest-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.2/README.md
--rw-r--r--   0        0        0     8062 2023-06-03 00:35:06.097996 bettertest-0.1.2/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.2/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.2/bettertest/test.py
--rw-r--r--   0        0        0      335 2023-06-03 00:35:02.201279 bettertest-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.3/README.md
+-rw-r--r--   0        0        0     8073 2023-06-03 00:36:56.722609 bettertest-0.1.3/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.3/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.3/bettertest/test.py
+-rw-r--r--   0        0        0      335 2023-06-03 00:36:59.133906 bettertest-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.3/PKG-INFO
```

### Comparing `bettertest-0.1.2/bettertest/__init__.py` & `bettertest-0.1.3/bettertest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
 import os 
 from collections import Counter
-from promptTemplate import promptTemplate
+from bettertest.promptTemplate import promptTemplate
 import concurrent.futures
 import threading
 import uuid
 import builtins
 import inspect
```

### Comparing `bettertest-0.1.2/bettertest/promptTemplate.py` & `bettertest-0.1.3/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.2/bettertest/test.py` & `bettertest-0.1.3/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.2/PKG-INFO` & `bettertest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

