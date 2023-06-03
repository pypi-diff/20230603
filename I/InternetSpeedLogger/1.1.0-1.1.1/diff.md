# Comparing `tmp/InternetSpeedLogger-1.1.0.tar.gz` & `tmp/InternetSpeedLogger-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternetSpeedLogger-1.1.0.tar", last modified: Sat Jun  3 12:12:35 2023, max compression
+gzip compressed data, was "InternetSpeedLogger-1.1.1.tar", last modified: Sat Jun  3 13:02:15 2023, max compression
```

## Comparing `InternetSpeedLogger-1.1.0.tar` & `InternetSpeedLogger-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.552125 InternetSpeedLogger-1.1.0/
--rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.1.0/LICENSE
--rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 12:12:35.552125 InternetSpeedLogger-1.1.0/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)     3893 2023-06-03 12:11:32.000000 InternetSpeedLogger-1.1.0/README.md
--rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-03 11:33:46.000000 InternetSpeedLogger-1.1.0/pyproject.toml
--rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-03 12:12:35.553125 InternetSpeedLogger-1.1.0/setup.cfg
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.544125 InternetSpeedLogger-1.1.0/src/
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.547124 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/
--rw-r--r--   0 andreas   (1000) apache      (48)     4969 2023-06-03 12:11:39.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/InternetSpeedLogger.py
--rw-r--r--   0 andreas   (1000) apache      (48)        0 2023-06-03 07:33:53.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/__init__.py
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.551125 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/
--rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.236197 InternetSpeedLogger-1.1.1/
+-rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.1.1/LICENSE
+-rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 13:02:15.235197 InternetSpeedLogger-1.1.1/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)     3893 2023-06-03 12:11:32.000000 InternetSpeedLogger-1.1.1/README.md
+-rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-03 13:01:24.000000 InternetSpeedLogger-1.1.1/pyproject.toml
+-rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-03 13:02:15.236197 InternetSpeedLogger-1.1.1/setup.cfg
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.220197 InternetSpeedLogger-1.1.1/src/
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.225197 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/
+-rw-r--r--   0 andreas   (1000) apache      (48)     5026 2023-06-03 13:01:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/InternetSpeedLogger.py
+-rw-r--r--   0 andreas   (1000) apache      (48)        0 2023-06-03 07:33:53.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/__init__.py
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.234197 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/
+-rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/top_level.txt
```

### Comparing `InternetSpeedLogger-1.1.0/LICENSE` & `InternetSpeedLogger-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `InternetSpeedLogger-1.1.0/PKG-INFO` & `InternetSpeedLogger-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `InternetSpeedLogger-1.1.0/README.md` & `InternetSpeedLogger-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `InternetSpeedLogger-1.1.0/pyproject.toml` & `InternetSpeedLogger-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InternetSpeedLogger"
-version = "1.1.0"
+version = "1.1.1"
 dependencies = [
     "speedtest_cli"
 ]
 authors = [
   { name="Andreas Menzel", email="mail@andreas-menzel.com" },
 ]
 description = "A Python script that continuously monitors and logs your internet speed."
```

### Comparing `InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/InternetSpeedLogger.py` & `InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/InternetSpeedLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from datetime import datetime
 from pathlib import Path
 from signal import signal, SIGINT
 from speedtest import Speedtest
 from time import sleep
 
 
-script_version = '1.1.0'
+script_version = '1.1.1'
 
 
 def argparse_check_positive(value):
     ivalue = int(value)
     if ivalue <= 0:
         raise argparse.ArgumentTypeError("%s is an invalid positive int value" % value)
     return ivalue
@@ -59,15 +59,15 @@
                         type=argparse_check_positive,
                         default=60)
     parser.add_argument('-d', '--duration',
                         help='Duration of the entire test runs. The script will automatically end after this duration. Set to <= 0 for infinite. (default: %(default)s)',
                         type=int,
                         default=0)
     parser.add_argument('-l', '--log_file',
-                        help='Filename for the log-file. NOTE: ".csv" will be automatically appended to the filename!',
+                        help='Filename for the log-file. NOTE: The file will be overwritten if it already exists. NOTE: ".csv" will be automatically appended to the filename!',
                         default='')
     return parser.parse_args()
 
 
 def main():
     args = setupArgumentParser()
 
@@ -104,15 +104,15 @@
         print(f'\tDownload: ', end='')
         download = st.download()
         print(f'{round(download / 1000000)} Mbps')
         print(f'\tUpload: ', end='')
         upload = st.upload()
         print(f'{round(upload / 1000000)} Mbps')
 
-        with open(csv_file, mode='w') as file:
+        with open(csv_file, mode='a') as file:
             writer = csv.writer(file)
             writer.writerow([
                 testing_timestamp,
                 download,
                 upload,
 
                 testing_time.strftime("%Y-%m-%d %H:%M:%S"),
```

### Comparing `InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/PKG-INFO` & `InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

