# Comparing `tmp/ersciyt-1.99.tar.gz` & `tmp/ersciyt-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.99.tar", last modified: Sat Jun  3 06:58:41 2023, max compression
+gzip compressed data, was "ersciyt-2.0.tar", last modified: Sat Jun  3 11:20:49 2023, max compression
```

## Comparing `ersciyt-1.99.tar` & `ersciyt-2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.994082 ersciyt-1.99/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 06:58:36.000000 ersciyt-1.99/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 06:58:36.000000 ersciyt-1.99/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:58:41.994082 ersciyt-1.99/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 06:58:36.000000 ersciyt-1.99/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.992081 ersciyt-1.99/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/apps.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.993082 ersciyt-1.99/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.994082 ersciyt-1.99/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/inst
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/s
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.993082 ersciyt-1.99/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-03 06:58:41.994082 ersciyt-1.99/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 06:58:36.000000 ersciyt-1.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.109858 ersciyt-2.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 11:20:42.000000 ersciyt-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 11:20:42.000000 ersciyt-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:20:49.109858 ersciyt-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 11:20:42.000000 ersciyt-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.107857 ersciyt-2.0/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.108857 ersciyt-2.0/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.109858 ersciyt-2.0/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 11:20:42.000000 ersciyt-2.0/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:20:49.108857 ersciyt-2.0/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 11:20:48.000000 ersciyt-2.0/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      664 2023-06-03 11:20:49.110858 ersciyt-2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 11:20:42.000000 ersciyt-2.0/setup.py
```

### Comparing `ersciyt-1.99/LICENSE` & `ersciyt-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.99/PKG-INFO` & `ersciyt-2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.99
+Version: 2.0
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.99/ersciyt/inst.py` & `ersciyt-2.0/ersciyt/inst.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os,re
 
-
+def del():
+    os.system('rm -r proj')
+    
 def run():
     try:
         os.system('''
         sudo apt install -y nginx
         sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default
         sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default
         sudo service nginx restart
```

### Comparing `ersciyt-1.99/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-2.0/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.99/ersciyt/static/inst` & `ersciyt-2.0/ersciyt/static/inst`

 * *Files identical despite different names*

### Comparing `ersciyt-1.99/ersciyt/urls.py` & `ersciyt-2.0/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.99/ersciyt/views.py` & `ersciyt-2.0/ersciyt/views.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.99/ersciyt.egg-info/PKG-INFO` & `ersciyt-2.0/ersciyt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.99
+Version: 2.0
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

