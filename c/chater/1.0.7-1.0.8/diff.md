# Comparing `tmp/chater-1.0.7.tar.gz` & `tmp/chater-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chater-1.0.7.tar", last modified: Sat Jun  3 11:17:27 2023, max compression
+gzip compressed data, was "chater-1.0.8.tar", last modified: Sat Jun  3 12:22:27 2023, max compression
```

## Comparing `chater-1.0.7.tar` & `chater-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 11:17:18.000000 chater-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-03 11:17:27.902948 chater-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-03 11:17:18.000000 chater-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.898948 chater-1.0.7/chater/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-03 11:17:18.000000 chater-1.0.7/chater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater/api/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater/api/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/abstract/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/chabot.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/stream_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-03 11:17:18.000000 chater-1.0.7/chater/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:17:27.902948 chater-1.0.7/chater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 11:17:27.000000 chater-1.0.7/chater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 11:17:27.902948 chater-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-03 11:17:18.000000 chater-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:22:27.212616 chater-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 12:22:13.000000 chater-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-03 12:22:27.212616 chater-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-03 12:22:13.000000 chater-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:22:27.204616 chater-1.0.8/chater/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-03 12:22:13.000000 chater-1.0.8/chater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:22:27.208616 chater-1.0.8/chater/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:22:27.212616 chater-1.0.8/chater/api/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/abstract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/abstract/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/chabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/stream_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-03 12:22:13.000000 chater-1.0.8/chater/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:22:27.208616 chater-1.0.8/chater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-03 12:22:27.000000 chater-1.0.8/chater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-03 12:22:27.000000 chater-1.0.8/chater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:22:27.000000 chater-1.0.8/chater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 12:22:27.000000 chater-1.0.8/chater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 12:22:27.000000 chater-1.0.8/chater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:22:27.212616 chater-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-03 12:22:13.000000 chater-1.0.8/setup.py
```

### Comparing `chater-1.0.7/LICENSE` & `chater-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/PKG-INFO` & `chater-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.7
+Version: 1.0.8
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -53,12 +53,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()         # openai account models list
+models = chater.Models.list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

### Comparing `chater-1.0.7/README.md` & `chater-1.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()         # openai account models list
+models = chater.Models.list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

### Comparing `chater-1.0.7/chater/api/abstract/client.py` & `chater-1.0.8/chater/api/abstract/client.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater/api/abstract/typings.py` & `chater-1.0.8/chater/api/abstract/typings.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater/api/auth.py` & `chater-1.0.8/chater/api/auth.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater/api/billing.py` & `chater-1.0.8/chater/api/billing.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater/api/chabot.py` & `chater-1.0.8/chater/api/chabot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         messages_list = []
 
         while True:
             print('\033[31mUser: \033[0m', end='')
             
             prompt = input()
 
-            messages_list.append({'role': 'user', 'content': list})
+            messages_list.append({'role': 'user', 'content': prompt})
 
             print('\033[33mAssistant: \033[0m', end='')
 
             try:
                 content = StreamCompletion.create(
                     messages=messages_list,
                     **kwargs
```

### Comparing `chater-1.0.7/chater/api/models.py` & `chater-1.0.8/chater/api/models.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater/api/stream_completion.py` & `chater-1.0.8/chater/api/stream_completion.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.7/chater.egg-info/PKG-INFO` & `chater-1.0.8/chater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.7
+Version: 1.0.8
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -53,12 +53,12 @@
 
 ## Other
 ```python
 import chater
 
 chater.openai_api_key = 'your api key'
 
-models = chater.Models.models_list()         # openai account models list
+models = chater.Models.list()         # openai account models list
 
 usage = chater.Billing.usage()                # openai account usage
 subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

