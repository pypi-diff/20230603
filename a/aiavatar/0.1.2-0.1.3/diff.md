# Comparing `tmp/aiavatar-0.1.2-py3-none-any.whl.zip` & `tmp/aiavatar-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 18435 bytes, number of entries: 19
+Zip file size: 19376 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-May-27 09:17 aiavatar/avatar.py
--rw-r--r--  2.0 unx     5217 b- defN 23-Jun-02 13:14 aiavatar/bot.py
+-rw-r--r--  2.0 unx     5501 b- defN 23-Jun-03 08:34 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
 -rw-r--r--  2.0 unx     2535 b- defN 23-Jun-03 02:13 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx      888 b- defN 23-May-27 09:19 aiavatar/face/__init__.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Jun-03 08:21 aiavatar/face/vrchat.py
 -rw-r--r--  2.0 unx     6210 b- defN 23-Jun-03 02:23 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-24 12:01 aiavatar/listeners/voicerequest.py
 -rw-r--r--  2.0 unx     1007 b- defN 23-Jun-03 02:44 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     2151 b- defN 23-May-27 08:42 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
 -rw-r--r--  2.0 unx     2794 b- defN 23-Jun-02 14:22 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7665 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1549 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/RECORD
-19 files, 46755 bytes uncompressed, 15905 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7901 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/RECORD
+20 files, 49064 bytes uncompressed, 16724 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: aiavatar/device/audio.py
 Comment: 
 
 Filename: aiavatar/face/__init__.py
 Comment: 
 
+Filename: aiavatar/face/vrchat.py
+Comment: 
+
 Filename: aiavatar/listeners/__init__.py
 Comment: 
 
 Filename: aiavatar/listeners/voicerequest.py
 Comment: 
 
 Filename: aiavatar/listeners/wakeword.py
@@ -36,23 +39,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.1.2.dist-info/LICENSE
+Filename: aiavatar-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.1.2.dist-info/METADATA
+Filename: aiavatar-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.1.2.dist-info/WHEEL
+Filename: aiavatar-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.1.2.dist-info/top_level.txt
+Filename: aiavatar-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.1.2.dist-info/RECORD
+Filename: aiavatar-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/bot.py

```diff
@@ -81,26 +81,30 @@
         face_controller = face_controller or FaceControllerDummy()
         self.avatar_controller = AvatarController(speech_controller, animation_controller, face_controller, avatar_request_parser)
 
         # Chat
         self.chat_task = None
         self.start_voice = start_voice
 
-    async def chat(self, skip_start_voice=False):
+    async def chat(self, request_on_start: str=None, skip_start_voice: bool=False):
         if not skip_start_voice:
             try:
                 await self.avatar_controller.speech_controller.speak(self.start_voice)
             except Exception as ex:
                 self.logger.error(f"Error at starting chat: {str(ex)}\n{traceback.format_exc()}")
 
         while True:
             try:
-                req = await self.request_listener.get_request()
-                if not req:
-                    break
+                if request_on_start:
+                    req = request_on_start
+                    request_on_start = None
+                else:
+                    req = await self.request_listener.get_request()
+                    if not req:
+                        break
 
                 self.logger.info(f"User: {req}")
                 self.logger.info("AI:")
 
                 avatar_task = asyncio.create_task(self.avatar_controller.start())
 
                 stream_buffer = ""
@@ -114,15 +118,15 @@
 
                 self.avatar_controller.set_stop()
                 await avatar_task
             
             except Exception as ex:
                 self.logger.error(f"Error at chatting loop: {str(ex)}\n{traceback.format_exc()}")
 
-    async def start_chat(self):
+    async def start_chat(self, request_on_start: str=None, skip_start_voice: bool=False):
         self.stop_chat()
-        self.chat_task = asyncio.create_task(self.chat())
+        self.chat_task = asyncio.create_task(self.chat(request_on_start, skip_start_voice))
         await self.chat_task
 
     def stop_chat(self):
         if self.chat_task is not None:
             self.chat_task.cancel()
```

## Comparing `aiavatar-0.1.2.dist-info/LICENSE` & `aiavatar-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.1.2.dist-info/METADATA` & `aiavatar-0.1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -151,14 +151,22 @@
     VV_SPEAKER,
     system_message_content=system_message_content,
     input_device=6      # Listen sound from VRChat
     output_device=13,   # Speak to VRChat microphone
 )
 ```
 
+You can also set the name of audio devices instead of index (partial match, ignore case).
+
+```python
+    input_device="CABLE-B Out"      # Listen sound from VRChat
+    output_device="cable-a input",   # Speak to VRChat microphone
+```
+
+
 Run it.
 
 ```bash
 $ run.py
 ```
 
 Launch VRChat as desktop mode on the machine that runs `run.py` and log in with the account for AIAvatar. Then set `VB-Cable-A` to microphone in VRChat setting window.
```

## Comparing `aiavatar-0.1.2.dist-info/RECORD` & `aiavatar-0.1.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 aiavatar/__init__.py,sha256=SqrO15owXtN32q55sRbSxKqRJyOZ32gao4a-SQwJTA8,351
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
-aiavatar/bot.py,sha256=FchkWPxSjxYJOO4rlaEpSR-baUvyt7t1RKISiWYKOww,5217
+aiavatar/bot.py,sha256=G5vIAvW7sNhiaIjdsUoSMYLB8MhKQ2JYIQj-PGplXNo,5501
 aiavatar/animation/__init__.py,sha256=cE0zS3FgTUd0c6LcsLUnDVSTlFrCF0ZiH7-4NJxiQnU,284
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
 aiavatar/device/audio.py,sha256=oCqxsY3lB6ZULTA9EhausaTgKYMxrSBhKYytr2FQap0,2535
 aiavatar/face/__init__.py,sha256=nrnFS0NUhqwdW81vM2OVdQIYd2vSi7VKIEdO4ys7_Co,888
+aiavatar/face/vrchat.py,sha256=xcwUs3CWG3pX0_ODuGBytbV0SSMfekORCLh0FFuQtM4,1709
 aiavatar/listeners/__init__.py,sha256=7EU4Ea6AdJa9soe5WtgBcJ8rsKb43M-0cmBQfUvUQXY,6210
 aiavatar/listeners/voicerequest.py,sha256=6636rbXDJ0Dw6EPD0kSsF3f46A4H0zjyY7fAMzpAvkc,788
 aiavatar/listeners/wakeword.py,sha256=UMM-1HMmEFXQpIt9C2EOuGSoxJHj1fQdrz_e9adJiGs,1007
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=snlUw6eYS__j_PM8ab7YZmE4CcalXKQLpdO_4JQa_h0,2151
 aiavatar/speech/__init__.py,sha256=yiveD86ikoWYYVnpdi1r_6ou5bXr-SOkmnri6ry_qHI,275
 aiavatar/speech/voicevox.py,sha256=SsR-yFHb7fLYvA4M08wPw_eqiq9ZyISkeqHeiV2Epco,2794
-aiavatar-0.1.2.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.1.2.dist-info/METADATA,sha256=qznLvQ6Lmz9-TN9ZxPoqf6Scpq8zEI7Jl8Ewbq8GOAw,7665
-aiavatar-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiavatar-0.1.2.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.1.2.dist-info/RECORD,,
+aiavatar-0.1.3.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.1.3.dist-info/METADATA,sha256=gTrc1823_rkBoSiHjBd4MgSwacTRpVNvu52NLNqgGxk,7901
+aiavatar-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiavatar-0.1.3.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.1.3.dist-info/RECORD,,
```

