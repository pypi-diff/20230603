# Comparing `tmp/curtely-0.0.2.tar.gz` & `tmp/curtely-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtely-0.0.2.tar", last modified: Mon Apr 17 06:09:24 2023, max compression
+gzip compressed data, was "curtely-0.0.3.tar", last modified: Sat Jun  3 06:51:26 2023, max compression
```

## Comparing `curtely-0.0.2.tar` & `curtely-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 06:09:24.542222 curtely-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-04-10 12:21:17.000000 curtely-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      915 2023-04-17 06:09:24.542222 curtely-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-17 06:06:22.000000 curtely-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 06:09:24.533848 curtely-0.0.2/curtely/
-drwxrwxrwx   0        0        0        0 2023-04-17 06:09:24.533848 curtely-0.0.2/curtely/curtely.egg-info/
--rw-rw-rw-   0        0        0      915 2023-04-17 06:09:24.000000 curtely-0.0.2/curtely/curtely.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-17 06:09:24.000000 curtely-0.0.2/curtely/curtely.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 06:09:24.000000 curtely-0.0.2/curtely/curtely.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 06:09:24.000000 curtely-0.0.2/curtely/curtely.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4104 2023-04-17 05:54:25.000000 curtely-0.0.2/curtely/curtely.py
--rw-rw-rw-   0        0        0       42 2023-04-17 06:09:24.542222 curtely-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-04-17 06:05:14.000000 curtely-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:51:26.245496 curtely-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 06:03:42.000000 curtely-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      892 2023-06-03 06:51:26.244496 curtely-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-06-03 06:46:07.000000 curtely-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 06:51:26.239495 curtely-0.0.3/curtely/
+drwxrwxrwx   0        0        0        0 2023-06-03 06:51:26.243502 curtely-0.0.3/curtely/curtely.egg-info/
+-rw-rw-rw-   0        0        0      892 2023-06-03 06:51:26.000000 curtely-0.0.3/curtely/curtely.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-03 06:51:26.000000 curtely-0.0.3/curtely/curtely.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 06:51:26.000000 curtely-0.0.3/curtely/curtely.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 06:51:26.000000 curtely-0.0.3/curtely/curtely.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4141 2023-06-03 06:45:40.000000 curtely-0.0.3/curtely/curtely.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 06:51:26.245496 curtely-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-06-03 06:47:59.000000 curtely-0.0.3/setup.py
```

### Comparing `curtely-0.0.2/LICENSE` & `curtely-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curtely-0.0.2/PKG-INFO` & `curtely-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: curtely
-Version: 0.0.2
+Version: 0.0.3
 Summary: a 🧑‍💻Telegram API🧑‍💻 wrapper
 Home-page: https://github.com/CURVoid/curtely
 Author: VOID
 License: APACHE 2.0
 Keywords: telegram,api,curtely,messenger
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Curtely v0.0.2 Telegram API wrapper
+## Curtely v0.0.3 Telegram API wrapper
 ## Change log
-- Added `message_handler` decoretor and renamed `handle_updates` to `run`
+- Added `chat_id()` to `Message`
+- Renamed `TelegramAPI` on `Bot`
 ## Usage
 ```python
 # Here is an example of an easy echo bot
 import curtely
 
 TOKEN = "your-token-here"
 
-bot = curtely.TelegramAPI(TOKEN)
+bot = curtely.Bot(TOKEN)
 
 @curtely.message_handler(bot)
-def message_handler(api: curtely.TelegramAPI, message: curtely.Message):
+def message_handler(api: curtely.Bot, message: curtely.Message):
     api.send_message(message.reply(message.content()))
 
 bot.run()
 ```
```

### Comparing `curtely-0.0.2/curtely/curtely.egg-info/PKG-INFO` & `curtely-0.0.3/curtely/curtely.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: curtely
-Version: 0.0.2
+Version: 0.0.3
 Summary: a 🧑‍💻Telegram API🧑‍💻 wrapper
 Home-page: https://github.com/CURVoid/curtely
 Author: VOID
 License: APACHE 2.0
 Keywords: telegram,api,curtely,messenger
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Curtely v0.0.2 Telegram API wrapper
+## Curtely v0.0.3 Telegram API wrapper
 ## Change log
-- Added `message_handler` decoretor and renamed `handle_updates` to `run`
+- Added `chat_id()` to `Message`
+- Renamed `TelegramAPI` on `Bot`
 ## Usage
 ```python
 # Here is an example of an easy echo bot
 import curtely
 
 TOKEN = "your-token-here"
 
-bot = curtely.TelegramAPI(TOKEN)
+bot = curtely.Bot(TOKEN)
 
 @curtely.message_handler(bot)
-def message_handler(api: curtely.TelegramAPI, message: curtely.Message):
+def message_handler(api: curtely.Bot, message: curtely.Message):
     api.send_message(message.reply(message.content()))
 
 bot.run()
 ```
```

### Comparing `curtely-0.0.2/curtely/curtely.py` & `curtely-0.0.3/curtely/curtely.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import threading
 import requests
 import time
 
-from typing import List, Type, Callable
+from typing import List, Callable
 
 class Message:
     def __init__(self, content: str, chat_id: str, author_username: str = None, author_name: str = None, author_id: str = None):
         self._content = content
         self._chat_id = chat_id
         self._author_username = author_username
         self._author_name = author_name
         self._author_id = author_id
 
     def reply(self, content: str):
         return Message(content, self._chat_id)
     
+    def chat_id(self) -> str:
+        return self._chat_id
+    
     def content(self) -> str:
         return self._content
     
     def author_name(self) -> str:
         return self._author_name
     
     def author_username(self) -> str:
@@ -29,15 +32,15 @@
     
 class Command:
     def __init__(self, name: str, description: str, callback: str):
         self._name = name
         self._description = description
         self._callback = callback
 
-class TelegramAPI:
+class Bot:
     def __init__(self, token: str):
         self.token = token
         self._update_id = None
         self._message_handler = None
 
     def send_message(self, message: Message):
         url = f"https://api.telegram.org/bot{self.token}/sendMessage"
@@ -114,11 +117,11 @@
                     threads.append(thread)
                 
             except Exception as e:
                 print(f"error: {e}")
             finally:
                 time.sleep(read_cooldown)
 
-def message_handler(api: TelegramAPI):
-    def wrapper(func: Callable[[TelegramAPI, Message], None]):
+def message_handler(api: Bot):
+    def wrapper(func: Callable[[Bot, Message], None]):
         api.set_message_handler(func)
     return wrapper
```

### Comparing `curtely-0.0.2/setup.py` & `curtely-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 ]
 
 CURRENT_VERSION = sys.version_info[:2]
 REQUIRED_VERSION = (3, 7)
 
 if CURRENT_VERSION < REQUIRED_VERSION:
     sys.stderr.write(
-        f"""Current python version ({CURRENT_VERSION[0]}.{CURRENT_VERSION[1]}) is lower than required ({REQUIRED_VERSION[0]}.{REQUIRED_VERSION[1]})
-        """
+        f"""Current python version ({CURRENT_VERSION[0]}.{CURRENT_VERSION[1]}) is lower than required ({REQUIRED_VERSION[0]}.{REQUIRED_VERSION[1]})"""
     )
 
 setup(
     name="curtely",
-    version="0.0.2",
+    version="0.0.3",
     description="a 🧑‍💻Telegram API🧑‍💻 wrapper",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/CURVoid/curtely",
     author="VOID",
     license="APACHE 2.0", 
     keywords=["telegram", "api", "curtely", "messenger"],
     package_dir={"": "curtely"},
     py_modules=["curtely"],
     classifiers=classifiers,
-)
+)
```

