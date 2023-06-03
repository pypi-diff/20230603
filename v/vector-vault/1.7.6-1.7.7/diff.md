# Comparing `tmp/vector_vault-1.7.6.tar.gz` & `tmp/vector_vault-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.6.tar", last modified: Sat Jun  3 06:57:48 2023, max compression
+gzip compressed data, was "vector_vault-1.7.7.tar", last modified: Sat Jun  3 21:45:42 2023, max compression
```

## Comparing `vector_vault-1.7.6.tar` & `vector_vault-1.7.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.135571 vector_vault-1.7.6/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:57:48.135391 vector_vault-1.7.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 06:57:48.135605 vector_vault-1.7.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 06:57:44.000000 vector_vault-1.7.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.132430 vector_vault-1.7.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 06:57:48.000000 vector_vault-1.7.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 06:57:48.134996 vector_vault-1.7.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.6/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 06:47:29.000000 vector_vault-1.7.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 06:47:22.000000 vector_vault-1.7.6/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.6/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    27483 2023-06-03 06:57:38.000000 vector_vault-1.7.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.6/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.657993 vector_vault-1.7.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 21:45:42.657856 vector_vault-1.7.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 21:45:42.658029 vector_vault-1.7.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 21:45:34.000000 vector_vault-1.7.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.654966 vector_vault-1.7.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 21:45:42.000000 vector_vault-1.7.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 21:45:42.657437 vector_vault-1.7.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7707 2023-06-03 21:28:12.000000 vector_vault-1.7.7/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 21:45:10.000000 vector_vault-1.7.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 21:45:08.000000 vector_vault-1.7.7/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.7/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26431 2023-06-03 21:45:19.000000 vector_vault-1.7.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.7/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.7/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.6/LICENSE` & `vector_vault-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/PKG-INFO` & `vector_vault-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.6
+Version: 1.7.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.6/README.md` & `vector_vault-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/setup.py` & `vector_vault-1.7.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.6",
+    version="1.7.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.7/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.6
+Version: 1.7.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.6/vectorvault/__init__.py` & `vector_vault-1.7.7/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/ai.py` & `vector_vault-1.7.7/vectorvault/ai.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,21 +61,23 @@
                             yield content
                         
                     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', stream=False):
         prompt_template = """
         Use the following pieces of context to answer the question at the end. 
-        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't preface, and don't give any warnings at the end.
+        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't give any disclaimers or warnings at the end.
 
-        {context}
+        Our Conversation History (if any): {history}
+
+        Context - Context - Context: {context}
 
         Question: {question}
 
-        (answer the question directly. Most importantly, make your answer interesting, engaging, and helpful) 
+        (answer the question directly. Most importantly, answer interesting, engaging, and helpful) 
         Answer:"""
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
 
@@ -100,21 +102,20 @@
                 if double_check > 4096:
                     remainder = double_check - 4096
                     char_to_take_away = remainder * 5
                     context = context[char_to_take_away:]
 
         # Format the prompt
         user_input = history + user_input
-        prompt = prompt_template.format(context=context, question=user_input)
-
+        prompt = prompt_template.format(context=context, history=history, question=user_input)
         if stream == False:
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
-                    {"role": "user", "content": f"{prompt}"}]
+                    {"role": "user", "content": f"{prompt}"}],
             )
             return response['choices'][0]['message']['content']
         elif stream == True:
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
                     {"role": "user", "content": f"{prompt}"}],
```

### Comparing `vector_vault-1.7.6/vectorvault/cloudmanager.py` & `vector_vault-1.7.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/creds.py` & `vector_vault-1.7.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/download.py` & `vector_vault-1.7.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/itemize.py` & `vector_vault-1.7.7/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/signup.py` & `vector_vault-1.7.7/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/vault.py` & `vector_vault-1.7.7/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
     def get_chat_cloud(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         return call_get_chat(self.user, self.vault, self.api, text, history, summary, get_context, n_context, return_context, expansion, history_search, model, include_context_meta)
     
-    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
+    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage: 
             `response = vault.get_chat(text)`
@@ -395,22 +395,14 @@
                 raise('No input. Add text input to continue')
             self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
             if self.verbose == True:
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
 
-            if expansion:
-                iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
-                intent_expansion = self.ai.llm(iq)
-                kq = f"be general, direct, and short. Don't give an answer, only topics this question falls under to this question: {segment}"
-                knowledge_expansion = self.ai.llm(kq)
-                segment = f'question_intent: {intent_expansion} | {knowledge_expansion}\n\
-                Question: {segment}'
-
             while True:
                 try:
                     if summary and not get_context:
                         response += self.ai.summarize(segment, model=model)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
@@ -439,15 +431,15 @@
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
             return response
         elif return_context == True:
             return {'response': response, 'context': context}
         
-    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False):
+    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage: 
             `response = vault.get_chat(text)`
@@ -521,22 +513,14 @@
                 raise('No input. Add text input to continue')
             self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
             if self.verbose == True:
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
 
-            if expansion:
-                iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
-                intent_expansion = self.ai.llm(iq)
-                kq = f"be general, direct, and short. Don't give an answer, only topics this question falls under to this question: {segment}"
-                knowledge_expansion = self.ai.llm(kq)
-                segment = f'question_intent: {intent_expansion} | {knowledge_expansion}\n\
-                Question: {segment}'
-
             while True:
                 try:
                     if summary and not get_context:
                         response += self.ai.summarize(segment, model=model)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
```

### Comparing `vector_vault-1.7.6/vectorvault/vecreq.py` & `vector_vault-1.7.7/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.6/vectorvault/wrap.py` & `vector_vault-1.7.7/vectorvault/wrap.py`

 * *Files identical despite different names*

