# Comparing `tmp/apinum-0.1.5.tar.gz` & `tmp/apinum-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinum-0.1.5.tar", last modified: Sat Jun  3 18:01:03 2023, max compression
+gzip compressed data, was "apinum-0.1.6.tar", last modified: Sat Jun  3 18:08:22 2023, max compression
```

## Comparing `apinum-0.1.5.tar` & `apinum-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:01:03.641565 apinum-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 18:00:53.000000 apinum-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 18:01:03.641565 apinum-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 18:00:53.000000 apinum-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-03 18:00:53.000000 apinum-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:01:03.641565 apinum-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:01:03.637565 apinum-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:01:03.641565 apinum-0.1.5/src/apinum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:00:53.000000 apinum-0.1.5/src/apinum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-03 18:00:53.000000 apinum-0.1.5/src/apinum/apinum.py
--rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 18:00:53.000000 apinum-0.1.5/src/apinum/well_number_to_state_county.json
--rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 18:00:53.000000 apinum-0.1.5/src/apinum/well_numbers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:01:03.641565 apinum-0.1.5/src/apinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 18:01:03.000000 apinum-0.1.5/src/apinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 18:01:03.000000 apinum-0.1.5/src/apinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:01:03.000000 apinum-0.1.5/src/apinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 18:01:03.000000 apinum-0.1.5/src/apinum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 18:01:03.000000 apinum-0.1.5/src/apinum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:01:03.641565 apinum-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 18:00:53.000000 apinum-0.1.5/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:08:22.815743 apinum-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 18:08:11.000000 apinum-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 18:08:22.815743 apinum-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 18:08:11.000000 apinum-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-03 18:08:11.000000 apinum-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:08:22.815743 apinum-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:08:22.811743 apinum-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:08:22.811743 apinum-0.1.6/src/apinum/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 18:08:11.000000 apinum-0.1.6/src/apinum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-03 18:08:11.000000 apinum-0.1.6/src/apinum/apinum.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 18:08:11.000000 apinum-0.1.6/src/apinum/well_number_to_state_county.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 18:08:11.000000 apinum-0.1.6/src/apinum/well_numbers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:08:22.815743 apinum-0.1.6/src/apinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 18:08:22.000000 apinum-0.1.6/src/apinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 18:08:22.000000 apinum-0.1.6/src/apinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:08:22.000000 apinum-0.1.6/src/apinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 18:08:22.000000 apinum-0.1.6/src/apinum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 18:08:22.000000 apinum-0.1.6/src/apinum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:08:22.815743 apinum-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 18:08:11.000000 apinum-0.1.6/tests/tests.py
```

### Comparing `apinum-0.1.5/src/apinum/apinum.py` & `apinum-0.1.6/src/apinum/apinum.py`

 * *Files identical despite different names*

### Comparing `apinum-0.1.5/src/apinum/well_number_to_state_county.json` & `apinum-0.1.6/src/apinum/well_number_to_state_county.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.5/src/apinum/well_numbers.json` & `apinum-0.1.6/src/apinum/well_numbers.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.5/tests/tests.py` & `apinum-0.1.6/tests/tests.py`

 * *Files identical despite different names*

