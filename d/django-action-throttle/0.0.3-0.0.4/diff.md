# Comparing `tmp/django-action-throttle-0.0.3.tar.gz` & `tmp/django-action-throttle-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-action-throttle-0.0.3.tar", last modified: Sat Jun  3 10:37:44 2023, max compression
+gzip compressed data, was "django-action-throttle-0.0.4.tar", last modified: Sat Jun  3 11:44:08 2023, max compression
```

## Comparing `django-action-throttle-0.0.3.tar` & `django-action-throttle-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 10:37:44.372758 django-action-throttle-0.0.3/
--rwxrwxrwx   0 s         (1000) s         (1000)       11 2023-06-03 10:03:48.000000 django-action-throttle-0.0.3/LICENCE
--rwxrwxrwx   0 s         (1000) s         (1000)       37 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/MANIFEST.in
--rwxrwxrwx   0 s         (1000) s         (1000)      652 2023-06-03 10:37:44.388530 django-action-throttle-0.0.3/PKG-INFO
--rwxrwxrwx   0 s         (1000) s         (1000)       24 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/README.rst
-drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 10:37:44.168616 django-action-throttle-0.0.3/action_throttle/
--rwxrwxrwx   0 s         (1000) s         (1000)      555 2023-06-03 10:27:58.000000 django-action-throttle-0.0.3/action_throttle/__init__.py
--rwxrwxrwx   0 s         (1000) s         (1000)      173 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/admin.py
--rwxrwxrwx   0 s         (1000) s         (1000)      161 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/apps.py
--rwxrwxrwx   0 s         (1000) s         (1000)     1578 2023-06-03 10:23:20.000000 django-action-throttle-0.0.3/action_throttle/middleware.py
--rwxrwxrwx   0 s         (1000) s         (1000)     3594 2023-06-03 09:38:04.000000 django-action-throttle-0.0.3/action_throttle/models.py
--rwxrwxrwx   0 s         (1000) s         (1000)     1262 2023-06-03 10:23:20.000000 django-action-throttle-0.0.3/action_throttle/rest.py
--rwxrwxrwx   0 s         (1000) s         (1000)       63 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/tests.py
--rwxrwxrwx   0 s         (1000) s         (1000)     7288 2023-06-03 10:23:20.000000 django-action-throttle-0.0.3/action_throttle/throttle.py
--rwxrwxrwx   0 s         (1000) s         (1000)      565 2023-06-03 09:45:42.000000 django-action-throttle-0.0.3/action_throttle/throttle_settings.py
--rwxrwxrwx   0 s         (1000) s         (1000)       50 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/urls.py
--rwxrwxrwx   0 s         (1000) s         (1000)      239 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/utils.py
--rwxrwxrwx   0 s         (1000) s         (1000)       66 2023-06-02 21:32:39.000000 django-action-throttle-0.0.3/action_throttle/views.py
-drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 10:37:44.341499 django-action-throttle-0.0.3/django_action_throttle.egg-info/
--rwxrwxrwx   0 s         (1000) s         (1000)      652 2023-06-03 10:37:43.000000 django-action-throttle-0.0.3/django_action_throttle.egg-info/PKG-INFO
--rwxrwxrwx   0 s         (1000) s         (1000)      599 2023-06-03 10:37:43.000000 django-action-throttle-0.0.3/django_action_throttle.egg-info/SOURCES.txt
--rwxrwxrwx   0 s         (1000) s         (1000)        1 2023-06-03 10:37:43.000000 django-action-throttle-0.0.3/django_action_throttle.egg-info/dependency_links.txt
--rwxrwxrwx   0 s         (1000) s         (1000)       19 2023-06-03 10:37:43.000000 django-action-throttle-0.0.3/django_action_throttle.egg-info/requires.txt
--rwxrwxrwx   0 s         (1000) s         (1000)       16 2023-06-03 10:37:43.000000 django-action-throttle-0.0.3/django_action_throttle.egg-info/top_level.txt
--rwxrwxrwx   0 s         (1000) s         (1000)      685 2023-06-03 10:37:44.408801 django-action-throttle-0.0.3/setup.cfg
--rwxrwxrwx   0 s         (1000) s         (1000)      324 2023-06-03 10:00:21.000000 django-action-throttle-0.0.3/setup.py
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 11:44:08.320795 django-action-throttle-0.0.4/
+-rwxrwxrwx   0 s         (1000) s         (1000)       11 2023-06-03 10:03:48.000000 django-action-throttle-0.0.4/LICENCE
+-rwxrwxrwx   0 s         (1000) s         (1000)       37 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 s         (1000) s         (1000)      652 2023-06-03 11:44:08.320795 django-action-throttle-0.0.4/PKG-INFO
+-rwxrwxrwx   0 s         (1000) s         (1000)       24 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/README.rst
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 11:44:08.114060 django-action-throttle-0.0.4/action_throttle/
+-rwxrwxrwx   0 s         (1000) s         (1000)      567 2023-06-03 11:42:13.000000 django-action-throttle-0.0.4/action_throttle/__init__.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      173 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/admin.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      161 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/apps.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     1578 2023-06-03 10:23:20.000000 django-action-throttle-0.0.4/action_throttle/middleware.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     3594 2023-06-03 09:38:04.000000 django-action-throttle-0.0.4/action_throttle/models.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     1262 2023-06-03 10:23:20.000000 django-action-throttle-0.0.4/action_throttle/rest.py
+-rwxrwxrwx   0 s         (1000) s         (1000)       63 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/tests.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     7288 2023-06-03 10:23:20.000000 django-action-throttle-0.0.4/action_throttle/throttle.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      565 2023-06-03 09:45:42.000000 django-action-throttle-0.0.4/action_throttle/throttle_settings.py
+-rwxrwxrwx   0 s         (1000) s         (1000)       50 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/urls.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      239 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/utils.py
+-rwxrwxrwx   0 s         (1000) s         (1000)       66 2023-06-02 21:32:39.000000 django-action-throttle-0.0.4/action_throttle/views.py
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2023-06-03 11:44:08.274082 django-action-throttle-0.0.4/django_action_throttle.egg-info/
+-rwxrwxrwx   0 s         (1000) s         (1000)      652 2023-06-03 11:44:07.000000 django-action-throttle-0.0.4/django_action_throttle.egg-info/PKG-INFO
+-rwxrwxrwx   0 s         (1000) s         (1000)      599 2023-06-03 11:44:07.000000 django-action-throttle-0.0.4/django_action_throttle.egg-info/SOURCES.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)        1 2023-06-03 11:44:07.000000 django-action-throttle-0.0.4/django_action_throttle.egg-info/dependency_links.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)       19 2023-06-03 11:44:07.000000 django-action-throttle-0.0.4/django_action_throttle.egg-info/requires.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)       16 2023-06-03 11:44:07.000000 django-action-throttle-0.0.4/django_action_throttle.egg-info/top_level.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)      685 2023-06-03 11:44:08.338233 django-action-throttle-0.0.4/setup.cfg
+-rwxrwxrwx   0 s         (1000) s         (1000)      324 2023-06-03 10:44:05.000000 django-action-throttle-0.0.4/setup.py
```

### Comparing `django-action-throttle-0.0.3/PKG-INFO` & `django-action-throttle-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-action-throttle
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django Action Throttle
 Home-page: https://github.com/amir4v/django-action-throttle/
 Author: Amirhosein Ghorbani
 License: MIT License
 Keywords: django action throttle
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-action-throttle-0.0.3/action_throttle/__init__.py` & `django-action-throttle-0.0.4/action_throttle/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Django Action Throttle
 """
 
-from .throttle import action_throttle, action_throttle_using_cache
-from .middleware import ThrottleMiddleware
-from .rest import ActionThrottle
+# from .throttle import action_throttle, action_throttle_using_cache
+# from .middleware import ThrottleMiddleware
+# from .rest import ActionThrottle
 
 __title__ = 'Django Action Throttle'
-__version__ = open('version', 'r').read()
+# __version__ = open('version', 'r').read()
 __author__ = 'Amirhosein Ghorbani'
-__license__ = open('LICENSE', 'r').read()
+# __license__ = open('LICENSE', 'r').read()
 __copyright__ = 'Copyright 2022-'
 
 # Version synonym
-VERSION = __version__
+# VERSION = __version__
 
 __all__ = ['admin', 'apps', 'middleware', 'models', 'rest', 'tests', 'throttle', 'throttle_settings', 'urls', 'utils', 'views',]
```

### Comparing `django-action-throttle-0.0.3/action_throttle/middleware.py` & `django-action-throttle-0.0.4/action_throttle/middleware.py`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/action_throttle/models.py` & `django-action-throttle-0.0.4/action_throttle/models.py`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/action_throttle/rest.py` & `django-action-throttle-0.0.4/action_throttle/rest.py`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/action_throttle/throttle.py` & `django-action-throttle-0.0.4/action_throttle/throttle.py`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/action_throttle/throttle_settings.py` & `django-action-throttle-0.0.4/action_throttle/throttle_settings.py`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/django_action_throttle.egg-info/PKG-INFO` & `django-action-throttle-0.0.4/django_action_throttle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-action-throttle
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django Action Throttle
 Home-page: https://github.com/amir4v/django-action-throttle/
 Author: Amirhosein Ghorbani
 License: MIT License
 Keywords: django action throttle
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-action-throttle-0.0.3/django_action_throttle.egg-info/SOURCES.txt` & `django-action-throttle-0.0.4/django_action_throttle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-action-throttle-0.0.3/setup.cfg` & `django-action-throttle-0.0.4/setup.cfg`

 * *Files identical despite different names*

