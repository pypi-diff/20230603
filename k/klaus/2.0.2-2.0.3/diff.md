# Comparing `tmp/klaus-2.0.2.tar.gz` & `tmp/klaus-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaus-2.0.2.tar", last modified: Sun Sep 11 18:34:38 2022, max compression
+gzip compressed data, was "klaus-2.0.3.tar", last modified: Sat Jun  3 15:15:02 2023, max compression
```

## Comparing `klaus-2.0.2.tar` & `klaus-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,59 @@
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.474374 klaus-2.0.2/
--rw-r--r--   0 j          (501) staff       (20)     1130 2014-11-11 20:33:15.000000 klaus-2.0.2/LICENSE
--rw-r--r--   0 j          (501) staff       (20)       85 2018-11-10 16:15:28.000000 klaus-2.0.2/MANIFEST.in
--rw-r--r--   0 j          (501) staff       (20)     4854 2022-09-11 18:34:38.474238 klaus-2.0.2/PKG-INFO
--rw-r--r--   0 j          (501) staff       (20)     4151 2020-10-12 09:56:06.000000 klaus-2.0.2/README.rst
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.468995 klaus-2.0.2/klaus/
--rw-r--r--   0 j          (501) staff       (20)     9728 2022-09-11 18:33:45.000000 klaus-2.0.2/klaus/__init__.py
--rw-r--r--   0 j          (501) staff       (20)     4279 2022-08-20 09:51:05.000000 klaus-2.0.2/klaus/cli.py
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.470879 klaus-2.0.2/klaus/contrib/
--rw-r--r--   0 j          (501) staff       (20)        0 2014-11-11 20:33:14.000000 klaus-2.0.2/klaus/contrib/__init__.py
--rw-r--r--   0 j          (501) staff       (20)      789 2022-08-20 09:08:53.000000 klaus-2.0.2/klaus/contrib/app_args.py
--rw-r--r--   0 j          (501) staff       (20)      317 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/contrib/wsgi.py
--rw-r--r--   0 j          (501) staff       (20)      804 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/contrib/wsgi_autoreload.py
--rw-r--r--   0 j          (501) staff       (20)     1466 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/contrib/wsgi_autoreloading.py
--rw-r--r--   0 j          (501) staff       (20)     7559 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/ctagscache.py
--rw-r--r--   0 j          (501) staff       (20)     1404 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/ctagsutils.py
--rw-r--r--   0 j          (501) staff       (20)     2605 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/diff.py
--rw-r--r--   0 j          (501) staff       (20)     4728 2022-08-20 09:48:42.000000 klaus-2.0.2/klaus/highlighting.py
--rw-r--r--   0 j          (501) staff       (20)     1329 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/markup.py
--rw-r--r--   0 j          (501) staff       (20)    13781 2022-09-11 18:26:40.000000 klaus-2.0.2/klaus/repo.py
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.471578 klaus-2.0.2/klaus/static/
--rw-r--r--   0 j          (501) staff       (20)     2876 2014-11-11 20:33:14.000000 klaus-2.0.2/klaus/static/favicon.png
--rw-r--r--   0 j          (501) staff       (20)     9557 2019-07-06 10:39:06.000000 klaus-2.0.2/klaus/static/klaus.css
--rw-r--r--   0 j          (501) staff       (20)     1912 2016-04-12 10:52:50.000000 klaus-2.0.2/klaus/static/klaus.js
--rw-r--r--   0 j          (501) staff       (20)     3422 2015-09-11 15:16:21.000000 klaus-2.0.2/klaus/static/pygments.css
--rw-r--r--   0 j          (501) staff       (20)      201 2016-04-12 10:52:50.000000 klaus-2.0.2/klaus/static/robots.txt
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.473815 klaus-2.0.2/klaus/templates/
--rw-r--r--   0 j          (501) staff       (20)     1362 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/base.html
--rw-r--r--   0 j          (501) staff       (20)     1254 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/blame_blob.html
--rw-r--r--   0 j          (501) staff       (20)      448 2022-08-20 09:08:55.000000 klaus-2.0.2/klaus/templates/history.html
--rw-r--r--   0 j          (501) staff       (20)     2146 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/history.inc.html
--rw-r--r--   0 j          (501) staff       (20)      395 2022-08-20 09:08:55.000000 klaus-2.0.2/klaus/templates/index.html
--rw-r--r--   0 j          (501) staff       (20)     1887 2022-08-20 09:08:53.000000 klaus-2.0.2/klaus/templates/repo_list.html
--rw-r--r--   0 j          (501) staff       (20)      945 2017-06-08 13:17:08.000000 klaus-2.0.2/klaus/templates/skeleton.html
--rw-r--r--   0 j          (501) staff       (20)      503 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/submodule.html
--rw-r--r--   0 j          (501) staff       (20)      884 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/tree.inc.html
--rw-r--r--   0 j          (501) staff       (20)     1722 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/view_blob.html
--rw-r--r--   0 j          (501) staff       (20)     5966 2020-10-19 19:57:04.000000 klaus-2.0.2/klaus/templates/view_commit.html
--rw-r--r--   0 j          (501) staff       (20)     8721 2022-08-20 09:49:20.000000 klaus-2.0.2/klaus/utils.py
--rw-r--r--   0 j          (501) staff       (20)    18031 2022-09-11 18:26:40.000000 klaus-2.0.2/klaus/views.py
--rw-r--r--   0 j          (501) staff       (20)     1435 2022-08-20 09:08:53.000000 klaus-2.0.2/klaus.1
-drwxr-xr-x   0 j          (501) staff       (20)        0 2022-09-11 18:34:38.470377 klaus-2.0.2/klaus.egg-info/
--rw-r--r--   0 j          (501) staff       (20)     4854 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/PKG-INFO
--rw-r--r--   0 j          (501) staff       (20)     1014 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/SOURCES.txt
--rw-r--r--   0 j          (501) staff       (20)        1 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/dependency_links.txt
--rw-r--r--   0 j          (501) staff       (20)       41 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/entry_points.txt
--rw-r--r--   0 j          (501) staff       (20)        1 2015-06-24 22:26:37.000000 klaus-2.0.2/klaus.egg-info/not-zip-safe
--rw-r--r--   0 j          (501) staff       (20)      143 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/requires.txt
--rw-r--r--   0 j          (501) staff       (20)        6 2022-09-11 18:34:38.000000 klaus-2.0.2/klaus.egg-info/top_level.txt
--rw-r--r--   0 j          (501) staff       (20)       38 2022-09-11 18:34:38.474414 klaus-2.0.2/setup.cfg
--rw-r--r--   0 j          (501) staff       (20)     1709 2022-09-11 18:33:32.000000 klaus-2.0.2/setup.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.889720 klaus-2.0.3/
+-rw-r--r--   0 j          (501) wheel        (0)     1130 2023-06-03 15:11:57.000000 klaus-2.0.3/LICENSE
+-rw-r--r--   0 j          (501) wheel        (0)       85 2023-06-03 15:11:57.000000 klaus-2.0.3/MANIFEST.in
+-rw-r--r--   0 j          (501) wheel        (0)     4902 2023-06-03 15:15:02.889603 klaus-2.0.3/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     4151 2023-06-03 15:11:57.000000 klaus-2.0.3/README.rst
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.886407 klaus-2.0.3/klaus/
+-rw-r--r--   0 j          (501) wheel        (0)     9728 2023-06-03 15:14:33.000000 klaus-2.0.3/klaus/__init__.py
+-rw-r--r--   0 j          (501) wheel        (0)     4279 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/cli.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.887559 klaus-2.0.3/klaus/contrib/
+-rw-r--r--   0 j          (501) wheel        (0)        0 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/__init__.py
+-rw-r--r--   0 j          (501) wheel        (0)      789 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/app_args.py
+-rw-r--r--   0 j          (501) wheel        (0)      317 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi.py
+-rw-r--r--   0 j          (501) wheel        (0)      804 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi_autoreload.py
+-rw-r--r--   0 j          (501) wheel        (0)     1466 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi_autoreloading.py
+-rw-r--r--   0 j          (501) wheel        (0)     7559 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/ctagscache.py
+-rw-r--r--   0 j          (501) wheel        (0)     1404 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/ctagsutils.py
+-rw-r--r--   0 j          (501) wheel        (0)     2605 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/diff.py
+-rw-r--r--   0 j          (501) wheel        (0)     4728 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/highlighting.py
+-rw-r--r--   0 j          (501) wheel        (0)     1329 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/markup.py
+-rw-r--r--   0 j          (501) wheel        (0)    14878 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/repo.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.888007 klaus-2.0.3/klaus/static/
+-rw-r--r--   0 j          (501) wheel        (0)     2876 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/favicon.png
+-rw-r--r--   0 j          (501) wheel        (0)     9557 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/klaus.css
+-rw-r--r--   0 j          (501) wheel        (0)     1912 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/klaus.js
+-rw-r--r--   0 j          (501) wheel        (0)     3422 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/pygments.css
+-rw-r--r--   0 j          (501) wheel        (0)      201 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/robots.txt
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.888957 klaus-2.0.3/klaus/templates/
+-rw-r--r--   0 j          (501) wheel        (0)     1362 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/base.html
+-rw-r--r--   0 j          (501) wheel        (0)     1254 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/blame_blob.html
+-rw-r--r--   0 j          (501) wheel        (0)      448 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/history.html
+-rw-r--r--   0 j          (501) wheel        (0)     2146 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/history.inc.html
+-rw-r--r--   0 j          (501) wheel        (0)      395 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/index.html
+-rw-r--r--   0 j          (501) wheel        (0)     1887 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/repo_list.html
+-rw-r--r--   0 j          (501) wheel        (0)      945 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/skeleton.html
+-rw-r--r--   0 j          (501) wheel        (0)      503 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/submodule.html
+-rw-r--r--   0 j          (501) wheel        (0)      884 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/tree.inc.html
+-rw-r--r--   0 j          (501) wheel        (0)     1722 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/view_blob.html
+-rw-r--r--   0 j          (501) wheel        (0)     5966 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/view_commit.html
+-rw-r--r--   0 j          (501) wheel        (0)     8779 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/utils.py
+-rw-r--r--   0 j          (501) wheel        (0)    18137 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/views.py
+-rw-r--r--   0 j          (501) wheel        (0)     1435 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus.1
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.887125 klaus-2.0.3/klaus.egg-info/
+-rw-r--r--   0 j          (501) wheel        (0)     4902 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     1156 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/SOURCES.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/dependency_links.txt
+-rw-r--r--   0 j          (501) wheel        (0)       41 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/entry_points.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/not-zip-safe
+-rw-r--r--   0 j          (501) wheel        (0)      143 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/requires.txt
+-rw-r--r--   0 j          (501) wheel        (0)        6 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/top_level.txt
+-rw-r--r--   0 j          (501) wheel        (0)       81 2023-06-03 15:11:57.000000 klaus-2.0.3/pyproject.toml
+-rw-r--r--   0 j          (501) wheel        (0)       38 2023-06-03 15:15:02.889749 klaus-2.0.3/setup.cfg
+-rw-r--r--   0 j          (501) wheel        (0)     1756 2023-06-03 15:14:26.000000 klaus-2.0.3/setup.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.889465 klaus-2.0.3/tests/
+-rw-r--r--   0 j          (501) wheel        (0)     1011 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_blame.py
+-rw-r--r--   0 j          (501) wheel        (0)     4552 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_contrib.py
+-rw-r--r--   0 j          (501) wheel        (0)     5937 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_make_app.py
+-rw-r--r--   0 j          (501) wheel        (0)     1095 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_manpage.py
+-rw-r--r--   0 j          (501) wheel        (0)     1222 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_utils.py
+-rw-r--r--   0 j          (501) wheel        (0)     2906 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_views.py
```

### Comparing `klaus-2.0.2/LICENSE` & `klaus-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/PKG-INFO` & `klaus-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: klaus
-Version: 2.0.2
+Version: 2.0.3
 Summary: The first Git web viewer that Just Works™.
 Home-page: https://github.com/jonashaag/klaus
 Author: Jonas Haag
 Author-email: jonas@lophus.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 |travis-badge| |gitter-badge|
 
 .. |travis-badge| image:: https://travis-ci.org/jonashaag/klaus.svg?branch=master
     :target: https://travis-ci.org/jonashaag/klaus
```

### Comparing `klaus-2.0.2/README.rst` & `klaus-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/__init__.py` & `klaus-2.0.3/klaus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import httpauth
 import dulwich.web
 from dulwich.errors import NotGitRepository
 from klaus import views, utils
 from klaus.repo import FancyRepo, InvalidRepo
 
 
-KLAUS_VERSION = utils.guess_git_revision() or "2.0.2"
+KLAUS_VERSION = utils.guess_git_revision() or "2.0.3"
 
 
 class Klaus(flask.Flask):
     jinja_options = {
         "extensions": [] if jinja2_autoescape_builtin else ["jinja2.ext.autoescape"],
         "undefined": jinja2.StrictUndefined,
     }
```

### Comparing `klaus-2.0.2/klaus/cli.py` & `klaus-2.0.3/klaus/cli.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/contrib/app_args.py` & `klaus-2.0.3/klaus/contrib/app_args.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/contrib/wsgi_autoreload.py` & `klaus-2.0.3/klaus/contrib/wsgi_autoreload.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/contrib/wsgi_autoreloading.py` & `klaus-2.0.3/klaus/contrib/wsgi_autoreloading.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/ctagscache.py` & `klaus-2.0.3/klaus/ctagscache.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/ctagsutils.py` & `klaus-2.0.3/klaus/ctagsutils.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/diff.py` & `klaus-2.0.3/klaus/diff.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/highlighting.py` & `klaus-2.0.3/klaus/highlighting.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/markup.py` & `klaus-2.0.3/klaus/markup.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/repo.py` & `klaus-2.0.3/klaus/repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import os
+import functools
 import io
+import os
 import stat
 import subprocess
+import threading
 
 from dulwich.objects import S_ISGITLINK
 from dulwich.object_store import tree_lookup_path
 from dulwich.objects import Blob
 from dulwich.errors import NotTreeError
 import dulwich, dulwich.patch
 
@@ -34,129 +36,159 @@
     data, old_validator = _cache.get(key, (None, NOT_SET))
     if old_validator != validator:
         data = producer()
     _cache[key] = (data, validator)
     return data
 
 
-class FancyRepo(dulwich.repo.Repo):
+def synchronized(func, lock=threading.RLock()):
+    @functools.wraps(func)
+    def synchronized_func(*args, **kwargs):
+        with lock:
+            return func(*args, **kwargs)
+    return synchronized_func
+
+
+class FancyRepo(object):
     """A wrapper around Dulwich's Repo that adds some helper methods."""
 
     def __init__(self, path, namespace):
-        super(FancyRepo, self).__init__(path)
+        self.dulwich_repo = dulwich.repo.Repo(path)
         self.namespace = namespace
 
     @property
+    def path(self):
+        return self.dulwich_repo.path
+
+    @property
     def name(self):
         return repo_human_name(self.path)
 
     @property
     def namespaced_name(self):
         if self.namespace:
             return "~{}/{}".format(self.namespace, self.name)
         else:
             return self.name
 
+    @synchronized
+    def __getitem__(self, key):
+        return self.dulwich_repo[key]
+
     # TODO: factor out stuff into dulwich
+    @synchronized
     def get_last_updated_at(self):
-        """Get datetime of last commit to this repository."""
-        # Cache result to speed up repo_list.html template.
-        # If self.get_refs() has changed, we should invalidate the cache.
-        all_refs = self.get_refs()
-        return cached_call(
-            key=(id(self), "get_last_updated_at"),
-            validator=all_refs,
-            producer=lambda: self._get_last_updated_at(all_refs),
-        )
+        """Get datetime of last commit to this repository.
 
-    def _get_last_updated_at(self, all_refs):
-        resolveable_refs = []
-        for ref_hash in all_refs:
+        Caches the result to speed up the repo_list page.
+        Cache is invalidated if one of the ref targets changes,
+        eg. a new commit has been made and 'refs/heads/master' was changed.
+        """
+        def _get_commit_time_cached(ref_id):
+            return cached_call(
+                key=(ref_id, "_get_commit_time"),
+                validator=None,
+                producer=lambda: _get_commit_time(ref_id),
+            )
+
+        def _get_commit_time(ref_id):
             try:
-                resolveable_refs.append(self[ref_hash])
-            except KeyError:
-                # Whoops. The ref points at a non-existant object
-                pass
-        resolveable_refs.sort(
-            key=lambda obj: getattr(obj, "commit_time", float("-inf")), reverse=True
-        )
-        for ref in resolveable_refs:
-            # Find the latest ref that has a commit_time; tags do not
-            # have a commit time
-            if hasattr(ref, "commit_time"):
-                return ref.commit_time
-        return None
+                return self[ref_id].commit_time
+            except (KeyError, AttributeError):
+                # Missing or non-commit object
+                return None
+
+        max_refs = 1000
+        if len(self.dulwich_repo.refs.keys()) > max_refs:
+            # If we have too many refs, look at the branches only. (And HEAD, see below.)
+            base = b"refs/heads"
+        else:
+            base = None
+        all_ids = list(self.dulwich_repo.refs.as_dict(base).values())
+        # If we still have too many refs, keep only some.
+        if len(all_ids) > max_refs:
+            all_ids = sorted(all_ids)[:max_refs]
+        # Always add HEAD.
+        try:
+            all_ids.append(self.dulwich_repo.refs[b"HEAD"])
+        except KeyError:
+            pass
+
+        commit_times = filter(None, map(_get_commit_time_cached, all_ids))
+        try:
+            return max(commit_times)
+        except ValueError:
+            # Python 2 does not support max(..., default=)
+            return None
 
     @property
+    @synchronized
     def cloneurl(self):
         """Retrieve the gitweb notion of the public clone URL of this repo."""
-        f = self.get_named_file("cloneurl")
+        f = self.dulwich_repo.get_named_file("cloneurl")
         if f is not None:
             return force_unicode(f.read())
-        c = self.get_config()
+        c = self.dulwich_repo.get_config()
         try:
             return force_unicode(c.get(b"gitweb", b"url"))
         except KeyError:
             return None
 
+    @synchronized
     def get_description(self):
         """Like Dulwich's `get_description`, but returns None if the file
         contains Git's default text "Unnamed repository[...]".
         """
         # Cache result to speed up repo_list.html template.
         # If description file mtime has changed, we should invalidate the cache.
-        description_file = os.path.join(self._controldir, "description")
+        description_file = os.path.join(self.dulwich_repo._controldir, "description")
         try:
             description_mtime = os.stat(description_file).st_mtime
         except OSError:
             description_mtime = None
 
         return cached_call(
             key=(id(self), "get_description"),
             validator=description_mtime,
             producer=self._get_description,
         )
 
     def _get_description(self):
-        description = super(FancyRepo, self).get_description()
+        description = self.dulwich_repo.get_description()
         if description:
             description = force_unicode(description)
             if not description.startswith("Unnamed repository;"):
                 return force_unicode(description)
 
+    @synchronized
     def get_commit(self, rev):
         """Get commit object identified by `rev` (SHA or branch or tag name)."""
         for prefix in ["refs/heads/", "refs/tags/", ""]:
             key = prefix + rev
             try:
                 obj = self[encode_for_git(key)]
                 if isinstance(obj, dulwich.objects.Tag):
                     obj = self[obj.object[1]]
                 return obj
             except KeyError:
                 pass
         raise KeyError(rev)
 
+    @synchronized
     def get_default_branch(self):
         """Tries to guess the default repo branch name."""
         for candidate in ["master", "main", "trunk", "default", "gh-pages"]:
             try:
                 self.get_commit(candidate)
                 return candidate
             except InaccessibleRef:
                 pass
-        for name in self.get_branch_names():
-            try:
-                self.get_commit(name)
-                return name
-            except InaccessibleRef:
-                pass
-        else:
-            return None
+        return None
 
+    @synchronized
     def get_ref_names_ordered_by_last_commit(self, prefix, exclude=None):
         """Return a list of ref names that begin with `prefix`, ordered by the
         time they have been committed to last.
         """
 
         def get_commit_time(refname):
             try:
@@ -165,36 +197,40 @@
                 # Default to 0, i.e. sorting refs that point at non-existant
                 # objects last.
                 return 0
             if isinstance(obj, dulwich.objects.Tag):
                 return obj.tag_time
             return obj.commit_time
 
-        refs = self.refs.as_dict(encode_for_git(prefix))
+        refs = self.dulwich_repo.refs.as_dict(encode_for_git(prefix))
         if exclude:
             refs.pop(prefix + exclude, None)
         sorted_names = sorted(refs.keys(), key=get_commit_time, reverse=True)
         return [decode_from_git(ref) for ref in sorted_names]
 
+    @synchronized
     def get_branch_names(self, exclude=None):
         """Return a list of branch names of this repo, ordered by the time they
         have been committed to last.
         """
         return self.get_ref_names_ordered_by_last_commit("refs/heads", exclude)
 
+    @synchronized
     def get_tag_names(self):
         """Return a list of tag names of this repo, ordered by creation time."""
         return self.get_ref_names_ordered_by_last_commit("refs/tags")
 
+    @synchronized
     def get_tag_and_branch_shas(self):
         """Return a list of SHAs of all tags and branches."""
-        tag_shas = self.refs.as_dict(b"refs/tags/").values()
-        branch_shas = self.refs.as_dict(b"refs/heads/").values()
+        tag_shas = self.dulwich_repo.refs.as_dict(b"refs/tags/").values()
+        branch_shas = self.dulwich_repo.refs.as_dict(b"refs/heads/").values()
         return set(tag_shas) | set(branch_shas)
 
+    @synchronized
     def history(self, commit, path=None, max_commits=None, skip=0):
         """Return a list of all commits that affected `path`, starting at branch
         or commit `commit`. `skip` can be used for pagination, `max_commits`
         to limit the number of commits returned.
 
         Similar to `git log [branch/commit] [--skip skip] [-n max_commits]`.
         """
@@ -214,39 +250,42 @@
         if path:
             cmd.extend(["--", path])
 
         output = subprocess.check_output(cmd, cwd=os.path.abspath(self.path))
         sha1_sums = output.strip().split(b"\n")
         return [self[sha1] for sha1 in sha1_sums]
 
+    @synchronized
     def blame(self, commit, path):
         """Return a 'git blame' list for the file at `path`: For each line in
         the file, the list contains the commit that last changed that line.
         """
         # XXX see comment in `.history()`
         cmd = ["git", "blame", "-ls", "--root", decode_from_git(commit.id), "--", path]
         output = subprocess.check_output(cmd, cwd=os.path.abspath(self.path))
         sha1_sums = [line[:40] for line in output.strip().split(b"\n") if line]
         return [
             None if self[sha1] is None else decode_from_git(self[sha1].id)
             for sha1 in sha1_sums
         ]
 
+    @synchronized
     def get_blob_or_tree(self, commit, path):
         """Return the Git tree or blob object for `path` at `commit`."""
         try:
             (mode, oid) = tree_lookup_path(
-                self.__getitem__, commit.tree, encode_for_git(path)
+                self.dulwich_repo.__getitem__, commit.tree, encode_for_git(path)
             )
         except NotTreeError:
             # Some part of the path was a file where a folder was expected.
             # Example: path="/path/to/foo.txt" but "to" is a file in "/path".
             raise KeyError
         return self[oid]
 
+    @synchronized
     def listdir(self, commit, path):
         """Return a list of submodules, directories and files in given
         directory: Lists of (link name, target path) tuples.
         """
         submodules, dirs, files = [], [], []
         for entry_rel in self.get_blob_or_tree(commit, path).items():
             # entry_rel: Entry('foo.txt', ...)
@@ -257,46 +296,48 @@
             if S_ISGITLINK(entry_abs.mode):
                 submodules.append(item)
             elif stat.S_ISDIR(entry_abs.mode):
                 dirs.append(item)
             else:
                 files.append(item)
 
-        keyfunc = lambda tpl: tpl[0].lower()
+        def keyfunc(tpl):
+            return tpl[0].lower()
         submodules.sort(key=keyfunc)
         files.sort(key=keyfunc)
         dirs.sort(key=keyfunc)
 
         if path:
             dirs.insert(0, ("..", parent_directory(path)))
 
         return {"submodules": submodules, "dirs": dirs, "files": files}
 
+    @synchronized
     def commit_diff(self, commit):
         """Return the list of changes introduced by `commit`."""
         from klaus.utils import guess_is_binary
 
         if commit.parents:
             parent_tree = self[commit.parents[0]].tree
         else:
             parent_tree = None
 
         summary = {"nfiles": 0, "nadditions": 0, "ndeletions": 0}
         file_changes = []  # the changes in detail
 
-        dulwich_changes = self.object_store.tree_changes(parent_tree, commit.tree)
+        dulwich_changes = self.dulwich_repo.object_store.tree_changes(parent_tree, commit.tree)
         for (oldpath, newpath), (oldmode, newmode), (oldsha, newsha) in dulwich_changes:
             summary["nfiles"] += 1
             try:
-                oldblob = self.object_store[oldsha] if oldsha else Blob.from_string(b"")
+                oldblob = self.dulwich_repo.object_store[oldsha] if oldsha else Blob.from_string(b"")
             except KeyError:
                 # probably related to submodules; Dulwich will handle that.
                 oldblob = Blob.from_string(b"")
             try:
-                newblob = self.object_store[newsha] if newsha else Blob.from_string(b"")
+                newblob = self.dulwich_repo.object_store[newsha] if newsha else Blob.from_string(b"")
             except KeyError:
                 # probably related to submodules; Dulwich will handle that.
                 newblob = Blob.from_string(b"")
 
             # Check for binary files -- can't show diffs for these
             if guess_is_binary(newblob) or guess_is_binary(oldblob):
                 file_changes.append(
@@ -322,22 +363,23 @@
             }
             summary["nadditions"] += additions
             summary["ndeletions"] += deletions
             file_changes.append(change)
 
         return summary, file_changes
 
+    @synchronized
     def raw_commit_diff(self, commit):
         if commit.parents:
             parent_tree = self[commit.parents[0]].tree
         else:
             parent_tree = None
         bytesio = io.BytesIO()
         dulwich.patch.write_tree_diff(
-            bytesio, self.object_store, parent_tree, commit.tree
+            bytesio, self.dulwich_repo.object_store, parent_tree, commit.tree
         )
         return bytesio.getvalue()
 
     def freeze(self):
         return FrozenFancyRepo(self)
```

### Comparing `klaus-2.0.2/klaus/static/favicon.png` & `klaus-2.0.3/klaus/static/favicon.png`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/static/klaus.css` & `klaus-2.0.3/klaus/static/klaus.css`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/static/klaus.js` & `klaus-2.0.3/klaus/static/klaus.js`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/static/pygments.css` & `klaus-2.0.3/klaus/static/pygments.css`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/base.html` & `klaus-2.0.3/klaus/templates/base.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/blame_blob.html` & `klaus-2.0.3/klaus/templates/blame_blob.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/history.inc.html` & `klaus-2.0.3/klaus/templates/history.inc.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/repo_list.html` & `klaus-2.0.3/klaus/templates/repo_list.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/skeleton.html` & `klaus-2.0.3/klaus/templates/skeleton.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/tree.inc.html` & `klaus-2.0.3/klaus/templates/tree.inc.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/view_blob.html` & `klaus-2.0.3/klaus/templates/view_blob.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/templates/view_commit.html` & `klaus-2.0.3/klaus/templates/view_commit.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus/utils.py` & `klaus-2.0.3/klaus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,31 +139,33 @@
         # Python < 3
         text_type = unicode
     except NameError:
         text_type = str
     if isinstance(s, text_type):
         return s
 
-    last_exc = None
     # Try some default encodings:
     try:
         return s.decode("utf-8")
-    except UnicodeDecodeError as exc:
+    except UnicodeDecodeError:
         pass
 
     try:
         return s.decode(locale.getpreferredencoding())
     except UnicodeDecodeError:
         pass
 
     if chardet is not None:
         # Try chardet, if available
         encoding = chardet.detect(s)["encoding"]
         if encoding is not None:
-            return s.decode(encoding)
+            try:
+                return s.decode(encoding, 'replace')
+            except LookupError:
+                pass
 
     return s.decode('latin1', 'replace')
 
 
 def extract_author_name(email):
     """Extract the name from an email address --
     >>> extract_author_name("John <john@example.com>")
```

### Comparing `klaus-2.0.2/klaus/views.py` & `klaus-2.0.3/klaus/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,19 @@
         invalid_repos = [
             r
             for r in invalid_repos
             if search_query.lower() in r.namespaced_name.lower()
         ]
 
     if order_by == "name":
-        sort_key = lambda repo: repo.namespaced_name
+        def sort_key(repo):
+            return repo.namespaced_name
     else:
-        sort_key = lambda repo: (
-            -(repo.fast_get_last_updated_at() or -1),
-            repo.namespaced_name,
-        )
+        def sort_key(repo):
+            return -(repo.fast_get_last_updated_at() or -1), repo.namespaced_name
 
     repos = sorted(repos, key=sort_key)
     invalid_repos = sorted(invalid_repos, key=lambda repo: repo.namespaced_name)
 
     return render_template(
         "repo_list.html",
         repos=repos,
@@ -106,15 +105,19 @@
         repo = current_app.valid_repos[repo_key]
     except KeyError:
         raise NotFound("No such repository %r" % repo)
 
     if rev is None:
         rev = repo.get_default_branch()
         if rev is None:
-            raise NotFound("Empty repository")
+            rev = "HEAD"
+            try:
+                repo.get_commit("HEAD")
+            except KeyError:
+                raise NotFound("No commits yet")
 
     i = len(rev)
     while i > 0:
         try:
             commit = repo.get_commit(rev[:i])
             path = rev[i:].strip("/")
             rev = rev[:i]
```

### Comparing `klaus-2.0.2/klaus.1` & `klaus-2.0.3/klaus.1`

 * *Files identical despite different names*

### Comparing `klaus-2.0.2/klaus.egg-info/PKG-INFO` & `klaus-2.0.3/klaus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: klaus
-Version: 2.0.2
+Version: 2.0.3
 Summary: The first Git web viewer that Just Works™.
 Home-page: https://github.com/jonashaag/klaus
 Author: Jonas Haag
 Author-email: jonas@lophus.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 |travis-badge| |gitter-badge|
 
 .. |travis-badge| image:: https://travis-ci.org/jonashaag/klaus.svg?branch=master
     :target: https://travis-ci.org/jonashaag/klaus
```

### Comparing `klaus-2.0.2/klaus.egg-info/SOURCES.txt` & `klaus-2.0.3/klaus.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 klaus.1
+pyproject.toml
 setup.py
 klaus/__init__.py
 klaus/cli.py
 klaus/ctagscache.py
 klaus/ctagsutils.py
 klaus/diff.py
 klaus/highlighting.py
@@ -36,8 +37,14 @@
 klaus/templates/history.inc.html
 klaus/templates/index.html
 klaus/templates/repo_list.html
 klaus/templates/skeleton.html
 klaus/templates/submodule.html
 klaus/templates/tree.inc.html
 klaus/templates/view_blob.html
-klaus/templates/view_commit.html
+klaus/templates/view_commit.html
+tests/test_blame.py
+tests/test_contrib.py
+tests/test_make_app.py
+tests/test_manpage.py
+tests/test_utils.py
+tests/test_views.py
```

### Comparing `klaus-2.0.2/setup.py` & `klaus-2.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "humanize",
     'dulwich>=0.19.3;python_version>="3.5"',
     'dulwich>=0.19.3,<0.20;python_version<"3.5"',
 ]
 
 setup(
     name="klaus",
-    version="2.0.2",
+    version="2.0.3",
     author="Jonas Haag",
     author_email="jonas@lophus.org",
     packages=["klaus", "klaus.contrib"],
     include_package_data=True,
     zip_safe=False,
     url="https://github.com/jonashaag/klaus",
     description="The first Git web viewer that Just Works™.",
@@ -44,13 +44,14 @@
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Software Development :: Version Control",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
     ],
     install_requires=requires,
     entry_points={
         "console_scripts": ["klaus=klaus.cli:main"],
     },
 )
```

