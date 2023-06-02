# Comparing `tmp/guardshield-1.0.2.tar.gz` & `tmp/guardshield-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.0.2.tar", last modified: Fri May 19 17:13:30 2023, max compression
+gzip compressed data, was "dist\guardshield-1.0.4.tar", last modified: Fri Jun  2 22:42:52 2023, max compression
```

## Comparing `guardshield-1.0.2.tar` & `guardshield-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.405916 guardshield-1.0.2/
--rw-rw-rw-   0        0        0      232 2023-05-19 17:13:30.404919 guardshield-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2323 2023-05-19 17:02:01.000000 guardshield-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.378993 guardshield-1.0.2/guardshield/
--rw-rw-rw-   0        0        0       87 2023-05-18 23:49:41.000000 guardshield-1.0.2/guardshield/__init__.py
--rw-rw-rw-   0        0        0    17408 2023-05-18 23:20:40.000000 guardshield-1.0.2/guardshield/lib.dll
--rw-rw-rw-   0        0        0     1818 2023-05-19 17:13:16.000000 guardshield-1.0.2/guardshield/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.403921 guardshield-1.0.2/guardshield.egg-info/
--rw-rw-rw-   0        0        0      232 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 17:13:30.405916 guardshield-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-05-19 17:12:35.000000 guardshield-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:42:52.666231 guardshield-1.0.4/
+-rw-rw-rw-   0        0        0     3138 2023-06-02 22:42:52.665233 guardshield-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2023-05-19 17:02:01.000000 guardshield-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 22:42:52.648279 guardshield-1.0.4/guardshield/
+-rw-rw-rw-   0        0        0       89 2023-06-02 21:51:47.000000 guardshield-1.0.4/guardshield/__init__.py
+-rw-rw-rw-   0        0        0    52713 2023-06-02 22:31:41.000000 guardshield-1.0.4/guardshield/dll_bytes.py
+-rw-rw-rw-   0        0        0     2009 2023-06-02 22:34:17.000000 guardshield-1.0.4/guardshield/main.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:42:52.664236 guardshield-1.0.4/guardshield.egg-info/
+-rw-rw-rw-   0        0        0     3138 2023-06-02 22:42:52.000000 guardshield-1.0.4/guardshield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-02 22:42:52.000000 guardshield-1.0.4/guardshield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 22:42:52.000000 guardshield-1.0.4/guardshield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 22:42:52.000000 guardshield-1.0.4/guardshield.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-06-02 22:42:52.000000 guardshield-1.0.4/guardshield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 22:42:52.667228 guardshield-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      585 2023-06-02 22:42:23.000000 guardshield-1.0.4/setup.py
```

### Comparing `guardshield-1.0.2/README.md` & `guardshield-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.2/guardshield/main.py` & `guardshield-1.0.4/guardshield/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os, ctypes, threading, time, sys
-import pkg_resources
+import os, ctypes, threading, time, io, tempfile
+from .dll_bytes import dll_bytes
 
 timeout = 0.1
 
 
 class AntiDebugger:
 
     def __init__(self, dll, settings):
@@ -42,18 +42,22 @@
         self.settings = {
             "anti_debugger" : anti_debugger,
             "kill_on_debug" : kill_on_debug,
             "custom_function_on_detection" : custom_function_on_detection
         }
 
     def load_dll(self) -> None:
+        #path = pkg_resources.resource_filename(__name__, 'lib.dll')
 
-        path = pkg_resources.resource_filename(__name__, 'lib.dll')
-        self.dll = ctypes.WinDLL(path)
-    
+        temp_file = tempfile.NamedTemporaryFile(suffix='.dll', delete=False)
+        temp_file.write(dll_bytes)
+        temp_file.close()
+        self.dll = ctypes.WinDLL(temp_file.name)
+        
+            
     def check_security(self) -> None:
 
         if self.settings['anti_debugger'] == True:
             AntiDebugger(
                 dll = self.dll,
                 settings = self.settings
             )
```

