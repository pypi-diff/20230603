# Comparing `tmp/xpymon-1.8.tar.gz` & `tmp/xpymon-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpymon-1.8.tar", last modified: Wed Jul 17 07:38:01 2019, max compression
+gzip compressed data, was "dist/xpymon-1.9.tar", last modified: Thu Jul 18 16:28:21 2019, max compression
```

## Comparing `xpymon-1.8.tar` & `xpymon-1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-07-17 07:38:01.000000 xpymon-1.8/
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     2686 2019-07-17 07:38:01.000000 xpymon-1.8/PKG-INFO
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     1660 2019-07-17 07:05:36.000000 xpymon-1.8/README.md
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       38 2019-07-17 07:38:01.000000 xpymon-1.8/setup.cfg
--rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)      974 2019-07-17 07:37:05.000000 xpymon-1.8/setup.py
--rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)    15806 2019-07-17 07:35:53.000000 xpymon-1.8/xpymon
-drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     2686 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/PKG-INFO
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)      174 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/SOURCES.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/dependency_links.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       24 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/requires.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-07-17 07:38:01.000000 xpymon-1.8/xpymon.egg-info/top_level.txt
+drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-07-18 16:28:21.000000 xpymon-1.9/
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     2686 2019-07-18 16:28:21.000000 xpymon-1.9/PKG-INFO
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     1660 2019-07-17 07:05:36.000000 xpymon-1.9/README.md
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       38 2019-07-18 16:28:21.000000 xpymon-1.9/setup.cfg
+-rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)      974 2019-07-18 16:28:05.000000 xpymon-1.9/setup.py
+-rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)    15767 2019-07-18 16:27:09.000000 xpymon-1.9/xpymon
+drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-07-18 16:28:21.000000 xpymon-1.9/xpymon.egg-info/
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     2686 2019-07-18 16:28:20.000000 xpymon-1.9/xpymon.egg-info/PKG-INFO
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)      174 2019-07-18 16:28:20.000000 xpymon-1.9/xpymon.egg-info/SOURCES.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-07-18 16:28:20.000000 xpymon-1.9/xpymon.egg-info/dependency_links.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       24 2019-07-18 16:28:20.000000 xpymon-1.9/xpymon.egg-info/requires.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-07-18 16:28:20.000000 xpymon-1.9/xpymon.egg-info/top_level.txt
```

### Comparing `xpymon-1.8/PKG-INFO` & `xpymon-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpymon
-Version: 1.8
+Version: 1.9
 Summary: A versatile WiFi/network/battery/CPU/video system monitor on Linux
 Home-page: https://github.com/h-ohsaki/xpymon.git
 Author: Hiroyuki Ohsaki
 Author-email: ohsaki@lsnl.jp
 License: UNKNOWN
 Description: # NAME
```

### Comparing `xpymon-1.8/README.md` & `xpymon-1.9/README.md`

 * *Files identical despite different names*

### Comparing `xpymon-1.8/setup.py` & `xpymon-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='xpymon',
-    version='1.8',
+    version='1.9',
     author='Hiroyuki Ohsaki',
     author_email='ohsaki@lsnl.jp',
     description='A versatile WiFi/network/battery/CPU/video system monitor on Linux',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/h-ohsaki/xpymon.git',
     packages=setuptools.find_packages(),
```

### Comparing `xpymon-1.8/xpymon` & `xpymon-1.9/xpymon`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
 #
 # A versatile WiFi/network/battery/CPU/video system monitor on Linux.
 # Copyright (c) 2018-2019, Hiroyuki Ohsaki.
 # All rights reserved.
 #
-# $Id: xpymon,v 1.36 2019/07/03 13:42:29 ohsaki Exp $
-#
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -38,14 +36,15 @@
     (75, 'aquamarine2'),
     (50, 'aquamarine3'),
     (25, 'orange'),
 )
 
 UPDATE_INTERVAL = 1.
 BATTERY_WARN_THRESH = .05
+TIMEZONE_FILE = '/usr/share/zoneinfo/Europe/Brussels'
 
 def usage():
     die("""\
 usage: {} [-T] [file...]
   -T    test mode
 """.format(sys.argv[0]))
 
@@ -244,16 +243,15 @@
 
     def time_string(self):
         """Return two strings representing the local time and the time in
         another time zone."""
         clock = time.strftime('%Y/%m/%d(%a) %H:%M:%S')
         patterns = [['(\d\d:\d\d:\d\d)', 1, str]]
         # FIXME: avoid hard-coding
-        matches = parse_cmd_output(
-            ['zdump', '/usr/share/zoneinfo/Europe/Brussels'], patterns)
+        matches = parse_cmd_output(['zdump', TIMEZONE_FILE], patterns)
         return clock, matches[0]
 
     def compose_wifi_status(self, iface, addr):
         essid, ap, rate, quality, level, supplicant = self.wifi_status(iface)
         if not essid:
             essid = '--------'
         if not ap:
```

### Comparing `xpymon-1.8/xpymon.egg-info/PKG-INFO` & `xpymon-1.9/xpymon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpymon
-Version: 1.8
+Version: 1.9
 Summary: A versatile WiFi/network/battery/CPU/video system monitor on Linux
 Home-page: https://github.com/h-ohsaki/xpymon.git
 Author: Hiroyuki Ohsaki
 Author-email: ohsaki@lsnl.jp
 License: UNKNOWN
 Description: # NAME
```

