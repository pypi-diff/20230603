# Comparing `tmp/iamlistening-0.1.5.tar.gz` & `tmp/iamlistening-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.5.tar", max compression
+gzip compressed data, was "iamlistening-0.1.6.tar", max compression
```

## Comparing `iamlistening-0.1.5.tar` & `iamlistening-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-03 16:37:52.170408 iamlistening-0.1.5/LICENSE
--rw-r--r--   0        0        0     1504 2023-06-03 16:37:52.170408 iamlistening-0.1.5/README.md
--rw-r--r--   0        0        0       99 2023-06-03 16:37:52.866416 iamlistening-0.1.5/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3661 2023-06-03 16:37:52.170408 iamlistening-0.1.5/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-03 16:37:52.866416 iamlistening-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 iamlistening-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-03 21:17:10.508288 iamlistening-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1719 2023-06-03 21:17:10.508288 iamlistening-0.1.6/README.md
+-rw-r--r--   0        0        0       99 2023-06-03 21:17:11.308343 iamlistening-0.1.6/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-03 21:17:10.508288 iamlistening-0.1.6/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-03 21:17:10.508288 iamlistening-0.1.6/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4053 2023-06-03 21:17:10.508288 iamlistening-0.1.6/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-03 21:17:11.308343 iamlistening-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 iamlistening-0.1.6/PKG-INFO
```

### Comparing `iamlistening-0.1.5/LICENSE` & `iamlistening-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.5/README.md` & `iamlistening-0.1.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,25 @@
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
-  from iamlistening import Listerner as bot
-  bot.start()
+  listener = Listener()
+  task = asyncio.create_task(listener.run_forever())
+  while True:
+    try:
+        msg = await listener.get_latest_message()
+        if msg:
+            print(f"Frasier👂: {msg}")
+
+    except Exception as error:
+        print(error)
+  await task
   
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
```

### Comparing `iamlistening-0.1.5/iamlistening/config.py` & `iamlistening-0.1.6/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.5/iamlistening/main.py` & `iamlistening-0.1.6/iamlistening/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
  IAmListening Main
 """
 
-import os
-import sys
 import asyncio
-import logging 
+import logging
+import threading
 
-import apprise
-from apprise import NotifyFormat
-from telethon import TelegramClient, events
 import discord
+from telethon import TelegramClient, events
 import simplematrixbotlib as botlib
 
 from .config import settings
 
 
-# 🤖BOT
-
 class Listener:
-    """ iamlistening class """
+    """ 👂 Listener class """
 
     def __init__(self):
         self.logger = logging.getLogger("Listener")
         self.latest_message = None
-
+        self.loop = asyncio.get_event_loop()
+        self.lock = threading.Lock()
+        self.stopped = False
+    
     async def start(self):
         """start"""
         if settings.discord_webhook_id:
             # DISCORD
             intents = discord.Intents.default()
             intents.message_content = True
             bot = discord.Bot(intents=intents)
@@ -37,71 +35,87 @@
             async def on_ready():
                 await self.post_init()
 
             @bot.event
             async def on_message(message: discord.Message):
                 await self.handle_message(message.content)
             await bot.start(settings.bot_token)
-        # elif settings.matrix_hostname:
-        #     # MATRIX
-        #     config = botlib.Config()
-        #     config.emoji_verify = True
-        #     config.ignore_unverified_devices = True
-        #     config.store_path = './config/matrix/'
-        #     creds = botlib.Creds(
-        #                 settings.matrix_hostname,
-        #                 settings.matrix_user,
-        #                 settings.matrix_pass
-        #                 )
-        #     bot = botlib.Bot(creds, config)
-
-        #     @bot.listener.on_startup
-        #     async def room_joined(room):
-        #         await self.post_init()
-
-        #     @bot.listener.on_message_event
-        #     async def on_matrix_message(room, message):
-        #         await self.handle_message(message.body)
-        #     await bot.api.login()
-        #     bot.api.async_client.callbacks = botlib.Callbacks(
-        #                                         bot.api.async_client, bot
-        #                                         )
-        #     await bot.api.async_client.callbacks.setup_callbacks()
-        #     for action in bot.listener._startup_registry:
-        #         for room_id in bot.api.async_client.rooms:
-        #             await action(room_id)
-        #     await bot.api.async_client.sync_forever(
-        #                                             timeout=3000,
-        #                                             full_state=True
-        #                                         )
-        # elif settings.telethon_api_id:
-        #     # TELEGRAM
-        #     bot = await TelegramClient(
-        #                 None,
-        #                 settings.telethon_api_id,
-        #                 settings.telethon_api_hash
-        #                 ).start(bot_token=settings.bot_token)
-        #     await self.post_init()
-
-        #     @bot.on(events.NewMessage())
-        #     async def telethon(event):
-        #         await self.handle_message(event.message.message)
+        elif settings.matrix_hostname:
+            # MATRIX
+            config = botlib.Config()
+            config.emoji_verify = True
+            config.ignore_unverified_devices = True
+            config.store_path = './config/matrix/'
+            creds = botlib.Creds(
+                        settings.matrix_hostname,
+                        settings.matrix_user,
+                        settings.matrix_pass
+                        )
+            bot = botlib.Bot(creds, config)
+
+            @bot.listener.on_startup
+            async def room_joined(room):
+                await self.post_init()
 
-        #     await bot.run_until_disconnected()
+            @bot.listener.on_message_event
+            async def on_matrix_message(room, message):
+                await self.handle_message(message.body)
+            await bot.api.login()
+            bot.api.async_client.callbacks = botlib.Callbacks(
+                                                bot.api.async_client, bot
+                                                )
+            await bot.api.async_client.callbacks.setup_callbacks()
+            for action in bot.listener._startup_registry:
+                for room_id in bot.api.async_client.rooms:
+                    await action(room_id)
+            await bot.api.async_client.sync_forever(
+                                                    timeout=3000,
+                                                    full_state=True
+                                                )
+        elif settings.telethon_api_id:
+            # TELEGRAM
+            bot = await TelegramClient(
+                        None,
+                        settings.telethon_api_id,
+                        settings.telethon_api_hash
+                        ).start(bot_token=settings.bot_token)
+            await self.post_init()
+
+            @bot.on(events.NewMessage())
+            async def telethon(event):
+                await self.handle_message(event.message.message)
+
+            await bot.run_until_disconnected()
         else:
             self.logger.warning("Check settings")
             await asyncio.sleep(7200)
 
     async def get_latest_message(self):
         """Return the latest message."""
-        self.logger.debug(f"Latest message: {self.latest_message}")
-        return self.latest_message
+        while True:
+            with self.lock:
+                if self.latest_message is not None:
+                    msg = self.latest_message
+                    self.latest_message = None
+                    # self.logger.debug(f"Latest message: {msg}")
+                    return msg
+
+            await asyncio.sleep(0.1)
 
     async def handle_message(self, message_content):
         """Handle a new message."""
-        self.logger.debug(f"Message received: {message_content}")
+        # self.logger.debug(f"Message received: {message_content}")
         self.latest_message = message_content
-        self.logger.debug(f"self.latest_message: {self.latest_message}")
-        print(self.get_latest_message())
+        # self.logger.debug(f"handle_message self.latest_message: {self.latest_message}")
+
+
+    async def run_forever(self):
+        """Run the listener forever."""
+        while not self.stopped:
+            await self.start()
 
     async def post_init(self):
-        return
+        return
+
+    def stop(self):
+        """Stop the listener."""
+        self.stopped = True
```

### Comparing `iamlistening-0.1.5/pyproject.toml` & `iamlistening-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.5"
+version = "0.1.6"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.5/PKG-INFO` & `iamlistening-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,16 +35,25 @@
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
-  from iamlistening import Listerner as bot
-  bot.start()
+  listener = Listener()
+  task = asyncio.create_task(listener.run_forever())
+  while True:
+    try:
+        msg = await listener.get_latest_message()
+        if msg:
+            print(f"Frasier👂: {msg}")
+
+    except Exception as error:
+        print(error)
+  await task
   
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
```

