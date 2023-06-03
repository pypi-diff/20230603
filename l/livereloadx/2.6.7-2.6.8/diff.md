# Comparing `tmp/livereloadx-2.6.7.tar.gz` & `tmp/livereloadx-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livereloadx-2.6.7.tar", last modified: Sat Jun  3 05:09:05 2023, max compression
+gzip compressed data, was "livereloadx-2.6.8.tar", last modified: Sat Jun  3 05:19:36 2023, max compression
```

## Comparing `livereloadx-2.6.7.tar` & `livereloadx-2.6.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.125701 livereloadx-2.6.7/
--rw-r--r--   0 tuanchau   (503) staff       (20)     1510 2023-06-03 04:52:10.000000 livereloadx-2.6.7/LICENSE
--rw-r--r--   0 tuanchau   (503) staff       (20)       76 2023-06-03 04:52:10.000000 livereloadx-2.6.7/MANIFEST.in
--rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:09:05.125778 livereloadx-2.6.7/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      987 2023-06-03 05:05:06.000000 livereloadx-2.6.7/README.md
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.122762 livereloadx-2.6.7/livereload/
--rw-r--r--   0 tuanchau   (503) staff       (20)      366 2023-06-03 05:08:39.000000 livereloadx-2.6.7/livereload/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1381 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/cli.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     6721 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/handlers.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.118238 livereloadx-2.6.7/livereload/management/
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.123288 livereloadx-2.6.7/livereload/management/commands/
--rw-r--r--   0 tuanchau   (503) staff       (20)        0 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/management/commands/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1720 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/management/commands/livereload.py
--rw-r--r--   0 tuanchau   (503) staff       (20)    12650 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/server.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.123563 livereloadx-2.6.7/livereload/vendors/
--rw-r--r--   0 tuanchau   (503) staff       (20)    37411 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/vendors/livereload.js
--rw-r--r--   0 tuanchau   (503) staff       (20)     7410 2023-06-03 04:52:10.000000 livereloadx-2.6.7/livereload/watcher.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.125211 livereloadx-2.6.7/livereloadx.egg-info/
--rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      510 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/SOURCES.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/dependency_links.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       51 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/entry_points.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        8 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/requires.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       11 2023-06-03 05:09:05.000000 livereloadx-2.6.7/livereloadx.egg-info/top_level.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       74 2023-06-03 05:09:05.126178 livereloadx-2.6.7/setup.cfg
--rw-r--r--   0 tuanchau   (503) staff       (20)     2024 2023-06-03 05:04:02.000000 livereloadx-2.6.7/setup.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:09:05.125470 livereloadx-2.6.7/tests/
--rw-r--r--   0 tuanchau   (503) staff       (20)     4939 2023-06-03 04:52:10.000000 livereloadx-2.6.7/tests/test_watcher.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.302477 livereloadx-2.6.8/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1510 2023-06-03 04:52:10.000000 livereloadx-2.6.8/LICENSE
+-rw-r--r--   0 tuanchau   (503) staff       (20)       76 2023-06-03 04:52:10.000000 livereloadx-2.6.8/MANIFEST.in
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:19:36.302561 livereloadx-2.6.8/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      987 2023-06-03 05:05:06.000000 livereloadx-2.6.8/README.md
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.298585 livereloadx-2.6.8/livereload/
+-rw-r--r--   0 tuanchau   (503) staff       (20)      366 2023-06-03 05:19:25.000000 livereloadx-2.6.8/livereload/__init__.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1381 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/cli.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     6725 2023-06-03 05:19:15.000000 livereloadx-2.6.8/livereload/handlers.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.294805 livereloadx-2.6.8/livereload/management/
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.299304 livereloadx-2.6.8/livereload/management/commands/
+-rw-r--r--   0 tuanchau   (503) staff       (20)        0 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/management/commands/__init__.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1720 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/management/commands/livereload.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)    12650 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/server.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.299635 livereloadx-2.6.8/livereload/vendors/
+-rw-r--r--   0 tuanchau   (503) staff       (20)    37411 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/vendors/livereload.js
+-rw-r--r--   0 tuanchau   (503) staff       (20)     7410 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/watcher.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.301832 livereloadx-2.6.8/livereloadx.egg-info/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      510 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/SOURCES.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/dependency_links.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       51 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/entry_points.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        8 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/requires.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       11 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/top_level.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       74 2023-06-03 05:19:36.302877 livereloadx-2.6.8/setup.cfg
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2024 2023-06-03 05:04:02.000000 livereloadx-2.6.8/setup.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.302171 livereloadx-2.6.8/tests/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     4939 2023-06-03 04:52:10.000000 livereloadx-2.6.8/tests/test_watcher.py
```

### Comparing `livereloadx-2.6.7/LICENSE` & `livereloadx-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/PKG-INFO` & `livereloadx-2.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livereloadx
-Version: 2.6.7
+Version: 2.6.8
 Summary: Python LiveReload is an awesome tool for web developers
 Home-page: https://github.com/lepture/python-livereload
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `livereloadx-2.6.7/README.md` & `livereloadx-2.6.8/README.md`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereload/cli.py` & `livereloadx-2.6.8/livereload/cli.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereload/handlers.py` & `livereloadx-2.6.8/livereload/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             ioloop.PeriodicCallback(cls.poll_tasks, 800).start()
 
     @classmethod
     def poll_tasks(cls):
         filepath, delay = cls.watcher.examine()
         if not filepath or delay == 'forever' or not cls.waiters:
             return
-        reload_time = DEFAULT_RELOAD_TIME
+        reload_time = cls.DEFAULT_RELOAD_TIME
 
         if delay:
             reload_time = max(3 - delay, 1)
         if filepath == '__livereload__':
             reload_time = 0
 
         if time.time() - cls._last_reload_time < reload_time:
```

### Comparing `livereloadx-2.6.7/livereload/management/commands/livereload.py` & `livereloadx-2.6.8/livereload/management/commands/livereload.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereload/server.py` & `livereloadx-2.6.8/livereload/server.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereload/vendors/livereload.js` & `livereloadx-2.6.8/livereload/vendors/livereload.js`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereload/watcher.py` & `livereloadx-2.6.8/livereload/watcher.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/livereloadx.egg-info/PKG-INFO` & `livereloadx-2.6.8/livereloadx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livereloadx
-Version: 2.6.7
+Version: 2.6.8
 Summary: Python LiveReload is an awesome tool for web developers
 Home-page: https://github.com/lepture/python-livereload
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `livereloadx-2.6.7/setup.py` & `livereloadx-2.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.7/tests/test_watcher.py` & `livereloadx-2.6.8/tests/test_watcher.py`

 * *Files identical despite different names*

