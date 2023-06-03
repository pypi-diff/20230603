# Comparing `tmp/chater-1.0.6.tar.gz` & `tmp/chater-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chater-1.0.6.tar", last modified: Sat Jun  3 05:27:23 2023, max compression
+gzip compressed data, was "chater-1.0.7.tar", last modified: Sat Jun  3 11:17:27 2023, max compression
```

## Comparing `chater-1.0.6.tar` & `chater-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 05:27:13.000000 chater-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-03 05:27:23.765367 chater-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-03 05:27:13.000000 chater-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.761367 chater-1.0.6/chater/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-03 05:27:13.000000 chater-1.0.6/chater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/chater/api/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/chater/api/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/stream_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.761367 chater-1.0.6/chater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:27:23.765367 chater-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-03 05:27:13.000000 chater-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 11:17:18.000000 chater-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-03 11:17:27.902948 chater-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-03 11:17:18.000000 chater-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.898948 chater-1.0.7/chater/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-03 11:17:18.000000 chater-1.0.7/chater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater/api/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/chabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/stream_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 11:17:27.902948 chater-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-03 11:17:18.000000 chater-1.0.7/setup.py
```

### Comparing `chater-1.0.6/LICENSE` & `chater-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chater-1.0.6/PKG-INFO` & `chater-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.6
+Version: 1.0.7
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -27,15 +27,15 @@
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chater
 
 chater.api_key = 'your api key'
 
 chater.StreamCompletion.create('Hey!')
-chater.StreamCompletion.create('Hello world!')
+chater.StreamCompletion.create('Hello world!', temperature=1)
 ```
 
 ```python
 import chater
 
 chater.StreamCompletion.create('Hello world!', openai_api_key='your api key')
 ```
@@ -53,12 +53,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()          # openai account models list
+models = chater.Models.models_list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

### Comparing `chater-1.0.6/README.md` & `chater-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chater
 
 chater.api_key = 'your api key'
 
 chater.StreamCompletion.create('Hey!')
-chater.StreamCompletion.create('Hello world!')
+chater.StreamCompletion.create('Hello world!', temperature=1)
 ```
 
 ```python
 import chater
 
 chater.StreamCompletion.create('Hello world!', openai_api_key='your api key')
 ```
@@ -43,12 +43,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()          # openai account models list
+models = chater.Models.models_list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

### Comparing `chater-1.0.6/chater/api/abstract/client.py` & `chater-1.0.7/chater/api/abstract/client.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.6/chater/api/abstract/typings.py` & `chater-1.0.7/chater/api/abstract/typings.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.6/chater/api/auth.py` & `chater-1.0.7/chater/api/auth.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.6/chater/api/billing.py` & `chater-1.0.7/chater/api/billing.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.6/chater/api/models.py` & `chater-1.0.7/chater/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 
 import chater
 
 class Models:
-    def models_list(openai_api_key: str = None, openai_api_base: str = None) -> dict:
+    def list(openai_api_key: str = None, openai_api_base: str = None) -> dict:
         """Lists the currently available models"""
         if not openai_api_key:
             openai_api_key = chater.openai_api_key
         if not openai_api_base:
             openai_api_base = chater.openai_api_base
 
         api_url = f'{openai_api_base}/models'
```

### Comparing `chater-1.0.6/chater/api/stream_completion.py` & `chater-1.0.7/chater/api/stream_completion.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         messages:          Union[list[dict], str],
         model:             str = 'gpt-3.5-turbo',
         temperature:       float = 1.0,
         presence_penalty:  float = 0,
         frequency_penalty: float = 0,
         openai_api_key:    str = None,
         openai_api_base:   str = None,
-    ) -> None:
+    ) -> str:
         if isinstance(messages, str):
             messages = [{"role": "user", "content": messages}]
 
         if not openai_api_key:
             openai_api_key = chater.openai_api_key
 
         if not openai_api_base:
@@ -45,23 +45,26 @@
             'frequency_penalty': frequency_penalty
         }
 
         response = requests.post(
             api_url, headers=headers, json=json, stream=True)
 
         if response.ok:
-            StreamCompletion.stream_handle(response)
+            return StreamCompletion.stream_handle(response)
         else:
             raise Exception(response.json()['error'])
 
     @staticmethod
-    def stream_handle(response: requests.Response) -> None:
+    def stream_handle(response: requests.Response) -> str:
+        full_content = ''
         for line in response.iter_lines():
             if line:
                 response_str = line.decode('utf-8').replace('data: ', '')
                 if response_str == '[DONE]':  # stream terminated
                     break
                 response_dict = loads(response_str)
                 completion = StreamCompletionResponse(**response_dict)
                 content = completion.choices[0].delta.content
                 if content:
+                    full_content = full_content + content
                     print(content, end='', flush=True)
+        return full_content
```

### Comparing `chater-1.0.6/chater.egg-info/PKG-INFO` & `chater-1.0.7/chater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.6
+Version: 1.0.7
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -27,15 +27,15 @@
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chater
 
 chater.api_key = 'your api key'
 
 chater.StreamCompletion.create('Hey!')
-chater.StreamCompletion.create('Hello world!')
+chater.StreamCompletion.create('Hello world!', temperature=1)
 ```
 
 ```python
 import chater
 
 chater.StreamCompletion.create('Hello world!', openai_api_key='your api key')
 ```
@@ -53,12 +53,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()          # openai account models list
+models = chater.Models.models_list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

