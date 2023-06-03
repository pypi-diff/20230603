# Comparing `tmp/django-selenium-clean-0.3.3.tar.gz` & `tmp/django-selenium-clean-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-selenium-clean-0.3.3.tar", last modified: Thu Apr  8 15:24:16 2021, max compression
+gzip compressed data, was "django-selenium-clean-0.3.4.tar", last modified: Sat Jun  3 08:45:26 2023, max compression
```

## Comparing `django-selenium-clean-0.3.3.tar` & `django-selenium-clean-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1222 2021-04-08 15:15:57.000000 django-selenium-clean-0.3.3/CHANGES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1541 2015-09-03 11:26:35.000000 django-selenium-clean-0.3.3/LICENSE.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2015-09-03 11:42:50.000000 django-selenium-clean-0.3.3/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10700 2017-05-23 10:37:09.000000 django-selenium-clean-0.3.3/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/django_selenium_clean/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7012 2021-04-08 15:00:42.000000 django-selenium-clean-0.3.3/django_selenium_clean/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2021-04-08 15:24:15.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      409 2021-04-08 15:24:15.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2021-04-08 15:24:15.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       33 2021-04-08 15:24:15.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2021-04-08 15:24:15.000000 django-selenium-clean-0.3.3/django_selenium_clean.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1004 2021-04-08 15:23:43.000000 django-selenium-clean-0.3.3/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-04-08 15:24:16.000000 django-selenium-clean-0.3.3/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2017-05-21 21:39:39.000000 django-selenium-clean-0.3.3/tests/__init__.py
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1299 2021-04-08 14:57:28.000000 django-selenium-clean-0.3.3/tests/manage.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1407 2021-04-08 14:57:28.000000 django-selenium-clean-0.3.3/tests/settings.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8478 2021-04-08 14:57:28.000000 django-selenium-clean-0.3.3/tests/tests.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       95 2021-04-08 15:15:57.000000 django-selenium-clean-0.3.3/tests/urls.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      104 2021-04-08 14:57:28.000000 django-selenium-clean-0.3.3/tests/views.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1349 2023-06-03 08:43:37.000000 django-selenium-clean-0.3.4/CHANGES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1541 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/LICENSE.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10700 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/django_selenium_clean/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7002 2023-06-03 08:43:37.000000 django-selenium-clean-0.3.4/django_selenium_clean/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      409 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       33 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1004 2023-06-03 08:44:26.000000 django-selenium-clean-0.3.4/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/__init__.py
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1299 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/manage.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1407 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/settings.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8478 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/tests.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       95 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/urls.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      104 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-selenium-clean-0.3.3/CHANGES.txt` & `django-selenium-clean-0.3.4/CHANGES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.3.4 (2023-06-03)
+------------------
+
+- Fixed an initialization problem that occurred sometimes in recent
+  Python versions.
+
 0.3.3 (2021-04-08)
 ------------------
 
 - Updated dependencies so that it is compatible with Django 3.
 
 0.3.2 (2019-08-30)
 ------------------
```

### Comparing `django-selenium-clean-0.3.3/LICENSE.txt` & `django-selenium-clean-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.3/PKG-INFO` & `django-selenium-clean-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-selenium-clean
-Version: 0.3.3
+Version: 0.3.4
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/aptiko/django-selenium-clean
 Author: Antonis Christofides
 Author-email: antonis@djangodeployment.com
 License: BSD 3-Clause License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-selenium-clean-0.3.3/README.rst` & `django-selenium-clean-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.3/django_selenium_clean/__init__.py` & `django-selenium-clean-0.3.4/django_selenium_clean/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 
 class SeleniumWrapper(object):
-    _instance = None
-
     def __new__(cls, *args, **kwargs):
-        if not cls._instance:
+        if not hasattr(cls, "_instance"):
             cls._instance = super(SeleniumWrapper, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     def __init__(self):
         SELENIUM_WEBDRIVERS = getattr(settings, "SELENIUM_WEBDRIVERS", {})
         if not SELENIUM_WEBDRIVERS:
             return
```

### Comparing `django-selenium-clean-0.3.3/django_selenium_clean.egg-info/PKG-INFO` & `django-selenium-clean-0.3.4/django_selenium_clean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-selenium-clean
-Version: 0.3.3
+Version: 0.3.4
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/aptiko/django-selenium-clean
 Author: Antonis Christofides
 Author-email: antonis@djangodeployment.com
 License: BSD 3-Clause License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-selenium-clean-0.3.3/setup.py` & `django-selenium-clean-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Topic :: Software Development :: Testing",
     ],
     name="django-selenium-clean",
-    version="0.3.3",
+    version="0.3.4",
     license="BSD 3-Clause License",
     description="Write clean Selenium tests in Django",
     author="Antonis Christofides",
     author_email="antonis@djangodeployment.com",
     url="https://github.com/aptiko/django-selenium-clean",
     packages=find_packages(),
     install_requires=["django>=2.2,<4", "selenium>=2.40,<4"],
```

### Comparing `django-selenium-clean-0.3.3/tests/manage.py` & `django-selenium-clean-0.3.4/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.3/tests/settings.py` & `django-selenium-clean-0.3.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.3/tests/tests.py` & `django-selenium-clean-0.3.4/tests/tests.py`

 * *Files identical despite different names*

