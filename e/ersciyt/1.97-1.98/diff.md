# Comparing `tmp/ersciyt-1.97.tar.gz` & `tmp/ersciyt-1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.97.tar", last modified: Thu Jun  1 07:22:31 2023, max compression
+gzip compressed data, was "ersciyt-1.98.tar", last modified: Sat Jun  3 06:38:51 2023, max compression
```

## Comparing `ersciyt-1.97.tar` & `ersciyt-1.98.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:22:31.443291 ersciyt-1.97/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-01 07:22:23.000000 ersciyt-1.97/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 07:22:23.000000 ersciyt-1.97/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 07:22:31.444290 ersciyt-1.97/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-01 07:22:23.000000 ersciyt-1.97/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:22:31.441290 ersciyt-1.97/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/apps.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:22:31.442290 ersciyt-1.97/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:22:31.443291 ersciyt-1.97/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/static/inst
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/static/s
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-06-01 07:22:23.000000 ersciyt-1.97/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:22:31.442290 ersciyt-1.97/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 07:22:31.000000 ersciyt-1.97/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-01 07:22:31.000000 ersciyt-1.97/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 07:22:31.000000 ersciyt-1.97/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 07:22:31.000000 ersciyt-1.97/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 07:22:31.000000 ersciyt-1.97/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-01 07:22:31.444290 ersciyt-1.97/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 07:22:23.000000 ersciyt-1.97/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.510579 ersciyt-1.98/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-03 06:38:35.000000 ersciyt-1.98/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-03 06:38:35.000000 ersciyt-1.98/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:38:51.510579 ersciyt-1.98/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-03 06:38:35.000000 ersciyt-1.98/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.508579 ersciyt-1.98/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.509579 ersciyt-1.98/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.510579 ersciyt-1.98/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-03 06:38:35.000000 ersciyt-1.98/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:38:51.509579 ersciyt-1.98/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-03 06:38:51.000000 ersciyt-1.98/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-03 06:38:51.510579 ersciyt-1.98/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-03 06:38:35.000000 ersciyt-1.98/setup.py
```

### Comparing `ersciyt-1.97/LICENSE` & `ersciyt-1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.97/PKG-INFO` & `ersciyt-1.98/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.97
+Version: 1.98
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -26,7 +26,14 @@
 2.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('yt/', include('ersciyt.urls')),
 ```
 
 3.Visit http://127.0.0.1:8000/yt/ to create users and its cards.
+
+4.run this command if you on shell.cloud.google:
+```
+python
+>>>from ersciyt import inst
+>>>inst.run()
+```
```

### Comparing `ersciyt-1.97/ersciyt/inst.py` & `ersciyt-1.98/ersciyt/static/inst`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-import os
-
-def inst():
-    try:
-        os.system('''
-        sudo apt install -y nginx
-        sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default
-        sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default
-        sudo service nginx restart
-        /usr/local/bin/django-admin  startproject proj
-        sed -i "s/ALLOWED_HOSTS = \[/&'*'/" proj/proj/settings.py
-        sed -i "s/INSTALLED_APPS = \[/& \n\t\t'ersciyt',/" proj/proj/settings.py
-        sed -i "s/STATIC_URL = 'static\/'/& \nERSCIYT_LINK = 'https:\/\/80-$WEB_HOST'/" proj/proj/settings.py
-        sed -i "s/from django.urls import path/&,include/" proj/proj/urls.py
-        sed -i "s/urlpatterns = \[/&\n\t\tpath('', include('ersciyt.urls')),/"  proj/proj/urls.py
-        python proj/manage.py runserver
-        ''')
-    except:
-        print('Error in command')
-        
+sudo apt install -y nginx
+sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default
+sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default
+sudo service nginx restart
+/usr/local/bin/django-admin  startproject proj
+sed -i "s/ALLOWED_HOSTS = \[/&'*'/" proj/proj/settings.py
+sed -i "s/INSTALLED_APPS = \[/& \n\t\t'ersciyt',/" proj/proj/settings.py
+sed -i "s/STATIC_URL = 'static\/'/& \nERSCIYT_LINK = 'https:\/\/80-$WEB_HOST'/" proj/proj/settings.py
+sed -i "s/from django.urls import path/&,include/" proj/proj/urls.py
+sed -i "s/urlpatterns = \[/&\n\t\tpath('', include('ersciyt.urls')),/"  proj/proj/urls.py
+python proj/manage.py runserver
```

### Comparing `ersciyt-1.97/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.98/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.97/ersciyt/urls.py` & `ersciyt-1.98/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.97/ersciyt/views.py` & `ersciyt-1.98/ersciyt/views.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.97/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.98/ersciyt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.97
+Version: 1.98
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -26,7 +26,14 @@
 2.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('yt/', include('ersciyt.urls')),
 ```
 
 3.Visit http://127.0.0.1:8000/yt/ to create users and its cards.
+
+4.run this command if you on shell.cloud.google:
+```
+python
+>>>from ersciyt import inst
+>>>inst.run()
+```
```

### Comparing `ersciyt-1.97/setup.cfg` & `ersciyt-1.98/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.97
+version = 1.98
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

