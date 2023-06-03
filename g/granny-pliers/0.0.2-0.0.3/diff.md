# Comparing `tmp/granny-pliers-0.0.2.tar.gz` & `tmp/granny-pliers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.2.tar", last modified: Sat Jun  3 16:39:48 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.3.tar", last modified: Sat Jun  3 18:43:39 2023, max compression
```

## Comparing `granny-pliers-0.0.2.tar` & `granny-pliers-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,28 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 16:39:48.612045 granny-pliers-0.0.2/
--rw-r--r--   0 pd         (501) staff       (20)    11347 2023-06-03 16:31:16.000000 granny-pliers-0.0.2/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13849 2023-06-03 16:39:48.611665 granny-pliers-0.0.2/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.2/README.md
--rw-r--r--   0 pd         (501) staff       (20)     1643 2023-06-03 16:39:35.000000 granny-pliers-0.0.2/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-03 16:39:48.612122 granny-pliers-0.0.2/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 16:39:48.608648 granny-pliers-0.0.2/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 16:39:48.609800 granny-pliers-0.0.2/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)        0 2023-06-03 16:26:43.000000 granny-pliers-0.0.2/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 16:39:48.611269 granny-pliers-0.0.2/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13849 2023-06-03 16:39:48.000000 granny-pliers-0.0.2/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      266 2023-06-03 16:39:48.000000 granny-pliers-0.0.2/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-03 16:39:48.000000 granny-pliers-0.0.2/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      220 2023-06-03 16:39:48.000000 granny-pliers-0.0.2/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-03 16:39:48.000000 granny-pliers-0.0.2/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.855710 granny-pliers-0.0.3/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-03 18:43:39.855428 granny-pliers-0.0.3/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.3/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1666 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-03 18:43:39.855793 granny-pliers-0.0.3/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.848601 granny-pliers-0.0.3/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.850184 granny-pliers-0.0.3/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.853227 granny-pliers-0.0.3/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      865 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4527 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1662 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     5918 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.854366 granny-pliers-0.0.3/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      859 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.854930 granny-pliers-0.0.3/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5091 2023-06-03 18:43:25.000000 granny-pliers-0.0.3/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 18:43:39.851762 granny-pliers-0.0.3/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-03 18:43:39.000000 granny-pliers-0.0.3/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      687 2023-06-03 18:43:39.000000 granny-pliers-0.0.3/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-03 18:43:39.000000 granny-pliers-0.0.3/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      235 2023-06-03 18:43:39.000000 granny-pliers-0.0.3/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-03 18:43:39.000000 granny-pliers-0.0.3/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.2/LICENSE` & `granny-pliers-0.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 Dmytro Stepanenko
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `granny-pliers-0.0.2/PKG-INFO` & `granny-pliers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2022 Dmytro Stepanenko
+           Copyright {yyyy} {name of copyright owner}
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `granny-pliers-0.0.2/pyproject.toml` & `granny-pliers-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "granny-pliers"
-version = "0.0.2"
+version = "0.0.3"
 
 authors = [
     { name = "Dmytro Stepanenko", email = "dmitrijstepanenko@gmail.com" },
 ]
 
 license = { file = "LICENSE" }
 
@@ -46,27 +46,28 @@
     "PyYAML>=6.0; python_version>='3.8'",
 ]
 
 [project.optional-dependencies]
 # Dev dependencies.
 dev = [
     "black>=22.3.0",
+    "pylint>=2.17.4",
 ]
 
 # Test dependencies.
 test = [
     "coverage>=7.2.7",
     "pytest>=7.3.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dimastepanenko/granny-pliers.git"
 
 [tool.black]
-line-length = 79
+line-length = 120
 include = '\.pyi?$' # All Python files
 exclude = '''
 /(
     \.git
   | build
   | dist
   | tool-belt
```

### Comparing `granny-pliers-0.0.2/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.3/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2022 Dmytro Stepanenko
+           Copyright {yyyy} {name of copyright owner}
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

