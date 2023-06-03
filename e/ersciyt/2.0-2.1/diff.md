# Comparing `tmp/ersciyt-2.0.tar.gz` & `tmp/ersciyt-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-2.0.tar", last modified: Sat Jun  3 11:20:49 2023, max compression
+gzip compressed data, was "ersciyt-2.1.tar", last modified: Sat Jun  3 11:26:50 2023, max compression
```

## Comparing `ersciyt-2.0.tar` & `ersciyt-2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.109858 ersciyt-2.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 11:20:42.000000 ersciyt-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 11:20:42.000000 ersciyt-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:20:49.109858 ersciyt-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 11:20:42.000000 ersciyt-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.107857 ersciyt-2.0/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/apps.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.108857 ersciyt-2.0/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.109858 ersciyt-2.0/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/inst
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/s
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.108857 ersciyt-2.0/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      664 2023-06-03 11:20:49.110858 ersciyt-2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 11:20:42.000000 ersciyt-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:26:50.727749 ersciyt-2.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 11:26:38.000000 ersciyt-2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 11:26:38.000000 ersciyt-2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:26:50.728749 ersciyt-2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 11:26:38.000000 ersciyt-2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:26:50.725749 ersciyt-2.1/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:26:50.726749 ersciyt-2.1/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:26:50.727749 ersciyt-2.1/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 11:26:38.000000 ersciyt-2.1/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:26:50.726749 ersciyt-2.1/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:26:50.000000 ersciyt-2.1/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 11:26:50.000000 ersciyt-2.1/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 11:26:50.000000 ersciyt-2.1/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 11:26:50.000000 ersciyt-2.1/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 11:26:50.000000 ersciyt-2.1/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      664 2023-06-03 11:26:50.728749 ersciyt-2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 11:26:38.000000 ersciyt-2.1/setup.py
```

### Comparing `ersciyt-2.0/LICENSE` & `ersciyt-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-2.0/PKG-INFO` & `ersciyt-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 2.0
+Version: 2.1
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-2.0/ersciyt/inst.py` & `ersciyt-2.1/ersciyt/inst.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os,re
 
-def del():
+def delproj():
     os.system('rm -r proj')
     
 def run():
     try:
         os.system('''
         sudo apt install -y nginx
         sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default
```

### Comparing `ersciyt-2.0/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-2.1/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-2.0/ersciyt/static/inst` & `ersciyt-2.1/ersciyt/static/inst`

 * *Files identical despite different names*

### Comparing `ersciyt-2.0/ersciyt/urls.py` & `ersciyt-2.1/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-2.0/ersciyt/views.py` & `ersciyt-2.1/ersciyt/views.py`

 * *Files identical despite different names*

### Comparing `ersciyt-2.0/ersciyt.egg-info/PKG-INFO` & `ersciyt-2.1/ersciyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 2.0
+Version: 2.1
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-2.0/setup.cfg` & `ersciyt-2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 2.0
+version = 2.1
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

