# Comparing `tmp/hathitrust-downloader-1.1.4.tar.gz` & `tmp/hathitrust-downloader-1.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hathitrust-downloader-1.1.4.tar", last modified: Sat Jun  3 11:08:06 2023, max compression
+gzip compressed data, was "hathitrust-downloader-1.1.4rc1.tar", last modified: Sat Jun  3 11:01:39 2023, max compression
```

## Comparing `hathitrust-downloader-1.1.4.tar` & `hathitrust-downloader-1.1.4rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:08:06.738592 hathitrust-downloader-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 11:07:55.000000 hathitrust-downloader-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-03 11:08:06.738592 hathitrust-downloader-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-03 11:07:55.000000 hathitrust-downloader-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:08:06.738592 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-03 11:08:06.000000 hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:08:06.738592 hathitrust-downloader-1.1.4/hathitrustdownloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 11:07:55.000000 hathitrust-downloader-1.1.4/hathitrustdownloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-03 11:07:55.000000 hathitrust-downloader-1.1.4/hathitrustdownloader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 11:08:06.738592 hathitrust-downloader-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-03 11:07:55.000000 hathitrust-downloader-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:01:39.175970 hathitrust-downloader-1.1.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 11:01:25.000000 hathitrust-downloader-1.1.4rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-03 11:01:39.175970 hathitrust-downloader-1.1.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-03 11:01:25.000000 hathitrust-downloader-1.1.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:01:39.175970 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-03 11:01:38.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 11:01:39.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:01:38.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 11:01:38.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-03 11:01:38.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-03 11:01:38.000000 hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:01:39.175970 hathitrust-downloader-1.1.4rc1/hathitrustdownloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 11:01:25.000000 hathitrust-downloader-1.1.4rc1/hathitrustdownloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-03 11:01:25.000000 hathitrust-downloader-1.1.4rc1/hathitrustdownloader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 11:01:39.175970 hathitrust-downloader-1.1.4rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-03 11:01:25.000000 hathitrust-downloader-1.1.4rc1/setup.py
```

### Comparing `hathitrust-downloader-1.1.4/LICENSE` & `hathitrust-downloader-1.1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hathitrust-downloader-1.1.4/PKG-INFO` & `hathitrust-downloader-1.1.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hathitrust-downloader
-Version: 1.1.4
+Version: 1.1.4rc1
 Summary: Downloads multiple pages from Hathitrust from the CLI.
 Home-page: http://github.com/addono/hathitrust-downloader
 Author: Adriaan Knapen
 Author-email: hi@aknapen.nl
 License: MIT
 Description: # HathiTrust Downloader
         [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square&logo=pypi)][pypi]
```

### Comparing `hathitrust-downloader-1.1.4/README.md` & `hathitrust-downloader-1.1.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `hathitrust-downloader-1.1.4/hathitrust_downloader.egg-info/PKG-INFO` & `hathitrust-downloader-1.1.4rc1/hathitrust_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hathitrust-downloader
-Version: 1.1.4
+Version: 1.1.4rc1
 Summary: Downloads multiple pages from Hathitrust from the CLI.
 Home-page: http://github.com/addono/hathitrust-downloader
 Author: Adriaan Knapen
 Author-email: hi@aknapen.nl
 License: MIT
 Description: # HathiTrust Downloader
         [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square&logo=pypi)][pypi]
```

### Comparing `hathitrust-downloader-1.1.4/hathitrustdownloader/cli.py` & `hathitrust-downloader-1.1.4rc1/hathitrustdownloader/cli.py`

 * *Files identical despite different names*

### Comparing `hathitrust-downloader-1.1.4/setup.py` & `hathitrust-downloader-1.1.4rc1/setup.py`

 * *Files identical despite different names*

