# Comparing `tmp/django-simple-notification-1.0.2.tar.gz` & `tmp/django-simple-notification-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notification-1.0.2.tar", last modified: Sat Jun  3 15:49:47 2023, max compression
+gzip compressed data, was "django-simple-notification-1.0.3.tar", last modified: Sat Jun  3 16:00:52 2023, max compression
```

## Comparing `django-simple-notification-1.0.2.tar` & `django-simple-notification-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.586196 django-simple-notification-1.0.2/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.2/LICENSE
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2352 2023-06-03 15:49:47.585977 django-simple-notification-1.0.2/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1382 2023-06-02 18:17:41.000000 django-simple-notification-1.0.2/README.md
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.581838 django-simple-notification-1.0.2/django_simple_notification.egg-info/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2352 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      722 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/SOURCES.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/dependency_links.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/requires.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/top_level.txt
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.584307 django-simple-notification-1.0.2/notifications/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.2/notifications/admin.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.2/notifications/apps.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.2/notifications/consumers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.2/notifications/handlers.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.585017 django-simple-notification-1.0.2/notifications/migrations/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.2/notifications/migrations/0001_initial.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/migrations/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.2/notifications/models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.2/notifications/serializers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.2/notifications/setup.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.585660 django-simple-notification-1.0.2/notifications/tests/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.2/notifications/tests/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.2/notifications/tests/test_models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.2/notifications/tests/test_views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/tests.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.2/notifications/urls.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.2/notifications/views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-03 15:49:47.586256 django-simple-notification-1.0.2/setup.cfg
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1292 2023-06-03 15:49:44.000000 django-simple-notification-1.0.2/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.024272 django-simple-notification-1.0.3/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.3/LICENSE
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2774 2023-06-03 16:00:52.024054 django-simple-notification-1.0.3/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1797 2023-06-03 16:00:29.000000 django-simple-notification-1.0.3/README.md
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.019340 django-simple-notification-1.0.3/django_simple_notification.egg-info/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2774 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      722 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/requires.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/top_level.txt
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.022679 django-simple-notification-1.0.3/notifications/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.3/notifications/admin.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.3/notifications/apps.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.3/notifications/consumers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.3/notifications/handlers.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.023156 django-simple-notification-1.0.3/notifications/migrations/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.3/notifications/migrations/0001_initial.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/migrations/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.3/notifications/models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.3/notifications/serializers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.3/notifications/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.023726 django-simple-notification-1.0.3/notifications/tests/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.3/notifications/tests/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.3/notifications/tests/test_models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.3/notifications/tests/test_views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/tests.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.3/notifications/urls.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.3/notifications/views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-03 16:00:52.024333 django-simple-notification-1.0.3/setup.cfg
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1299 2023-06-03 16:00:49.000000 django-simple-notification-1.0.3/setup.py
```

### Comparing `django-simple-notification-1.0.2/LICENSE` & `django-simple-notification-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/PKG-INFO` & `django-simple-notification-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple user notification management for the Django web framework
-Home-page: https://github.com/fritill-team/django_translation.git
+Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -42,28 +42,34 @@
 user: an instance of User model (the one who will recieve the notification)
 type: is a notification tag (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
-![img.png](read_me_media/img.png)
-<br/><br/><br/>
+<br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
 
-![img_1.png](read_me_media/img_1.png)
+![img_1.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_1.png?raw=true)
 <br/><br/><br/>
 
 ``notifications/unread/``:GET: get all unread notifications
 
-![img_2.png](read_me_media/img_2.png)
+![img_2.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_2.png?raw=true)
+
+## 3.how the client side recieve the message from the server via websocket
+![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
+
+
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
 
+
+in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
     ...   
 ]
@@ -77,12 +83,19 @@
 }
 ```
 
 ```python
 AUTH_USER_MODEL = "users.User"
 ```
 
+in ``urls.py``
+
 ```python
     path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+run make migrate:
+
+```shell
+python manage.py migrate
+```
```

### Comparing `django-simple-notification-1.0.2/README.md` & `django-simple-notification-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,28 +18,34 @@
 user: an instance of User model (the one who will recieve the notification)
 type: is a notification tag (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
-![img.png](read_me_media/img.png)
-<br/><br/><br/>
+<br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
 
-![img_1.png](read_me_media/img_1.png)
+![img_1.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_1.png?raw=true)
 <br/><br/><br/>
 
 ``notifications/unread/``:GET: get all unread notifications
 
-![img_2.png](read_me_media/img_2.png)
+![img_2.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_2.png?raw=true)
+
+## 3.how the client side recieve the message from the server via websocket
+![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
+
+
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
 
+
+in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
     ...   
 ]
@@ -53,12 +59,19 @@
 }
 ```
 
 ```python
 AUTH_USER_MODEL = "users.User"
 ```
 
+in ``urls.py``
+
 ```python
     path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+run make migrate:
+
+```shell
+python manage.py migrate
+```
```

### Comparing `django-simple-notification-1.0.2/django_simple_notification.egg-info/PKG-INFO` & `django-simple-notification-1.0.3/django_simple_notification.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple user notification management for the Django web framework
-Home-page: https://github.com/fritill-team/django_translation.git
+Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -42,28 +42,34 @@
 user: an instance of User model (the one who will recieve the notification)
 type: is a notification tag (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
-![img.png](read_me_media/img.png)
-<br/><br/><br/>
+<br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
 
-![img_1.png](read_me_media/img_1.png)
+![img_1.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_1.png?raw=true)
 <br/><br/><br/>
 
 ``notifications/unread/``:GET: get all unread notifications
 
-![img_2.png](read_me_media/img_2.png)
+![img_2.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img_2.png?raw=true)
+
+## 3.how the client side recieve the message from the server via websocket
+![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
+
+
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
 
+
+in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
     ...   
 ]
@@ -77,12 +83,19 @@
 }
 ```
 
 ```python
 AUTH_USER_MODEL = "users.User"
 ```
 
+in ``urls.py``
+
 ```python
     path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+run make migrate:
+
+```shell
+python manage.py migrate
+```
```

### Comparing `django-simple-notification-1.0.2/django_simple_notification.egg-info/SOURCES.txt` & `django-simple-notification-1.0.3/django_simple_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/consumers.py` & `django-simple-notification-1.0.3/notifications/consumers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/handlers.py` & `django-simple-notification-1.0.3/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/migrations/0001_initial.py` & `django-simple-notification-1.0.3/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/tests/test_models.py` & `django-simple-notification-1.0.3/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/tests/test_views.py` & `django-simple-notification-1.0.3/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/notifications/views.py` & `django-simple-notification-1.0.3/notifications/views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.2/setup.py` & `django-simple-notification-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-simple-notification',
-    version='1.0.2',
+    version='1.0.3',
     author='Mahmoud Nasser',
     author_email='mahmoud.nasser.abdulhamed@gmail.com',
     description='Simple user notification management for the Django web framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/fritill-team/django_translation.git',
+    url='https://github.com/MahmoudNasser01/django_simple_notification',
     license='MIT',
     platform='any',
     keywords='django notification simple custom',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
```

