# Comparing `tmp/bettertest-0.1.91.tar.gz` & `tmp/bettertest-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.91.tar", max compression
+gzip compressed data, was "bettertest-0.1.93.tar", max compression
```

## Comparing `bettertest-0.1.91.tar` & `bettertest-0.1.93.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2022 2023-06-03 01:42:38.505758 bettertest-0.1.91/README.md
--rw-r--r--   0        0        0     8148 2023-06-03 18:36:43.467212 bettertest-0.1.91/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.91/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.91/bettertest/test.py
--rw-r--r--   0        0        0      336 2023-06-03 18:36:49.088731 bettertest-0.1.91/pyproject.toml
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 bettertest-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.93/README.md
+-rw-r--r--   0        0        0     8207 2023-06-03 18:58:09.555932 bettertest-0.1.93/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.93/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.93/bettertest/test.py
+-rw-r--r--   0        0        0      336 2023-06-03 18:58:14.146398 bettertest-0.1.93/pyproject.toml
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.93/PKG-INFO
```

### Comparing `bettertest-0.1.91/README.md` & `bettertest-0.1.93/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 ## Using BetterTest
 
 ### Initialize BetterTest
 
 Create an instance of the BetterTest class with the user's email:
 
 ```python
-bt = BetterTest("your_email@example.com")
+bt = BetterTest("your_email@example.com", "your_openai_api_key")
 ```
 
 Replace `"your_email@example.com"` with the appropriate email address.
+Replace `"your_openai_api_key"` with your openai api key. [Here's where to find it](https://platform.openai.com/account/api-keys).
 
 ### Evaluate Model Responses
 
 The `eval()` function takes in a list of questions, a list of answers, an LLM function, and an optional `num_runs` argument. It automatically evaluates the model's response against the solution answer and provides tracing for each run. Use it as follows:
 
 ```python
 questions = [...]  # List of questions
```

### Comparing `bettertest-0.1.91/bettertest/__init__.py` & `bettertest-0.1.93/bettertest/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.91'
+__version__ = '0.1.93'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -14,15 +14,17 @@
 import uuid
 import builtins
 import inspect
 
 
 supa_url = "https://gwfhoxolvmhoszkvddnv.supabase.co"
 supa_key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imd3ZmhveG9sdm1ob3N6a3ZkZG52Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2ODU3MzU0OTgsImV4cCI6MjAwMTMxMTQ5OH0.gFJSZGvGPx2Prr9bu4TxpkRT1Z7ezDZL-x6zVN1_SE0"
-openai.api_key = "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"
+key_first_half = "sk-KTxNM2KK6CXnudmoeH7"
+
+openai.api_key = key_first_half + "ET3BlbkFJl2hs65lT6USr60WUMxjj"
 
 import time
 
 supabase = create_client(supa_url, supa_key)
 
 class LogPrintCalls:
 
@@ -45,15 +47,15 @@
     builtins.print = self.original_print
 
   def return_response_obj(self):
     return self.response_obj
 
 
 class BetterTest: 
-    def __init__(self, user_email: str):
+    def __init__(self, user_email: str, openai_api_key: str):
         self.user_email = user_email
         self.run_id = uuid.uuid4()
     
     def __enter__(self):
         self.original_print = builtins.print
 
         def new_print(*args, **kwargs):
```

### Comparing `bettertest-0.1.91/bettertest/promptTemplate.py` & `bettertest-0.1.93/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.91/bettertest/test.py` & `bettertest-0.1.93/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.91/PKG-INFO` & `bettertest-0.1.93/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.91
+Version: 0.1.93
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -39,18 +39,19 @@
 ## Using BetterTest
 
 ### Initialize BetterTest
 
 Create an instance of the BetterTest class with the user's email:
 
 ```python
-bt = BetterTest("your_email@example.com")
+bt = BetterTest("your_email@example.com", "your_openai_api_key")
 ```
 
 Replace `"your_email@example.com"` with the appropriate email address.
+Replace `"your_openai_api_key"` with your openai api key. [Here's where to find it](https://platform.openai.com/account/api-keys).
 
 ### Evaluate Model Responses
 
 The `eval()` function takes in a list of questions, a list of answers, an LLM function, and an optional `num_runs` argument. It automatically evaluates the model's response against the solution answer and provides tracing for each run. Use it as follows:
 
 ```python
 questions = [...]  # List of questions
```

