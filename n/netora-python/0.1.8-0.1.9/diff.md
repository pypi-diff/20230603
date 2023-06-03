# Comparing `tmp/netora-python-0.1.8.tar.gz` & `tmp/netora-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.8.tar", last modified: Sat Jun  3 05:37:52 2023, max compression
+gzip compressed data, was "netora-python-0.1.9.tar", last modified: Sat Jun  3 06:14:12 2023, max compression
```

## Comparing `netora-python-0.1.8.tar` & `netora-python-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:37:52.034060 netora-python-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:37:51.979096 netora-python-0.1.8/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:37:51.999043 netora-python-0.1.8/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13940 2023-06-03 05:37:33.000000 netora-python-0.1.8/NetoraPy/NetoraTube/NetoraTube.py
--rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.8/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.8/NetoraPy/NetoraTube/app.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.8/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 05:37:52.033062 netora-python-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 05:37:52.030071 netora-python-0.1.8/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 05:37:52.035059 netora-python-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 05:37:49.000000 netora-python-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:14:12.528654 netora-python-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-06-03 06:14:12.467290 netora-python-0.1.9/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 06:14:12.486755 netora-python-0.1.9/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13944 2023-06-03 06:13:27.000000 netora-python-0.1.9/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.9/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.9/NetoraPy/NetoraTube/app.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.9/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 06:14:12.526662 netora-python-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 06:14:12.520676 netora-python-0.1.9/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 06:14:12.000000 netora-python-0.1.9/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-03 06:14:12.000000 netora-python-0.1.9/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 06:14:12.000000 netora-python-0.1.9/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 06:14:12.000000 netora-python-0.1.9/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 06:14:12.000000 netora-python-0.1.9/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 06:14:12.529652 netora-python-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 06:14:04.000000 netora-python-0.1.9/setup.py
```

### Comparing `netora-python-0.1.8/NetoraPy/NetoraTube/NetoraTube.py` & `netora-python-0.1.9/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,24 +284,24 @@
         elif video_format_id:
             option = {
                 'format': f'{video_format_id}/{self.options.selected_option[0].format}',
                 'outtmpl': filename_convert(f'{self.title}.{self.options.selected_option[0].format}'),
                 'progress_hooks': [self.__on_progress]
             }
 
-            output_filename = filename_convert(f'{self.title}.{self.options.selected_option[0].format}')
+            output_filename = [filename_convert(f'{self.title}.{self.options.selected_option[0].format}')]
         
         elif audio_format_id:
             option = {
                 'format': f'{audio_format_id}/{self.options.selected_option[1].format}',
                 'outtmpl': filename_convert(f'{self.title}.{self.options.selected_option[1].format}'),
                 'progress_hooks': [self.__on_progress]
             }
 
-            output_filename = filename_convert(f'{self.title}.{self.options.selected_option[1].format}')
+            output_filename = [filename_convert(f'{self.title}.{self.options.selected_option[1].format}')]
         
         else:
             return "[Error] Download Option Not Selected"
         
         print(
             f"[DOWNLOADER] Downloading Video '{self.title}'\n------------------------------\n",
             f"[DOWNLOADER] Attached Video Format-ID: {video_format_id}\n" if video_format_id else "[DOWNLOADER] No Video Attached\n",
```

### Comparing `netora-python-0.1.8/setup.py` & `netora-python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

