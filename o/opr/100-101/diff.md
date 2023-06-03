# Comparing `tmp/opr-100.tar.gz` & `tmp/opr-101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-100.tar", last modified: Sat Jun  3 11:44:20 2023, max compression
+gzip compressed data, was "opr-101.tar", last modified: Sat Jun  3 14:08:59 2023, max compression
```

## Comparing `opr-100.tar` & `opr-101.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.046117 opr-100/
--rw-r--r--   0 nop       (1000) nop       (1000)     2731 2023-06-03 11:44:20.046117 opr-100/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1854 2023-06-03 03:54:50.000000 opr-100/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.042117 opr-100/bin/
--rwxr-xr-x   0 nop       (1000) nop       (1000)     2314 2023-06-03 11:16:54.000000 opr-100/bin/opr
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.046117 opr-100/opr/
--rw-r--r--   0 nop       (1000) nop       (1000)     1287 2023-06-03 03:54:50.000000 opr-100/opr/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      570 2023-06-03 03:54:50.000000 opr-100/opr/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1088 2023-06-03 03:54:50.000000 opr-100/opr/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1747 2023-06-03 03:54:50.000000 opr-100/opr/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      161 2023-06-03 03:54:50.000000 opr-100/opr/configs.py
--rw-r--r--   0 nop       (1000) nop       (1000)      798 2023-06-03 03:54:50.000000 opr-100/opr/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      379 2023-06-03 03:54:50.000000 opr-100/opr/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)      302 2023-06-03 03:54:50.000000 opr-100/opr/defines.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1325 2023-06-03 03:54:50.000000 opr-100/opr/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      350 2023-06-03 03:54:50.000000 opr-100/opr/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1970 2023-06-03 03:54:50.000000 opr-100/opr/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      941 2023-06-03 03:54:50.000000 opr-100/opr/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      443 2023-06-03 03:54:50.000000 opr-100/opr/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      942 2023-06-03 03:54:50.000000 opr-100/opr/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.046117 opr-100/opr/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)      491 2023-06-03 11:44:04.000000 opr-100/opr/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      578 2023-06-03 03:54:50.000000 opr-100/opr/modules/cfg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      209 2023-06-03 03:54:50.000000 opr-100/opr/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      706 2023-06-03 03:54:50.000000 opr-100/opr/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      420 2023-06-03 03:54:50.000000 opr-100/opr/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      966 2023-06-03 03:54:50.000000 opr-100/opr/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    20772 2023-06-03 03:54:50.000000 opr-100/opr/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      707 2023-06-03 03:54:50.000000 opr-100/opr/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)      179 2023-06-03 03:54:50.000000 opr-100/opr/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7712 2023-06-03 03:54:50.000000 opr-100/opr/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      348 2023-06-03 03:54:50.000000 opr-100/opr/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      941 2023-06-03 03:54:50.000000 opr-100/opr/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-06-03 03:54:50.000000 opr-100/opr/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      220 2023-06-03 03:54:50.000000 opr-100/opr/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      175 2023-06-03 03:54:50.000000 opr-100/opr/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2013 2023-06-03 03:54:50.000000 opr-100/opr/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2136 2023-06-03 03:54:50.000000 opr-100/opr/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1812 2023-06-03 03:54:50.000000 opr-100/opr/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4721 2023-06-03 03:54:50.000000 opr-100/opr/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      357 2023-06-03 03:54:50.000000 opr-100/opr/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2684 2023-06-03 11:17:22.000000 opr-100/opr/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      896 2023-06-03 03:54:50.000000 opr-100/opr/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2935 2023-06-03 03:54:50.000000 opr-100/opr/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.046117 opr-100/opr.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     2731 2023-06-03 11:44:19.000000 opr-100/opr.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-06-03 11:44:19.000000 opr-100/opr.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-03 11:44:19.000000 opr-100/opr.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        4 2023-06-03 11:44:19.000000 opr-100/opr.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-03 11:44:19.000000 opr-100/opr.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-06-03 11:44:20.046117 opr-100/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      871 2023-06-03 11:33:00.000000 opr-100/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 11:44:20.046117 opr-100/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      712 2023-06-03 11:34:45.000000 opr-100/test/test_composite.py
--rw-r--r--   0 nop       (1000) nop       (1000)      510 2023-06-03 11:34:57.000000 opr-100/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      408 2023-06-03 11:40:46.000000 opr-100/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      912 2023-06-03 11:34:30.000000 opr-100/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4597 2023-06-03 11:36:29.000000 opr-100/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)      661 2023-06-03 11:36:47.000000 opr-100/test/test_recursive.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1092 2023-06-03 11:37:40.000000 opr-100/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.169899 opr-101/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4513 2023-06-03 14:08:59.169899 opr-101/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     2692 2023-06-03 12:49:04.000000 opr-101/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.165899 opr-101/bin/
+-rwxr-xr-x   0 nop       (1000) nop       (1000)     2345 2023-06-03 13:35:22.000000 opr-101/bin/opr
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.169899 opr-101/opr/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1504 2023-06-03 14:05:27.000000 opr-101/opr/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      600 2023-06-03 13:25:23.000000 opr-101/opr/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1110 2023-06-03 13:25:44.000000 opr-101/opr/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1622 2023-06-03 14:04:39.000000 opr-101/opr/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      180 2023-06-03 13:27:34.000000 opr-101/opr/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      817 2023-06-03 13:27:58.000000 opr-101/opr/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      379 2023-06-03 12:03:57.000000 opr-101/opr/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      302 2023-06-03 12:03:57.000000 opr-101/opr/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1344 2023-06-03 13:28:14.000000 opr-101/opr/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      359 2023-06-03 13:28:24.000000 opr-101/opr/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      956 2023-06-03 13:41:26.000000 opr-101/opr/evented.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1974 2023-06-03 13:45:58.000000 opr-101/opr/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      954 2023-06-03 13:28:48.000000 opr-101/opr/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      466 2023-06-03 13:29:09.000000 opr-101/opr/logging.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.169899 opr-101/opr/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)      530 2023-06-03 13:48:26.000000 opr-101/opr/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      578 2023-06-03 12:03:57.000000 opr-101/opr/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      209 2023-06-03 12:03:57.000000 opr-101/opr/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      706 2023-06-03 12:03:57.000000 opr-101/opr/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      420 2023-06-03 12:03:57.000000 opr-101/opr/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      966 2023-06-03 12:03:57.000000 opr-101/opr/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    20766 2023-06-03 13:48:07.000000 opr-101/opr/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      707 2023-06-03 12:03:57.000000 opr-101/opr/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      179 2023-06-03 12:03:57.000000 opr-101/opr/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7712 2023-06-03 12:03:57.000000 opr-101/opr/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      348 2023-06-03 12:03:57.000000 opr-101/opr/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      941 2023-06-03 12:03:57.000000 opr-101/opr/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-06-03 12:03:57.000000 opr-101/opr/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      220 2023-06-03 12:03:57.000000 opr-101/opr/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      175 2023-06-03 12:03:57.000000 opr-101/opr/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2033 2023-06-03 13:30:28.000000 opr-101/opr/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2181 2023-06-03 13:31:04.000000 opr-101/opr/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1839 2023-06-03 13:31:20.000000 opr-101/opr/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4739 2023-06-03 13:31:40.000000 opr-101/opr/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      380 2023-06-03 13:32:04.000000 opr-101/opr/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2705 2023-06-03 13:48:48.000000 opr-101/opr/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      896 2023-06-03 12:03:57.000000 opr-101/opr/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2935 2023-06-03 12:03:57.000000 opr-101/opr/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.169899 opr-101/opr.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4513 2023-06-03 14:08:59.000000 opr-101/opr.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-06-03 14:08:59.000000 opr-101/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-03 14:08:59.000000 opr-101/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        4 2023-06-03 14:08:59.000000 opr-101/opr.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-03 14:08:59.000000 opr-101/opr.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-06-03 14:08:59.169899 opr-101/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      871 2023-06-03 14:05:57.000000 opr-101/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-03 14:08:59.169899 opr-101/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      710 2023-06-03 12:03:57.000000 opr-101/test/test_composite.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      494 2023-06-03 14:01:11.000000 opr-101/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      382 2023-06-03 14:04:29.000000 opr-101/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      907 2023-06-03 13:57:36.000000 opr-101/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4581 2023-06-03 14:04:13.000000 opr-101/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      663 2023-06-03 13:55:14.000000 opr-101/test/test_recursive.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1075 2023-06-03 14:03:53.000000 opr-101/test/test_storage.py
```

### Comparing `opr-100/bin/opr` & `opr-101/bin/opr`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 #
 # pylint: disable=E0012,C0114,C0115,C0116,C0413,E0401,W0212,W0611,W1514,R1732
 # pylint: disable=E0611
 # flake8: noqa: E402
 # pylama: ignore=W0611,E402
 
 
+"object programming runtime"
+
+
 import os
 import readline
 import sys
 import termios
 import time
```

### Comparing `opr-100/opr/clients.py` & `opr-101/opr/clients.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116,W0613
 
 
+"user interfacing handlers"
+
+
 from .command import Commands
 from .handler import Handler
 from .listens import Listens
 
 
 def __dir__():
     return (
```

### Comparing `opr-100/opr/clocked.py` & `opr-101/opr/clocked.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116
 
 
+"execute at a time"
+
+
 import threading
 import time
 
 
 from .objects import Object
 from .runtime import launch
```

### Comparing `opr-100/opr/command.py` & `opr-101/opr/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116,W0703
 
 
+"commands and their handling"
+
+
 import inspect
-import sys
 
 
 from .errored import Errors
+from .evented import Event
 from .logging import Logging
-from .message import Message
 from .objects import Object, copy
 
 
 def __dir__():
     return (
             'Commands',
            )
@@ -32,30 +34,27 @@
 
     @staticmethod
     def add(cmd, func) -> None:
         setattr(Commands.cmds, cmd, func)
         setattr(Commands.modnames, cmd, func.__module__)
 
     @staticmethod
-    def handle(evt) -> Message:
+    def handle(evt) -> Event:
         evt.parse(evt.txt)
         func = getattr(Commands.cmds, evt.cmd, None)
         if Commands.ondemand and not func:
             modname = getattr(Commands.modnames, evt.cmd, None)
             mod = None
             if modname:
-                if modname in sys.modules:
-                    mod = sys.modules[modname]
-                if not mod:
-                    Logging.debug(f"load {modname}")
-                    mod = getattr(
-                                  Commands.modules,
-                                  modname.split(".")[-1],
-                                  None
-                                 )
+                Logging.debug(f"load {modname}")
+                mod = getattr(
+                              Commands.modules,
+                              modname.split(".")[-1],
+                              None
+                             )
                 func = getattr(mod, evt.cmd, None)
         if func:
             try:
                 func(evt)
                 evt.show()
             except Exception as ex:
                 Errors.handle(ex)
```

### Comparing `opr-100/opr/decoder.py` & `opr-101/opr/decoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116
 
 
+"json to object"
+
+
 import json
 
 
 from .objects import Object, copy
 
 
 def __dir__():
```

### Comparing `opr-100/opr/encoder.py` & `opr-101/opr/encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116
 
 
+"object to json"
+
+
 import json
 
 
 from .objects import Object
 
 
 def __dir__():
```

### Comparing `opr-100/opr/handler.py` & `opr-101/opr/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=R,C0114,C0115,C0116,W0613,W0212,W0703
 
 
+"teh handler"
+
+
 import queue
 import ssl
 import threading
 
 
 from .errored import Errors
+from .evented import Event
 from .objects import Object
-from .message import Message
 from .runtime import Cfg, launch
 
 
 def __dir__():
     return (
             'Handler',
            )
@@ -25,22 +28,22 @@
     def __init__(self):
         Object.__init__(self)
         self.cbs = Object()
         self.queue = queue.Queue()
         self.stopped = threading.Event()
         self.threaded = True
 
-    def event(self, txt) -> Message:
-        msg = Message()
+    def event(self, txt) -> Event:
+        msg = Event()
         msg.type = 'command'
         msg.orig = repr(self)
         msg.parse(txt)
         return msg
 
-    def handle(self, evt) -> Message:
+    def handle(self, evt) -> Event:
         func = getattr(self.cbs, evt.type, None)
         if func:
             if "t" in Cfg.opts:
                 evt._thr = launch(dispatch, func, evt, name=evt.cmd)
             else:
                 dispatch(func, evt)
         return evt
@@ -49,18 +52,18 @@
         while not self.stopped.is_set():
             try:
                 self.handle(self.poll())
             except (ssl.SSLError, EOFError, KeyboardInterrupt) as ex:
                 Errors.handle(ex)
                 self.restart()
 
-    def one(self, txt) -> Message:
+    def one(self, txt) -> Event:
         return self.handle(self.event(txt))
 
-    def poll(self) -> Message:
+    def poll(self) -> Event:
         return self.queue.get()
 
     def put(self, evt) -> None:
         self.queue.put_nowait(evt)
 
     def register(self, cmd, func) -> None:
         setattr(self.cbs, cmd, func)
```

### Comparing `opr-100/opr/listens.py` & `opr-101/opr/listens.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116
 
 
+"as a bus"
+
+
 from .objects import Object
 
 
 def __dir__():
     return (
             'Listens',
            )
```

### Comparing `opr-100/opr/message.py` & `opr-101/opr/evented.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0115,C0116
 
 
+"default event"
+
+
 import threading
 
 
 from .default import Default
 from .listens import Listens
 from .parsers import parse as evtparse
 
 
 def __dir__():
     return (
-            'Message',
+            'Event',
            )
 
 
-class Message(Default):
+class Event(Default):
 
     __slots__ = ('_ready', '_thr')
 
     def __init__(self, *args, **kwargs):
         Default.__init__(self, *args, **kwargs)
         self._ready = threading.Event()
         self._thr = None
```

### Comparing `opr-100/opr/modules/cfg.py` & `opr-101/opr/modules/cfg.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/err.py` & `opr-101/opr/modules/err.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/fnd.py` & `opr-101/opr/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/irc.py` & `opr-101/opr/modules/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import _thread
 
 
 from ..clients import Client
 from ..command import Commands
 from ..default import Default
 from ..errored import Errors
-from ..message import Message
+from ..evented import Event
 from ..listens import Listens
 from ..logging import Logging
 from ..objects import Object, copy, keys, update
 from ..objfunc import edit, prt
 from ..persist import Persist, last, write
 from ..runtime import Cfg, launch
 from ..utility import elapsed, fntime
@@ -416,15 +416,15 @@
             self.command('NOTICE', event.channel, txt)
 
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         Logging.debug(txt)
-        obj = Message()
+        obj = Event()
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
             obj.origin = arguments[0]
         else:
@@ -505,15 +505,15 @@
             elif event.txt.startswith('%s:' % self.cfg.nick):
                 event.txt = event.txt[len(self.cfg.nick)+1:]
             else:
                 return
             if self.cfg.users and not Users.allowed(event.origin, 'USER'):
                 return
             Logging.debug(f"command from {event.origin}: {event.txt}")
-            msg = Message()
+            msg = Event()
             copy(msg, event)
             msg.type = 'command'
             msg.parse(event.txt)
             self.handle(msg)
 
     def quit(self, event):
         Logging.debug(f"quit from {self.cfg.server}")
```

### Comparing `opr-100/opr/modules/log.py` & `opr-101/opr/modules/log.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/rss.py` & `opr-101/opr/modules/rss.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/tdo.py` & `opr-101/opr/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/modules/thr.py` & `opr-101/opr/modules/thr.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/objects.py` & `opr-101/opr/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
 
 
+"clean namespace"
+
+
 import datetime
 import os
 import uuid
 
 
 def __dir__():
     return (
```

### Comparing `opr-100/opr/objfunc.py` & `opr-101/opr/objfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C0114,C0116
 # pylama: ignore=C901
 
 
+"functions using object as first argument"
+
+
 from .objects import Object, copy, items, keys
 
 
 def __dir__():
     return (
             'edit',
             'prt',
```

### Comparing `opr-100/opr/parsers.py` & `opr-101/opr/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=R,C0114,C0116
 # pylama: ignore=C901
 
 
+"parse text for command"
+
+
 from .default import Default
 from .utility import spl
 
 
 def __dir__():
     return (
             'parse',
```

### Comparing `opr-100/opr/persist.py` & `opr-101/opr/persist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=R,C0114,C0115,C0116,W0613,E1101
 
 
+"store to disk"
+
+
 import os
 import _thread
 
 
 from .decoder import load
 from .default import Default
 from .encoder import dump
```

### Comparing `opr-100/opr/runtime.py` & `opr-101/opr/runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # This file is placed in the Pubic Domain.
 #
 # pylint: disable=C0114,C0115,C0116,W0613,W0212
 
 
+"object programming runtime"
+
+
 import functools
 import io
 import time
 import traceback
 
 
+from .evented import Event
 from .objects import update
 from .logging import Logging
 from .command import Commands
 from .configs import Cfg
 from .errored import Errors
-from .message import Message
 from .threads import Thread
 from .utility import spl
 
 
 def __dir__():
     return (
             'DATE',
@@ -37,25 +40,25 @@
 
 
 Cfg.debug = False
 Cfg.mod = "cmd,err,flt,mod,sts,thr,upt,ver"
 Cfg.name = "opr"
 Cfg.skip = "PING,PONG,PRIVMSG"
 Cfg.threaded = False
-Cfg.version = "100"
+Cfg.version = "101"
 
 
 # FUNCTIONS
 
 
 def banner():
     Logging.debug(f"{Cfg.name.upper()} started at {DATE}")
 
 
-def command(cli, txt) -> Message:
+def command(cli, txt) -> Event:
     evt = cli.event(txt)
     Commands.handle(evt)
     evt.ready()
     return evt
 
 
 def scanstr(pkg, mods, init=None, doall=False, wait=False) -> None:
@@ -80,19 +83,19 @@
 def launch(func, *args, **kwargs) -> Thread:
     thrname = kwargs.get('name', '')
     thr = Thread(func, thrname, *args)
     thr.start()
     return thr
 
 
-def parse_cli(txt) -> Message:
-    msg = Message()
-    msg.parse(txt)
-    update(Cfg, msg, False)
-    Cfg.mod += msg.mods
+def parse_cli(txt) -> Cfg:
+    evt = Event()
+    evt.parse(txt)
+    update(Cfg, evt, False)
+    Cfg.mod += evt.mods
     return Cfg
 
 
 def threaded(func, *args, **kwargs) -> None:
 
     @functools.wraps(func)
     def threadedfunc(*args, **kwargs):
```

### Comparing `opr-100/opr/threads.py` & `opr-101/opr/threads.py`

 * *Files identical despite different names*

### Comparing `opr-100/opr/utility.py` & `opr-101/opr/utility.py`

 * *Files identical despite different names*

### Comparing `opr-100/setup.py` & `opr-101/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name='opr',
-    version='100',
+    version='101',
     url='https://github.com/bthate/opr',
     author='Bart Thate',
     author_email='bthate@dds.nl',
     description="object programming runtime",
     long_description=read(),
     long_description_content_type='text/x-rst',
     license='Public Domain',
```

### Comparing `opr-100/test/test_composite.py` & `opr-101/test/test_composite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # This file is placed in the Public Domain.
-#
 # pylint: disable=C0114,C0115,C0116,C0413,E1101,R1732
 # pylama: ignore=W0611,E265,E402
 
 
 import sys
 import unittest
```

### Comparing `opr-100/test/test_inherit.py` & `opr-101/test/test_inherit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylama: ignore=E402,E302,E265,E303
+# pylama: ignore=E402,E302,E265
 
 
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
```

### Comparing `opr-100/test/test_objects.py` & `opr-101/test/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=E1101
-# pylama: ignore=E402,E302,E265,E303
+# pylama: ignore=E402
 
 
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
@@ -64,15 +64,14 @@
           '__sizeof__',
           '__slots__',
           '__str__',
           '__subclasshook__'
          )
 
 
-
 class TestObject(unittest.TestCase):
 
     def test_constructor(self):
         obj = Object()
         self.assertTrue(type(obj), Object)
 
     def test__class(self):
```

### Comparing `opr-100/test/test_recursive.py` & `opr-101/test/test_recursive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is placed in the Public Domain.
-#
 # pylint: disable=C0413,C0115,C0116,E1101
 # pylama: ignore=W0611,E303,E402
 
 
 """
-    >>> import opr.defines as opr
+    >>> import opr
     >>> o = opr.Object()
     >>> o.o = opr.Object()
     >>> o.o.a = "test"
     >>> print(o)
     {'o': {'a': 'test'}}
 
 """
@@ -29,9 +28,10 @@
 
 
     def testrecursive(self):
         obj = Object()
         obj.obj = Object()
         obj.obj.a = "test"
         pth = writerec(obj)
+        print(pth)
         readrec(obj, pth)
         self.assertEqual(obj.obj.a, "test")
```

### Comparing `opr-100/test/test_storage.py` & `opr-101/test/test_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # This file is placed in the Public Domain.
 #
-# pylama: ignore=E402,E302,E265,E303
-
+# pylama: ignore=E402
 
 import os
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
 
 
-
 from opr.objects import Object
 from opr.persist import Persist, write
 
 
 import opr.persist
```

