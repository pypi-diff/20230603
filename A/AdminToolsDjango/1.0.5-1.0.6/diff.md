# Comparing `tmp/AdminToolsDjango-1.0.5.tar.gz` & `tmp/AdminToolsDjango-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdminToolsDjango-1.0.5.tar", last modified: Sat Jun  3 12:29:14 2023, max compression
+gzip compressed data, was "AdminToolsDjango-1.0.6.tar", last modified: Sat Jun  3 12:37:28 2023, max compression
```

## Comparing `AdminToolsDjango-1.0.5.tar` & `AdminToolsDjango-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.661996 AdminToolsDjango-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.638040 AdminToolsDjango-1.0.5/AdminToolsDjango/
--rw-rw-rw-   0        0        0     7761 2023-06-03 12:27:57.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/CreateProject.py
--rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.644052 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/
--rw-rw-rw-   0        0        0     3956 2023-05-31 15:42:58.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/admin_script.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.651004 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/__init__.py
--rw-rw-rw-   0        0        0       63 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/admin.py
--rw-rw-rw-   0        0        0      147 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.652002 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/migrations/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/migrations/__init__.py
--rw-rw-rw-   0        0        0       57 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/models.py
--rw-rw-rw-   0        0        0      450 2023-05-31 09:51:36.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/tests.py
--rw-rw-rw-   0        0        0      142 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/urls.py
--rw-rw-rw-   0        0        0      148 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/views.py
--rw-rw-rw-   0        0        0      792 2023-05-31 08:06:12.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/manage.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.658982 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/
--rw-rw-rw-   0        0        0        0 2022-11-25 16:12:43.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/__init__.py
--rw-rw-rw-   0        0        0      411 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/asgi.py
--rw-rw-rw-   0        0        0     4259 2023-06-03 12:26:07.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/settings.py
--rw-rw-rw-   0        0        0      896 2023-05-31 15:40:42.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/urls.py
--rw-rw-rw-   0        0        0      177 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/uwsgi.ini
--rw-rw-rw-   0        0        0      419 2023-05-31 07:46:15.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.659999 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/static/
--rw-rw-rw-   0        0        0       22 2023-05-31 09:51:09.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/static/test.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.642029 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/
--rw-rw-rw-   0        0        0     1112 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1112 2023-06-03 12:29:14.661001 AdminToolsDjango-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      990 2023-06-03 12:28:33.000000 AdminToolsDjango-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 12:29:14.661996 AdminToolsDjango-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-06-03 12:28:05.000000 AdminToolsDjango-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.465453 AdminToolsDjango-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.443548 AdminToolsDjango-1.0.6/AdminToolsDjango/
+-rw-rw-rw-   0        0        0     7761 2023-06-03 12:27:57.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/CreateProject.py
+-rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.448619 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/
+-rw-rw-rw-   0        0        0     3956 2023-05-31 15:42:58.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/admin_script.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.455602 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/admin.py
+-rw-rw-rw-   0        0        0      147 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.457449 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/migrations/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/models.py
+-rw-rw-rw-   0        0        0      450 2023-05-31 09:51:36.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/tests.py
+-rw-rw-rw-   0        0        0      142 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/urls.py
+-rw-rw-rw-   0        0        0      148 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/app_test/views.py
+-rw-rw-rw-   0        0        0      792 2023-05-31 08:06:12.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/manage.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.462460 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/
+-rw-rw-rw-   0        0        0        0 2022-11-25 16:12:43.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/asgi.py
+-rw-rw-rw-   0        0        0     4259 2023-06-03 12:26:07.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/settings.py
+-rw-rw-rw-   0        0        0      896 2023-05-31 15:40:42.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/urls.py
+-rw-rw-rw-   0        0        0      177 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/uwsgi.ini
+-rw-rw-rw-   0        0        0      419 2023-05-31 07:46:15.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.463467 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/static/
+-rw-rw-rw-   0        0        0       22 2023-05-31 09:51:09.000000 AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/static/test.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 12:37:28.447525 AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/
+-rw-rw-rw-   0        0        0     1112 2023-06-03 12:37:28.000000 AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-06-03 12:37:28.000000 AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:37:28.000000 AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-03 12:37:28.000000 AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1112 2023-06-03 12:37:28.465453 AdminToolsDjango-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2023-06-03 12:28:33.000000 AdminToolsDjango-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:37:28.465453 AdminToolsDjango-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-06-03 12:37:07.000000 AdminToolsDjango-1.0.6/setup.py
```

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango/CreateProject.py` & `AdminToolsDjango-1.0.6/AdminToolsDjango/CreateProject.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/admin_script.py` & `AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/admin_script.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/manage.py` & `AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/manage.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/settings.py` & `AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/settings.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/urls.py` & `AdminToolsDjango-1.0.6/AdminToolsDjango/template-1.0/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/PKG-INFO` & `AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdminToolsDjango
-Version: 1.0.5
+Version: 1.0.6
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 ## AdminToolsDjango
 
 使用模板 自动创建Django项目
 ## 介绍：
```

### Comparing `AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/SOURCES.txt` & `AdminToolsDjango-1.0.6/AdminToolsDjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.5/PKG-INFO` & `AdminToolsDjango-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdminToolsDjango
-Version: 1.0.5
+Version: 1.0.6
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 ## AdminToolsDjango
 
 使用模板 自动创建Django项目
 ## 介绍：
```

### Comparing `AdminToolsDjango-1.0.5/README.md` & `AdminToolsDjango-1.0.6/README.md`

 * *Files identical despite different names*

