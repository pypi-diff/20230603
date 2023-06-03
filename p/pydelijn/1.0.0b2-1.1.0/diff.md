# Comparing `tmp/pydelijn-1.0.0b2.tar.gz` & `tmp/pydelijn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelijn-1.0.0b2.tar", last modified: Fri Jan 14 20:27:56 2022, max compression
+gzip compressed data, was "pydelijn-1.1.0.tar", last modified: Sat Jun  3 21:52:14 2023, max compression
```

## Comparing `pydelijn-1.0.0b2.tar` & `pydelijn-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 20:27:56.397673 pydelijn-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-01-14 20:27:56.397673 pydelijn-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 20:27:56.393674 pydelijn-1.0.0b2/pydelijn/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/pydelijn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11733 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/pydelijn/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/pydelijn/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 20:27:56.397673 pydelijn-1.0.0b2/pydelijn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-01-14 20:27:56.000000 pydelijn-1.0.0b2/pydelijn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-14 20:27:56.000000 pydelijn-1.0.0b2/pydelijn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 20:27:56.000000 pydelijn-1.0.0b2/pydelijn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-14 20:27:56.000000 pydelijn-1.0.0b2/pydelijn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-14 20:27:56.000000 pydelijn-1.0.0b2/pydelijn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-01-14 20:27:56.397673 pydelijn-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-01-14 20:27:39.000000 pydelijn-1.0.0b2/setup.py
+drwxr-xr-x   0 emil      (1000) emil      (1000)        0 2023-06-03 21:52:14.696821 pydelijn-1.1.0/
+-rw-r--r--   0 emil      (1000) emil      (1000)     1070 2020-03-02 20:08:29.000000 pydelijn-1.1.0/LICENSE
+-rw-r--r--   0 emil      (1000) emil      (1000)     3567 2023-06-03 21:52:14.696821 pydelijn-1.1.0/PKG-INFO
+-rw-r--r--   0 emil      (1000) emil      (1000)     2859 2021-11-14 22:07:46.000000 pydelijn-1.1.0/README.md
+drwxr-xr-x   0 emil      (1000) emil      (1000)        0 2023-06-03 21:52:14.696821 pydelijn-1.1.0/pydelijn/
+-rw-r--r--   0 emil      (1000) emil      (1000)       71 2023-06-03 21:42:32.000000 pydelijn-1.1.0/pydelijn/__init__.py
+-rw-r--r--   0 emil      (1000) emil      (1000)    12090 2023-06-03 21:39:50.000000 pydelijn-1.1.0/pydelijn/api.py
+-rw-r--r--   0 emil      (1000) emil      (1000)     2594 2023-06-03 21:24:40.000000 pydelijn-1.1.0/pydelijn/common.py
+drwxr-xr-x   0 emil      (1000) emil      (1000)        0 2023-06-03 21:52:14.696821 pydelijn-1.1.0/pydelijn.egg-info/
+-rw-r--r--   0 emil      (1000) emil      (1000)     3567 2023-06-03 21:52:14.000000 pydelijn-1.1.0/pydelijn.egg-info/PKG-INFO
+-rw-r--r--   0 emil      (1000) emil      (1000)      251 2023-06-03 21:52:14.000000 pydelijn-1.1.0/pydelijn.egg-info/SOURCES.txt
+-rw-r--r--   0 emil      (1000) emil      (1000)        1 2023-06-03 21:52:14.000000 pydelijn-1.1.0/pydelijn.egg-info/dependency_links.txt
+-rw-r--r--   0 emil      (1000) emil      (1000)       59 2023-06-03 21:52:14.000000 pydelijn-1.1.0/pydelijn.egg-info/requires.txt
+-rw-r--r--   0 emil      (1000) emil      (1000)        9 2023-06-03 21:52:14.000000 pydelijn-1.1.0/pydelijn.egg-info/top_level.txt
+-rw-r--r--   0 emil      (1000) emil      (1000)      129 2023-06-03 21:52:14.696821 pydelijn-1.1.0/setup.cfg
+-rw-r--r--   0 emil      (1000) emil      (1000)     1261 2021-11-11 22:04:48.000000 pydelijn-1.1.0/setup.py
```

### Comparing `pydelijn-1.0.0b2/LICENSE` & `pydelijn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelijn-1.0.0b2/PKG-INFO` & `pydelijn-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydelijn
-Version: 1.0.0b2
+Version: 1.1.0
 Summary: Get realtime info on stop passages of De Lijn (api.delijn.be)
 Home-page: https://github.com/bollewolle/pydelijn
 Author: bollewolle
 Author-email: dev@bollewolle.be
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -92,9 +91,7 @@
             line['line_number_colourBackBorderHex']))
 
 
 LOOP = asyncio.get_event_loop()
 LOOP.run_until_complete(test_pydelijn())
 LOOP.close()
 
-
-
```

### Comparing `pydelijn-1.0.0b2/README.md` & `pydelijn-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydelijn-1.0.0b2/pydelijn/api.py` & `pydelijn-1.1.0/pydelijn/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,18 +125,24 @@
                         direction = passage.get("richting")
                         final_destination = passage.get("bestemming")
                         due_at_schedule = passage.get("dienstregelingTijdstip")
                         due_at_realtime = passage.get("real-timeTijdstip")
                         realtime_info = passage.get("predictionStatussen")
                         if realtime_info[0] == "GEENREALTIME":
                             is_realtime = False
+                            cancelled = False
                         elif realtime_info[0] == "REALTIME":
                             is_realtime = True
+                            cancelled = False
+                        elif realtime_info[0] == "GESCHRAPT":
+                            is_realtime = False
+                            cancelled = True
                         else:
                             is_realtime = False
+                            cancelled = False
                             LOGGER.warning("unknown realtime info: %s", realtime_info)
 
                         due_in_min = None
 
                         timeformat = "%Y-%m-%dT%H:%M:%S"
                         if self.utcoutput is True:
                             if due_at_realtime is not None:
@@ -211,14 +217,15 @@
                                         "line_number": linenumber,
                                         "direction": direction,
                                         "final_destination": final_destination,
                                         "due_at_schedule": due_at_schedule,
                                         "due_at_realtime": due_at_realtime,
                                         "due_in_min": due_in_min,
                                         "is_realtime": is_realtime,
+                                        "cancelled": cancelled,
                                         "line_number_public": linenumberpublic,
                                         "line_desc": linedesc,
                                         "line_transport_type": linetransporttype,
                                         "line_number_colourFront": linenumcolfront,
                                         "line_number_colourFrontHex": linenumcolfronthex,
                                         "line_number_colourBack": linenumcolback,
                                         "line_number_colourBackHex": linenumcolbackhex,
```

### Comparing `pydelijn-1.0.0b2/pydelijn/common.py` & `pydelijn-1.1.0/pydelijn/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Common attributes and functions."""
 import logging
 import asyncio
 import async_timeout
 import aiohttp
 
 LOGGER = logging.getLogger(__name__)
-BASE_URL = "https://api.delijn.be/DLKernOpenData/v1/beta/"
+BASE_URL = "https://api.delijn.be/DLKernOpenData/api/v1/"
 
 
 class CommonFunctions:
     """A class for common functions."""
 
     def __init__(self, session, subscriptionkey):
         """Initialize the class."""
@@ -31,23 +31,23 @@
                         data = await response.json()
                     except ValueError as exception:
                         message = "Server gave incorrect data"
                         raise Exception(message) from exception
 
                 elif response.status == 401:
                     message = "401: Acces token might be incorrect"
-                    raise HttpException(message, await response.text(), response.status)
+                    raise HttpException(message, await response.text(), response.status, endpoint, headers)
 
                 elif response.status == 404:
                     message = "404: incorrect API request"
-                    raise HttpException(message, await response.text(), response.status)
+                    raise HttpException(message, await response.text(), response.status, endpoint, headers)
 
                 else:
                     message = f"Unexpected status code {response.status}."
-                    raise HttpException(message, await response.text(), response.status)
+                    raise HttpException(message, await response.text(), response.status, endpoint, headers)
 
         except aiohttp.ClientError as error:
             LOGGER.error("Error connecting to De Lijn API: %s", error)
         except asyncio.TimeoutError as error:
             LOGGER.debug("Timeout connecting to De Lijn API: %s", error)
         return data
 
@@ -55,13 +55,15 @@
         """Close the session."""
         await self.session.close()
 
 
 class HttpException(Exception):
     """HTTP exception class with message text, and status code."""
 
-    def __init__(self, message, text, status_code):
+    def __init__(self, message, text, status_code, url, headers):
         """Initialize the class."""
-        super().__init__(message)
+        super().__init__("message: " + message + ", url: " + url + ", headers: " + str(headers))
 
         self.status_code = status_code
         self.text = text
+        self.url = url
+        self.headers = headers
```

### Comparing `pydelijn-1.0.0b2/pydelijn.egg-info/PKG-INFO` & `pydelijn-1.1.0/pydelijn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydelijn
-Version: 1.0.0b2
+Version: 1.1.0
 Summary: Get realtime info on stop passages of De Lijn (api.delijn.be)
 Home-page: https://github.com/bollewolle/pydelijn
 Author: bollewolle
 Author-email: dev@bollewolle.be
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -92,9 +91,7 @@
             line['line_number_colourBackBorderHex']))
 
 
 LOOP = asyncio.get_event_loop()
 LOOP.run_until_complete(test_pydelijn())
 LOOP.close()
 
-
-
```

### Comparing `pydelijn-1.0.0b2/setup.py` & `pydelijn-1.1.0/setup.py`

 * *Files identical despite different names*

