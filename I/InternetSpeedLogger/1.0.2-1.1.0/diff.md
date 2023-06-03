# Comparing `tmp/InternetSpeedLogger-1.0.2.tar.gz` & `tmp/InternetSpeedLogger-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternetSpeedLogger-1.0.2.tar", last modified: Sat Jun  3 09:01:34 2023, max compression
+gzip compressed data, was "InternetSpeedLogger-1.1.0.tar", last modified: Sat Jun  3 12:12:35 2023, max compression
```

## Comparing `InternetSpeedLogger-1.0.2.tar` & `InternetSpeedLogger-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 09:01:34.972960 InternetSpeedLogger-1.0.2/
--rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.0.2/LICENSE
--rw-r--r--   0 andreas   (1000) apache      (48)     4839 2023-06-03 09:01:34.971960 InternetSpeedLogger-1.0.2/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)     2919 2023-06-03 08:31:40.000000 InternetSpeedLogger-1.0.2/README.md
--rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-03 09:01:16.000000 InternetSpeedLogger-1.0.2/pyproject.toml
--rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-03 09:01:34.972960 InternetSpeedLogger-1.0.2/setup.cfg
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 09:01:34.958960 InternetSpeedLogger-1.0.2/src/
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 09:01:34.964960 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger/
--rw-r--r--   0 andreas   (1000) apache      (48)     1984 2023-06-03 08:57:19.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger/InternetSpeedLogger.py
--rw-r--r--   0 andreas   (1000) apache      (48)        0 2023-06-03 07:33:53.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger/__init__.py
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 09:01:34.970960 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/
--rw-r--r--   0 andreas   (1000) apache      (48)     4839 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-03 09:01:34.000000 InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.552125 InternetSpeedLogger-1.1.0/
+-rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.1.0/LICENSE
+-rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 12:12:35.552125 InternetSpeedLogger-1.1.0/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)     3893 2023-06-03 12:11:32.000000 InternetSpeedLogger-1.1.0/README.md
+-rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-03 11:33:46.000000 InternetSpeedLogger-1.1.0/pyproject.toml
+-rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-03 12:12:35.553125 InternetSpeedLogger-1.1.0/setup.cfg
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.544125 InternetSpeedLogger-1.1.0/src/
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.547124 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/
+-rw-r--r--   0 andreas   (1000) apache      (48)     4969 2023-06-03 12:11:39.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/InternetSpeedLogger.py
+-rw-r--r--   0 andreas   (1000) apache      (48)        0 2023-06-03 07:33:53.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger/__init__.py
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 12:12:35.551125 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/
+-rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-03 12:12:35.000000 InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/top_level.txt
```

### Comparing `InternetSpeedLogger-1.0.2/LICENSE` & `InternetSpeedLogger-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InternetSpeedLogger-1.0.2/PKG-INFO` & `InternetSpeedLogger-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,44 +41,66 @@
 
 This Python script periodically tests the internet speed of your network and
 logs the results in a CSV file. It uses the
 [speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
 internet speed. You can control the frequency of testing and duration of the
 entire test run via the script's parameters.
 
-## Dependencies
+## Installation
 
-The script relies on the
-[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure the
-internet speed.
-
-If you are installing InternetSpeedLogger manually, make sure that you have
-already installed all requirements:
+Just install using pip:
 
 ```bash
-pip install -r requirements.txt
+pip install InternetSpeedLogger
 ```
 
 ## Usage
 
-Simply run the script using Python 3:
+If you installed InternetSpeedLogger with pip, you should be able to simply
+execute the script from anywhere:
 
 ```bash
-python3 InternetSpeedTest.py
+InternetSpeedLogger
 ```
 
-You can configure the script by modifying the following variables:
+Type `InternetSpeedLogger --help` to get detailed execution information:
+
+```
+usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION]
+                           [-l LOG_FILE]
 
-- **interval_in_secs**: The frequency of testing in seconds. Make sure that the
-  interval is not shorter than the time needed for a single test.
-- **testing_duration_secs**: The total duration of the test run in seconds. The
-  script will automatically terminate after this duration. Set it to `<= 0` for
-  an infinite duration.
-- **csv_file**: The filename of the CSV file in which the test results will be
-  logged.
+A Python script that continuously monitors and logs your internet
+speed. It tests both download and upload speeds at regular intervals
+and records the data in a CSV file for easy analysis and tracking.
+Ideal for auditing your network performance or ISP reliability over
+time.
+            
+
+options:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -i INTERVAL, --interval INTERVAL
+                        Testing interval in seconds. Make sure that the
+                        interval is not shorter than the time needed for
+                        testing. (default: 60)
+  -d DURATION, --duration DURATION
+                        Duration of the entire test runs. The script will
+                        automatically end after this duration. Set to <= 0 for
+                        infinite. (default: 0)
+  -l LOG_FILE, --log_file LOG_FILE
+                        Filename for the log-file. NOTE: ".csv" will be
+                        automatically appended to the filename!
+
+Default location of the log-file:
+    A .csv-file will be created, which will contain all logged information.
+    Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
+    Default Location: typically "/home/<username>" on Linux
+                      typically "C:\Users\<username>" on Windows
+                      typically "/Users/<username>" on macOS
+```
 
 ## Contribution
 
 We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
 and work can make a real difference to its development.
 
 There are many ways to contribute:
```

### Comparing `InternetSpeedLogger-1.0.2/README.md` & `InternetSpeedLogger-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,44 +4,66 @@
 
 This Python script periodically tests the internet speed of your network and
 logs the results in a CSV file. It uses the
 [speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
 internet speed. You can control the frequency of testing and duration of the
 entire test run via the script's parameters.
 
-## Dependencies
+## Installation
 
-The script relies on the
-[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure the
-internet speed.
-
-If you are installing InternetSpeedLogger manually, make sure that you have
-already installed all requirements:
+Just install using pip:
 
 ```bash
-pip install -r requirements.txt
+pip install InternetSpeedLogger
 ```
 
 ## Usage
 
-Simply run the script using Python 3:
+If you installed InternetSpeedLogger with pip, you should be able to simply
+execute the script from anywhere:
 
 ```bash
-python3 InternetSpeedTest.py
+InternetSpeedLogger
 ```
 
-You can configure the script by modifying the following variables:
+Type `InternetSpeedLogger --help` to get detailed execution information:
+
+```
+usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION]
+                           [-l LOG_FILE]
 
-- **interval_in_secs**: The frequency of testing in seconds. Make sure that the
-  interval is not shorter than the time needed for a single test.
-- **testing_duration_secs**: The total duration of the test run in seconds. The
-  script will automatically terminate after this duration. Set it to `<= 0` for
-  an infinite duration.
-- **csv_file**: The filename of the CSV file in which the test results will be
-  logged.
+A Python script that continuously monitors and logs your internet
+speed. It tests both download and upload speeds at regular intervals
+and records the data in a CSV file for easy analysis and tracking.
+Ideal for auditing your network performance or ISP reliability over
+time.
+            
+
+options:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -i INTERVAL, --interval INTERVAL
+                        Testing interval in seconds. Make sure that the
+                        interval is not shorter than the time needed for
+                        testing. (default: 60)
+  -d DURATION, --duration DURATION
+                        Duration of the entire test runs. The script will
+                        automatically end after this duration. Set to <= 0 for
+                        infinite. (default: 0)
+  -l LOG_FILE, --log_file LOG_FILE
+                        Filename for the log-file. NOTE: ".csv" will be
+                        automatically appended to the filename!
+
+Default location of the log-file:
+    A .csv-file will be created, which will contain all logged information.
+    Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
+    Default Location: typically "/home/<username>" on Linux
+                      typically "C:\Users\<username>" on Windows
+                      typically "/Users/<username>" on macOS
+```
 
 ## Contribution
 
 We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
 and work can make a real difference to its development.
 
 There are many ways to contribute:
```

### Comparing `InternetSpeedLogger-1.0.2/pyproject.toml` & `InternetSpeedLogger-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InternetSpeedLogger"
-version = "1.0.2"
+version = "1.1.0"
 dependencies = [
     "speedtest_cli"
 ]
 authors = [
   { name="Andreas Menzel", email="mail@andreas-menzel.com" },
 ]
 description = "A Python script that continuously monitors and logs your internet speed."
```

### Comparing `InternetSpeedLogger-1.0.2/src/InternetSpeedLogger.egg-info/PKG-INFO` & `InternetSpeedLogger-1.1.0/src/InternetSpeedLogger.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,44 +41,66 @@
 
 This Python script periodically tests the internet speed of your network and
 logs the results in a CSV file. It uses the
 [speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
 internet speed. You can control the frequency of testing and duration of the
 entire test run via the script's parameters.
 
-## Dependencies
+## Installation
 
-The script relies on the
-[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure the
-internet speed.
-
-If you are installing InternetSpeedLogger manually, make sure that you have
-already installed all requirements:
+Just install using pip:
 
 ```bash
-pip install -r requirements.txt
+pip install InternetSpeedLogger
 ```
 
 ## Usage
 
-Simply run the script using Python 3:
+If you installed InternetSpeedLogger with pip, you should be able to simply
+execute the script from anywhere:
 
 ```bash
-python3 InternetSpeedTest.py
+InternetSpeedLogger
 ```
 
-You can configure the script by modifying the following variables:
+Type `InternetSpeedLogger --help` to get detailed execution information:
+
+```
+usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION]
+                           [-l LOG_FILE]
 
-- **interval_in_secs**: The frequency of testing in seconds. Make sure that the
-  interval is not shorter than the time needed for a single test.
-- **testing_duration_secs**: The total duration of the test run in seconds. The
-  script will automatically terminate after this duration. Set it to `<= 0` for
-  an infinite duration.
-- **csv_file**: The filename of the CSV file in which the test results will be
-  logged.
+A Python script that continuously monitors and logs your internet
+speed. It tests both download and upload speeds at regular intervals
+and records the data in a CSV file for easy analysis and tracking.
+Ideal for auditing your network performance or ISP reliability over
+time.
+            
+
+options:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -i INTERVAL, --interval INTERVAL
+                        Testing interval in seconds. Make sure that the
+                        interval is not shorter than the time needed for
+                        testing. (default: 60)
+  -d DURATION, --duration DURATION
+                        Duration of the entire test runs. The script will
+                        automatically end after this duration. Set to <= 0 for
+                        infinite. (default: 0)
+  -l LOG_FILE, --log_file LOG_FILE
+                        Filename for the log-file. NOTE: ".csv" will be
+                        automatically appended to the filename!
+
+Default location of the log-file:
+    A .csv-file will be created, which will contain all logged information.
+    Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
+    Default Location: typically "/home/<username>" on Linux
+                      typically "C:\Users\<username>" on Windows
+                      typically "/Users/<username>" on macOS
+```
 
 ## Contribution
 
 We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
 and work can make a real difference to its development.
 
 There are many ways to contribute:
```

