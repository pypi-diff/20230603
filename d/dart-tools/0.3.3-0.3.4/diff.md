# Comparing `tmp/dart-tools-0.3.3.tar.gz` & `tmp/dart-tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.3.tar", last modified: Sat Jun  3 08:11:34 2023, max compression
+gzip compressed data, was "dart-tools-0.3.4.tar", last modified: Sat Jun  3 17:38:16 2023, max compression
```

## Comparing `dart-tools-0.3.3.tar` & `dart-tools-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.682972 dart-tools-0.3.3/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.3/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 08:11:34.682638 dart-tools-0.3.3/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.3/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.678812 dart-tools-0.3.3/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.3/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    12980 2023-06-03 08:09:36.000000 dart-tools-0.3.3/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.3/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 08:11:34.682001 dart-tools-0.3.3/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-03 08:11:34.000000 dart-tools-0.3.3/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-03 08:09:48.000000 dart-tools-0.3.3/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-03 08:11:34.683100 dart-tools-0.3.3/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.996176 dart-tools-0.3.4/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.4/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 17:38:16.995762 dart-tools-0.3.4/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.4/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.989977 dart-tools-0.3.4/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.4/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    12986 2023-06-03 17:35:56.000000 dart-tools-0.3.4/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.4/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.994329 dart-tools-0.3.4/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.994825 dart-tools-0.3.4/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.4/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-03 17:36:01.000000 dart-tools-0.3.4/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-03 17:38:16.996348 dart-tools-0.3.4/setup.cfg
```

### Comparing `dart-tools-0.3.3/LICENSE` & `dart-tools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.3/PKG-INFO` & `dart-tools-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.3 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.4 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.3/README.md` & `dart-tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.3/dart/dart.py` & `dart-tools-0.3.4/dart/dart.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 _ROOT_API_URL_FRAG = "/api/v0"
 _CSRF_URL_FRAG = _ROOT_API_URL_FRAG + "/csrf-token"
 _LOGIN_URL_FRAG = _ROOT_API_URL_FRAG + "/login"
 _CURRENT_USER_URL_FRAG = _ROOT_API_URL_FRAG + "/current-user"
 _CREATE_TASK_URL_FRAG = _ROOT_API_URL_FRAG + "/tasks/create"
 _COPY_BRANCH_URL_FRAG = _ROOT_API_URL_FRAG + "/vcs/copy-branch-link"
 
-_CONFIG_FPATH = os.path.expanduser("~/.dart")
+_CONFIG_FPATH = os.path.expanduser("~/.dart-tools")
 _CSRF_TOKEN_COOKIE = "csrftoken"
 _SESSION_ID_COOKIE = "sessionid"
 _CLIENT_DUID_KEY = "clientDuid"
 _HOST_KEY = "host"
 _HOSTS_KEY = "hosts"
 _CSRF_TOKEN_KEY = "csrfToken"
 _SESSION_ID_KEY = "sessionId"
```

### Comparing `dart-tools-0.3.3/dart/order_manager.py` & `dart-tools-0.3.4/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.3/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.4/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.3 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.4 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.3/pyproject.toml` & `dart-tools-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.3"
+version = "0.3.4"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

