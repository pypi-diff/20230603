# Comparing `tmp/chater-1.0.5.tar.gz` & `tmp/chater-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chater-1.0.5.tar", last modified: Fri Jun  2 16:52:40 2023, max compression
+gzip compressed data, was "chater-1.0.6.tar", last modified: Sat Jun  3 05:27:23 2023, max compression
```

## Comparing `chater-1.0.5.tar` & `chater-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:52:40.563632 chater-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:52:27.000000 chater-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:52:40.563632 chater-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 16:52:27.000000 chater-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:52:40.563632 chater-1.0.5/chater/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:52:27.000000 chater-1.0.5/chater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:52:40.563632 chater-1.0.5/chater/api/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:52:40.563632 chater-1.0.5/chater/api/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/abstract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/abstract/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/stream_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 16:52:27.000000 chater-1.0.5/chater/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:52:40.563632 chater-1.0.5/chater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:52:40.000000 chater-1.0.5/chater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 16:52:40.000000 chater-1.0.5/chater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:52:40.000000 chater-1.0.5/chater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:52:40.000000 chater-1.0.5/chater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 16:52:40.000000 chater-1.0.5/chater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:52:40.563632 chater-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-02 16:52:27.000000 chater-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 05:27:13.000000 chater-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-03 05:27:23.765367 chater-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-03 05:27:13.000000 chater-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.761367 chater-1.0.6/chater/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-03 05:27:13.000000 chater-1.0.6/chater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/chater/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.765367 chater-1.0.6/chater/api/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/abstract/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/stream_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-03 05:27:13.000000 chater-1.0.6/chater/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:27:23.761367 chater-1.0.6/chater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 05:27:23.000000 chater-1.0.6/chater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:27:23.765367 chater-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-03 05:27:13.000000 chater-1.0.6/setup.py
```

### Comparing `chater-1.0.5/LICENSE` & `chater-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chater-1.0.5/PKG-INFO` & `chater-1.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.5
+Version: 1.0.6
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Chatbot
+# Chater
 
 Using ChatGPT in Python.
 
 Use the same format for the messages as you would for the [official OpenAI API](https://platform.openai.com/docs/api-reference/chat).
 
 ## Installation
 
 Download or clone this GitHub repo  
 install requirements with:
 
 ```bash
 pip install chater
 ```
 
-## A Simple Example
+## Simple Example
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
-import chatbot
+import chater
 
-chatbot.api_key = ''
-chatbot.StreamCompletion.create('Hello world!')
+chater.api_key = 'your api key'
 
+chater.StreamCompletion.create('Hey!')
+chater.StreamCompletion.create('Hello world!')
 ```
+
+```python
+import chater
+
+chater.StreamCompletion.create('Hello world!', openai_api_key='your api key')
+```
+
 ### 2. Accessing GPT through an Access Token (Free 3.5).
 ```python
-import chatbot
+import chater
+
+chater.openai_email = 'your openai email'
+chater.openai_password = 'your openai password'
+chater.openai_api_key = chater.Auth().access_token
+
+chater.StreamCompletion.create('Hello world!')
+```
+
+## Other
+```python
+import chater
+
+chater.openai_api_key = 'your api key'
+
+models = chater.Models.models_list()          # openai account models list
 
-auth = chatbot.Auth('email', 'password')
-chatbot.api_key = auth.get_access_token()
-chatbot.StreamCompletion.create('Hello world!')
+usage = chater.Billing.usage()                # openai account usage
+subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

### Comparing `chater-1.0.5/chater/api/abstract/typings.py` & `chater-1.0.6/chater/api/abstract/typings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-from pydantic import BaseModel
 from datetime import datetime
 from typing import List, Optional
 
+from pydantic import BaseModel
+
+
 class AuthTokenResponse(BaseModel):
     scope: str
-    access_token: str
     expires_in: datetime
     token_type: str
+    access_token: str
 
 
 class Plan(BaseModel):
-    id:    str
+    id: str
     title: str
 
 
 class SubscriptionResponse(BaseModel):
-    plan:                  Plan
-    object:                str
-    account_name:          str
-    soft_limit_usd:        float
-    hard_limit_usd:        float
+    plan: Plan
+    object: str
+    account_name: str
+    soft_limit_usd: float
+    hard_limit_usd: float
     system_hard_limit_usd: float
-    has_payment_method:    bool
-    access_until:          datetime
+    has_payment_method: bool
+    access_until: datetime
 
 
 class Message(BaseModel):
-    role:     Optional[str]
-    content:  Optional[str]
+    role: Optional[str]
+    content: Optional[str]
 
 
 class Choice(BaseModel):
-    index:         int
-    delta:         Message
+    index: int
+    delta: Message
     finish_reason: Optional[str]
 
 
 class StreamCompletionResponse(BaseModel):
-    id:      str
-    object:  str
+    id: str
+    object: str
     created: int
-    model:   str
-    choices: List[Choice]
+    model: str
+    choices: List[Choice]
```

### Comparing `chater-1.0.5/chater/api/auth.py` & `chater-1.0.6/chater/api/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,77 @@
 from urllib.parse import urlparse, parse_qs
 
+import chater
 from .utils import generate_random_token, generate_code_challenge
-
 from .abstract.client import HttpClient
 from .abstract.typings import AuthTokenResponse
 
 
 class Auth:
-    def __init__(self, email: str, password: str) -> None:
-        self.email = email
-        self.password = password
+    def __init__(self, email: str = None, password: str = None) -> None:
+        if not email:
+            self.email = chater.openai_email
+        if not password:
+            self.password = chater.openai_password
 
         self._req = HttpClient()
         self._code_verifier = generate_random_token()
         self._state = self._get_state()
 
-        self.auth_token = self._auth_token()
-
-    def get_access_token(self) -> str:
-        return self.auth_token.access_token
+        self._auth_token_resp = self._auth_token()
 
-    def get_token_expires(self):
-        return self.auth_token.expires_in
+        self.access_token = self._auth_token_resp.access_token
+        self.access_token_expires_in = self._auth_token_resp.expires_in
 
     def _get_state(self) -> str:
         url = 'https://auth0.openai.com/authorize'
         params = {
-            'client_id': 'pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh',
-            'audience': 'https://api.openai.com/v1',
-            'redirect_uri': 'com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback',
-            'scope': 'openid email profile offline_access model.request model.read organization.read offline',
-            'response_type': 'code',
-            'code_challenge': f'{generate_code_challenge(self._code_verifier)}',
-            'code_challenge_method': 'S256',
-            'prompt': 'login'
+            'scope':            'openid email profile offline_access model.request model.read organization.read offline',
+            'prompt':           'login',
+            'client_id':        'pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh',
+            'audience':         'https://api.openai.com/v1',
+            'redirect_uri':     'com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback',
+            'response_type':    'code',
+            'code_challenge':  f'{generate_code_challenge(self._code_verifier)}',
+            'code_challenge_method': 'S256'
         }
-
         response = self._req.get(url, params=params, allow_redirects=True)
 
         if response.ok:
             response_url_params = parse_qs(urlparse(response.url).query)
             return response_url_params['state'][0]
 
     def _identifier(self) -> None:
         url = 'https://auth0.openai.com/u/login/identifier'
         params = {'state': self._state}
-        json_data = {
-            'state': self._state,
-            'username': self.email,
-            'action': 'default',
-            'is-brave': 'false',
-            'js-available': 'true',
-            'webauthn-available': 'true',
+        json = {
+            'state':                self._state,
+            'username':             self.email,
+            'action':               'default',
+            'is-brave':             'false',
+            'js-available':         'true',
+            'webauthn-available':   'true',
             'webauthn-platform-available': 'false',
         }
 
-        self._req.post(url, json=json_data, params=params,
+        self._req.post(url, json=json, params=params,
                        allow_redirects=False)
 
     def _login_password(self) -> str:
         url = 'https://auth0.openai.com/u/login/password'
         params = {'state': self._state}
-        json_data = {
-            'state': self._state,
-            'username': self.email,
-            'password': self.password,
-            'action': 'default',
+        json = {
+            'state':     self._state,
+            'username':  self.email,
+            'password':  self.password,
+            'action':    'default',
         }
 
         response = self._req.post(
-            url, params=params, json=json_data, allow_redirects=False)
+            url, params=params, json=json, allow_redirects=False)
 
         if response.status_code == 302:
             location = response.headers['Location']
 
         response = self._req.get(
             f'https://auth0.openai.com{location}', allow_redirects=False)
 
@@ -84,20 +82,20 @@
         self._identifier()
 
         location = self._login_password()
 
         param_code = parse_qs(urlparse(location).query)['code'][0]
 
         url = 'https://auth0.openai.com/oauth/token'
-        json_data = {
-            'code': param_code,
-            'code_verifier': self._code_verifier,
-            'grant_type': 'authorization_code',
-            'client_id': 'pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh',
-            'redirect_uri': 'com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback'
+        json = {
+            'code':           param_code,
+            'code_verifier':  self._code_verifier,
+            'grant_type':     'authorization_code',
+            'client_id':      'pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh',
+            'redirect_uri':   'com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback'
         }
 
         response = self._req.post(
-            url, json=json_data, allow_redirects=False)
+            url, json=json, allow_redirects=False)
 
         if response.status_code == 200:
             return AuthTokenResponse(**response.json())
```

### Comparing `chater-1.0.5/chater/api/stream_completion.py` & `chater-1.0.6/chater/api/stream_completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,23 +13,31 @@
     @staticmethod
     def create(
         messages:          Union[list[dict], str],
         model:             str = 'gpt-3.5-turbo',
         temperature:       float = 1.0,
         presence_penalty:  float = 0,
         frequency_penalty: float = 0,
+        openai_api_key:    str = None,
+        openai_api_base:   str = None,
     ) -> None:
         if isinstance(messages, str):
             messages = [{"role": "user", "content": messages}]
 
-        api_url = f'{chater.api_base}/chat/completions'
+        if not openai_api_key:
+            openai_api_key = chater.openai_api_key
+
+        if not openai_api_base:
+            openai_api_base = chater.openai_api_base
+
+        api_url = f'{openai_api_base}/chat/completions'
 
         headers = {
             'Content-Type':    'application/json',
-            'Authorization':  f'Bearer {chater.api_key}'
+            'Authorization':  f'Bearer {openai_api_key}'
         }
 
         json = {
             'stream':            True,
             'model':             model,
             'messages':          messages,
             'temperature':       temperature,
@@ -42,15 +50,15 @@
 
         if response.ok:
             StreamCompletion.stream_handle(response)
         else:
             raise Exception(response.json()['error'])
 
     @staticmethod
-    def stream_handle(response: requests.Response):
+    def stream_handle(response: requests.Response) -> None:
         for line in response.iter_lines():
             if line:
                 response_str = line.decode('utf-8').replace('data: ', '')
                 if response_str == '[DONE]':  # stream terminated
                     break
                 response_dict = loads(response_str)
                 completion = StreamCompletionResponse(**response_dict)
```

### Comparing `chater-1.0.5/chater.egg-info/PKG-INFO` & `chater-1.0.6/chater.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.5
+Version: 1.0.6
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Chatbot
+# Chater
 
 Using ChatGPT in Python.
 
 Use the same format for the messages as you would for the [official OpenAI API](https://platform.openai.com/docs/api-reference/chat).
 
 ## Installation
 
 Download or clone this GitHub repo  
 install requirements with:
 
 ```bash
 pip install chater
 ```
 
-## A Simple Example
+## Simple Example
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
-import chatbot
+import chater
 
-chatbot.api_key = ''
-chatbot.StreamCompletion.create('Hello world!')
+chater.api_key = 'your api key'
 
+chater.StreamCompletion.create('Hey!')
+chater.StreamCompletion.create('Hello world!')
 ```
+
+```python
+import chater
+
+chater.StreamCompletion.create('Hello world!', openai_api_key='your api key')
+```
+
 ### 2. Accessing GPT through an Access Token (Free 3.5).
 ```python
-import chatbot
+import chater
+
+chater.openai_email = 'your openai email'
+chater.openai_password = 'your openai password'
+chater.openai_api_key = chater.Auth().access_token
+
+chater.StreamCompletion.create('Hello world!')
+```
+
+## Other
+```python
+import chater
+
+chater.openai_api_key = 'your api key'
+
+models = chater.Models.models_list()          # openai account models list
 
-auth = chatbot.Auth('email', 'password')
-chatbot.api_key = auth.get_access_token()
-chatbot.StreamCompletion.create('Hello world!')
+usage = chater.Billing.usage()                # openai account usage
+subscription = chater.Billing.subscription()  # openai account subscription
 ```
```

