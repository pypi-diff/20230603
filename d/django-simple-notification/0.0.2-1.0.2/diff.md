# Comparing `tmp/django-simple-notification-0.0.2.tar.gz` & `tmp/django-simple-notification-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notification-0.0.2.tar", last modified: Fri Jun  2 16:50:52 2023, max compression
+gzip compressed data, was "django-simple-notification-1.0.2.tar", last modified: Sat Jun  3 15:49:47 2023, max compression
```

## Comparing `django-simple-notification-0.0.2.tar` & `django-simple-notification-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 16:50:52.379711 django-simple-notification-0.0.2/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-0.0.2/LICENSE
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      992 2023-06-02 16:50:52.379497 django-simple-notification-0.0.2/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       21 2023-06-02 16:16:44.000000 django-simple-notification-0.0.2/README.md
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 16:50:52.375678 django-simple-notification-0.0.2/django_simple_notification.egg-info/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      992 2023-06-02 16:50:52.000000 django-simple-notification-0.0.2/django_simple_notification.egg-info/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      682 2023-06-02 16:50:52.000000 django-simple-notification-0.0.2/django_simple_notification.egg-info/SOURCES.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-02 16:50:52.000000 django-simple-notification-0.0.2/django_simple_notification.egg-info/dependency_links.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-02 16:50:52.000000 django-simple-notification-0.0.2/django_simple_notification.egg-info/requires.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-02 16:50:52.000000 django-simple-notification-0.0.2/django_simple_notification.egg-info/top_level.txt
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 16:50:52.378438 django-simple-notification-0.0.2/notifications/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-0.0.2/notifications/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-0.0.2/notifications/admin.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-0.0.2/notifications/apps.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-0.0.2/notifications/consumers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      958 2023-06-01 21:29:23.000000 django-simple-notification-0.0.2/notifications/handlers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      294 2023-05-22 21:58:17.000000 django-simple-notification-0.0.2/notifications/handlers_reader.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 16:50:52.379217 django-simple-notification-0.0.2/notifications/migrations/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1023 2023-05-24 17:44:35.000000 django-simple-notification-0.0.2/notifications/migrations/0001_initial.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      405 2023-06-01 21:29:07.000000 django-simple-notification-0.0.2/notifications/migrations/0002_notification_type.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-0.0.2/notifications/migrations/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      689 2023-06-01 21:28:58.000000 django-simple-notification-0.0.2/notifications/models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      223 2023-06-01 21:17:19.000000 django-simple-notification-0.0.2/notifications/serializers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-0.0.2/notifications/tests.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-0.0.2/notifications/urls.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1272 2023-06-01 21:38:09.000000 django-simple-notification-0.0.2/notifications/views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-02 16:50:52.379777 django-simple-notification-0.0.2/setup.cfg
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1292 2023-06-02 16:50:40.000000 django-simple-notification-0.0.2/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.586196 django-simple-notification-1.0.2/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.2/LICENSE
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2352 2023-06-03 15:49:47.585977 django-simple-notification-1.0.2/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1382 2023-06-02 18:17:41.000000 django-simple-notification-1.0.2/README.md
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.581838 django-simple-notification-1.0.2/django_simple_notification.egg-info/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2352 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      722 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/requires.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-03 15:49:47.000000 django-simple-notification-1.0.2/django_simple_notification.egg-info/top_level.txt
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.584307 django-simple-notification-1.0.2/notifications/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.2/notifications/admin.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.2/notifications/apps.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.2/notifications/consumers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.2/notifications/handlers.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.585017 django-simple-notification-1.0.2/notifications/migrations/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.2/notifications/migrations/0001_initial.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/migrations/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.2/notifications/models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.2/notifications/serializers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.2/notifications/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 15:49:47.585660 django-simple-notification-1.0.2/notifications/tests/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.2/notifications/tests/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.2/notifications/tests/test_models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.2/notifications/tests/test_views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.2/notifications/tests.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.2/notifications/urls.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.2/notifications/views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-03 15:49:47.586256 django-simple-notification-1.0.2/setup.cfg
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1292 2023-06-03 15:49:44.000000 django-simple-notification-1.0.2/setup.py
```

### Comparing `django-simple-notification-0.0.2/LICENSE` & `django-simple-notification-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notification-0.0.2/django_simple_notification.egg-info/SOURCES.txt` & `django-simple-notification-1.0.2/django_simple_notification.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 django_simple_notification.egg-info/requires.txt
 django_simple_notification.egg-info/top_level.txt
 notifications/__init__.py
 notifications/admin.py
 notifications/apps.py
 notifications/consumers.py
 notifications/handlers.py
-notifications/handlers_reader.py
 notifications/models.py
 notifications/serializers.py
+notifications/setup.py
 notifications/tests.py
 notifications/urls.py
 notifications/views.py
 notifications/migrations/0001_initial.py
-notifications/migrations/0002_notification_type.py
-notifications/migrations/__init__.py
+notifications/migrations/__init__.py
+notifications/tests/__init__.py
+notifications/tests/test_models.py
+notifications/tests/test_views.py
```

### Comparing `django-simple-notification-0.0.2/notifications/consumers.py` & `django-simple-notification-1.0.2/notifications/consumers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-0.0.2/notifications/handlers.py` & `django-simple-notification-1.0.2/notifications/handlers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from typing import Dict
-
 from asgiref.sync import async_to_sync
 from channels.layers import get_channel_layer
 
-from apps.notifications.models import Notification
-from apps.notifications.serializers import NotificationSerializer
+from .models import Notification
+from .serializers import NotificationSerializer
 
 channel_layer = get_channel_layer()
 
 
 def send_message(message, user, type: str):
     notification = Notification.objects.create(user=user, content=message, type=type)
 
@@ -18,21 +16,9 @@
             'type': 'notification',
             'notification_type': type,
             'data': dict(NotificationSerializer(notification).data)
         }
     )
 
 
-def receive_handler(data: Dict):
-    print(data)
-
-
 def get_user_inbox_key(user_id):
     return f'inbox_{user_id}'
-
-
-def post_like_notification(message, user):
-    send_message(message, user, 'like_post')
-
-
-def new_offer_notification(message, user):
-    send_message(message, user, 'new_offer')
```

### Comparing `django-simple-notification-0.0.2/notifications/migrations/0001_initial.py` & `django-simple-notification-1.0.2/notifications/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-05-24 17:44
+# Generated by Django 4.2.1 on 2023-06-02 17:38
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
@@ -14,18 +14,15 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='Notification',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', models.DateTimeField(auto_now_add=True, db_index=True)),
-                ('modified', models.DateTimeField(auto_now=True)),
                 ('is_read', models.BooleanField(default=False)),
                 ('content', models.TextField()),
+                ('type', models.CharField(blank=True, max_length=100, null=True)),
+                ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
             ],
-            options={
-                'abstract': False,
-            },
         ),
     ]
```

### Comparing `django-simple-notification-0.0.2/notifications/views.py` & `django-simple-notification-1.0.2/notifications/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.shortcuts import render
 from rest_framework import status
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from apps.notifications.models import Notification
-from apps.notifications.serializers import NotificationSerializer
+from notifications.models import Notification
+from notifications.serializers import NotificationSerializer
 
 
 def index(request):
     return render(request, 'notifications_index.html')
 
 
 class FetchUnreadNotifications(APIView):
```

### Comparing `django-simple-notification-0.0.2/setup.py` & `django-simple-notification-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-simple-notification',
-    version='0.0.2',
+    version='1.0.2',
     author='Mahmoud Nasser',
     author_email='mahmoud.nasser.abdulhamed@gmail.com',
     description='Simple user notification management for the Django web framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/fritill-team/django_translation.git',
     license='MIT',
```

