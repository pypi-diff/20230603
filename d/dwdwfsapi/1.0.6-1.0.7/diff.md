# Comparing `tmp/dwdwfsapi-1.0.6.tar.gz` & `tmp/dwdwfsapi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdwfsapi-1.0.6.tar", last modified: Sat Oct  1 04:38:15 2022, max compression
+gzip compressed data, was "dwdwfsapi-1.0.7.tar", last modified: Sat Jun  3 05:33:56 2023, max compression
```

## Comparing `dwdwfsapi-1.0.6.tar` & `dwdwfsapi-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-10-01 04:38:15.931692 dwdwfsapi-1.0.6/
--rw-rw-rw-   0        0        0      764 2022-10-01 04:31:27.000000 dwdwfsapi-1.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1088 2020-04-19 12:09:02.000000 dwdwfsapi-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       70 2020-04-19 07:25:26.000000 dwdwfsapi-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6244 2022-10-01 04:38:15.931692 dwdwfsapi-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5627 2022-10-01 04:31:44.000000 dwdwfsapi-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-10-01 04:38:15.916067 dwdwfsapi-1.0.6/dwdwfsapi/
--rw-rw-rw-   0        0        0      168 2020-09-24 17:26:36.000000 dwdwfsapi-1.0.6/dwdwfsapi/__init__.py
--rw-rw-rw-   0        0        0     1611 2022-03-13 05:00:27.000000 dwdwfsapi-1.0.6/dwdwfsapi/core.py
--rw-rw-rw-   0        0        0    12398 2022-10-01 04:31:27.000000 dwdwfsapi-1.0.6/dwdwfsapi/weatherwarnings.py
-drwxrwxrwx   0        0        0        0 2022-10-01 04:38:15.931692 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/
--rw-rw-rw-   0        0        0     6244 2022-10-01 04:38:15.000000 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2022-10-01 04:38:15.000000 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-01 04:38:15.000000 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2022-10-01 04:38:15.000000 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-01 04:38:15.000000 dwdwfsapi-1.0.6/dwdwfsapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-01 04:38:15.931692 dwdwfsapi-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1306 2022-10-01 04:33:25.000000 dwdwfsapi-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-01 04:38:15.931692 dwdwfsapi-1.0.6/tests/
--rw-rw-rw-   0        0        0     5583 2022-10-01 04:31:27.000000 dwdwfsapi-1.0.6/tests/test_weatherwarnings.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/
+-rw-rw-rw-   0        0        0      832 2023-06-03 05:31:22.000000 dwdwfsapi-1.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1088 2020-04-19 12:09:02.000000 dwdwfsapi-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       70 2020-04-19 07:25:26.000000 dwdwfsapi-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6244 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5627 2022-10-01 04:31:44.000000 dwdwfsapi-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/dwdwfsapi/
+-rw-rw-rw-   0        0        0      168 2020-09-24 17:26:36.000000 dwdwfsapi-1.0.7/dwdwfsapi/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-04-23 04:39:19.000000 dwdwfsapi-1.0.7/dwdwfsapi/core.py
+-rw-rw-rw-   0        0        0    12398 2022-10-01 04:31:27.000000 dwdwfsapi-1.0.7/dwdwfsapi/weatherwarnings.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/
+-rw-rw-rw-   0        0        0     6244 2023-06-03 05:33:56.000000 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-03 05:33:56.000000 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:33:56.000000 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-03 05:33:56.000000 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 05:33:56.000000 dwdwfsapi-1.0.7/dwdwfsapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-06-03 05:30:17.000000 dwdwfsapi-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:33:56.393510 dwdwfsapi-1.0.7/tests/
+-rw-rw-rw-   0        0        0     5583 2022-10-01 04:31:27.000000 dwdwfsapi-1.0.7/tests/test_weatherwarnings.py
```

### Comparing `dwdwfsapi-1.0.6/CHANGELOG.md` & `dwdwfsapi-1.0.7/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.0.7 (2023-06-03)
+### Changed
+- Update urllib3 requirement
+
 ## 1.0.6 (2022-09-30)
 ### Changed
 - Add option to use a GPS location for the object creation that's used to retrieve the warncell ID
 
 ## 1.0.5 (2022-01-23)
 ### Changed
 - Revert changes done in 1.0.4
```

### Comparing `dwdwfsapi-1.0.6/LICENSE` & `dwdwfsapi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdwfsapi-1.0.6/PKG-INFO` & `dwdwfsapi-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdwfsapi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python client to retrieve data provided by DWD via their geoserver WFS API
 Home-page: https://github.com/stephan192/dwdwfsapi
 Author: stephan192
 Author-email: stephan192@outlook.com
 License: MIT
 Keywords: dwd ows wfs deutscher wetterdienst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dwdwfsapi-1.0.6/README.md` & `dwdwfsapi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dwdwfsapi-1.0.6/dwdwfsapi/core.py` & `dwdwfsapi-1.0.7/dwdwfsapi/core.py`

 * *Files identical despite different names*

### Comparing `dwdwfsapi-1.0.6/dwdwfsapi/weatherwarnings.py` & `dwdwfsapi-1.0.7/dwdwfsapi/weatherwarnings.py`

 * *Files identical despite different names*

### Comparing `dwdwfsapi-1.0.6/dwdwfsapi.egg-info/PKG-INFO` & `dwdwfsapi-1.0.7/dwdwfsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdwfsapi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python client to retrieve data provided by DWD via their geoserver WFS API
 Home-page: https://github.com/stephan192/dwdwfsapi
 Author: stephan192
 Author-email: stephan192@outlook.com
 License: MIT
 Keywords: dwd ows wfs deutscher wetterdienst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dwdwfsapi-1.0.6/setup.py` & `dwdwfsapi-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     "WFS API"
 )
 KEYWORDS = "dwd ows wfs deutscher wetterdienst"
 URL = "https://github.com/stephan192/dwdwfsapi"
 EMAIL = "stephan192@outlook.com"
 AUTHOR = "stephan192"
 REQUIRES_PYTHON = ">=3.6"
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 
 # Define required packages
-REQUIRES = ["requests>=2.23.0,<3", "ciso8601>=2.1.3,<3", "urllib3>=1.25.8,<2"]
+REQUIRES = ["requests>=2.23.0,<3", "ciso8601>=2.1.3,<3", "urllib3>=1.25.8,<3"]
 
 # Import README.md and CHANGELOG.md
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Calling setup
 setup(
```

### Comparing `dwdwfsapi-1.0.6/tests/test_weatherwarnings.py` & `dwdwfsapi-1.0.7/tests/test_weatherwarnings.py`

 * *Files identical despite different names*

