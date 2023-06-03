# Comparing `tmp/tablepy_lib-0.7.0.tar.gz` & `tmp/tablepy_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.7.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.8.0.tar", max compression
```

## Comparing `tablepy_lib-0.7.0.tar` & `tablepy_lib-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0      504 2023-05-29 19:12:21.590034 tablepy_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1830 2023-05-29 18:11:55.249238 tablepy_lib-0.7.0/README.md
--rw-r--r--   0        0        0      496 2023-05-29 19:12:41.683383 tablepy_lib-0.7.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     4552 2023-05-29 19:12:26.039182 tablepy_lib-0.7.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 tablepy_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0      504 2023-06-03 14:57:18.526235 tablepy_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2023-06-03 14:40:56.423707 tablepy_lib-0.8.0/README.md
+-rw-r--r--   0        0        0      496 2023-05-29 19:12:41.683383 tablepy_lib-0.8.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     4552 2023-06-03 14:21:25.503566 tablepy_lib-0.8.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 tablepy_lib-0.8.0/PKG-INFO
```

### Comparing `tablepy_lib-0.7.0/LICENSE` & `tablepy_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.7.0/README.md` & `tablepy_lib-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # tablepy Lib
 
 This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 
-## Usage - Markdown
+## Download Stats
+
+https://pypistats.org/packages/tablepy-lib
+
+## Notebook for testing
+
+https://github.com/JordiCorbilla/tablepy-lib/blob/main/Test%20Package.ipynb
+
+## Usage: Output as Markdown/console
 
 ```python
 from tablepy_lib import markdown
 
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
@@ -32,15 +40,15 @@
 | Name    | Age      | Country   | Data      | 
 | ------- | -------- | --------- | --------- | 
 | John    | -28.0    | USA       | USA       | 
 | Emily   | 3002.6   | Canada    | Canada    | 
 | Tom     | 25.0     | UK        | UK        | 
 | JC      | 2.0      | DE        | 3434243   | 
 
-## Usage - SQL Insert
+## Usage: Output as SQL Insert
 
 ```python
 from tablepy_lib import sql_insert
 
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
```

### Comparing `tablepy_lib-0.7.0/tablepy_lib/consoleFormatter.py` & `tablepy_lib-0.8.0/tablepy_lib/consoleFormatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #----------------------------------------------------------------------------
 # Created By  : Jordi Corbilla
 # Created Date: 2023
-# version ='0.7.0'
+# version ='0.8.0'
 # ---------------------------------------------------------------------------
 
 import pandas as pd
 
 class ConsoleFormatter:
     def __init__(self, data):
         if isinstance(data, dict):
```

### Comparing `tablepy_lib-0.7.0/PKG-INFO` & `tablepy_lib-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: tablepy-lib
-Version: 0.7.0
+Version: 0.8.0
 Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 Author: Jordi Corbilla
 Author-email: jordi.coll.corbilla@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # tablepy Lib
 
 This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 
-## Usage - Markdown
+## Download Stats
+
+https://pypistats.org/packages/tablepy-lib
+
+## Notebook for testing
+
+https://github.com/JordiCorbilla/tablepy-lib/blob/main/Test%20Package.ipynb
+
+## Usage: Output as Markdown/console
 
 ```python
 from tablepy_lib import markdown
 
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
@@ -45,15 +53,15 @@
 | Name    | Age      | Country   | Data      | 
 | ------- | -------- | --------- | --------- | 
 | John    | -28.0    | USA       | USA       | 
 | Emily   | 3002.6   | Canada    | Canada    | 
 | Tom     | 25.0     | UK        | UK        | 
 | JC      | 2.0      | DE        | 3434243   | 
 
-## Usage - SQL Insert
+## Usage: Output as SQL Insert
 
 ```python
 from tablepy_lib import sql_insert
 
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
```

