# Comparing `tmp/bettertest-0.1.94.tar.gz` & `tmp/bettertest-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.94.tar", max compression
+gzip compressed data, was "bettertest-0.1.96.tar", max compression
```

## Comparing `bettertest-0.1.94.tar` & `bettertest-0.1.96.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.94/README.md
--rw-r--r--   0        0        0     8133 2023-06-03 19:03:35.408389 bettertest-0.1.94/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.94/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.94/bettertest/test.py
--rw-r--r--   0        0        0      336 2023-06-03 19:03:38.461756 bettertest-0.1.94/pyproject.toml
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0     2176 2023-06-03 18:46:39.615567 bettertest-0.1.96/README.md
+-rw-r--r--   0        0        0     8413 2023-06-03 20:00:16.980530 bettertest-0.1.96/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.96/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    26031 2023-06-03 19:48:49.262447 bettertest-0.1.96/bettertest/test.py
+-rw-r--r--   0        0        0      336 2023-06-03 20:00:25.188351 bettertest-0.1.96/pyproject.toml
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 bettertest-0.1.96/PKG-INFO
```

### Comparing `bettertest-0.1.94/README.md` & `bettertest-0.1.96/README.md`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.94/bettertest/__init__.py` & `bettertest-0.1.96/bettertest/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-__version__ = '0.1.94'
+__version__ = '0.1.96'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
 import os 
 from collections import Counter
-from bettertest.promptTemplate import promptTemplate
+# from bettertest.promptTemplate import promptTemplate
+from promptTemplate import promptTemplate
 import concurrent.futures
 import threading
 import uuid
 import builtins
 import inspect
+import webbrowser
 
 
 supa_url = "https://gwfhoxolvmhoszkvddnv.supabase.co"
 supa_key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imd3ZmhveG9sdm1ob3N6a3ZkZG52Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2ODU3MzU0OTgsImV4cCI6MjAwMTMxMTQ5OH0.gFJSZGvGPx2Prr9bu4TxpkRT1Z7ezDZL-x6zVN1_SE0"
 
 import time
 
@@ -64,14 +66,18 @@
     def eval(self, questions, answers, llm_function, num_runs=1):
         try:
             start_time = time.time()
             try:
                 print("🧪 Generating your answers")
                 print("🚀 Go to see your logs: https://better-test.vercel.app/"+str(self.run_id))
                 print("⌛️ It might take 4-5s for your results to start loading...")
+                link = "https://better-test.vercel.app/" + str(self.run_id)
+                print("🚀 Go to see your logs:", link)
+                # Open the link in the browser
+                webbrowser.open(link)
                 model_answer_start_time = time.time()
                 model_answers = self.llm_query_async(questions, answers, llm_function)
                 model_answer_end_time = time.time()
                 print("model answer time: ", model_answer_end_time - model_answer_start_time)
             except:
                 traceback.print_exc()
             # accuracy_scores = []
```

### Comparing `bettertest-0.1.94/bettertest/promptTemplate.py` & `bettertest-0.1.96/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.94/bettertest/test.py` & `bettertest-0.1.96/bettertest/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,10 +90,10 @@
 #  "Berri ingests your data, chunks it, creates embeddings. When user's ask questions, berri does a similarity search and retrieves the most similar chunks to answer the questions. These chunks are then fed into the llm to answer the question"]
     
     answers = ['Sometimes users ask questions that require multiple pieces of context (e.g. What is the age of the actress who plays Meg in Family Guy? -> This requires us to know - Who plays Meg in Family Guy? Mila Kunis + What is Mila Kunis’s age?). To tackle this, we first run the user question through chatGPT, and have it break down that question into sub-components (as seen in the previous example) -> Find the most relevant chunks for each sub-question -> Feed that into chatGPT/GPT-4/whichever model you chose to get the answer to the users question.',
  "You can either create an app with an input_url this way you won't need to scrape the website https://docs.berri.ai/api-reference/endpoint/create_app if this does not work you can also manually scrape the website yourself and create an instance with raw text by passing in JSON chunks to berri",
  "You can either create an app with an input_url this way you won't need to scrape the website https://docs.berri.ai/api-reference/endpoint/create_app if this does not work you can also manually scrape the website yourself and create an instance with raw text by passing in JSON chunks to berri",
  "Berri ingests your data, chunks it, creates embeddings. When user's ask questions, berri does a similarity search and retrieves the most similar chunks to answer the questions. These chunks are then fed into the llm to answer the question"]
 
-    bt = BetterTest("krrish@berri.ai")
+    bt = BetterTest("krrish@berri.ai", "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")
     
     bt.eval(questions, answers, call_openai)
```

### Comparing `bettertest-0.1.94/PKG-INFO` & `bettertest-0.1.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.94
+Version: 0.1.96
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

