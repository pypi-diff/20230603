# Comparing `tmp/bettertest-0.1.93.tar.gz` & `tmp/bettertest-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.93.tar", max compression
+gzip compressed data, was "bettertest-0.1.94.tar", max compression
```

## Comparing `bettertest-0.1.93.tar` & `bettertest-0.1.94.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.93/README.md
--rw-r--r--   0        0        0     8207 2023-06-03 18:58:09.555932 bettertest-0.1.93/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.93/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.93/bettertest/test.py
--rw-r--r--   0        0        0      336 2023-06-03 18:58:14.146398 bettertest-0.1.93/pyproject.toml
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.94/README.md
+-rw-r--r--   0        0        0     8133 2023-06-03 19:03:35.408389 bettertest-0.1.94/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.94/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.94/bettertest/test.py
+-rw-r--r--   0        0        0      336 2023-06-03 19:03:38.461756 bettertest-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.94/PKG-INFO
```

### Comparing `bettertest-0.1.93/README.md` & `bettertest-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.93/bettertest/__init__.py` & `bettertest-0.1.94/bettertest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.93'
+__version__ = '0.1.94'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -14,17 +14,14 @@
 import uuid
 import builtins
 import inspect
 
 
 supa_url = "https://gwfhoxolvmhoszkvddnv.supabase.co"
 supa_key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imd3ZmhveG9sdm1ob3N6a3ZkZG52Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2ODU3MzU0OTgsImV4cCI6MjAwMTMxMTQ5OH0.gFJSZGvGPx2Prr9bu4TxpkRT1Z7ezDZL-x6zVN1_SE0"
-key_first_half = "sk-KTxNM2KK6CXnudmoeH7"
-
-openai.api_key = key_first_half + "ET3BlbkFJl2hs65lT6USr60WUMxjj"
 
 import time
 
 supabase = create_client(supa_url, supa_key)
 
 class LogPrintCalls:
 
@@ -50,15 +47,15 @@
     return self.response_obj
 
 
 class BetterTest: 
     def __init__(self, user_email: str, openai_api_key: str):
         self.user_email = user_email
         self.run_id = uuid.uuid4()
-    
+        openai.api_key = openai_api_key
     def __enter__(self):
         self.original_print = builtins.print
 
         def new_print(*args, **kwargs):
             self.log_function("print", *args)
             self.original_print(*args, **kwargs)
```

### Comparing `bettertest-0.1.93/bettertest/promptTemplate.py` & `bettertest-0.1.94/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.93/bettertest/test.py` & `bettertest-0.1.94/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.93/PKG-INFO` & `bettertest-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.93
+Version: 0.1.94
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

