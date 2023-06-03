# Comparing `tmp/polywrapper-0.1.0.tar.gz` & `tmp/polywrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrapper-0.1.0.tar", last modified: Sat Jun  3 20:37:54 2023, max compression
+gzip compressed data, was "polywrapper-0.1.1.tar", last modified: Sat Jun  3 21:08:36 2023, max compression
```

## Comparing `polywrapper-0.1.0.tar` & `polywrapper-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 20:37:54.974179 polywrapper-0.1.0/
--rw-r--r--   0 david     (1000) david     (1000)     1065 2023-03-13 22:24:52.000000 polywrapper-0.1.0/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 20:37:54.974179 polywrapper-0.1.0/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 20:37:54.974179 polywrapper-0.1.0/polywrapper/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-03 20:17:23.000000 polywrapper-0.1.0/polywrapper/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     3715 2023-06-03 20:19:54.000000 polywrapper-0.1.0/polywrapper/polywrapper.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 20:37:54.974179 polywrapper-0.1.0/polywrapper.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 20:37:54.000000 polywrapper-0.1.0/polywrapper.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 20:37:54.000000 polywrapper-0.1.0/polywrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-03 20:37:54.000000 polywrapper-0.1.0/polywrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       17 2023-06-03 20:37:54.000000 polywrapper-0.1.0/polywrapper.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       12 2023-06-03 20:37:54.000000 polywrapper-0.1.0/polywrapper.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-03 20:37:54.974179 polywrapper-0.1.0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-03 20:18:37.000000 polywrapper-0.1.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:08:36.684252 polywrapper-0.1.1/
+-rw-r--r--   0 david     (1000) david     (1000)     1065 2023-03-13 22:24:52.000000 polywrapper-0.1.1/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:08:36.684252 polywrapper-0.1.1/PKG-INFO
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:08:36.684252 polywrapper-0.1.1/polywrapper/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-03 20:47:56.000000 polywrapper-0.1.1/polywrapper/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     3714 2023-06-03 20:49:10.000000 polywrapper-0.1.1/polywrapper/polywrapper.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:08:36.684252 polywrapper-0.1.1/polywrapper.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:08:36.000000 polywrapper-0.1.1/polywrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:08:36.000000 polywrapper-0.1.1/polywrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-03 21:08:36.000000 polywrapper-0.1.1/polywrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       17 2023-06-03 21:08:36.000000 polywrapper-0.1.1/polywrapper.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       12 2023-06-03 21:08:36.000000 polywrapper-0.1.1/polywrapper.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-03 21:08:36.684252 polywrapper-0.1.1/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-03 21:08:33.000000 polywrapper-0.1.1/setup.py
```

### Comparing `polywrapper-0.1.0/LICENSE` & `polywrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polywrapper-0.1.0/polywrapper/polywrapper.py` & `polywrapper-0.1.1/polywrapper/polywrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from websocket import create_connection
 import json
 import websocket
-class PolyWrapper:
+class PolyClient:
     def __init__(self, connection_url: str, password: str, db_name: str) -> None:
         """
         Initialize a PolyWrapper instance.
 
         Args:
             connection_url (str): The URL of the WebSocket connection.
             password (str): The password for accessing the database.
```

