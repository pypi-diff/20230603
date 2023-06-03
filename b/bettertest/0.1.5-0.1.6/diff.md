# Comparing `tmp/bettertest-0.1.5.tar.gz` & `tmp/bettertest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.5.tar", max compression
+gzip compressed data, was "bettertest-0.1.6.tar", max compression
```

## Comparing `bettertest-0.1.5.tar` & `bettertest-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.5/README.md
--rw-r--r--   0        0        0     8093 2023-06-03 01:02:26.169850 bettertest-0.1.5/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.5/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.5/bettertest/test.py
--rw-r--r--   0        0        0      335 2023-06-03 01:02:27.775111 bettertest-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.6/README.md
+-rw-r--r--   0        0        0     8089 2023-06-03 01:03:57.395021 bettertest-0.1.6/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.6/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.6/bettertest/test.py
+-rw-r--r--   0        0        0      335 2023-06-03 01:04:00.981675 bettertest-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.6/PKG-INFO
```

### Comparing `bettertest-0.1.5/bettertest/__init__.py` & `bettertest-0.1.6/bettertest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -116,15 +116,15 @@
     @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
     def llm_query_async(self, question_list, answer_list, llm_function):
         try:
             answers = []
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 for batch in range(0, len(question_list), 250):  # batch process 250 at a time
                     tasks = [
-                        executor.submit(self.run_test_func, llm_function, question, answer_list[batch+i], index)
+                        executor.submit(self.run_test_func, llm_function, question, answer_list[batch+i], i)
                         for i, question in enumerate(question_list[batch:batch + 250])
                     ]
                     answer = [task.result() for task in tasks]
                     answers.extend(answer)
             return answers
         except:
             traceback.print_exc()
```

### Comparing `bettertest-0.1.5/bettertest/promptTemplate.py` & `bettertest-0.1.6/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.5/bettertest/test.py` & `bettertest-0.1.6/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.5/PKG-INFO` & `bettertest-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

