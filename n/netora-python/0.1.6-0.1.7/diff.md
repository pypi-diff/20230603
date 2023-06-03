# Comparing `tmp/netora-python-0.1.6.tar.gz` & `tmp/netora-python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.6.tar", last modified: Sat Jun  3 05:32:32 2023, max compression
+gzip compressed data, was "netora-python-0.1.7.tar", last modified: Sat Jun  3 05:34:52 2023, max compression
```

## Comparing `netora-python-0.1.6.tar` & `netora-python-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:32:32.909299 netora-python-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:32:32.855443 netora-python-0.1.6/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:32:32.876393 netora-python-0.1.6/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13861 2023-06-03 05:30:27.000000 netora-python-0.1.6/NetoraPy/NetoraTube/NetoraTube.py
--rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.6/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.6/NetoraPy/NetoraTube/app.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.6/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 05:32:32.908301 netora-python-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 05:32:32.905319 netora-python-0.1.6/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 05:32:32.000000 netora-python-0.1.6/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-03 05:32:32.000000 netora-python-0.1.6/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:32:32.000000 netora-python-0.1.6/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 05:32:32.000000 netora-python-0.1.6/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 05:32:32.000000 netora-python-0.1.6/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 05:32:32.910296 netora-python-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 05:32:28.000000 netora-python-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.130513 netora-python-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.070908 netora-python-0.1.7/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.086531 netora-python-0.1.7/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13934 2023-06-03 05:34:30.000000 netora-python-0.1.7/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.7/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-06-03 05:32:18.000000 netora-python-0.1.7/NetoraPy/NetoraTube/app.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.7/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:34:52.129516 netora-python-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 05:34:52.126526 netora-python-0.1.7/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 05:34:51.000000 netora-python-0.1.7/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:34:52.130513 netora-python-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 05:34:42.000000 netora-python-0.1.7/setup.py
```

### Comparing `netora-python-0.1.6/NetoraPy/NetoraTube/NetoraTube.py` & `netora-python-0.1.7/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,18 @@
         YoutubeDL(option).download(self.url)
 
         for f in output_format:
             if os.path.exists(f):
                 output_format = f
                 break
             else:
-                return "[Error] Output Format Error"
+                continue
+        
+        if type(output_format) == list:
+            return "[Error] Output Format Error"
 
         if not(not output_format or output_format == output_filename[::-1].split('.')[0][::-1]):
             os.system(f'ffmpeg -i "{output_filename}" -c:v copy "{filename_convert(f"{self.title}.{output_format}")}"')
             os.remove(output_filename)
 
             print(
                 f'\n[DOWNLOADER] Video/Audio \'{filename_convert(f"{self.title}.{output_format}")}\' downloaded successfully'
```

### Comparing `netora-python-0.1.6/setup.py` & `netora-python-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

