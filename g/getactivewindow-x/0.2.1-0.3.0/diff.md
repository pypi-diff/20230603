# Comparing `tmp/getactivewindow_x-0.2.1.tar.gz` & `tmp/getactivewindow_x-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getactivewindow_x-0.2.1.tar", last modified: Sat Oct 23 14:31:03 2021, max compression
+gzip compressed data, was "getactivewindow_x-0.3.0.tar", last modified: Sat Jun  3 11:52:08 2023, max compression
```

## Comparing `getactivewindow_x-0.2.1.tar` & `getactivewindow_x-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 14:31:03.810447 getactivewindow_x-0.2.1/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2021-10-23 08:47:20.000000 getactivewindow_x-0.2.1/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)    35149 2021-10-23 08:47:20.000000 getactivewindow_x-0.2.1/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1615 2021-10-23 14:31:03.810447 getactivewindow_x-0.2.1/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      824 2021-10-23 14:07:25.000000 getactivewindow_x-0.2.1/README.md
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 14:31:03.810447 getactivewindow_x-0.2.1/getactivewindow/
--rw-r--r--   0 user202729  (1000) user202729  (1000)      524 2021-10-23 14:28:44.000000 getactivewindow_x-0.2.1/getactivewindow/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:49:14.000000 getactivewindow_x-0.2.1/getactivewindow/py.typed
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 14:31:03.810447 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1615 2021-10-23 14:31:03.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      340 2021-10-23 14:31:03.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 14:31:03.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       24 2021-10-23 14:31:03.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/requires.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       16 2021-10-23 14:31:03.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/top_level.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 08:59:29.000000 getactivewindow_x-0.2.1/getactivewindow_x.egg-info/zip-safe
--rw-r--r--   0 user202729  (1000) user202729  (1000)      672 2021-10-23 14:31:03.810447 getactivewindow_x-0.2.1/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)       39 2021-10-23 08:48:11.000000 getactivewindow_x-0.2.1/setup.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-03 11:52:08.550190 getactivewindow_x-0.3.0/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2021-10-23 08:47:20.000000 getactivewindow_x-0.3.0/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    35149 2021-10-23 08:47:20.000000 getactivewindow_x-0.3.0/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1522 2023-06-03 11:52:08.550190 getactivewindow_x-0.3.0/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      972 2023-06-03 11:50:35.000000 getactivewindow_x-0.3.0/README.md
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-03 11:52:08.550190 getactivewindow_x-0.3.0/getactivewindow/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1016 2023-06-03 02:30:07.000000 getactivewindow_x-0.3.0/getactivewindow/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:49:14.000000 getactivewindow_x-0.3.0/getactivewindow/py.typed
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-03 11:52:08.550190 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1522 2023-06-03 11:52:08.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      340 2023-06-03 11:52:08.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-03 11:52:08.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-03 11:52:08.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/requires.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       16 2023-06-03 11:52:08.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/top_level.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 08:59:29.000000 getactivewindow_x-0.3.0/getactivewindow_x.egg-info/zip-safe
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      679 2023-06-03 11:52:08.553524 getactivewindow_x-0.3.0/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       39 2021-10-23 08:48:11.000000 getactivewindow_x-0.3.0/setup.py
```

### Comparing `getactivewindow_x-0.2.1/.gitignore` & `getactivewindow_x-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `getactivewindow_x-0.2.1/LICENSE` & `getactivewindow_x-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getactivewindow_x-0.2.1/README.md` & `getactivewindow_x-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # getactivewindow-x
+
+# Deprecated
+
+maybe use `pywinctl` instead or one of the solutions in https://stackoverflow.com/q/10266281/5267751
+
+See also https://github.com/Kalmat/PyWinCtl/issues/64
+
+-----
+
 Separate component to get information on the active window in X.
 
+
 ### Why?
 
 In an attempt to be portable between operating systems.
 
 The user can install another package that provides the same interface.
 
 ### Internal details
 
-Use a fork of `python-libxdo`.
-
 There's another branch [user202729/getactivewindow-x at spawn-xdotool-xprop-process](https://github.com/user202729/getactivewindow-x/tree/spawn-xdotool-xprop-process)
 that uses subprocess, `xdotool` and `xprop`.
 
 ### API
 
 Currently there are only these functions.
```

### Comparing `getactivewindow_x-0.2.1/setup.cfg` & `getactivewindow_x-0.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = getactivewindow_x
-version = 0.2.1
+version = 0.3.0
 author = user202729
 description = Separate component to get information on the active window in X.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU General Public License v3 or later (GPLv3+)
 url = https://github.com/user202729/getactivewindow-x
 classifiers = 
@@ -14,13 +14,14 @@
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = True
 packages = 
 	getactivewindow
 install_requires = 
-	python-libxdo-ng==0.1.4
+	python-xlib~=0.29
+	ewmh~=0.1.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

