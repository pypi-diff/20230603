# Comparing `tmp/django_admin_buttons-0.2.4.tar.gz` & `tmp/django-admin-buttons-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_buttons-0.2.4.tar", last modified: Tue Sep 13 14:41:02 2022, max compression
+gzip compressed data, was "django-admin-buttons-0.2.5.tar", last modified: Sat Jun  3 12:38:57 2023, max compression
```

## Comparing `django_admin_buttons-0.2.4.tar` & `django-admin-buttons-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/
--rw-rw-r--   0 mina      (1000) mina      (1000)       70 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/MANIFEST.in
--rw-rw-r--   0 mina      (1000) mina      (1000)     2139 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/PKG-INFO
--rw-rw-r--   0 mina      (1000) mina      (1000)     1275 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/README.rst
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons/
--rw-rw-r--   0 mina      (1000) mina      (1000)      654 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/django_admin_buttons/admin_button.py
--rw-rw-r--   0 mina      (1000) mina      (1000)      503 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/django_admin_buttons/boot_django.py
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons/static/
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons/static/django_admin_buttons/
--rw-rw-r--   0 mina      (1000) mina      (1000)     1508 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/django_admin_buttons/static/django_admin_buttons/django_admin_buttons.js
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons/templates/
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons/templates/admin/
--rw-rw-r--   0 mina      (1000) mina      (1000)      333 2022-09-10 23:02:12.000000 django_admin_buttons-0.2.4/django_admin_buttons/templates/admin/change_list.html
-drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/
--rw-rw-r--   0 mina      (1000) mina      (1000)     2139 2022-09-13 14:41:02.000000 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/PKG-INFO
--rw-rw-r--   0 mina      (1000) mina      (1000)      475 2022-09-13 14:41:02.000000 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/SOURCES.txt
--rw-rw-r--   0 mina      (1000) mina      (1000)        1 2022-09-13 14:41:02.000000 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/dependency_links.txt
--rw-rw-r--   0 mina      (1000) mina      (1000)       12 2022-09-13 14:41:02.000000 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/requires.txt
--rw-rw-r--   0 mina      (1000) mina      (1000)       21 2022-09-13 14:41:02.000000 django_admin_buttons-0.2.4/django_admin_buttons.egg-info/top_level.txt
--rw-rw-r--   0 mina      (1000) mina      (1000)      321 2022-09-13 14:41:00.000000 django_admin_buttons-0.2.4/pyproject.toml
--rw-rw-r--   0 mina      (1000) mina      (1000)      834 2022-09-13 14:41:02.510050 django_admin_buttons-0.2.4/setup.cfg
--rw-rw-r--   0 mina      (1000) mina      (1000)      673 2022-09-13 14:41:00.000000 django_admin_buttons-0.2.4/setup.py
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.270748 django-admin-buttons-0.2.5/
+-rw-rw-r--   0 mina      (1000) mina      (1000)       70 2022-09-10 23:02:12.000000 django-admin-buttons-0.2.5/MANIFEST.in
+-rw-rw-r--   0 mina      (1000) mina      (1000)     2174 2023-06-03 12:38:57.274748 django-admin-buttons-0.2.5/PKG-INFO
+-rw-rw-r--   0 mina      (1000) mina      (1000)     1275 2022-09-10 23:02:12.000000 django-admin-buttons-0.2.5/README.rst
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.270748 django-admin-buttons-0.2.5/django_admin_buttons/
+-rw-rw-r--   0 mina      (1000) mina      (1000)      654 2022-09-10 23:02:12.000000 django-admin-buttons-0.2.5/django_admin_buttons/admin_button.py
+-rw-rw-r--   0 mina      (1000) mina      (1000)      503 2022-09-10 23:02:12.000000 django-admin-buttons-0.2.5/django_admin_buttons/boot_django.py
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.266748 django-admin-buttons-0.2.5/django_admin_buttons/static/
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.270748 django-admin-buttons-0.2.5/django_admin_buttons/static/django_admin_buttons/
+-rw-rw-r--   0 mina      (1000) mina      (1000)     1525 2023-06-03 12:37:51.000000 django-admin-buttons-0.2.5/django_admin_buttons/static/django_admin_buttons/django_admin_buttons.js
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.266748 django-admin-buttons-0.2.5/django_admin_buttons/templates/
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.270748 django-admin-buttons-0.2.5/django_admin_buttons/templates/admin/
+-rw-rw-r--   0 mina      (1000) mina      (1000)      333 2022-09-10 23:02:12.000000 django-admin-buttons-0.2.5/django_admin_buttons/templates/admin/change_list.html
+drwxrwxr-x   0 mina      (1000) mina      (1000)        0 2023-06-03 12:38:57.270748 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/
+-rw-rw-r--   0 mina      (1000) mina      (1000)     2174 2023-06-03 12:38:57.000000 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/PKG-INFO
+-rw-rw-r--   0 mina      (1000) mina      (1000)      475 2023-06-03 12:38:57.000000 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/SOURCES.txt
+-rw-rw-r--   0 mina      (1000) mina      (1000)        1 2023-06-03 12:38:57.000000 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/dependency_links.txt
+-rw-rw-r--   0 mina      (1000) mina      (1000)        7 2023-06-03 12:38:57.000000 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/requires.txt
+-rw-rw-r--   0 mina      (1000) mina      (1000)       21 2023-06-03 12:38:57.000000 django-admin-buttons-0.2.5/django_admin_buttons.egg-info/top_level.txt
+-rw-rw-r--   0 mina      (1000) mina      (1000)      321 2023-06-03 12:37:18.000000 django-admin-buttons-0.2.5/pyproject.toml
+-rw-rw-r--   0 mina      (1000) mina      (1000)      834 2023-06-03 12:38:57.274748 django-admin-buttons-0.2.5/setup.cfg
+-rw-rw-r--   0 mina      (1000) mina      (1000)      673 2023-06-03 12:37:29.000000 django-admin-buttons-0.2.5/setup.py
```

### Comparing `django_admin_buttons-0.2.4/PKG-INFO` & `django-admin-buttons-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: django_admin_buttons
-Version: 0.2.4
-Summary: Django admin button
+Name: django-admin-buttons
+Version: 0.2.5
+Summary: django-admin-buttons for the Django Admin.
 Home-page: https://github.com/minaaaatef/Django-Admin-Buttons
 Author: Mina Atef
-Author-email: mina.atef0@gmail.com
+Author-email: Mina Atef <mina.atef0@gmail.com>
 License: MIT
 Keywords: django,buttons,admin,actions
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+Provides-Extra: dev
 
 Django-Admin-Buttons
 ====================
 
 This package used to add a button functionality to the change list
 columns in the django admin, it uses the action methods used in the
 **ModelAdmin**\ 
@@ -69,9 +69,7 @@
        # register the function
        actions = [Test_function] 
        
        # create the function that displays the button
        @admin.display()
        def button(self, obj):
            return AdminActionButton(obj.id, 'this', disabled = False, Class='btn-primary', label=None).render()
-
-
```

### Comparing `django_admin_buttons-0.2.4/README.rst` & `django-admin-buttons-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `django_admin_buttons-0.2.4/django_admin_buttons/admin_button.py` & `django-admin-buttons-0.2.5/django_admin_buttons/admin_button.py`

 * *Files identical despite different names*

### Comparing `django_admin_buttons-0.2.4/django_admin_buttons/static/django_admin_buttons/django_admin_buttons.js` & `django-admin-buttons-0.2.5/django_admin_buttons/static/django_admin_buttons/django_admin_buttons.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     }
     return cookieValue;
 }
 
 function button_action(id, action) {
     form = document.createElement('form');
     form.setAttribute('method', 'post');
-    form.setAttribute('action', '?');
+    form.setAttribute('action', window.location.href);
 
     action_input = document.createElement('input');
     action_input.setAttribute('type', 'hidden');
     action_input.setAttribute('name', 'action');
     action_input.setAttribute('value', action);
     form.appendChild(action_input);
```

### Comparing `django_admin_buttons-0.2.4/django_admin_buttons.egg-info/PKG-INFO` & `django-admin-buttons-0.2.5/django_admin_buttons.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-admin-buttons
-Version: 0.2.4
-Summary: Django admin button
+Version: 0.2.5
+Summary: django-admin-buttons for the Django Admin.
 Home-page: https://github.com/minaaaatef/Django-Admin-Buttons
 Author: Mina Atef
-Author-email: mina.atef0@gmail.com
+Author-email: Mina Atef <mina.atef0@gmail.com>
 License: MIT
 Keywords: django,buttons,admin,actions
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+Provides-Extra: dev
 
 Django-Admin-Buttons
 ====================
 
 This package used to add a button functionality to the change list
 columns in the django admin, it uses the action methods used in the
 **ModelAdmin**\ 
@@ -69,9 +69,7 @@
        # register the function
        actions = [Test_function] 
        
        # create the function that displays the button
        @admin.display()
        def button(self, obj):
            return AdminActionButton(obj.id, 'this', disabled = False, Class='btn-primary', label=None).render()
-
-
```

### Comparing `django_admin_buttons-0.2.4/setup.cfg` & `django-admin-buttons-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-admin-button
-version = 0.2.4
+version = 0.2.5
 description = Django admin button
 long_description = file:README.rst
 url = https://github.com/minaaaatef/Django-Admin-Buttons
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

### Comparing `django_admin_buttons-0.2.4/setup.py` & `django-admin-buttons-0.2.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from glob import glob
 
 
 setup(
     name='django_admin_buttons',
-    version='0.2.4',
+    version='0.2.5',
     license='MIT',
     author="Mina Atef",
     author_email='mina.atef0@gmail.com',
     packages=['django_admin_buttons','django_admin_buttons.templates','django_admin_buttons.static'],
         data_files = [
         ('templates', glob('templates/*')), # files in source_dir only - not recursive
         ('static', glob('static/*')), # includes sub-folders - recursive
```

