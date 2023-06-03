# Comparing `tmp/apinum-0.1.0.tar.gz` & `tmp/apinum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinum-0.1.0.tar", last modified: Sat Jun  3 17:13:26 2023, max compression
+gzip compressed data, was "apinum-0.1.1.tar", last modified: Sat Jun  3 17:37:55 2023, max compression
```

## Comparing `apinum-0.1.0.tar` & `apinum-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:26.745984 apinum-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:13:12.000000 apinum-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:13:26.745984 apinum-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:13:12.000000 apinum-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 17:13:12.000000 apinum-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:13:26.745984 apinum-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:26.741984 apinum-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:26.745984 apinum-0.1.0/src/apinum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:12.000000 apinum-0.1.0/src/apinum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-03 17:13:12.000000 apinum-0.1.0/src/apinum/apinum.py
--rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:13:12.000000 apinum-0.1.0/src/apinum/well_number_to_state_county.json
--rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:13:12.000000 apinum-0.1.0/src/apinum/well_numbers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:26.745984 apinum-0.1.0/src/apinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:13:26.000000 apinum-0.1.0/src/apinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:13:26.000000 apinum-0.1.0/src/apinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:13:26.000000 apinum-0.1.0/src/apinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 17:13:26.000000 apinum-0.1.0/src/apinum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:13:26.000000 apinum-0.1.0/src/apinum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:13:26.745984 apinum-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:13:12.000000 apinum-0.1.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.890182 apinum-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:37:44.000000 apinum-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:37:55.890182 apinum-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:37:44.000000 apinum-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 17:37:44.000000 apinum-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:37:55.890182 apinum-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/apinum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/apinum.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/well_number_to_state_county.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/well_numbers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/apinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.890182 apinum-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:37:44.000000 apinum-0.1.1/tests/tests.py
```

### Comparing `apinum-0.1.0/src/apinum/apinum.py` & `apinum-0.1.1/src/apinum/apinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 #     # If no well number is found, return None
 #     return None
 
 
 # Create a class for storing well numbers, parameters inlude, state code,
 # county code, well number, wellbore code, and completion code.
-class APINumber:
+class APINumber():
     """A class for storing API numbers. It accepts a string, a file_path
     to a LAS file, or a LASFile object as input. The class will attempt
     to extract the longest API number from the input.
 
     Args:
     -----
         input (str, LASFile): A string, a file_path to a LAS file, or a
```

### Comparing `apinum-0.1.0/src/apinum/well_number_to_state_county.json` & `apinum-0.1.1/src/apinum/well_number_to_state_county.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.0/src/apinum/well_numbers.json` & `apinum-0.1.1/src/apinum/well_numbers.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.0/tests/tests.py` & `apinum-0.1.1/tests/tests.py`

 * *Files identical despite different names*

