# Comparing `tmp/thiruchatgpt-0.0.1-py3-none-any.whl.zip` & `tmp/thiruchatgpt-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2294 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1862 b- defN 23-Jun-02 14:16 chatgpttwilio/__init__.py
--rw-rw-rw-  2.0 fat      676 b- defN 23-Jun-02 14:32 thiruchatgpt-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 14:32 thiruchatgpt-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-02 14:32 thiruchatgpt-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      399 b- defN 23-Jun-02 14:32 thiruchatgpt-0.0.1.dist-info/RECORD
-5 files, 3043 bytes uncompressed, 1546 bytes compressed:  49.2%
+Zip file size: 2204 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1792 b- defN 23-Jun-03 04:22 chatgpttwilio/__init__.py
+-rw-rw-rw-  2.0 fat      676 b- defN 23-Jun-03 04:23 thiruchatgpt-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 04:23 thiruchatgpt-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-03 04:23 thiruchatgpt-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      399 b- defN 23-Jun-03 04:23 thiruchatgpt-0.0.2.dist-info/RECORD
+5 files, 2973 bytes uncompressed, 1456 bytes compressed:  51.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: chatgpttwilio/__init__.py
 Comment: 
 
-Filename: thiruchatgpt-0.0.1.dist-info/METADATA
+Filename: thiruchatgpt-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: thiruchatgpt-0.0.1.dist-info/WHEEL
+Filename: thiruchatgpt-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: thiruchatgpt-0.0.1.dist-info/top_level.txt
+Filename: thiruchatgpt-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: thiruchatgpt-0.0.1.dist-info/RECORD
+Filename: thiruchatgpt-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chatgpttwilio/__init__.py

```diff
@@ -1,46 +1,47 @@
 from twilio.twiml.messaging_response import MessagingResponse
 from twilio.rest import Client
 import openai
 
 
-# app = Flask(__name__)
-# app.config['SECRET_KEY'] = 'top-secret!'
 
-account_sid = ''              # 'ACa51a0ff34c56f8347c2da4460cbef46c'                                                 # Twilio Account SID
-auth_token  = ''             # '51091ac3cef7ce5b18e2f401f29ba7d8'                                                    # Twilio Account Auth Token
-client = Client(account_sid, auth_token)
+account_sid = ''                 # Twilio Account SID
+auth_token  = ''                 # Twilio Account Auth Token
 
 openai_apikey = ''
 
-openai.api_key = openai_apikey  #"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"                                              # OPEN-AI API KEY
-completion = openai.Completion()
 
-start_chat_log = '''Human: Hello, who are you?
-AI: I am doing great. How can I help you today?
-'''
-
-def ask(question, chat_log=None):
-    if chat_log is None:
-        chat_log = start_chat_log
-    prompt = f'{chat_log}Human: {question}\nAI:'
-    prompt = question
-    response = completion.create(
-        prompt=prompt, engine="text-davinci-003", stop=['\nHuman'], temperature=0.2,
-        top_p=1, frequency_penalty=0.1, presence_penalty=0.0, best_of=1,
-        max_tokens=256)
-    answer = response.choices[0].text.strip()
-    return answer
-
-def append_interaction_to_chat_log(question, answer, chat_log=None):
-    if chat_log is None:
-        chat_log = start_chat_log
-    return f'{chat_log}Human: {question}\nAI: {answer}\n'
-
-
-def sendMessage(body_mess, phone_number):
-    message = client.messages.create(
-                                from_='whatsapp:+14155238886',                  # With Country Code
-                                body=body_mess,
-                                to='whatsapp:' + phone_number                   # With Country Code
-                            )
-    print(message)  
+if(account_sid and auth_token and openai_apikey):
+    client = Client(account_sid, auth_token)
+
+    openai.api_key = openai_apikey  #"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"                                              # OPEN-AI API KEY
+    completion = openai.Completion()
+
+    start_chat_log = '''Human: Hello, who are you?
+    AI: I am doing great. How can I help you today?
+    '''
+
+    def ask(question, chat_log=None):
+        if chat_log is None:
+            chat_log = start_chat_log
+        prompt = f'{chat_log}Human: {question}\nAI:'
+        prompt = question
+        response = completion.create(
+            prompt=prompt, engine="text-davinci-003", stop=['\nHuman'], temperature=0.2,
+            top_p=1, frequency_penalty=0.1, presence_penalty=0.0, best_of=1,
+            max_tokens=256)
+        answer = response.choices[0].text.strip()
+        return answer
+
+    def append_interaction_to_chat_log(question, answer, chat_log=None):
+        if chat_log is None:
+            chat_log = start_chat_log
+        return f'{chat_log}Human: {question}\nAI: {answer}\n'
+
+
+    def sendMessage(body_mess, phone_number):
+        message = client.messages.create(
+                                    from_='whatsapp:+14155238886',                  # With Country Code
+                                    body=body_mess,
+                                    to='whatsapp:' + phone_number                   # With Country Code
+                                )
+        print(message)
```

## Comparing `thiruchatgpt-0.0.1.dist-info/METADATA` & `thiruchatgpt-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thiruchatgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChatGPT In Whatsapp Using Twilio
 Home-page: UNKNOWN
 Author: Thirumalai K G
 License: UNKNOWN
 Keywords: python,openai,chatgpt,twilio,whatsapp,chatting
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

