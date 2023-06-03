# Comparing `tmp/lidl-plus-0.2.5.tar.gz` & `tmp/lidl-plus-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidl-plus-0.2.5.tar", last modified: Wed May 24 22:34:02 2023, max compression
+gzip compressed data, was "lidl-plus-0.2.6.tar", last modified: Sat Jun  3 13:19:15 2023, max compression
```

## Comparing `lidl-plus-0.2.5.tar` & `lidl-plus-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:02.749868 lidl-plus-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-24 22:34:02.749868 lidl-plus-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:02.749868 lidl-plus-0.2.5/lidl_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 22:34:02.000000 lidl-plus-0.2.5/lidl_plus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:02.749868 lidl-plus-0.2.5/lidlplus/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/lidlplus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5112 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/lidlplus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/lidlplus/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/lidlplus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:34:02.749868 lidl-plus-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-24 22:33:49.000000 lidl-plus-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:19:15.504104 lidl-plus-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-03 13:19:15.504104 lidl-plus-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:19:15.500104 lidl-plus-0.2.6/lidl_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 13:19:15.000000 lidl-plus-0.2.6/lidl_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:19:15.504104 lidl-plus-0.2.6/lidlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/lidlplus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5112 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/lidlplus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/lidlplus/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/lidlplus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:19:15.504104 lidl-plus-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-03 13:19:03.000000 lidl-plus-0.2.6/setup.py
```

### Comparing `lidl-plus-0.2.5/LICENCE` & `lidl-plus-0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `lidl-plus-0.2.5/PKG-INFO` & `lidl-plus-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidl-plus
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fetch receipts and more from Lidl Plus
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/lidl-plus
 Project-URL: PyPI, https://pypi.org/project/lidl-plus/
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lidl-plus-0.2.5/README.md` & `lidl-plus-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lidl-plus-0.2.5/lidl_plus.egg-info/PKG-INFO` & `lidl-plus-0.2.6/lidl_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidl-plus
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fetch receipts and more from Lidl Plus
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/lidl-plus
 Project-URL: PyPI, https://pypi.org/project/lidl-plus/
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lidl-plus-0.2.5/lidlplus/__main__.py` & `lidl-plus-0.2.6/lidlplus/__main__.py`

 * *Files identical despite different names*

### Comparing `lidl-plus-0.2.5/lidlplus/api.py` & `lidl-plus-0.2.6/lidlplus/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class LidlPlusApi:
     """Lidl Plus api connector"""
 
     _CLIENT_ID = "LidlPlusNativeClient"
     _AUTH_API = "https://accounts.lidl.com"
-    _TICKET_API = "https://tickets.lidlplus.com/api/v1"
+    _TICKET_API = "https://tickets.lidlplus.com/api/v2"
     _APP = "com.lidlplus.app"
     _OS = "iOs"
     _TIMEOUT = 10
 
     def __init__(self, language, country, refresh_token=""):
         self._login_url = ""
         self._code_verifier = ""
@@ -235,20 +235,20 @@
             "Operating-System": self._OS,
             "App": "com.lidl.eci.lidl.plus",
             "Accept-Language": self._language,
         }
 
     def tickets(self):
         """Get list of all tickets"""
-        url = f"{self._TICKET_API}/{self._country}/list"
+        url = f"{self._TICKET_API}/{self._country}/tickets"
         kwargs = {"headers": self._default_headers(), "timeout": self._TIMEOUT}
-        ticket = requests.get(f"{url}/1", **kwargs).json()
-        tickets = ticket["records"]
+        ticket = requests.get(f"{url}?pageNumber=1", **kwargs).json()
+        tickets = ticket["tickets"]
         for i in range(2, int(ticket["totalCount"] / ticket["size"] + 2)):
-            tickets += requests.get(f"{url}/{i}", **kwargs).json()["records"]
+            tickets += requests.get(f"{url}?pageNumber={i}", **kwargs).json()["tickets"]
         return tickets
 
     def ticket(self, ticket_id):
         """Get full data of single ticket by id"""
         kwargs = {"headers": self._default_headers(), "timeout": self._TIMEOUT}
         url = f"{self._TICKET_API}/{self._country}/tickets"
         return requests.get(f"{url}/{ticket_id}", **kwargs).json()
```

### Comparing `lidl-plus-0.2.5/setup.py` & `lidl-plus-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lidl-plus",
-    version="0.2.5",
+    version="0.2.6",
     author="Andre Basche",
     description="Fetch receipts and more from Lidl Plus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/lidl-plus",
         "PyPI": "https://pypi.org/project/lidl-plus/",
```

