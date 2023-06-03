# Comparing `tmp/openedx-django-pyfs-3.2.1.tar.gz` & `tmp/openedx-django-pyfs-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-django-pyfs-3.2.1.tar", last modified: Fri Jan 27 18:20:46 2023, max compression
+gzip compressed data, was "openedx-django-pyfs-3.3.0.tar", last modified: Sat Jun  3 12:11:10 2023, max compression
```

## Comparing `openedx-django-pyfs-3.2.1.tar` & `openedx-django-pyfs-3.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/djpyfs/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/djpyfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5933 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/djpyfs/djpyfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/djpyfs/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13103 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/djpyfs/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/example/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/example/example/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/example/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/example/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/example/sample/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/sample/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/sample/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/example/sample/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-01-27 18:20:46.000000 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-27 18:20:46.000000 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-27 18:20:46.000000 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-27 18:20:46.000000 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-27 18:20:46.000000 openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-27 18:20:46.915455 openedx-django-pyfs-3.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-01-27 18:20:46.919455 openedx-django-pyfs-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-01-27 18:20:43.000000 openedx-django-pyfs-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/djpyfs/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6183 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/djpyfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13272 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/example/example/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/example/sample/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/setup.py
```

### Comparing `openedx-django-pyfs-3.2.1/LICENSE` & `openedx-django-pyfs-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/PKG-INFO` & `openedx-django-pyfs-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: openedx-django-pyfs
-Version: 3.2.1
+Version: 3.3.0
 Summary: Django pyfilesystem integration
 Home-page: https://github.com/openedx/django-pyfs
 Author: Open edX
 Author-email: oscm@tcril.org
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -112,9 +111,7 @@
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/openedx-django-pyfs.svg
     :target: https://pypi.python.org/pypi/openedx-django-pyfs
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/openedx/django-pyfs.svg
     :target: https://github.com/openedx/django-pyfs/blob/master/LICENSE.txt
     :alt: License
-
-
```

### Comparing `openedx-django-pyfs-3.2.1/README.rst` & `openedx-django-pyfs-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/djpyfs/djpyfs.py` & `openedx-django-pyfs-3.3.0/djpyfs/djpyfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 task can garbage-collect those objects.
 """
 
 import os
 import os.path
 import types
 
-from boto.s3.connection import S3Connection
+import boto3
 from django.conf import settings
 from fs.osfs import OSFS
 from fs_s3fs import S3FS
 
 from .models import FSExpirations
 
 if hasattr(settings, 'DJFS'):
@@ -127,14 +127,15 @@
     key_id = DJFS_SETTINGS.get('aws_access_key_id', None)
     key_secret = DJFS_SETTINGS.get('aws_secret_access_key', None)
 
     fullpath = namespace
 
     if 'prefix' in DJFS_SETTINGS:
         fullpath = os.path.join(DJFS_SETTINGS['prefix'], fullpath)
+
     s3fs = S3FS(DJFS_SETTINGS['bucket'], fullpath, aws_secret_access_key=key_id, aws_access_key_id=key_secret)
 
     def get_s3_url(self, filename, timeout=60):  # pylint: disable=unused-argument
         """
         Patch method to returns a signed S3 url for the given filename
 
         Note that this will return a url whether or not the requested file
@@ -149,22 +150,34 @@
         Returns:
             str: A signed url to the requested file in S3
         """
         global S3CONN
 
         try:
             if not S3CONN:
-                S3CONN = S3Connection(aws_access_key_id=key_id, aws_secret_access_key=key_secret)
-            return S3CONN.generate_url(
-                timeout, 'GET', bucket=DJFS_SETTINGS['bucket'], key=os.path.join(fullpath, filename)
+                S3CONN = boto3.client('s3', aws_access_key_id=key_id, aws_secret_access_key=key_secret)
+
+            return S3CONN.generate_presigned_url(
+                "get_object",
+                Params={
+                    "Bucket": DJFS_SETTINGS['bucket'],
+                    "Key": os.path.join(fullpath, filename),
+                },
+                ExpiresIn=timeout
             )
+
         except Exception:  # pylint: disable=broad-except
             # Retry on error; typically, if the connection has timed out, but
             # the broad except covers all errors.
-            S3CONN = S3Connection(aws_access_key_id=key_id, aws_secret_access_key=key_secret)
+            S3CONN = boto3.client('s3', aws_access_key_id=key_id, aws_secret_access_key=key_secret)
 
-            return S3CONN.generate_url(
-                timeout, 'GET', bucket=DJFS_SETTINGS['bucket'], key=os.path.join(fullpath, filename)
+            return S3CONN.generate_presigned_url(
+                "get_object",
+                Params={
+                    "Bucket": DJFS_SETTINGS['bucket'],
+                    "Key": os.path.join(fullpath, filename),
+                },
+                ExpiresIn=timeout
             )
 
     s3fs = patch_fs(s3fs, namespace, get_s3_url)
     return s3fs
```

### Comparing `openedx-django-pyfs-3.2.1/djpyfs/models.py` & `openedx-django-pyfs-3.3.0/djpyfs/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/djpyfs/tests.py` & `openedx-django-pyfs-3.3.0/djpyfs/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Database models for django-pyfs
 """
 
 
 import os
 import shutil
 import unittest
-from unittest import mock
+from unittest.mock import patch
 
 import boto3
 from django.test import TestCase
 from django.utils import timezone
 from fs.memoryfs import MemoryFS
 from moto import mock_s3
 
@@ -300,15 +300,15 @@
         'aws_secret_access_key': 'bar',
         'bucket': 'test_bucket'
     }
 
     def setUp(self):
         super().setUp()
 
-        self.expected_url_prefix = (f"https://{djpyfs.DJFS_SETTINGS['bucket']}.s3.amazonaws.com:443/"
+        self.expected_url_prefix = (f"https://s3.amazonaws.com/{djpyfs.DJFS_SETTINGS['bucket']}/"
                                     f"{self.namespace}/{self.relative_path_to_test_file}")
 
         self._setUpS3()
 
     def _setUpS3(self):
         """setup class"""
 
@@ -319,20 +319,21 @@
         # Create our fake bucket in fake s3
         self.conn = boto3.resource('s3')
         self.conn.create_bucket(Bucket=djpyfs.DJFS_SETTINGS['bucket'])
 
     # This test is only relevant for S3. Generate some fake errors to make
     # sure we cover the retry code.
     def test_get_url_retry(self):
-        with mock.patch("boto.s3.connection.S3Connection.generate_url") as mock_exception:
-            mock_exception.side_effect = AttributeError("test mock exception")
-            fs = djpyfs.get_filesystem(self.namespace)
-
-            with self.assertRaises(AttributeError):
-                fs.get_url(self.relative_path_to_test_file).startswith(self.expected_url_prefix)
+        with patch('boto3.client') as mock_client:
+            mock_client.side_effect = AttributeError("Some attribute error occurred")
+            with patch.object(djpyfs.S3CONN, "generate_presigned_url") as mock_client:
+                    mock_client.side_effect = AttributeError("Some attribute error occurred")
+                    fs = djpyfs.get_filesystem(self.namespace)
+                    with self.assertRaises(AttributeError):
+                        fs.get_url(self.relative_path_to_test_file).startswith(self.expected_url_prefix)
 
     def tearDown(self):
         self.mock_s3.stop()
         super().tearDown()
 
 
 # pylint: disable=test-inherits-tests
@@ -350,11 +351,11 @@
         'bucket': 'test_bucket',
         'prefix': 'prefix'
     }
 
     def setUp(self):
         super().setUp()
 
-        self.expected_url_prefix = (f"https://{djpyfs.DJFS_SETTINGS['bucket']}.s3.amazonaws.com:443/"
+        self.expected_url_prefix = (f"https://s3.amazonaws.com/{djpyfs.DJFS_SETTINGS['bucket']}/"
                                     f"{djpyfs.DJFS_SETTINGS['prefix']}/{self.namespace}/"
                                     f"{self.relative_path_to_test_file}")
         self._setUpS3()
```

### Comparing `openedx-django-pyfs-3.2.1/example/example/settings.py` & `openedx-django-pyfs-3.3.0/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/example/example/urls.py` & `openedx-django-pyfs-3.3.0/example/example/urls.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/example/example/wsgi.py` & `openedx-django-pyfs-3.3.0/example/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/example/sample/views.py` & `openedx-django-pyfs-3.3.0/example/sample/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/PKG-INFO` & `openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: openedx-django-pyfs
-Version: 3.2.1
+Version: 3.3.0
 Summary: Django pyfilesystem integration
 Home-page: https://github.com/openedx/django-pyfs
 Author: Open edX
 Author-email: oscm@tcril.org
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -112,9 +111,7 @@
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/openedx-django-pyfs.svg
     :target: https://pypi.python.org/pypi/openedx-django-pyfs
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/openedx/django-pyfs.svg
     :target: https://github.com/openedx/django-pyfs/blob/master/LICENSE.txt
     :alt: License
-
-
```

### Comparing `openedx-django-pyfs-3.2.1/openedx_django_pyfs.egg-info/SOURCES.txt` & `openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/requirements/constraints.txt` & `openedx-django-pyfs-3.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.2.1/setup.py` & `openedx-django-pyfs-3.3.0/setup.py`

 * *Files identical despite different names*

