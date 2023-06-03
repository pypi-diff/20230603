# Comparing `tmp/eot-0.1.0.tar.gz` & `tmp/eot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eot-0.1.0.tar", last modified: Sat May 20 01:01:35 2023, max compression
+gzip compressed data, was "eot-0.1.1.tar", last modified: Sat Jun  3 19:54:25 2023, max compression
```

## Comparing `eot-0.1.0.tar` & `eot-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.155204 eot-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 01:01:35.155204 eot-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 01:01:14.000000 eot-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/eot/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/eot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/eot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 01:01:25.000000 eot-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-20 01:01:35.155204 eot-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 19:54:25.131075 eot-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 19:54:04.000000 eot-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.127075 eot-0.1.1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/pkg/eot/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-03 19:54:16.000000 eot-0.1.1/pkg/eot/eot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:54:25.131075 eot-0.1.1/pkg/eot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 19:54:25.000000 eot-0.1.1/pkg/eot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-03 19:54:16.000000 eot-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-03 19:54:25.135075 eot-0.1.1/setup.cfg
```

### Comparing `eot-0.1.0/PKG-INFO` & `eot-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eot-0.1.0/pkg/eot/eot.py` & `eot-0.1.1/pkg/eot/eot.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		exact_hour = hour * one_hour
 		exact_minute = now.minute * one_minute
 		exact_second = now.second * one_second
 		exact_decimal = exact_day + exact_hour + exact_minute + exact_second
 		decimal = float('%.8f' % (exact_decimal))
 		# error = decimal * 365 - day_of_year - (hour / 24)
 		# error_hours = error * 24
-		stardate = year + decimal
+		stardate = format(year + decimal, '.8f')
 
 		# print("stardate for", year, day_of_year, hour)
 		# print("error:", error, "in hours:", error_hours)
 		return stardate
 
 	#Called when executing this as a functor.
 	def __call__(this):
```

### Comparing `eot-0.1.0/pkg/eot.egg-info/PKG-INFO` & `eot-0.1.1/pkg/eot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eot-0.1.0/setup.cfg` & `eot-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eot
-version = 0.1.0
+version = 0.1.1
 author = eons
 author_email = support@eons.llc
 description = Eons Official Time
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_eot
```

