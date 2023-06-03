# Comparing `tmp/aiavatar-0.1.1-py3-none-any.whl.zip` & `tmp/aiavatar-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 17457 bytes, number of entries: 19
+Zip file size: 18435 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-May-27 09:17 aiavatar/avatar.py
--rw-r--r--  2.0 unx     4475 b- defN 23-May-29 11:57 aiavatar/bot.py
+-rw-r--r--  2.0 unx     5217 b- defN 23-Jun-02 13:14 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
--rw-r--r--  2.0 unx      836 b- defN 23-May-27 03:48 aiavatar/device/audio.py
+-rw-r--r--  2.0 unx     2535 b- defN 23-Jun-03 02:13 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx      888 b- defN 23-May-27 09:19 aiavatar/face/__init__.py
--rw-r--r--  2.0 unx     6184 b- defN 23-May-29 12:08 aiavatar/listeners/__init__.py
+-rw-r--r--  2.0 unx     6210 b- defN 23-Jun-03 02:23 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-24 12:01 aiavatar/listeners/voicerequest.py
--rw-r--r--  2.0 unx      877 b- defN 23-May-29 11:39 aiavatar/listeners/wakeword.py
+-rw-r--r--  2.0 unx     1007 b- defN 23-Jun-03 02:44 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     2151 b- defN 23-May-27 08:42 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
--rw-r--r--  2.0 unx     2794 b- defN 23-May-29 13:08 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5375 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1547 b- defN 23-May-29 13:10 aiavatar-0.1.1.dist-info/RECORD
-19 files, 41866 bytes uncompressed, 14927 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx     2794 b- defN 23-Jun-02 14:22 aiavatar/speech/voicevox.py
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7665 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1549 b- defN 23-Jun-03 02:52 aiavatar-0.1.2.dist-info/RECORD
+19 files, 46755 bytes uncompressed, 15905 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.1.1.dist-info/LICENSE
+Filename: aiavatar-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.1.1.dist-info/METADATA
+Filename: aiavatar-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.1.1.dist-info/WHEEL
+Filename: aiavatar-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.1.1.dist-info/top_level.txt
+Filename: aiavatar-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.1.1.dist-info/RECORD
+Filename: aiavatar-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/bot.py

```diff
@@ -35,27 +35,41 @@
 
         self.google_api_key = google_api_key
         self.openai_api_key = openai_api_key
         self.voicevox_url = voicevox_url
         self.voicevox_speaker_id = voicevox_speaker_id
 
         # Audio Devices
-        if input_device < 0:
-            input_device_info = AudioDevice.get_default_input_device_info()
+        if isinstance(input_device, int):
+            if input_device < 0:
+                input_device_info = AudioDevice.get_default_input_device_info()
+                input_device = input_device_info["index"]
+            else:
+                input_device_info = AudioDevice.get_device_info(input_device)
+        elif isinstance(input_device, str):
+            input_device_info = AudioDevice.get_input_device_by_name(input_device)
+            if input_device_info is None:
+                input_device_info = AudioDevice.get_default_input_device_info()
             input_device = input_device_info["index"]
-        else:
-            input_device_info = AudioDevice.get_device_info(input_device)
+
         self.input_device = input_device
         self.logger.info(f"Input device: [{input_device}] {input_device_info['name']}")
 
-        if output_device < 0:
-            output_device_info = AudioDevice.get_default_output_device_info()
+        if isinstance(output_device, int):
+            if output_device < 0:
+                output_device_info = AudioDevice.get_default_output_device_info()
+                output_device = output_device_info["index"]
+            else:
+                output_device_info = AudioDevice.get_device_info(output_device)
+        elif isinstance(output_device, str):
+            output_device_info = AudioDevice.get_output_device_by_name(output_device)
+            if output_device_info is None:
+                output_device_info = AudioDevice.get_default_output_device_info()
             output_device = output_device_info["index"]
-        else:
-            output_device_info = AudioDevice.get_device_info(output_device)
+
         self.output_device = output_device
         self.logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
 
         # Processor
         self.chat_processor = ChatGPTProcessor(self.openai_api_key, system_message_content=system_message_content)
 
         # Listeners
```

## aiavatar/device/audio.py

```diff
@@ -1,28 +1,78 @@
 from pyaudio import PyAudio
 
 class AudioDevice:
     @classmethod
     def get_default_input_device_info(cls):
-        return PyAudio().get_default_input_device_info()
+        pa = PyAudio()
+        ret = pa.get_default_input_device_info()
+        pa.terminate()
+        return ret
 
     @classmethod
     def get_default_output_device_info(cls):
-        return PyAudio().get_default_output_device_info()
+        pa = PyAudio()
+        ret = pa.get_default_output_device_info()
+        pa.terminate()
+        return ret
 
     @classmethod
     def get_device_info(cls, index: int):
-        return PyAudio().get_device_info_by_index(index)
+        pa = PyAudio()
+        ret = pa.get_device_info_by_index(index)
+        pa.terminate()
+        return ret
+
+    @classmethod
+    def get_input_device_by_name(cls, name: str):
+        for d in AudioDevice.get_audio_devices():
+            if d["maxInputChannels"] > 0:
+                if name.lower() in d["name"].lower():
+                    return d
+        return None
+
+    @classmethod
+    def get_output_device_by_name(cls, name: str):
+        for d in AudioDevice.get_audio_devices():
+            if d["maxOutputChannels"] > 0:
+                if name.lower() in d["name"].lower():
+                    return d
+        return None
+
+    @classmethod
+    def get_input_device_with_prompt(cls, prompt: str=None):
+        print("==== Input devices ====")
+        for d in AudioDevice.get_audio_devices():
+            if d["maxInputChannels"] > 0:
+                print(f'{d["index"]}: {d["name"]}')
+        idx = input(prompt or "Index of microphone device (Skip to use default): ")
+        if idx == "":
+            return cls.get_default_input_device_info()
+        else:
+            return cls.get_device_info(int(idx))
+
+    @classmethod
+    def get_output_device_with_prompt(cls, prompt: str=None):
+        print("==== Output devices ====")
+        for d in AudioDevice.get_audio_devices():
+            if d["maxOutputChannels"] > 0:
+                print(f'{d["index"]}: {d["name"]}')
+        idx = input(prompt or "Index of speaker device (Skip to use default): ")
+        if idx == "":
+            return cls.get_default_output_device_info()
+        else:
+            return cls.get_device_info(int(idx))
 
     @classmethod
     def get_audio_devices(cls):
         devices = []
         pa = PyAudio()
         for i in range(pa.get_device_count()):
             devices.append(pa.get_device_info_by_index(i))
+        pa.terminate()
         return devices
 
     @classmethod
     def list_audio_devices(cls):
         devices = cls.get_audio_devices()
         print("Available audio devices:")
         for d in devices:
```

## aiavatar/listeners/__init__.py

```diff
@@ -8,14 +8,15 @@
 import pyaudio
 
 class SpeechListenerBase:
     def __init__(self, api_key: str, on_speech_recognized: Callable, volume_threshold: int=3000, timeout: float=1.0, detection_timeout: float=0.0, min_duration: float=0.3, max_duration: float=20.0, lang: str="ja-JP", rate: int=44100, device_index: int=-1):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
+        self.pa = pyaudio.PyAudio()
         self.api_key = api_key
         self.on_speech_recognized = on_speech_recognized
         self.volume_threshold = volume_threshold
         self.timeout = timeout
         self.detection_timeout = detection_timeout
         self.min_duration = min_duration
         self.max_duration = max_duration
@@ -28,15 +29,15 @@
         audio_data = []
 
         def callback(in_data, frame_count, time_info, status):
             audio_data.append(in_data)
             return (None, pyaudio.paContinue)
 
         try:
-            stream = pyaudio.PyAudio().open(
+            stream = self.pa.open(
                 input_device_index=device_index,
                 format=pyaudio.paInt16,
                 channels=1,
                 rate=self.rate,
                 input=True,
                 stream_callback=callback
             )
```

## aiavatar/listeners/wakeword.py

```diff
@@ -1,19 +1,23 @@
 import asyncio
 from threading import Thread
 from typing import Callable
 from . import SpeechListenerBase
 
 class WakewordListener(SpeechListenerBase):
-    def __init__(self, api_key: str, wakewords: list, on_wakeword: Callable, volume_threshold: int=3000, timeout: float=0.3, min_duration: float=0.2, max_duration: float=2, lang: str="ja-JP", rate: int=44100, device_index: int=-1):
+    def __init__(self, api_key: str, wakewords: list, on_wakeword: Callable, volume_threshold: int=3000, timeout: float=0.3, min_duration: float=0.2, max_duration: float=2, lang: str="ja-JP", rate: int=44100, device_index: int=-1, verbose: bool=False):
         super().__init__(api_key, self.invoke_on_wakeword, volume_threshold, timeout, 0.0, min_duration, max_duration, lang, rate, device_index)
         self.wakewords = wakewords
         self.on_wakeword = on_wakeword
+        self.verbose = verbose
     
     async def invoke_on_wakeword(self, text: str):
+        if self.verbose:
+            self.logger.info(f"Recognized: {text}")
+
         if text in self.wakewords:
             await self.on_wakeword(text)
 
     def start(self):
         th = Thread(target=asyncio.run, args=(self.start_listening(),), daemon=True)
         th.start()
         return th
```

## Comparing `aiavatar-0.1.1.dist-info/LICENSE` & `aiavatar-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.1.1.dist-info/METADATA` & `aiavatar-0.1.2.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.1.1
+Version: 0.1.2
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -93,14 +93,18 @@
     on_wakeword=on_wakeword,
     device_index=app.input_device
 )
 
 # Start listening
 ww_thread = wakeword_listener.start()
 ww_thread.join()
+
+# Tips: To terminate with Ctrl+C on Windows, use `while` below instead of `ww_thread.join()`
+# while True:
+#     time.sleep(1)
 ```
 
 Start AIAvatar.
 
 ```bash
 $ python run.py
 ```
@@ -157,14 +161,93 @@
 $ run.py
 ```
 
 Launch VRChat as desktop mode on the machine that runs `run.py` and log in with the account for AIAvatar. Then set `VB-Cable-A` to microphone in VRChat setting window.
 
 That's all! Let's chat with the AIAvatar. Log in to VRChat on another machine (or Quest) and go to the world the AIAvatar is in.
 
+
+# 🎤 Testing audio I/O
+
+Using the script below to test the audio I/O before configuring AIAvatar.
+
+- Step-by-Step audio device configuration.
+- Speak immediately after start if the output device is correctly configured.
+- All recognized text will be shown in console if the input device is correctly configured.
+- Just echo on wakeword recognized.
+
+```python
+import asyncio
+import logging
+from aiavatar import (
+    AudioDevice,
+    VoicevoxSpeechController,
+    WakewordListener
+)
+
+GOOGLE_API_KEY = "YOUR_API_KEY"
+VV_URL = "http://127.0.0.1:50021"
+VV_SPEAKER = 46
+INPUT_DEVICE = -1
+OUTPUT_DEVICE = -1
+
+# Configure root logger
+logger = logging.getLogger()
+logger.setLevel(logging.INFO)
+log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
+streamHandler = logging.StreamHandler()
+streamHandler.setFormatter(log_format)
+logger.addHandler(streamHandler)
+
+# Select input device
+if INPUT_DEVICE < 0:
+    input_device_info = AudioDevice.get_input_device_with_prompt()
+else:
+    input_device_info = AudioDevice.get_device_info(INPUT_DEVICE)
+input_device = input_device_info["index"]
+
+# Select output device
+if OUTPUT_DEVICE < 0:
+    output_device_info = AudioDevice.get_output_device_with_prompt()
+else:
+    output_device_info = AudioDevice.get_device_info(OUTPUT_DEVICE)
+output_device = output_device_info["index"]
+
+logger.info(f"Input device: [{input_device}] {input_device_info['name']}")
+logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
+
+# Create speaker
+speaker = VoicevoxSpeechController(
+    VV_URL,
+    VV_SPEAKER,
+    device_index=output_device
+)
+
+asyncio.run(speaker.speak("オーディオデバイスのテスターを起動しました。私の声が聞こえていますか？"))
+
+# Create WakewordListener
+wakewords = ["こんにちは"]
+async def on_wakeword(text):
+    logger.info(f"Wakeword: {text}")
+    await speaker.speak(f"{text}")
+
+wakeword_listener = WakewordListener(
+    api_key=GOOGLE_API_KEY,
+    wakewords=["こんにちは"],
+    on_wakeword=on_wakeword,
+    verbose=True,
+    device_index=input_device
+)
+
+# Start listening
+ww_thread = wakeword_listener.start()
+ww_thread.join()
+```
+
+
 # ⚡️ Use custom listener
 
 It's very easy to add your original listeners. Just make it run on other thread and invoke `app.start_chat()` when the listener handles the event.
 
 Here the example of `FileSystemListener` that invokes chat when `test.txt` is found on the file system.
 
 ```python
```

## Comparing `aiavatar-0.1.1.dist-info/RECORD` & `aiavatar-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 aiavatar/__init__.py,sha256=SqrO15owXtN32q55sRbSxKqRJyOZ32gao4a-SQwJTA8,351
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
-aiavatar/bot.py,sha256=EntT-4oLEO2gt0yRk_vwQEyHVYu9TnBvQmeA7CCsmTQ,4475
+aiavatar/bot.py,sha256=FchkWPxSjxYJOO4rlaEpSR-baUvyt7t1RKISiWYKOww,5217
 aiavatar/animation/__init__.py,sha256=cE0zS3FgTUd0c6LcsLUnDVSTlFrCF0ZiH7-4NJxiQnU,284
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
-aiavatar/device/audio.py,sha256=zXzcrw-o6u3GxWtca_tPAf40_fqlEOOnBqMvOTeASBE,836
+aiavatar/device/audio.py,sha256=oCqxsY3lB6ZULTA9EhausaTgKYMxrSBhKYytr2FQap0,2535
 aiavatar/face/__init__.py,sha256=nrnFS0NUhqwdW81vM2OVdQIYd2vSi7VKIEdO4ys7_Co,888
-aiavatar/listeners/__init__.py,sha256=-yrJoDBZEat-dE05UVIjRh8PRwbWcaFBV2k5Fv1Zotg,6184
+aiavatar/listeners/__init__.py,sha256=7EU4Ea6AdJa9soe5WtgBcJ8rsKb43M-0cmBQfUvUQXY,6210
 aiavatar/listeners/voicerequest.py,sha256=6636rbXDJ0Dw6EPD0kSsF3f46A4H0zjyY7fAMzpAvkc,788
-aiavatar/listeners/wakeword.py,sha256=phePE_ycP-Om-hzoL3RdXrx9VAtmsLK_jSyYMyhhDHI,877
+aiavatar/listeners/wakeword.py,sha256=UMM-1HMmEFXQpIt9C2EOuGSoxJHj1fQdrz_e9adJiGs,1007
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=snlUw6eYS__j_PM8ab7YZmE4CcalXKQLpdO_4JQa_h0,2151
 aiavatar/speech/__init__.py,sha256=yiveD86ikoWYYVnpdi1r_6ou5bXr-SOkmnri6ry_qHI,275
 aiavatar/speech/voicevox.py,sha256=SsR-yFHb7fLYvA4M08wPw_eqiq9ZyISkeqHeiV2Epco,2794
-aiavatar-0.1.1.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.1.1.dist-info/METADATA,sha256=6wmLa3UyDmQmJtb1QIU6BUWGuD6LizSsm6VvOlNQGWk,5375
-aiavatar-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiavatar-0.1.1.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.1.1.dist-info/RECORD,,
+aiavatar-0.1.2.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.1.2.dist-info/METADATA,sha256=qznLvQ6Lmz9-TN9ZxPoqf6Scpq8zEI7Jl8Ewbq8GOAw,7665
+aiavatar-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiavatar-0.1.2.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.1.2.dist-info/RECORD,,
```

