# Comparing `tmp/autosrt-1.2.9.tar.gz` & `tmp/autosrt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.9.tar", last modified: Tue May  2 19:12:11 2023, max compression
+gzip compressed data, was "autosrt-1.3.0.tar", last modified: Sat Jun  3 21:10:09 2023, max compression
```

## Comparing `autosrt-1.2.9.tar` & `autosrt-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.342594 autosrt-1.2.9/
--rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.9/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 19:12:11.342956 autosrt-1.2.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5260 2023-04-30 04:22:31.000000 autosrt-1.2.9/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.334160 autosrt-1.2.9/autosrt/
--rwxrwxrwx   0 root         (0) root         (0)     9904 2023-05-02 18:58:47.000000 autosrt-1.2.9/autosrt/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    41313 2023-05-02 18:58:47.000000 autosrt-1.2.9/autosrt/autosrt.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.339510 autosrt-1.2.9/autosrt.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      112 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-02 19:12:11.344352 autosrt-1.2.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1723 2023-05-02 18:58:47.000000 autosrt-1.2.9/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.341842 autosrt-1.2.9/test/
--rwxrwxrwx   0 root         (0) root         (0)     7362 2023-05-02 18:58:47.000000 autosrt-1.2.9/test/test1.py
--rwxrwxrwx   0 root         (0) root         (0)     4465 2023-05-02 18:58:47.000000 autosrt-1.2.9/test/test2.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.605443 autosrt-1.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-03 21:10:09.606190 autosrt-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.504491 autosrt-1.3.0/autosrt/
+-rw-rw-rw-   0        0        0    15502 2023-06-03 21:05:35.000000 autosrt-1.3.0/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    55404 2023-06-03 21:09:04.000000 autosrt-1.3.0/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.585212 autosrt-1.3.0/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-03 21:10:09.000000 autosrt-1.3.0/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-03 21:10:09.609938 autosrt-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.601693 autosrt-1.3.0/test/
+-rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.0/test/test1.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.0/test/test2.py
+-rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.0/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.0/test/test4.py
```

### Comparing `autosrt-1.2.9/LICENSE` & `autosrt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.9/PKG-INFO` & `autosrt-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.9
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.3.0
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.9/README.md` & `autosrt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.9/autosrt/__init__.py` & `autosrt-1.3.0/test/test3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import argparse
 import os
 import sys
 import multiprocessing
 from glob import glob
 from progressbar import ProgressBar, Percentage, Bar, ETA
 
-from .autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
+from autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter, \
     stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, is_same_language, is_video_file, is_audio_file
 
 def show_progress(progress):
-    global pbar
+    global pbar, media_filepath
+    print("media_filepath = {}".format(media_filepath))
     pbar.update(progress)
 
 def show_error_messages(messages):
     print(messages)
 
 def main():
-    global pbar
+    global pbar, media_filepath
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     remove_temp_files("flac", error_messages_callback=show_error_messages)
@@ -107,15 +108,15 @@
         wav_filepath, sample_rate = wav_converter(media_filepath)
         pbar.finish()
 
         region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
         regions = region_finder(wav_filepath)
 
         converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
-        recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
+        recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, error_messages_callback=show_error_messages)
 
         pool = multiprocessing.Pool(args.concurrency)
 
         if regions:
             try:
                 widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
                 pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
@@ -162,31 +163,30 @@
             base, ext = os.path.splitext(media_filepath)
             subtitle_filepath = "{base}.{format}".format(base=base, format=subtitle_format)
 
         writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
         writer.write(subtitle_filepath)
 
         if do_translate:
+
             # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
             # NO NEED TO TRANSLATE ALL transcript IN transcripts
             # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
             # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
             timed_subtitles = writer.timed_subtitles
             created_regions = []
             created_subtitles = []
             for entry in timed_subtitles:
                 created_regions.append(entry[0])
                 created_subtitles.append(entry[1])
 
             prompt = "Translating from %8s to %8s   : " %(args.src_language, args.dst_language)
             widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-
             transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
-
             translated_subtitles = []
             for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                 translated_subtitles.append(translated_subtitle)
                 pbar.update(i)
             pbar.finish()
 
             translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
```

### Comparing `autosrt-1.2.9/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.0/autosrt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.9
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.3.0
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.9/setup.py` & `autosrt-1.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3.8
 from __future__ import unicode_literals
 import sys
+import warnings
+warnings.filterwarnings("ignore", category=DeprecationWarning, module='setuptools')
+warnings.filterwarnings("ignore", category=UserWarning, module='setuptools')
+warnings.filterwarnings("ignore", message=".*is deprecated*")
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 from autosrt import VERSION
 
@@ -15,29 +19,22 @@
     'generate transcriptions for those regions,  (optionally) translates them to a '
     'different language, and finally saves the resulting subtitles file to disk.   '
     'It supports a variety of input and output languages and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 install_requires=[
-        "requests>=2.3.0",
-        "pysrt>=1.0.1",
-        "progressbar2>=3.34.3",
-        "six>=1.11.0",
-        "ffmpeg_progress_yield>=0.7.2",
+    "requests>=2.3.0",
+    "httpx>=0.24.0",
+    "urllib3 >=1.26.0,<3.0",
+    "pysrt>=1.0.1",
+    "six>=1.11.0",
+    "progressbar2>=3.34.3",
 ]
 
-if sys.platform == "win32":
-    install_requires.append("python-magic>=0.4.27")
-    install_requires.append("python_magic_bin>=0.4.14")
-elif sys.platform == "linux":
-    install_requires.append("python-magic>=0.4.27")
-else:
-    install_requires.append("python-magic>=0.4.27")
-
 setup(
     name="autosrt",
     version=VERSION,
     description="a utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
```

### Comparing `autosrt-1.2.9/test/test1.py` & `autosrt-1.3.0/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.9/test/test2.py` & `autosrt-1.3.0/test/test2.py`

 * *Files identical despite different names*

