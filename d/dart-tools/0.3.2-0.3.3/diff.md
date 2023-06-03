# Comparing `tmp/dart-tools-0.3.2.tar.gz` & `tmp/dart-tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.2.tar", last modified: Fri Jun  2 19:36:14 2023, max compression
+gzip compressed data, was "dart-tools-0.3.3.tar", last modified: Sat Jun  3 08:11:34 2023, max compression
```

## Comparing `dart-tools-0.3.2.tar` & `dart-tools-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.269804 dart-tools-0.3.2/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.2/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:36:14.269264 dart-tools-0.3.2/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.2/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.265427 dart-tools-0.3.2/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.2/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    12953 2023-06-02 19:35:29.000000 dart-tools-0.3.2/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.2/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.268422 dart-tools-0.3.2/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-02 19:34:24.000000 dart-tools-0.3.2/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-02 19:36:14.270093 dart-tools-0.3.2/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.682972 dart-tools-0.3.3/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.3/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 08:11:34.682638 dart-tools-0.3.3/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.3/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.678812 dart-tools-0.3.3/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.3/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    12980 2023-06-03 08:09:36.000000 dart-tools-0.3.3/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.3/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.682001 dart-tools-0.3.3/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-03 08:09:48.000000 dart-tools-0.3.3/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-03 08:11:34.683100 dart-tools-0.3.3/setup.cfg
```

### Comparing `dart-tools-0.3.2/LICENSE` & `dart-tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.2/PKG-INFO` & `dart-tools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.2 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.3 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.2/README.md` & `dart-tools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.2/dart/dart.py` & `dart-tools-0.3.3/dart/dart.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
 def _get_task_url(host, duid):
     return f"{host}/search?t={duid}"
 
 
 class _Config:
     def __init__(self):
+        self._content = {}
         if os.path.isfile(_CONFIG_FPATH):
             with open(_CONFIG_FPATH, "r", encoding="UTF-8") as fin:
                 self._content = json.load(fin)
         self._content = {
             _CLIENT_DUID_KEY: _make_duid(),
             _HOST_KEY: _PROD_HOST,
             _HOSTS_KEY: {},
```

### Comparing `dart-tools-0.3.2/dart/order_manager.py` & `dart-tools-0.3.3/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.2/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.3/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.2 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.3 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.2/pyproject.toml` & `dart-tools-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.2"
+version = "0.3.3"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

