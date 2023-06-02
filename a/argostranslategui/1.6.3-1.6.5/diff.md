# Comparing `tmp/argostranslategui-1.6.3.tar.gz` & `tmp/argostranslategui-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argostranslategui-1.6.3.tar", last modified: Thu Dec 23 14:43:22 2021, max compression
+gzip compressed data, was "argostranslategui-1.6.5.tar", last modified: Fri Jun  2 23:52:00 2023, max compression
```

## Comparing `argostranslategui-1.6.3.tar` & `argostranslategui-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      857 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/PKG-INFO
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      409 2021-12-23 01:34:58.000000 argostranslategui-1.6.3/README.md
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/argostranslategui/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)        0 2021-12-23 02:36:36.000000 argostranslategui-1.6.3/argostranslategui/__init__.py
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)    17724 2021-12-23 13:58:32.000000 argostranslategui-1.6.3/argostranslategui/gui.py
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/argostranslategui.egg-info/
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      857 2021-12-23 14:43:21.000000 argostranslategui-1.6.3/argostranslategui.egg-info/PKG-INFO
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      301 2021-12-23 14:43:21.000000 argostranslategui-1.6.3/argostranslategui.egg-info/SOURCES.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)        1 2021-12-23 14:43:21.000000 argostranslategui-1.6.3/argostranslategui.egg-info/dependency_links.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       29 2021-12-23 14:43:21.000000 argostranslategui-1.6.3/argostranslategui.egg-info/requires.txt
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       18 2021-12-23 14:43:21.000000 argostranslategui-1.6.3/argostranslategui.egg-info/top_level.txt
-drwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)        0 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/bin/
--rwxrwxr-x   0 argosopentech  (1001) argosopentech  (1003)       71 2021-12-23 01:44:33.000000 argostranslategui-1.6.3/bin/argos-translate-gui
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)       38 2021-12-23 14:43:22.014015 argostranslategui-1.6.3/setup.cfg
--rw-rw-r--   0 argosopentech  (1001) argosopentech  (1003)      924 2021-12-23 13:59:32.000000 argostranslategui-1.6.3/setup.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-06-02 23:52:00.314861 argostranslategui-1.6.5/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1072 2023-06-02 23:35:22.000000 argostranslategui-1.6.5/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3337 2023-06-02 23:52:00.314861 argostranslategui-1.6.5/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3006 2023-06-02 23:35:22.000000 argostranslategui-1.6.5/README.md
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-06-02 23:52:00.310861 argostranslategui-1.6.5/argostranslategui/
+-rw-rw-r--   0 pj        (1000) pj        (1000)        0 2023-06-02 23:35:22.000000 argostranslategui-1.6.5/argostranslategui/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    17767 2023-06-02 23:46:11.000000 argostranslategui-1.6.5/argostranslategui/gui.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-06-02 23:52:00.314861 argostranslategui-1.6.5/argostranslategui.egg-info/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3337 2023-06-02 23:52:00.000000 argostranslategui-1.6.5/argostranslategui.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      309 2023-06-02 23:52:00.000000 argostranslategui-1.6.5/argostranslategui.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2023-06-02 23:52:00.000000 argostranslategui-1.6.5/argostranslategui.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       35 2023-06-02 23:52:00.000000 argostranslategui-1.6.5/argostranslategui.egg-info/requires.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       18 2023-06-02 23:52:00.000000 argostranslategui-1.6.5/argostranslategui.egg-info/top_level.txt
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-06-02 23:52:00.314861 argostranslategui-1.6.5/bin/
+-rwxrwxr-x   0 pj        (1000) pj        (1000)       71 2023-06-02 23:35:22.000000 argostranslategui-1.6.5/bin/argos-translate-gui
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2023-06-02 23:52:00.314861 argostranslategui-1.6.5/setup.cfg
+-rw-rw-r--   0 pj        (1000) pj        (1000)      924 2023-06-02 23:50:38.000000 argostranslategui-1.6.5/setup.py
```

### Comparing `argostranslategui-1.6.3/argostranslategui/gui.py` & `argostranslategui-1.6.5/argostranslategui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from pathlib import Path
 import os
-from functools import partial
 from enum import Enum
+from functools import partial
+from pathlib import Path
 
-from PyQt5.QtWidgets import *
-from PyQt5.QtGui import *
+from argostranslate import package, settings, translate, utils
+from argostranslate.utils import error, info
 from PyQt5.QtCore import *
+from PyQt5.QtGui import *
+from PyQt5.QtWidgets import *
 
-from argostranslate import translate, package, settings, utils
-from argostranslate.utils import info, error
 
 class WorkerThread(QThread):
     """Runs a bound function on a thread"""
 
     def __init__(self, bound_worker_function):
         """Args:
         bound_worker_function (functools.partial)
@@ -108,14 +108,15 @@
         self.STRETCH_COLUMN_MIN_PADDING = 50
         self.horizontalHeader().setDefaultAlignment(Qt.AlignLeft)
 
         self.installed_packages = package.get_installed_packages()
 
     def get_packages(self):
         if self.table_content == self.TableContent.AVAILABLE:
+            package.update_package_index()
             packages = package.get_available_packages()
         elif self.table_content == self.TableContent.INSTALLED:
             packages = package.get_installed_packages()
         else:
             raise Exception("Invalid table content")
 
         # Filter sbd packages in GUI
```

### Comparing `argostranslategui-1.6.3/setup.py` & `argostranslategui-1.6.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # py2app
 APP = ["bin/argos-translate-gui"]
 DATA_FILES = []
 OPTIONS = {"packages": ["sentencepiece"], "iconfile": "argostranslate/img/icon.icns"}
 
 setup(
     name="argostranslategui",
-    version="1.6.3",
+    version="1.6.5",
     description="Graphical user interface for Argos Translate",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Argos Open Technologies, LLC",
     author_email="admin@argosopentech.com",
     url="https://www.argosopentech.com",
     packages=find_packages(),
```

