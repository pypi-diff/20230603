# Comparing `tmp/bettertest-0.1.7.tar.gz` & `tmp/bettertest-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.7.tar", max compression
+gzip compressed data, was "bettertest-0.1.8.tar", max compression
```

## Comparing `bettertest-0.1.7.tar` & `bettertest-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.7/README.md
--rw-r--r--   0        0        0     8137 2023-06-03 01:05:52.182957 bettertest-0.1.7/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.7/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.7/bettertest/test.py
--rw-r--r--   0        0        0      335 2023-06-03 01:05:54.969847 bettertest-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.8/README.md
+-rw-r--r--   0        0        0     8147 2023-06-03 01:10:06.904519 bettertest-0.1.8/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.8/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.8/bettertest/test.py
+-rw-r--r--   0        0        0      335 2023-06-03 01:10:08.733344 bettertest-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.8/PKG-INFO
```

### Comparing `bettertest-0.1.7/bettertest/__init__.py` & `bettertest-0.1.8/bettertest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -63,14 +63,16 @@
         builtins.print = new_print
 
     def eval(self, questions, answers, llm_function, num_runs=1):
         try:
             start_time = time.time()
             try:
                 print("🧪 Generating your answers")
+                print("🚀 Go to see your logs: https://better-test.vercel.app/"+str(self.run_id))
+                print("⌛️ It might take 4-5s for your results to start loading...")
                 model_answer_start_time = time.time()
                 model_answers = self.llm_query_async(questions, answers, llm_function)
                 model_answer_end_time = time.time()
                 print("model answer time: ", model_answer_end_time - model_answer_start_time)
             except:
                 traceback.print_exc()
             # accuracy_scores = []
@@ -92,41 +94,37 @@
         }
         supabase.table('test_runs').insert(data).execute()
 
     async def async_get_data(self, llm_function, question):
         data = await asyncio.to_thread(llm_function, question)
         return data
     
-    def run_test_func(self, llm_function, question, solution_answer, index): 
-        print(index)
-        print(type(index))
+    def run_test_func(self, llm_function, question, solution_answer): 
         # Run the test function against each question
         log_print_calls = LogPrintCalls()
         with log_print_calls:
             result = llm_function(question)
         # log the results here
         log_output = log_print_calls.return_response_obj()
         tmp_obj = self.async_inner_func_internal_eval(question, result, solution_answer)
         for key in log_output.keys(): 
             if "bettertest" in log_output[key][0][0]:
                 tmp_obj["function_"+key] = log_output[key]
         self.write_to_supabase(tmp_obj)
-        if index == 0: 
-            print("🚀 Go to see your logs: https://better-test.vercel.app/"+str(self.run_id))
         return "Done!"
 
 
     @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
     def llm_query_async(self, question_list, answer_list, llm_function):
         try:
             answers = []
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 for batch in range(0, len(question_list), 250):  # batch process 250 at a time
                     tasks = [
-                        executor.submit(self.run_test_func, llm_function, question, answer_list[batch+i], i)
+                        executor.submit(self.run_test_func, llm_function, question, answer_list[batch+i])
                         for i, question in enumerate(question_list[batch:batch + 250])
                     ]
                     answer = [task.result() for task in tasks]
                     answers.extend(answer)
             return answers
         except:
             traceback.print_exc()
```

### Comparing `bettertest-0.1.7/bettertest/promptTemplate.py` & `bettertest-0.1.8/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.7/bettertest/test.py` & `bettertest-0.1.8/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.7/PKG-INFO` & `bettertest-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

