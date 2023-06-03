# Comparing `tmp/netora-python-0.1.7.tar.gz` & `tmp/netora-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.7.tar", last modified: Sat Jun  3 05:34:52 2023, max compression
+gzip compressed data, was "netora-python-0.1.8.tar", last modified: Sat Jun  3 05:37:52 2023, max compression
```

## Comparing `netora-python-0.1.7.tar` & `netora-python-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.130513 netora-python-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.070908 netora-python-0.1.7/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.086531 netora-python-0.1.7/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13934 2023-06-03 05:34:30.000000 netora-python-0.1.7/NetoraPy/NetoraTube/NetoraTube.py
--rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.7/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.7/NetoraPy/NetoraTube/app.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.7/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 05:34:52.129516 netora-python-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.126526 netora-python-0.1.7/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 05:34:52.130513 netora-python-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 05:34:42.000000 netora-python-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:37:52.034060 netora-python-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:37:51.979096 netora-python-0.1.8/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:37:51.999043 netora-python-0.1.8/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13940 2023-06-03 05:37:33.000000 netora-python-0.1.8/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.8/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.8/NetoraPy/NetoraTube/app.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.8/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:37:52.033062 netora-python-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 05:37:52.030071 netora-python-0.1.8/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 05:37:51.000000 netora-python-0.1.8/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:37:52.035059 netora-python-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 05:37:49.000000 netora-python-0.1.8/setup.py
```

### Comparing `netora-python-0.1.7/NetoraPy/NetoraTube/NetoraTube.py` & `netora-python-0.1.8/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,22 +310,22 @@
             f"[DOWNLOADER] Attached Audio Format-ID: {audio_format_id}\n" if audio_format_id else "[DOWNLOADER] No Audio Attached\n",
             f" - Format: {self.options.selected_option[1].format}\n" if audio_format_id else '',
             sep=''
         )
         
         YoutubeDL(option).download(self.url)
 
-        for f in output_format:
+        for f in output_filename:
             if os.path.exists(f):
-                output_format = f
+                output_filename = f
                 break
             else:
                 continue
         
-        if type(output_format) == list:
+        if type(output_filename) == list:
             return "[Error] Output Format Error"
 
         if not(not output_format or output_format == output_filename[::-1].split('.')[0][::-1]):
             os.system(f'ffmpeg -i "{output_filename}" -c:v copy "{filename_convert(f"{self.title}.{output_format}")}"')
             os.remove(output_filename)
 
             print(
```

### Comparing `netora-python-0.1.7/setup.py` & `netora-python-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

