# Comparing `tmp/screen-config-watcher-0.0.2.tar.gz` & `tmp/screen-config-watcher-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen-config-watcher-0.0.2.tar", last modified: Thu Mar  9 08:24:13 2023, max compression
+gzip compressed data, was "screen-config-watcher-0.0.3.tar", last modified: Sat Jun  3 17:10:22 2023, max compression
```

## Comparing `screen-config-watcher-0.0.2.tar` & `screen-config-watcher-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:13.442759 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-09 08:24:13.000000 screen-config-watcher-0.0.2/screen_config_watcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/scw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/scw/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/cli/screen_config_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/config_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/scw/screen_lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/screen_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/screen_lock/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-09 08:24:02.000000 screen-config-watcher-0.0.2/scw/watcher_app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 08:24:13.446759 screen-config-watcher-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 17:10:22.000000 screen-config-watcher-0.0.3/screen_config_watcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/scw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/scw/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/cli/screen_config_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/config_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/scw/screen_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/screen_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/screen_lock/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-03 17:10:10.000000 screen-config-watcher-0.0.3/scw/watcher_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:10:22.860153 screen-config-watcher-0.0.3/setup.cfg
```

### Comparing `screen-config-watcher-0.0.2/LICENSE` & `screen-config-watcher-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/PKG-INFO` & `screen-config-watcher-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-config-watcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to watch OS screen configuration changes and change the OBS profile and scene collection accordingly.
 Author-email: Dennis Sitelew <yowidin@gmail.com>
 Project-URL: homepage, https://github.com/yowidin/screen-config-watcher
 Project-URL: bugtrack, https://github.com/yowidin/screen-config-watcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `screen-config-watcher-0.0.2/pyproject.toml` & `screen-config-watcher-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "screen-config-watcher"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Dennis Sitelew", email = "yowidin@gmail.com" },
 ]
 description = "A tool to watch OS screen configuration changes and change the OBS profile and scene collection accordingly."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `screen-config-watcher-0.0.2/screen_config_watcher.egg-info/PKG-INFO` & `screen-config-watcher-0.0.3/screen_config_watcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-config-watcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to watch OS screen configuration changes and change the OBS profile and scene collection accordingly.
 Author-email: Dennis Sitelew <yowidin@gmail.com>
 Project-URL: homepage, https://github.com/yowidin/screen-config-watcher
 Project-URL: bugtrack, https://github.com/yowidin/screen-config-watcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `screen-config-watcher-0.0.2/screen_config_watcher.egg-info/SOURCES.txt` & `screen-config-watcher-0.0.3/screen_config_watcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/cli/screen_config_watcher.py` & `screen-config-watcher-0.0.3/scw/cli/screen_config_watcher.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/config.py` & `screen-config-watcher-0.0.3/scw/config.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/config_file_watcher.py` & `screen-config-watcher-0.0.3/scw/config_file_watcher.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/log.py` & `screen-config-watcher-0.0.3/scw/log.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/options.py` & `screen-config-watcher-0.0.3/scw/options.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/screen_lock/macos.py` & `screen-config-watcher-0.0.3/scw/screen_lock/macos.py`

 * *Files identical despite different names*

### Comparing `screen-config-watcher-0.0.2/scw/watcher_app.py` & `screen-config-watcher-0.0.3/scw/watcher_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from PySide6.QtCore import QTimer, Signal
 from PySide6.QtGui import QGuiApplication, QScreen
 from PySide6.QtWidgets import QMainWindow, QApplication
 
 import sys
 import signal
 
+from sys import platform
+
 from scw.log import Log
 from scw.options import Options
 from scw.config import Config
 from scw.config_file_watcher import ConfigFileWatcher
 
 from obwsc.cli.obws_command import main
 
@@ -120,15 +122,16 @@
 
     def __init__(self, options: Options):
         self.hide_dock()
         self.app = QApplication(sys.argv)
 
         signal.signal(signal.SIGINT, ScreenConfigWatcherApp.signal_handler)
         signal.signal(signal.SIGTERM, ScreenConfigWatcherApp.signal_handler)
-        signal.signal(signal.SIGQUIT, ScreenConfigWatcherApp.signal_handler)
+        if platform != 'win32':
+            signal.signal(signal.SIGQUIT, ScreenConfigWatcherApp.signal_handler)
 
         # Let the interpreter run each 500 ms, otherwise we can't receive signals
         self.signal_timer = QTimer()
         self.signal_timer.timeout.connect(lambda: None)
 
         self.widget = MainWindow(options)
```

