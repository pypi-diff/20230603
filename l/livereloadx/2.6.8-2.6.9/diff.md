# Comparing `tmp/livereloadx-2.6.8.tar.gz` & `tmp/livereloadx-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livereloadx-2.6.8.tar", last modified: Sat Jun  3 05:19:36 2023, max compression
+gzip compressed data, was "livereloadx-2.6.9.tar", last modified: Sat Jun  3 08:11:56 2023, max compression
```

## Comparing `livereloadx-2.6.8.tar` & `livereloadx-2.6.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.302477 livereloadx-2.6.8/
--rw-r--r--   0 tuanchau   (503) staff       (20)     1510 2023-06-03 04:52:10.000000 livereloadx-2.6.8/LICENSE
--rw-r--r--   0 tuanchau   (503) staff       (20)       76 2023-06-03 04:52:10.000000 livereloadx-2.6.8/MANIFEST.in
--rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:19:36.302561 livereloadx-2.6.8/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      987 2023-06-03 05:05:06.000000 livereloadx-2.6.8/README.md
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.298585 livereloadx-2.6.8/livereload/
--rw-r--r--   0 tuanchau   (503) staff       (20)      366 2023-06-03 05:19:25.000000 livereloadx-2.6.8/livereload/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1381 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/cli.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     6725 2023-06-03 05:19:15.000000 livereloadx-2.6.8/livereload/handlers.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.294805 livereloadx-2.6.8/livereload/management/
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.299304 livereloadx-2.6.8/livereload/management/commands/
--rw-r--r--   0 tuanchau   (503) staff       (20)        0 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/management/commands/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1720 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/management/commands/livereload.py
--rw-r--r--   0 tuanchau   (503) staff       (20)    12650 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/server.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.299635 livereloadx-2.6.8/livereload/vendors/
--rw-r--r--   0 tuanchau   (503) staff       (20)    37411 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/vendors/livereload.js
--rw-r--r--   0 tuanchau   (503) staff       (20)     7410 2023-06-03 04:52:10.000000 livereloadx-2.6.8/livereload/watcher.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.301832 livereloadx-2.6.8/livereloadx.egg-info/
--rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      510 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/SOURCES.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/dependency_links.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       51 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/entry_points.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        8 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/requires.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       11 2023-06-03 05:19:36.000000 livereloadx-2.6.8/livereloadx.egg-info/top_level.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       74 2023-06-03 05:19:36.302877 livereloadx-2.6.8/setup.cfg
--rw-r--r--   0 tuanchau   (503) staff       (20)     2024 2023-06-03 05:04:02.000000 livereloadx-2.6.8/setup.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 05:19:36.302171 livereloadx-2.6.8/tests/
--rw-r--r--   0 tuanchau   (503) staff       (20)     4939 2023-06-03 04:52:10.000000 livereloadx-2.6.8/tests/test_watcher.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.288874 livereloadx-2.6.9/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1510 2023-06-03 04:52:10.000000 livereloadx-2.6.9/LICENSE
+-rw-r--r--   0 tuanchau   (503) staff       (20)       76 2023-06-03 04:52:10.000000 livereloadx-2.6.9/MANIFEST.in
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 08:11:56.288964 livereloadx-2.6.9/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      987 2023-06-03 05:05:06.000000 livereloadx-2.6.9/README.md
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.285406 livereloadx-2.6.9/livereload/
+-rw-r--r--   0 tuanchau   (503) staff       (20)      366 2023-06-03 08:10:30.000000 livereloadx-2.6.9/livereload/__init__.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1381 2023-06-03 04:52:10.000000 livereloadx-2.6.9/livereload/cli.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     6725 2023-06-03 05:19:15.000000 livereloadx-2.6.9/livereload/handlers.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.281445 livereloadx-2.6.9/livereload/management/
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.286000 livereloadx-2.6.9/livereload/management/commands/
+-rw-r--r--   0 tuanchau   (503) staff       (20)        0 2023-06-03 04:52:10.000000 livereloadx-2.6.9/livereload/management/commands/__init__.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1720 2023-06-03 04:52:10.000000 livereloadx-2.6.9/livereload/management/commands/livereload.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)    12751 2023-06-03 08:02:48.000000 livereloadx-2.6.9/livereload/server.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.286270 livereloadx-2.6.9/livereload/vendors/
+-rw-r--r--   0 tuanchau   (503) staff       (20)    37411 2023-06-03 04:52:10.000000 livereloadx-2.6.9/livereload/vendors/livereload.js
+-rw-r--r--   0 tuanchau   (503) staff       (20)     7891 2023-06-03 08:08:27.000000 livereloadx-2.6.9/livereload/watcher.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.288279 livereloadx-2.6.9/livereloadx.egg-info/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2384 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      510 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/SOURCES.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/dependency_links.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       51 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/entry_points.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        8 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/requires.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       11 2023-06-03 08:11:56.000000 livereloadx-2.6.9/livereloadx.egg-info/top_level.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       74 2023-06-03 08:11:56.289304 livereloadx-2.6.9/setup.cfg
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2024 2023-06-03 05:04:02.000000 livereloadx-2.6.9/setup.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-06-03 08:11:56.288542 livereloadx-2.6.9/tests/
+-rw-r--r--   0 tuanchau   (503) staff       (20)     4939 2023-06-03 04:52:10.000000 livereloadx-2.6.9/tests/test_watcher.py
```

### Comparing `livereloadx-2.6.8/LICENSE` & `livereloadx-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/PKG-INFO` & `livereloadx-2.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livereloadx
-Version: 2.6.8
+Version: 2.6.9
 Summary: Python LiveReload is an awesome tool for web developers
 Home-page: https://github.com/lepture/python-livereload
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `livereloadx-2.6.8/README.md` & `livereloadx-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/livereload/cli.py` & `livereloadx-2.6.9/livereload/cli.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/livereload/handlers.py` & `livereloadx-2.6.9/livereload/handlers.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/livereload/management/commands/livereload.py` & `livereloadx-2.6.9/livereload/management/commands/livereload.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/livereload/server.py` & `livereloadx-2.6.9/livereload/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,29 @@
 
 import sys
 
 import errno
 
 if sys.version_info >= (3, 8) and sys.platform == 'win32':
     import asyncio
+
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 logger = logging.getLogger('livereload')
 
 HEAD_END = b'</head>'
 
 
 def set_header(fn, name, value):
     """Helper Function to Add HTTP headers to the server"""
+
     def set_default_headers(self, *args, **kwargs):
         fn(self, *args, **kwargs)
         self.set_header(name, value)
+
     return set_default_headers
 
 
 def shell(cmd, output=None, mode='w', cwd=None, shell=False):
     """Execute a shell command.
 
     You can add a shell command::
@@ -178,14 +181,15 @@
 
     :param app: a WSGI application instance
     :param watcher: A Watcher instance, you don't have to initialize
                     it by yourself. Under Linux, you will want to install
                     pyinotify and use INotifyWatcher() to avoid wasted
                     CPU usage.
     """
+
     def __init__(self, app=None, watcher=None):
         self.root = None
 
         self.app = app
         if not watcher:
             watcher_cls = get_watcher_class()
             watcher = watcher_cls()
@@ -203,18 +207,18 @@
             server.setHeader('Access-Control-Allow-Methods', '*')
             server.serve()
 
         :param name: The name of the header field to be defined.
         :param value: The value of the header field to be defined.
         """
         StaticFileHandler.set_default_headers = set_header(
-                StaticFileHandler.set_default_headers, name, value)
+            StaticFileHandler.set_default_headers, name, value)
         self.SFH = StaticFileHandler
 
-    def watch(self, filepath, func=None, delay=None, ignore=None):
+    def watch(self, filepath, func=None, delay=None, ignore=None, delay_exe=0):
         """Add the given filepath for watcher list.
 
         Once you have initialized a server, watch file changes before
         serve the server::
 
             server.watch('static/*.stylus', 'make static')
             def alert():
@@ -226,23 +230,24 @@
                          a directory, or a glob pattern
         :param func: the function to be called, it can be a string of
                      shell command, or any callable object without
                      parameters
         :param delay: Delay sending the reload message. Use 'forever' to
                       not send it. This is useful to compile sass files to
                       css, but reload on changed css files then only.
+        :param delay_exe: Delay execution of func
         :param ignore: A function return True to ignore a certain pattern of
                        filepath.
         """
         if isinstance(func, str):
             cmd = func
             func = shell(func)
             func.name = f"shell: {cmd}"
 
-        self.watcher.watch(filepath, func, delay, ignore=ignore)
+        self.watcher.watch(filepath, func, delay, ignore=ignore, delay_exe=delay_exe)
 
     def application(self, port, host, liveport=None, debug=None,
                     live_css=True):
         LiveReloadHandler.watcher = self.watcher
         LiveReloadHandler.live_css = live_css
         if debug is None and self.app:
             debug = True
@@ -264,15 +269,16 @@
             '+ "/livereload.js?port=" + port;'
             'document.head.appendChild(s);'
             '})();</script>'
         )
         if liveport:
             live_script = escape.utf8(live_script % liveport)
         else:
-            live_script = escape.utf8(live_script % "(window.location.port || (window.location.protocol == 'https:' ? 443: 80))")
+            live_script = escape.utf8(
+                live_script % "(window.location.port || (window.location.protocol == 'https:' ? 443: 80))")
 
         web_handlers = self.get_web_handlers(live_script)
 
         class ConfiguredTransform(LiveScriptInjector):
             script = live_script
 
         if not liveport:
@@ -333,18 +339,18 @@
         self.application(
             port, host, liveport=liveport, debug=debug, live_css=live_css)
 
         # Async open web browser after 5 sec timeout
         if open_url:
             logger.error('Use `open_url_delay` instead of `open_url`')
         if open_url_delay is not None:
-
             def opener():
                 time.sleep(open_url_delay)
                 webbrowser.open(f'http://{host}:{port}')
+
             threading.Thread(target=opener).start()
 
         try:
             self.watcher._changes.append(('__livereload__', restart_delay))
             LiveReloadHandler.start_tasks()
             add_reload_hook(lambda: IOLoop.instance().close(all_fds=True))
             IOLoop.instance().start()
```

### Comparing `livereloadx-2.6.8/livereload/vendors/livereload.js` & `livereloadx-2.6.9/livereload/vendors/livereload.js`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/livereload/watcher.py` & `livereloadx-2.6.9/livereload/watcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 """
 
 import glob
 import logging
 import os
 import time
 from inspect import signature
+from tornado import ioloop
 
 try:
     import pyinotify
 except ImportError:
     pyinotify = None
 
 logger = logging.getLogger('livereload')
 
 
 class Watcher:
     """A file watcher registry."""
+
     def __init__(self):
         self._tasks = {}
+        self._jobs = {}
 
         # modification time of filepaths for each task,
         # before and after checking for changes
         self._task_mtimes = {}
         self._new_mtimes = {}
 
         # setting changes
@@ -50,28 +53,30 @@
             self.ignored_dirs.remove(a)
 
     def ignore(self, filename):
         """Ignore a given filename or not."""
         _, ext = os.path.splitext(filename)
         return ext in ['.pyc', '.pyo', '.o', '.swp']
 
-    def watch(self, path, func=None, delay=0, ignore=None):
+    def watch(self, path, func=None, delay=0, ignore=None, delay_exe=0):
         """Add a task to watcher.
 
         :param path: a filepath or directory path or glob pattern
         :param func: the function to be executed when file changed
         :param delay: Delay sending the reload message. Use 'forever' to
                       not send it. This is useful to compile sass files to
                       css, but reload on changed css files then only.
+        :param delay_exe: Delay execution of func
         :param ignore: A function return True to ignore a certain pattern of
                        filepath.
         """
         self._tasks[path] = {
             'func': func,
             'delay': delay,
+            'delay_exe': delay_exe,
             'ignore': ignore,
             'mtimes': {},
         }
 
     def start(self, callback):
         """Start the watcher running, calling callback when changes are
         observed. If this returns False, regular polling will be used."""
@@ -81,41 +86,52 @@
         """Check if there are changes. If so, run the given task.
 
         Returns a tuple of modified filepath and reload delay.
         """
         if self._changes:
             return self._changes.pop()
 
+        def register_job(fun, delay_exe, changed):
+            name = getattr(fun, 'name', None)
+            if not name:
+                name = getattr(fun, '__name__', 'anonymous')
+            logger.info(
+                f"Running task: {name} (delay: {delay}) (delay run: {delay_exe})")
+            loop = ioloop.IOLoop.current()
+            if fun in self._jobs:
+                loop.remove_timeout(self._jobs[fun])
+
+            self._jobs[fun] = loop.call_later(delay_exe, job_exe, fun, changed)
+
+        def job_exe(fun, changed):
+            if len(signature(fun).parameters) > 0 and isinstance(changed, list):
+                fun(changed)
+            else:
+                fun()
+            self._jobs.pop(fun)
+
         # clean filepath
         self.filepath = None
         delays = set()
         for path in self._tasks:
             item = self._tasks[path]
             self._task_mtimes = item['mtimes']
             changed = self.is_changed(path, item['ignore'])
             if changed:
                 func = item['func']
                 delay = item['delay']
                 if delay and isinstance(delay, float) or delay == 'forever':
                     delays.add(delay)
                 if func:
-                    name = getattr(func, 'name', None)
-                    if not name:
-                        name = getattr(func, '__name__', 'anonymous')
-                    logger.info(
-                        f"Running task: {name} (delay: {delay})")
-                    if len(signature(func).parameters) > 0 and isinstance(changed, list):
-                        func(changed)
-                    else:
-                        func()
+                    register_job(func, item['delay_exe'], changed)
 
-        if delays == {'forever'}:
+        if 'forever' in delays:
             delay = 'forever'
         elif delays:
-            delay = max(delays - {'forever'})
+            delay = max(delays)
         else:
             delay = None
         return self.filepath, delay
 
     def is_changed(self, path, ignore=None):
         """Check if any filepaths have been added, modified, or removed.
```

### Comparing `livereloadx-2.6.8/livereloadx.egg-info/PKG-INFO` & `livereloadx-2.6.9/livereloadx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livereloadx
-Version: 2.6.8
+Version: 2.6.9
 Summary: Python LiveReload is an awesome tool for web developers
 Home-page: https://github.com/lepture/python-livereload
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `livereloadx-2.6.8/setup.py` & `livereloadx-2.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `livereloadx-2.6.8/tests/test_watcher.py` & `livereloadx-2.6.9/tests/test_watcher.py`

 * *Files identical despite different names*

