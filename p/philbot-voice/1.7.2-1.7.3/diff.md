# Comparing `tmp/philbot_voice-1.7.2.tar.gz` & `tmp/philbot_voice-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.2.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.3.tar", max compression
```

## Comparing `philbot_voice-1.7.2.tar` & `philbot_voice-1.7.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33127 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33153 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-03 17:28:22.051955 philbot_voice-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.3/PKG-INFO
```

### Comparing `philbot_voice-1.7.2/philbot-voice/voice.py` & `philbot_voice-1.7.3/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,13 +740,13 @@
     context = get_context(body['guild_id'])
     return 'true' if context and context.is_connected() else 'false'
 
 def main():
     for file in os.listdir('.'):
         if file.startswith('.state.') and file.endswith('.json'):
             get_context(file[len('.state.'):len(file) - len('.json')])
-        elif (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part')) and os.path.getmtime(file) + 60 * 60 * 24 < time_seconds():
+        elif (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part') or file.endswith('.ytdl')) and os.path.getmtime(file) + 60 * 60 * 24 < time_seconds():
             os.remove(file)
     print('VOICE ready')
     # app.run(port=HTTP_PORT, ssl_context='adhoc', threaded=True)
     app.run(port=HTTP_PORT, threaded=True)
```

### Comparing `philbot_voice-1.7.2/pyproject.toml` & `philbot_voice-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.2"
+version = "1.7.3"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.2/PKG-INFO` & `philbot_voice-1.7.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.2
+Version: 1.7.3
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

