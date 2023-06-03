# Comparing `tmp/apinum-0.1.1.tar.gz` & `tmp/apinum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinum-0.1.1.tar", last modified: Sat Jun  3 17:37:55 2023, max compression
+gzip compressed data, was "apinum-0.1.2.tar", last modified: Sat Jun  3 17:44:08 2023, max compression
```

## Comparing `apinum-0.1.1.tar` & `apinum-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.890182 apinum-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:37:44.000000 apinum-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:37:55.890182 apinum-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:37:44.000000 apinum-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 17:37:44.000000 apinum-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:37:55.890182 apinum-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/apinum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/apinum.py
--rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/well_number_to_state_county.json
--rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:37:44.000000 apinum-0.1.1/src/apinum/well_numbers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.886181 apinum-0.1.1/src/apinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:37:55.000000 apinum-0.1.1/src/apinum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:37:55.890182 apinum-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:37:44.000000 apinum-0.1.1/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:44:08.445268 apinum-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 17:43:58.000000 apinum-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:44:08.445268 apinum-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 17:43:58.000000 apinum-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 17:43:58.000000 apinum-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:44:08.445268 apinum-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:44:08.445268 apinum-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:44:08.445268 apinum-0.1.2/src/apinum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:43:58.000000 apinum-0.1.2/src/apinum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-03 17:43:58.000000 apinum-0.1.2/src/apinum/apinum.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144788 2023-06-03 17:43:58.000000 apinum-0.1.2/src/apinum/well_number_to_state_county.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49802 2023-06-03 17:43:58.000000 apinum-0.1.2/src/apinum/well_numbers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:44:08.445268 apinum-0.1.2/src/apinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 17:44:08.000000 apinum-0.1.2/src/apinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 17:44:08.000000 apinum-0.1.2/src/apinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:44:08.000000 apinum-0.1.2/src/apinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 17:44:08.000000 apinum-0.1.2/src/apinum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 17:44:08.000000 apinum-0.1.2/src/apinum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:44:08.445268 apinum-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-03 17:43:58.000000 apinum-0.1.2/tests/tests.py
```

### Comparing `apinum-0.1.1/src/apinum/apinum.py` & `apinum-0.1.2/src/apinum/apinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,7 +227,8 @@
                 self.wellbore_code
             )
             self.unformatted_10_digit = (
                 self.state_code +
                 self.county_code +
                 self.well_number
             )
+            return
```

### Comparing `apinum-0.1.1/src/apinum/well_number_to_state_county.json` & `apinum-0.1.2/src/apinum/well_number_to_state_county.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.1/src/apinum/well_numbers.json` & `apinum-0.1.2/src/apinum/well_numbers.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.1/tests/tests.py` & `apinum-0.1.2/tests/tests.py`

 * *Files identical despite different names*

