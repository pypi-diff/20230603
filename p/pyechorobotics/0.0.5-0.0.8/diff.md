# Comparing `tmp/pyechorobotics-0.0.5.tar.gz` & `tmp/pyechorobotics-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechorobotics-0.0.5.tar", last modified: Wed May 31 21:21:38 2023, max compression
+gzip compressed data, was "pyechorobotics-0.0.8.tar", last modified: Sat Jun  3 13:05:32 2023, max compression
```

## Comparing `pyechorobotics-0.0.5.tar` & `pyechorobotics-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:21:38.000968 pyechorobotics-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 21:21:38.000968 pyechorobotics-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 21:21:38.000968 pyechorobotics-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:21:37.996968 pyechorobotics-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:21:38.000968 pyechorobotics-0.0.5/src/echoroboticsapi/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/src/echoroboticsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/src/echoroboticsapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-31 21:21:21.000000 pyechorobotics-0.0.5/src/echoroboticsapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:21:38.000968 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 21:21:37.000000 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 21:21:37.000000 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:21:37.000000 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:21:37.000000 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:21:37.000000 pyechorobotics-0.0.5/src/pyechorobotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/echoroboticsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/smart_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/top_level.txt
```

### Comparing `pyechorobotics-0.0.5/LICENSE.md` & `pyechorobotics-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.5/PKG-INFO` & `pyechorobotics-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pyechorobotics
-Version: 0.0.5
-Summary: Access API for echorobotics robot lawn mowers
-Author-email: functionpointer <suspendfunction@gmail.com>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 pyechorobotics
 =============
 
 ![echorobotics_logo](https://brands.home-assistant.io/_/echorobotics/logo@2x.png)
 
 Allows control and reads status of robot lawn mowers by echorobotics.
 
@@ -36,10 +23,41 @@
 
 
 if __name__ == "__main__":
     logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     loop = asyncio.new_event_loop()
     loop.run_until_complete(main())
 
+```
+
+Unfortunately, the API doesn't tell is which mode the robot is in.
+We can make an educated guess though, depending on what we set ourselves, history events and the status.
+This is what SmartMode does:
+
+```python
+import sys
+
+import echoroboticsapi
+import aiohttp
+import asyncio
+import logging
+
+
+async def main():
+    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
+        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
+        smartmode = echoroboticsapi.SmartMode("your-robot-id")
+        api.register_smart_mode(smartmode)
+        
+        print(await api.history_list())
+        print(await api.last_statuses())
+        print(await smartmode.get_robot_mode())
+
+
+if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+
 ```
 
 See also src/main.py
```

### Comparing `pyechorobotics-0.0.5/pyproject.toml` & `pyechorobotics-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "pyechorobotics"
-version = "0.0.5"
+version = "0.0.8"
 dependencies = [
     "aiohttp",
     "yarl",
     "pydantic",
+    "python-dateutil"
 ]
 readme = "README.md"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
 description = "Access API for echorobotics robot lawn mowers"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyechorobotics-0.0.5/src/pyechorobotics.egg-info/PKG-INFO` & `pyechorobotics-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.5
+Version: 0.0.8
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
@@ -36,10 +36,41 @@
 
 
 if __name__ == "__main__":
     logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     loop = asyncio.new_event_loop()
     loop.run_until_complete(main())
 
+```
+
+Unfortunately, the API doesn't tell is which mode the robot is in.
+We can make an educated guess though, depending on what we set ourselves, history events and the status.
+This is what SmartMode does:
+
+```python
+import sys
+
+import echoroboticsapi
+import aiohttp
+import asyncio
+import logging
+
+
+async def main():
+    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
+        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
+        smartmode = echoroboticsapi.SmartMode("your-robot-id")
+        api.register_smart_mode(smartmode)
+        
+        print(await api.history_list())
+        print(await api.last_statuses())
+        print(await smartmode.get_robot_mode())
+
+
+if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+
 ```
 
 See also src/main.py
```

