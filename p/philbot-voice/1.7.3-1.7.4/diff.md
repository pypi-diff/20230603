# Comparing `tmp/philbot_voice-1.7.3.tar.gz` & `tmp/philbot_voice-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.3.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.4.tar", max compression
```

## Comparing `philbot_voice-1.7.3.tar` & `philbot_voice-1.7.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33153 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33608 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-03 20:46:40.368219 philbot_voice-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.4/PKG-INFO
```

### Comparing `philbot_voice-1.7.3/philbot-voice/voice.py` & `philbot_voice-1.7.4/philbot-voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,67 +494,83 @@
     def __ws_on_close(self, ws, close_code, close_message):
         print('VOICE GATEWAY ' + self.guild_id + ' close ' + (str(close_code) if close_code else '?') + ': ' + (close_message if close_message else 'unknown'))
         match close_code:
             case 4001: # invalid opcode
                 # fault must be in the code somewhere
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case 4002: # failed to decode payload
                 # fault must be in the code somewhere
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case 4003: # not authenticated
                 # we sent something before identifying, must be race condition
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case 4004: # authentication failed
                 # the token is incorrect
                 # lets reconnect and get a new one
                 with self.lock:
                     self.token = None
+                self.__stop()
                 threading.Thread(target=self.__callback_reconnect).start()
             case 4005: # already authenticated
                 # we sent a second identify message, fault, must be in the code
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case 4006: # session is no longer valid
                 # this can happen when we (only bot users) are alone for a while, then the session is killed
                 # lets reconnect and get a new session id, most likely we will not get a server update (and with it a new session id) until a real user joins, but that is fine, we will continue / complete connection as soon as a real user is here
                 with self.lock:
                     self.session_id = None
+                self.__stop()
                 threading.Thread(target=self.__callback_reconnect).start()
             case 4009: # session timeout
                 # lets try get a new one
                 with self.lock:
                     self.session_id = None
+                self.__stop()
                 threading.Thread(target=self.__callback_reconnect).start()
             case 4011: # server not found
                 # lets try get a new one
                 with self.lock:
                     self.endpoint = None
+                self.__stop()
                 threading.Thread(target=self.__callback_reconnect).start()
             case 4012: # unknown protocol
                 # not entirely sure what this refers to (the ws protocol, the first HTTP messages, the encoded frames), but either way, i guess the fault must lie in the code
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case 4014: # disconnected (channel was deleted, you were kicked, voice server changed, or the main gateway session was dropped)
                 # thats a tricky one, the doc says not to try reconnecting, and we shouldn't open a new gateway connection, but we should try to reconnect on a discord level EXCEPT if we got kicked out of the channel (not the server)
                 # we wanna do that because in some cases we can recover by globally reconnecting again (voice server changed, session was dropped) and for situations it doesnt make sense (we got kicked from the server, channel was deleted), the global discord reconnect fails anyway
                 # lets just try to reconnect, and IF we got kicked from the channel, then lets hope we get the voice state changed thingy first, so we shut down ourselves actually
                 # threading.Thread(target=self.__callback_reconnect).start()
+                self.__stop()
                 pass # lets NOT reconnect, otherwise stop is not working, gateway connection is closed before the voice state update event is sent!
             case 4015: # voice server crashed
                 # lets just try again, if the voice server restarts, we will get a different error as consequence and do it again
-                pass
+                self.__stop()
             case 4016: # unknown encryption mode
                 # fault must be in the code somewhere
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
+                self.__stop()
+                self.__try_start()
             case _: # something else
-                pass
-        self.__stop()
+                self.__stop()
     
     def __try_start(self):
         with self.lock:
             if self.ws or not self.channel_id or not self.session_id or not self.endpoint or not self.token or not self.url:
                 return
             print('VOICE GATEWAY ' + self.guild_id + ' connection starting')
             self.ws = websocket.WebSocketApp(self.endpoint + '?v=4', on_open=self.__ws_on_open, on_message=self.__ws_on_message, on_error=self.__ws_on_error, on_close=self.__ws_on_close)
@@ -584,15 +600,14 @@
             self.ssrc = None
             self.ip = None
             self.port = None
             self.ssrc = None
             self.secret_key = None
             self.ws = None
         print('VOICE GATEWAY ' + self.guild_id + ' connection shut down')
-        self.__try_start() # if we closed intentionally, channel id will be null
 
     def on_server_update(self, endpoint, token):
         self.__stop()
         with self.lock:
             self.endpoint = endpoint
             self.token = token
         self.__save()
```

### Comparing `philbot_voice-1.7.3/pyproject.toml` & `philbot_voice-1.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.3"
+version = "1.7.4"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.3/PKG-INFO` & `philbot_voice-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.3
+Version: 1.7.4
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

