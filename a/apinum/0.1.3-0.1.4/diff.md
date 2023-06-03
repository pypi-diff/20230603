# Comparing `tmp/apinum-0.1.3.tar.gz` & `tmp/apinum-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinum-0.1.3.tar", last modified: Sat Jun  3 17:48:22 2023, max compression
+gzip compressed data, was "apinum-0.1.4.tar", last modified: Sat Jun  3 17:54:16 2023, max compression
```

## Comparing `apinum-0.1.3.tar` & `apinum-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:22.356082 apinum-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:48:09.000000 apinum-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:48:22.356082 apinum-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:48:09.000000 apinum-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 17:48:09.000000 apinum-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:48:22.356082 apinum-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:22.356082 apinum-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:22.356082 apinum-0.1.3/src/apinum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:09.000000 apinum-0.1.3/src/apinum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-03 17:48:09.000000 apinum-0.1.3/src/apinum/apinum.py
--rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:48:09.000000 apinum-0.1.3/src/apinum/well_number_to_state_county.json
--rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:48:09.000000 apinum-0.1.3/src/apinum/well_numbers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:22.356082 apinum-0.1.3/src/apinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:48:22.000000 apinum-0.1.3/src/apinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:48:22.000000 apinum-0.1.3/src/apinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:48:22.000000 apinum-0.1.3/src/apinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 17:48:22.000000 apinum-0.1.3/src/apinum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:48:22.000000 apinum-0.1.3/src/apinum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:48:22.356082 apinum-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:48:09.000000 apinum-0.1.3/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:16.254599 apinum-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:54:05.000000 apinum-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:54:16.254599 apinum-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:54:05.000000 apinum-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-03 17:54:05.000000 apinum-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:54:16.254599 apinum-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:16.250599 apinum-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:16.250599 apinum-0.1.4/src/apinum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:05.000000 apinum-0.1.4/src/apinum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-03 17:54:05.000000 apinum-0.1.4/src/apinum/apinum.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:54:05.000000 apinum-0.1.4/src/apinum/well_number_to_state_county.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:54:05.000000 apinum-0.1.4/src/apinum/well_numbers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:16.254599 apinum-0.1.4/src/apinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:54:16.000000 apinum-0.1.4/src/apinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:54:16.000000 apinum-0.1.4/src/apinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:54:16.000000 apinum-0.1.4/src/apinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 17:54:16.000000 apinum-0.1.4/src/apinum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:54:16.000000 apinum-0.1.4/src/apinum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:54:16.254599 apinum-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:54:05.000000 apinum-0.1.4/tests/tests.py
```

### Comparing `apinum-0.1.3/src/apinum/apinum.py` & `apinum-0.1.4/src/apinum/apinum.py`

 * *Files identical despite different names*

### Comparing `apinum-0.1.3/src/apinum/well_number_to_state_county.json` & `apinum-0.1.4/src/apinum/well_number_to_state_county.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.3/src/apinum/well_numbers.json` & `apinum-0.1.4/src/apinum/well_numbers.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.3/tests/tests.py` & `apinum-0.1.4/tests/tests.py`

 * *Files identical despite different names*

