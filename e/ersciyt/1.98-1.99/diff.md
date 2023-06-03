# Comparing `tmp/ersciyt-1.98.tar.gz` & `tmp/ersciyt-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.98.tar", last modified: Sat Jun  3 06:38:51 2023, max compression
+gzip compressed data, was "ersciyt-1.99.tar", last modified: Sat Jun  3 06:58:41 2023, max compression
```

## Comparing `ersciyt-1.98.tar` & `ersciyt-1.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.510579 ersciyt-1.98/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 06:38:35.000000 ersciyt-1.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 06:38:35.000000 ersciyt-1.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:38:51.510579 ersciyt-1.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 06:38:35.000000 ersciyt-1.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.508579 ersciyt-1.98/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/apps.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.509579 ersciyt-1.98/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.510579 ersciyt-1.98/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/inst
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/s
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.509579 ersciyt-1.98/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-03 06:38:51.510579 ersciyt-1.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 06:38:35.000000 ersciyt-1.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.994082 ersciyt-1.99/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 06:58:36.000000 ersciyt-1.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 06:58:36.000000 ersciyt-1.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:58:41.994082 ersciyt-1.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 06:58:36.000000 ersciyt-1.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.992081 ersciyt-1.99/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.993082 ersciyt-1.99/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.994082 ersciyt-1.99/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 06:58:36.000000 ersciyt-1.99/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:58:41.993082 ersciyt-1.99/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 06:58:41.000000 ersciyt-1.99/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-03 06:58:41.994082 ersciyt-1.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 06:58:36.000000 ersciyt-1.99/setup.py
```

### Comparing `ersciyt-1.98/LICENSE` & `ersciyt-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.98/PKG-INFO` & `ersciyt-1.99/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.98
+Version: 1.99
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.98/ersciyt/inst.py` & `ersciyt-1.99/ersciyt/inst.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,19 @@
         /usr/local/bin/django-admin  startproject proj
         ''')
         f=open ('proj/proj/settings.py', 'r' )
         content = f.read()
         content_new = re.sub('(ALLOWED_HOSTS = \[)', r"\1'*'", content, flags = re.M)
         content_new = re.sub('(INSTALLED_APPS = \[)', r"\1\n'ersciyt',", content_new, flags = re.M)
         webhost=os.getenv('WEB_HOST')
-        content_new += "\nERSCIYT_LINK = 'https:\/\/80-{}'".format(webhost)
+        content_new += "\nERSCIYT_LINK = 'https://80-{}'".format(webhost)
         f.close()
         f=open ('proj/proj/settings.py', 'w' )
         f.write(content_new)
         f.close()
-
         f=open ('proj/proj/urls.py', 'r' )
         content = f.read()
         content_new = re.sub('(from django.urls import path)', r"\1,include", content, flags = re.M)
         content_new = re.sub('(urlpatterns = \[)', r"\1\n\t\tpath('', include('ersciyt.urls')),", content_new, flags = re.M)
         f.close()
         f=open ('proj/proj/urls.py', 'w' )
         f.write(content_new)
```

### Comparing `ersciyt-1.98/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.99/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.98/ersciyt/static/inst` & `ersciyt-1.99/ersciyt/static/inst`

 * *Files identical despite different names*

### Comparing `ersciyt-1.98/ersciyt/urls.py` & `ersciyt-1.99/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.98/ersciyt/views.py` & `ersciyt-1.99/ersciyt/views.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.98/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.99/ersciyt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.98
+Version: 1.99
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.98/setup.cfg` & `ersciyt-1.99/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.98
+version = 1.99
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

