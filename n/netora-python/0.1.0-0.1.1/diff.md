# Comparing `tmp/netora-python-0.1.0.tar.gz` & `tmp/netora-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netora-python-0.1.0.tar", last modified: Sat Jun  3 04:19:24 2023, max compression
+gzip compressed data, was "netora-python-0.1.1.tar", last modified: Sat Jun  3 04:25:10 2023, max compression
```

## Comparing `netora-python-0.1.0.tar` & `netora-python-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 04:19:24.687075 netora-python-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-03 04:19:24.648179 netora-python-0.1.0/NetoraPy/
-drwxrwxrwx   0        0        0        0 2023-06-03 04:19:24.663151 netora-python-0.1.0/NetoraPy/NetoraTube/
--rw-rw-rw-   0        0        0    13523 2023-06-03 03:39:40.000000 netora-python-0.1.0/NetoraPy/NetoraTube/NTTube.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:19:21.000000 netora-python-0.1.0/NetoraPy/NetoraTube/__init__.py
--rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.0/NetoraPy/__init__.py
--rw-rw-rw-   0        0        0      414 2023-06-03 04:19:24.686081 netora-python-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 04:19:24.683094 netora-python-0.1.0/netora_python.egg-info/
--rw-rw-rw-   0        0        0      414 2023-06-03 04:19:24.000000 netora-python-0.1.0/netora_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-03 04:19:24.000000 netora-python-0.1.0/netora_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 04:19:24.000000 netora-python-0.1.0/netora_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 04:19:24.000000 netora-python-0.1.0/netora_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 04:19:24.000000 netora-python-0.1.0/netora_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 04:19:24.688073 netora-python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-03 04:15:49.000000 netora-python-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:25:10.190595 netora-python-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-03 04:25:10.128727 netora-python-0.1.1/NetoraPy/
+drwxrwxrwx   0        0        0        0 2023-06-03 04:25:10.155653 netora-python-0.1.1/NetoraPy/NetoraTube/
+-rw-rw-rw-   0        0        0    13523 2023-06-03 04:24:46.000000 netora-python-0.1.1/NetoraPy/NetoraTube/NetoraTube.py
+-rw-rw-rw-   0        0        0       44 2023-06-03 04:24:42.000000 netora-python-0.1.1/NetoraPy/NetoraTube/__init__.py
+-rw-rw-rw-   0        0        0       40 2023-06-03 04:17:44.000000 netora-python-0.1.1/NetoraPy/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-03 04:25:10.189595 netora-python-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 04:25:10.187604 netora-python-0.1.1/netora_python.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-06-03 04:25:09.000000 netora-python-0.1.1/netora_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-06-03 04:25:10.000000 netora-python-0.1.1/netora_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 04:25:09.000000 netora-python-0.1.1/netora_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 04:25:09.000000 netora-python-0.1.1/netora_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 04:25:09.000000 netora-python-0.1.1/netora_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 04:25:10.190595 netora-python-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-03 04:25:01.000000 netora-python-0.1.1/setup.py
```

### Comparing `netora-python-0.1.0/NetoraPy/NetoraTube/NTTube.py` & `netora-python-0.1.1/NetoraPy/NetoraTube/NetoraTube.py`

 * *Files identical despite different names*

### Comparing `netora-python-0.1.0/setup.py` & `netora-python-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A package with lots of features'
 
 # Setting up
 setup(
     name="netora-python",
     version=VERSION,
     author="JacksonLin",
```

