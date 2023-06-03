# Comparing `tmp/netora-python-0.1.2.tar.gz` & `tmp/netora-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.2.tar", last modified: Sat Jun  3 05:04:18 2023, max compression
+gzip compressed data, was "netora-python-0.1.3.tar", last modified: Sat Jun  3 05:21:15 2023, max compression
```

## Comparing `netora-python-0.1.2.tar` & `netora-python-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:04:18.593409 netora-python-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:04:18.555509 netora-python-0.1.2/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:04:18.564490 netora-python-0.1.2/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13523 2023-06-03 04:24:46.000000 netora-python-0.1.2/NetoraPy/NetoraTube/NetoraTube.py
--rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.2/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.2/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 05:04:18.591414 netora-python-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 05:04:18.587424 netora-python-0.1.2/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 05:04:18.000000 netora-python-0.1.2/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-06-03 05:04:18.000000 netora-python-0.1.2/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:04:18.000000 netora-python-0.1.2/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 05:04:18.000000 netora-python-0.1.2/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 05:04:18.000000 netora-python-0.1.2/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 05:04:18.593409 netora-python-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 05:03:40.000000 netora-python-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.975868 netora-python-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.885112 netora-python-0.1.3/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.910045 netora-python-0.1.3/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13677 2023-06-03 05:20:38.000000 netora-python-0.1.3/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.3/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-06-03 05:12:42.000000 netora-python-0.1.3/NetoraPy/NetoraTube/app.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.3/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:21:15.974871 netora-python-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.972876 netora-python-0.1.3/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:21:15.976867 netora-python-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 05:21:13.000000 netora-python-0.1.3/setup.py
```

### Comparing `netora-python-0.1.2/NetoraPy/NetoraTube/NetoraTube.py` & `netora-python-0.1.3/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,23 +267,23 @@
                 'format': f'{video_format_id}+{audio_format_id}',
                 'requested_formats': [self.options.selected_option[0].format, self.options.selected_option[1].format],
                 'outtmpl': filename_convert(f'{self.title}'),
                 'progress_hooks': [self.__on_progress]
             }
 
             if option['requested_formats'][0] == option['requested_formats'][1]:
-                output_filename = filename_convert(f'{self.title}.{option["requested_formats"][0]}')
+                output_filename = [filename_convert(f'{self.title}.{option["requested_formats"][0]}')]
             elif option['requested_formats'][0] == 'mp4' and option['requested_formats'][1] == 'webm':
-                output_filename = filename_convert(f'{self.title}.webm')
+                output_filename = [filename_convert(f'{self.title}.mkv'), filename_convert(f'{self.title}.webm')]
             elif option['requested_formats'][0] == 'webm' and option['requested_formats'][1] == 'm4a':
-                output_filename = filename_convert(f'{self.title}.mkv')
+                output_filename = [filename_convert(f'{self.title}.mkv')]
             elif option['requested_formats'][0] == 'mp4' and option['requested_formats'][1] == 'm4a':
-                output_filename = filename_convert(f'{self.title}.mp4')
+                output_filename = [filename_convert(f'{self.title}.mp4')]
             else:
-                output_filename = filename_convert(f'{self.title}.mp4')
+                output_filename = [filename_convert(f'{self.title}.mp4')]
         
         elif video_format_id:
             option = {
                 'format': f'{video_format_id}/{self.options.selected_option[0].format}',
                 'outtmpl': filename_convert(f'{self.title}.{self.options.selected_option[0].format}'),
                 'progress_hooks': [self.__on_progress]
             }
@@ -310,14 +310,18 @@
             f"[DOWNLOADER] Attached Audio Format-ID: {audio_format_id}\n" if audio_format_id else "[DOWNLOADER] No Audio Attached\n",
             f" - Format: {self.options.selected_option[1].format}\n" if audio_format_id else '',
             sep=''
         )
         
         YoutubeDL(option).download(self.url)
 
+        for f in output_format:
+            if os.path.exists(f):
+                output_format = f
+
         if not(not output_format or output_format == output_filename[::-1].split('.')[0][::-1]):
             os.system(f'ffmpeg -i "{output_filename}" -c:v copy "{filename_convert(f"{self.title}.{output_format}")}"')
             os.remove(output_filename)
 
             print(
                 f'\n[DOWNLOADER] Video/Audio \'{filename_convert(f"{self.title}.{output_format}")}\' downloaded successfully'
             )
```

### Comparing `netora-python-0.1.2/setup.py` & `netora-python-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

