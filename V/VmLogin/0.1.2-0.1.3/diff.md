# Comparing `tmp/VmLogin-0.1.2.tar.gz` & `tmp/VmLogin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VmLogin-0.1.2.tar", last modified: Sat Apr  8 10:41:38 2023, max compression
+gzip compressed data, was "VmLogin-0.1.3.tar", last modified: Sat Jun  3 08:36:52 2023, max compression
```

## Comparing `VmLogin-0.1.2.tar` & `VmLogin-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 10:41:38.507516 VmLogin-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-04-07 08:00:35.000000 VmLogin-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-07 07:59:25.000000 VmLogin-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1157 2023-04-08 10:41:38.506510 VmLogin-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-04-08 01:01:03.000000 VmLogin-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 10:41:38.485511 VmLogin-0.1.2/VmLogin/
--rw-rw-rw-   0        0        0        2 2023-04-07 08:40:27.000000 VmLogin-0.1.2/VmLogin/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-07 08:05:58.000000 VmLogin-0.1.2/VmLogin/__version__.py
--rw-rw-rw-   0        0        0     2208 2023-04-07 10:42:23.000000 VmLogin-0.1.2/VmLogin/api.py
--rw-rw-rw-   0        0        0      724 2023-04-07 08:31:12.000000 VmLogin-0.1.2/VmLogin/error.py
-drwxrwxrwx   0        0        0        0 2023-04-08 10:41:38.499520 VmLogin-0.1.2/VmLogin/local/
--rw-rw-rw-   0        0        0     1442 2023-04-07 10:37:47.000000 VmLogin-0.1.2/VmLogin/local/__init__.py
--rw-rw-rw-   0        0        0    10444 2023-04-08 00:50:46.000000 VmLogin-0.1.2/VmLogin/local/browser.py
-drwxrwxrwx   0        0        0        0 2023-04-08 10:41:38.504516 VmLogin-0.1.2/VmLogin/online/
--rw-rw-rw-   0        0        0     1098 2023-04-07 10:01:29.000000 VmLogin-0.1.2/VmLogin/online/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-04-07 09:28:06.000000 VmLogin-0.1.2/VmLogin/online/groups.py
--rw-rw-rw-   0        0        0     3051 2023-04-08 10:32:09.000000 VmLogin-0.1.2/VmLogin/online/profiles.py
-drwxrwxrwx   0        0        0        0 2023-04-08 10:41:38.496516 VmLogin-0.1.2/VmLogin.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-04-08 10:41:38.000000 VmLogin-0.1.2/VmLogin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-08 10:41:38.000000 VmLogin-0.1.2/VmLogin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 10:41:38.000000 VmLogin-0.1.2/VmLogin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 10:41:38.000000 VmLogin-0.1.2/VmLogin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 10:41:38.000000 VmLogin-0.1.2/VmLogin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 10:41:38.507516 VmLogin-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3827 2023-04-08 10:40:49.000000 VmLogin-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:36:52.316751 VmLogin-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-07 08:00:35.000000 VmLogin-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-07 07:59:25.000000 VmLogin-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1157 2023-06-03 08:36:52.315766 VmLogin-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-04-08 01:01:03.000000 VmLogin-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 08:36:52.298763 VmLogin-0.1.3/VmLogin/
+-rw-rw-rw-   0        0        0        2 2023-04-07 08:40:27.000000 VmLogin-0.1.3/VmLogin/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-07 08:05:58.000000 VmLogin-0.1.3/VmLogin/__version__.py
+-rw-rw-rw-   0        0        0     2198 2023-06-03 08:31:52.000000 VmLogin-0.1.3/VmLogin/api.py
+-rw-rw-rw-   0        0        0      724 2023-04-07 08:31:12.000000 VmLogin-0.1.3/VmLogin/error.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:36:52.309750 VmLogin-0.1.3/VmLogin/local/
+-rw-rw-rw-   0        0        0     1442 2023-04-07 10:37:47.000000 VmLogin-0.1.3/VmLogin/local/__init__.py
+-rw-rw-rw-   0        0        0    10444 2023-06-03 07:47:20.000000 VmLogin-0.1.3/VmLogin/local/browser.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:36:52.314755 VmLogin-0.1.3/VmLogin/online/
+-rw-rw-rw-   0        0        0     1098 2023-04-07 10:01:29.000000 VmLogin-0.1.3/VmLogin/online/__init__.py
+-rw-rw-rw-   0        0        0     1655 2023-04-07 09:28:06.000000 VmLogin-0.1.3/VmLogin/online/groups.py
+-rw-rw-rw-   0        0        0     3051 2023-04-08 10:32:09.000000 VmLogin-0.1.3/VmLogin/online/profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:36:52.306737 VmLogin-0.1.3/VmLogin.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-03 08:36:52.000000 VmLogin-0.1.3/VmLogin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-06-03 08:36:52.000000 VmLogin-0.1.3/VmLogin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 08:36:52.000000 VmLogin-0.1.3/VmLogin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 08:36:52.000000 VmLogin-0.1.3/VmLogin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 08:36:52.000000 VmLogin-0.1.3/VmLogin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 08:36:52.317765 VmLogin-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3827 2023-06-03 08:35:03.000000 VmLogin-0.1.3/setup.py
```

### Comparing `VmLogin-0.1.2/LICENSE` & `VmLogin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/PKG-INFO` & `VmLogin-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VmLogin
-Version: 0.1.2
+Version: 0.1.3
 Summary: 操作VMLogin
 Home-page: https://github.com/chensav/VmLogin
 Author: chensav
 Author-email: chensav@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `VmLogin-0.1.2/README.md` & `VmLogin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/api.py` & `VmLogin-0.1.3/VmLogin/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,19 @@
         url = self.base_url + url_path
         payload["token"] = self.token
         if http_method == "GET":
             params = {
                 "url": url,
                 "params": payload,
             }
+
         else:
             params = {
                 "url": url,
-                "data": json.dumps(payload),
+                "data": payload,
             }
         response = self._dispatch_request(http_method)(**params)
         self._handle_exception(response)
         try:
             data = response.json()
         except ValueError:
             data = response.text
```

### Comparing `VmLogin-0.1.2/VmLogin/error.py` & `VmLogin-0.1.3/VmLogin/error.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/local/__init__.py` & `VmLogin-0.1.3/VmLogin/local/__init__.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/local/browser.py` & `VmLogin-0.1.3/VmLogin/local/browser.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/online/__init__.py` & `VmLogin-0.1.3/VmLogin/online/__init__.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/online/groups.py` & `VmLogin-0.1.3/VmLogin/online/groups.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin/online/profiles.py` & `VmLogin-0.1.3/VmLogin/online/profiles.py`

 * *Files identical despite different names*

### Comparing `VmLogin-0.1.2/VmLogin.egg-info/PKG-INFO` & `VmLogin-0.1.3/VmLogin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VmLogin
-Version: 0.1.2
+Version: 0.1.3
 Summary: 操作VMLogin
 Home-page: https://github.com/chensav/VmLogin
 Author: chensav
 Author-email: chensav@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `VmLogin-0.1.2/setup.py` & `VmLogin-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'VmLogin'
 DESCRIPTION = '操作VMLogin'
 URL = 'https://github.com/chensav/VmLogin'
 EMAIL = 'chensav@163.com'
 AUTHOR = 'chensav'
 REQUIRES_PYTHON = '>=3.8.16'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

