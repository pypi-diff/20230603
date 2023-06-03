# Comparing `tmp/philbot_voice-1.7.4.tar.gz` & `tmp/philbot_voice-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.4.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.5.tar", max compression
```

## Comparing `philbot_voice-1.7.4.tar` & `philbot_voice-1.7.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33608 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33620 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.5/PKG-INFO
```

### Comparing `philbot_voice-1.7.4/philbot-voice/voice.py` & `philbot_voice-1.7.5/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,15 +576,15 @@
             self.ws = websocket.WebSocketApp(self.endpoint + '?v=4', on_open=self.__ws_on_open, on_message=self.__ws_on_message, on_error=self.__ws_on_error, on_close=self.__ws_on_close)
             threading.Thread(target=self.ws.run_forever).start()
     
     def __stop(self):
         listener = None
         streamer = None
         with self.lock:
-            if not self.ws and self.socket and self.listener and self.streamer:
+            if not self.ws and not self.socket and not self.listener and not self.streamer:
                 return
             print('VOICE GATEWAY ' + self.guild_id + ' connection shutting down')
             listener = self.listener
             streamer = self.streamer
             self.listener = None
             self.streamer = None
             if self.socket:
```

### Comparing `philbot_voice-1.7.4/pyproject.toml` & `philbot_voice-1.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.4"
+version = "1.7.5"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.4/PKG-INFO` & `philbot_voice-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.4
+Version: 1.7.5
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

