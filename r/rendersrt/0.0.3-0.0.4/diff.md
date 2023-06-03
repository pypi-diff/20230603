# Comparing `tmp/rendersrt-0.0.3.tar.gz` & `tmp/rendersrt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.3.tar", last modified: Fri Jun  2 22:26:17 2023, max compression
+gzip compressed data, was "rendersrt-0.0.4.tar", last modified: Sat Jun  3 18:15:51 2023, max compression
```

## Comparing `rendersrt-0.0.3.tar` & `rendersrt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.460647 rendersrt-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1561 2023-06-02 22:26:17.460647 rendersrt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.435173 rendersrt-0.0.3/rendersrt/
--rw-rw-rw-   0        0        0     9265 2023-06-02 22:26:06.000000 rendersrt-0.0.3/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.458398 rendersrt-0.0.3/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1561 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-02 22:26:17.463641 rendersrt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-06-02 22:10:10.000000 rendersrt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.840502 rendersrt-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1561 2023-06-03 18:15:51.840502 rendersrt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.809772 rendersrt-0.0.4/rendersrt/
+-rw-rw-rw-   0        0        0     9549 2023-06-03 18:15:40.000000 rendersrt-0.0.4/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.838254 rendersrt-0.0.4/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1561 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-03 18:15:51.842749 rendersrt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-06-02 22:10:10.000000 rendersrt-0.0.4/setup.py
```

### Comparing `rendersrt-0.0.3/LICENSE` & `rendersrt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.3/PKG-INFO` & `rendersrt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.3/README.md` & `rendersrt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.3/rendersrt/__init__.py` & `rendersrt-0.0.4/rendersrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from progressbar import ProgressBar, Percentage, Bar, ETA
 from glob import glob, escape
 import shlex
 import json
 import pysrt
 from pathlib import Path
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 def check_file_type(file_path, error_messages_callback=None):
     try:
         ffprobe_cmd = ['ffprobe', '-v', 'error', '-show_format', '-show_streams', '-print_format', 'json', file_path]
         output = None
         if sys.platform == "win32":
             output = subprocess.check_output(ffprobe_cmd, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
@@ -60,14 +60,24 @@
 def show_error_messages(messages):
     print(messages)
 
 
 def render_media_with_subtitle(video_path, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
 
     try:
+        if "\\" in video_path:
+            video_path = video_path.replace("\\", "/")
+
+        if "\\" in subtitle_path:
+            subtitle_path = subtitle_path.replace("\\", "/")
+
+        if "\\" in output_path:
+            output_path = output_path.replace("\\", "/")
+
+
         ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{video_path}"'
         ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         total_duration = float(ffprobe_process.stdout.read().decode().strip())
 
         ffmpeg_command = f'ffmpeg -y -i "{video_path}" -vf "subtitles={shlex.quote(subtitle_path)}" "{output_path}"'
 
         widgets = [f"Rendering subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
```

### Comparing `rendersrt-0.0.3/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.4/rendersrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.3/setup.py` & `rendersrt-0.0.4/setup.py`

 * *Files identical despite different names*

