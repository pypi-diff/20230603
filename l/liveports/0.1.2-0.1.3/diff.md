# Comparing `tmp/liveports-0.1.2.tar.gz` & `tmp/liveports-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.2.tar", last modified: Fri Jun  2 21:54:24 2023, max compression
+gzip compressed data, was "liveports-0.1.3.tar", last modified: Fri Jun  2 22:07:49 2023, max compression
```

## Comparing `liveports-0.1.2.tar` & `liveports-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 21:54:24.249240 liveports-0.1.2/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 21:54:24.249240 liveports-0.1.2/PKG-INFO
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 21:54:24.249240 liveports-0.1.2/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.2/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1.2/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6083 2023-06-02 21:50:13.000000 liveports-0.1.2/liveports/client.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 21:54:24.249240 liveports-0.1.2/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 21:54:24.000000 liveports-0.1.2/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      245 2023-06-02 21:54:24.000000 liveports-0.1.2/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 21:54:24.000000 liveports-0.1.2/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 21:54:24.000000 liveports-0.1.2/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 21:54:24.000000 liveports-0.1.2/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 21:54:24.249240 liveports-0.1.2/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      421 2023-06-02 21:47:28.000000 liveports-0.1.2/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:07:49.350569 liveports-0.1.3/PKG-INFO
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.3/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1.3/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5942 2023-06-02 22:01:34.000000 liveports-0.1.3/liveports/client.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      277 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       17 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 22:07:49.350569 liveports-0.1.3/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      400 2023-06-02 22:03:35.000000 liveports-0.1.3/setup.py
```

### Comparing `liveports-0.1.2/liveports/blaster_utils.py` & `liveports-0.1.3/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1.2/liveports/client.py` & `liveports-0.1.3/liveports/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import socket
 import signal
+import requests
 from collections import deque
-import urllib3
 import os
 import sys
 import ssl
 import json
 import threading
 import http.server
 import http.client
 import urllib
 import socketserver
 import fcntl
-from blaster_utils import run_shell, CommandLineArgs, DummyObject
+from .blaster_utils import run_shell, CommandLineArgs, DummyObject
 
-http_requester = urllib3.PoolManager()
-
-urllib3.disable_warnings()
+requests.packages.urllib3.disable_warnings()
 
 ssl_context = ssl.create_default_context()
 ssl_context.check_hostname = False
 ssl_context.verify_mode = ssl.CERT_NONE
 
 socketserver.TCPServer.allow_reuse_address = True
 
@@ -163,24 +161,21 @@
 		cache = json.loads(os.path.isfile(SERVER_CACHED_RESP_FILE) and open(SERVER_CACHED_RESP_FILE).read().strip() or "{}")
 		cache_file = open(SERVER_CACHED_RESP_FILE, "w")
 		try:
 			fcntl.flock(cache_file.fileno(), fcntl.LOCK_EX)
 
 			prev_resp = cache.get(SOURCE) or {}
 			server_hostname = prev_resp.get("server_hostname") or "ports.live"
-			resp = json.loads(
-				http_requester.urlopen(
-					'POST', "https://" + server_hostname + "/api/register",
-					headers={'Content-Type': 'application/json'},
-					body=json.dumps({
-						"source": SOURCE,
-						"api_key": CommandLineArgs.get("api_key", prev_resp.get("api_key"))
-					})
-				).data.decode('utf-8')
-			)
+			resp = requests.post(
+				"https://" + server_hostname + "/api/register",
+				json={
+					"source": SOURCE,
+					"api_key": CommandLineArgs.get("api_key", prev_resp.get("api_key"))
+				}
+			).json()
 			# update the previously cached data and cache it
 			prev_resp.update(resp)
 			cache[SOURCE] = resp
 			cache_file.write(json.dumps(cache))
 
 			if(resp.get("errors")):
 				for k, v in resp["errors"].items():
```

