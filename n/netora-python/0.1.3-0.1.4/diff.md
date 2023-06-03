# Comparing `tmp/netora-python-0.1.3.tar.gz` & `tmp/netora-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.3.tar", last modified: Sat Jun  3 05:21:15 2023, max compression
+gzip compressed data, was "netora-python-0.1.4.tar", last modified: Sat Jun  3 05:25:01 2023, max compression
```

## Comparing `netora-python-0.1.3.tar` & `netora-python-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.975868 netora-python-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.885112 netora-python-0.1.3/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.910045 netora-python-0.1.3/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13677 2023-06-03 05:20:38.000000 netora-python-0.1.3/NetoraPy/NetoraTube/NetoraTube.py
--rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.3/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0      412 2023-06-03 05:12:42.000000 netora-python-0.1.3/NetoraPy/NetoraTube/app.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.3/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 05:21:15.974871 netora-python-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 05:21:15.972876 netora-python-0.1.3/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 05:21:15.000000 netora-python-0.1.3/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 05:21:15.976867 netora-python-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 05:21:13.000000 netora-python-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:25:01.327008 netora-python-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:25:01.270160 netora-python-0.1.4/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:25:01.293099 netora-python-0.1.4/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13750 2023-06-03 05:24:37.000000 netora-python-0.1.4/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.4/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-06-03 05:12:42.000000 netora-python-0.1.4/NetoraPy/NetoraTube/app.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.4/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:25:01.325016 netora-python-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 05:25:01.322021 netora-python-0.1.4/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:25:01.000000 netora-python-0.1.4/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-03 05:25:01.000000 netora-python-0.1.4/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:25:01.000000 netora-python-0.1.4/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 05:25:01.000000 netora-python-0.1.4/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 05:25:01.000000 netora-python-0.1.4/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:25:01.328006 netora-python-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 05:24:56.000000 netora-python-0.1.4/setup.py
```

### Comparing `netora-python-0.1.3/NetoraPy/NetoraTube/NetoraTube.py` & `netora-python-0.1.4/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,16 @@
         )
         
         YoutubeDL(option).download(self.url)
 
         for f in output_format:
             if os.path.exists(f):
                 output_format = f
+            else:
+                return "[Error] Output Format Error"
 
         if not(not output_format or output_format == output_filename[::-1].split('.')[0][::-1]):
             os.system(f'ffmpeg -i "{output_filename}" -c:v copy "{filename_convert(f"{self.title}.{output_format}")}"')
             os.remove(output_filename)
 
             print(
                 f'\n[DOWNLOADER] Video/Audio \'{filename_convert(f"{self.title}.{output_format}")}\' downloaded successfully'
```

### Comparing `netora-python-0.1.3/setup.py` & `netora-python-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

