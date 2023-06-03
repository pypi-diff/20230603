# Comparing `tmp/bettertest-0.1.6.tar.gz` & `tmp/bettertest-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.6.tar", max compression
+gzip compressed data, was "bettertest-0.1.7.tar", max compression
```

## Comparing `bettertest-0.1.6.tar` & `bettertest-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.6/README.md
--rw-r--r--   0        0        0     8089 2023-06-03 01:03:57.395021 bettertest-0.1.6/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.6/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.6/bettertest/test.py
--rw-r--r--   0        0        0      335 2023-06-03 01:04:00.981675 bettertest-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.7/README.md
+-rw-r--r--   0        0        0     8137 2023-06-03 01:05:52.182957 bettertest-0.1.7/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.7/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.7/bettertest/test.py
+-rw-r--r--   0        0        0      335 2023-06-03 01:05:54.969847 bettertest-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.7/PKG-INFO
```

### Comparing `bettertest-0.1.6/bettertest/__init__.py` & `bettertest-0.1.7/bettertest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -93,14 +93,16 @@
         supabase.table('test_runs').insert(data).execute()
 
     async def async_get_data(self, llm_function, question):
         data = await asyncio.to_thread(llm_function, question)
         return data
     
     def run_test_func(self, llm_function, question, solution_answer, index): 
+        print(index)
+        print(type(index))
         # Run the test function against each question
         log_print_calls = LogPrintCalls()
         with log_print_calls:
             result = llm_function(question)
         # log the results here
         log_output = log_print_calls.return_response_obj()
         tmp_obj = self.async_inner_func_internal_eval(question, result, solution_answer)
```

### Comparing `bettertest-0.1.6/bettertest/promptTemplate.py` & `bettertest-0.1.7/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.6/bettertest/test.py` & `bettertest-0.1.7/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.6/PKG-INFO` & `bettertest-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

