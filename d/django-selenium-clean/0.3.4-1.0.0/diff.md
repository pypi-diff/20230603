# Comparing `tmp/django-selenium-clean-0.3.4.tar.gz` & `tmp/django-selenium-clean-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-selenium-clean-0.3.4.tar", last modified: Sat Jun  3 08:45:26 2023, max compression
+gzip compressed data, was "django-selenium-clean-1.0.0.tar", last modified: Sat Jun  3 10:05:02 2023, max compression
```

## Comparing `django-selenium-clean-0.3.4.tar` & `django-selenium-clean-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1349 2023-06-03 08:43:37.000000 django-selenium-clean-0.3.4/CHANGES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1541 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/LICENSE.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10700 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/django_selenium_clean/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7002 2023-06-03 08:43:37.000000 django-selenium-clean-0.3.4/django_selenium_clean/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      409 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       33 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2023-06-03 08:45:26.000000 django-selenium-clean-0.3.4/django_selenium_clean.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1004 2023-06-03 08:44:26.000000 django-selenium-clean-0.3.4/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:45:26.736758 django-selenium-clean-0.3.4/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/__init__.py
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1299 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/manage.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1407 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/settings.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8478 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/tests.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       95 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/urls.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      104 2023-06-03 08:10:56.000000 django-selenium-clean-0.3.4/tests/views.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1410 2023-06-03 10:00:45.000000 django-selenium-clean-1.0.0/CHANGES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1541 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/LICENSE.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10700 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/django_selenium_clean/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7002 2023-06-03 08:43:37.000000 django-selenium-clean-1.0.0/django_selenium_clean/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      812 2023-06-03 10:05:02.000000 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      409 2023-06-03 10:05:02.000000 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-06-03 10:05:02.000000 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       30 2023-06-03 10:05:02.000000 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2023-06-03 10:05:02.000000 django-selenium-clean-1.0.0/django_selenium_clean.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       38 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1001 2023-06-03 10:04:02.000000 django-selenium-clean-1.0.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-06-03 10:05:02.804262 django-selenium-clean-1.0.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/tests/__init__.py
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1299 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/tests/manage.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1407 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/tests/settings.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8478 2023-06-03 09:49:47.000000 django-selenium-clean-1.0.0/tests/tests.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       95 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/tests/urls.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      104 2023-06-03 08:10:56.000000 django-selenium-clean-1.0.0/tests/views.py
```

### Comparing `django-selenium-clean-0.3.4/CHANGES.txt` & `django-selenium-clean-1.0.0/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.0.0 (2023-06-03)
+------------------
+
+- Support Selenium 4
+
 0.3.4 (2023-06-03)
 ------------------
 
 - Fixed an initialization problem that occurred sometimes in recent
   Python versions.
 
 0.3.3 (2021-04-08)
```

### Comparing `django-selenium-clean-0.3.4/LICENSE.txt` & `django-selenium-clean-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.4/PKG-INFO` & `django-selenium-clean-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-selenium-clean
-Version: 0.3.4
+Version: 1.0.0
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/aptiko/django-selenium-clean
 Author: Antonis Christofides
 Author-email: antonis@djangodeployment.com
 License: BSD 3-Clause License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-selenium-clean-0.3.4/README.rst` & `django-selenium-clean-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.4/django_selenium_clean/__init__.py` & `django-selenium-clean-1.0.0/django_selenium_clean/__init__.py`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.4/django_selenium_clean.egg-info/PKG-INFO` & `django-selenium-clean-1.0.0/django_selenium_clean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-selenium-clean
-Version: 0.3.4
+Version: 1.0.0
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/aptiko/django-selenium-clean
 Author: Antonis Christofides
 Author-email: antonis@djangodeployment.com
 License: BSD 3-Clause License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-selenium-clean-0.3.4/setup.py` & `django-selenium-clean-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,17 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Topic :: Software Development :: Testing",
     ],
     name="django-selenium-clean",
-    version="0.3.4",
+    version="1.0.0",
     license="BSD 3-Clause License",
     description="Write clean Selenium tests in Django",
     author="Antonis Christofides",
     author_email="antonis@djangodeployment.com",
     url="https://github.com/aptiko/django-selenium-clean",
     packages=find_packages(),
-    install_requires=["django>=2.2,<4", "selenium>=2.40,<4"],
+    install_requires=["django>=2.2,<4", "selenium>=3,<5"],
     test_suite="tests.tests",
 )
```

### Comparing `django-selenium-clean-0.3.4/tests/manage.py` & `django-selenium-clean-1.0.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.4/tests/settings.py` & `django-selenium-clean-1.0.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-selenium-clean-0.3.4/tests/tests.py` & `django-selenium-clean-1.0.0/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
             self.selenium.wait_until_n_windows(n=2, timeout=1)
 
         # Open a window and check again
         self.button_open_window.click()
         self.selenium.wait_until_n_windows(n=2, timeout=1)
 
         # Close the window
-        self.selenium.switch_to_window(self.selenium.window_handles[1])
+        self.selenium.switch_to.window(self.selenium.window_handles[1])
         self.selenium.close()
-        self.selenium.switch_to_window(self.selenium.window_handles[0])
+        self.selenium.switch_to.window(self.selenium.window_handles[0])
 
     def test_exists(self):
         self.selenium.get(self.live_server_url)
 
         # Element with id=togglable does not exist. Check that the various
         # waits and asserts are ok.
         self.togglable.wait_until_not_exists()
```

