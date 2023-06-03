# Comparing `tmp/fastf1-3.0.3.tar.gz` & `tmp/fastf1-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-3.0.3.tar", last modified: Fri May 19 20:53:28 2023, max compression
+gzip compressed data, was "fastf1-3.0.4.tar", last modified: Sat Jun  3 16:58:13 2023, max compression
```

## Comparing `fastf1-3.0.3.tar` & `fastf1-3.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 20:53:18.000000 fastf1-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 20:53:18.000000 fastf1-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 20:53:28.913574 fastf1-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-19 20:53:18.000000 fastf1-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.909574 fastf1-3.0.3/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   136246 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/ergast/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/req.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/events/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/events/_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/hubs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/hubs/_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/transports/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.909574 fastf1-3.0.3/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 20:53:18.000000 fastf1-3.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-19 20:53:28.917574 fastf1-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-19 20:53:18.000000 fastf1-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-03 16:57:57.000000 fastf1-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 16:57:57.000000 fastf1-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 16:58:13.087779 fastf1-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-03 16:57:57.000000 fastf1-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136246 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/hubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-03 16:58:13.000000 fastf1-3.0.4/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 16:57:57.000000 fastf1-3.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 16:58:13.087779 fastf1-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-03 16:57:57.000000 fastf1-3.0.4/setup.py
```

### Comparing `fastf1-3.0.3/LICENSE` & `fastf1-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/PKG-INFO` & `fastf1-3.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
         
@@ -49,16 +49,18 @@
         
         The official documentation can be found here:
         [docs.fastf1.dev](https://docs.fastf1.dev)
         
         
         ## Supporting the Project
         
-        If you want to support the continuous development of FastF1, you can buy me
-        a coffee.
+        If you want to support the continuous development of FastF1, you can sponsor me
+        on GitHub or buy me a coffee.
+        
+        https://github.com/sponsors/theOehrly
         
         <a href="https://www.buymeacoffee.com/fastf1" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         
         ## Notice
         
         FastF1 and this website are unofficial and are not associated in any way with
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.3 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.4 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
@@ -13,13 +13,14 @@
 caching for all API requests to speed up your scripts ## Installation It is
 recommended to install FastF1 using `pip`: ```commandline pip install fastf1
 ``` Note that Python 3.8 or higher is required. Alternatively, a wheel or a
 source distribution can be downloaded from Pypi. You can also install using
 `conda`: ```commandline conda install -c conda-forge fastf1 ``` ##
 Documentation The official documentation can be found here: [docs.fastf1.dev]
 (https://docs.fastf1.dev) ## Supporting the Project If you want to support the
-continuous development of FastF1, you can buy me a coffee. [Buy_Me_A_Coffee] ##
-Notice FastF1 and this website are unofficial and are not associated in any way
-with the Formula 1 companies. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD
+continuous development of FastF1, you can sponsor me on GitHub or buy me a
+coffee. https://github.com/sponsors/theOehrly [Buy_Me_A_Coffee] ## Notice
+FastF1 and this website are unofficial and are not associated in any way with
+the Formula 1 companies. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD
 CHAMPIONSHIP, GRAND PRIX and related marks are trade marks of Formula One
 Licensing B.V. Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-
 Type: text/markdown
```

### Comparing `fastf1-3.0.3/README.md` & `fastf1-3.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,18 @@
 
 The official documentation can be found here:
 [docs.fastf1.dev](https://docs.fastf1.dev)
 
 
 ## Supporting the Project
 
-If you want to support the continuous development of FastF1, you can buy me
-a coffee.
+If you want to support the continuous development of FastF1, you can sponsor me
+on GitHub or buy me a coffee.
+
+https://github.com/sponsors/theOehrly
 
 <a href="https://www.buymeacoffee.com/fastf1" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 
 ## Notice
 
 FastF1 and this website are unofficial and are not associated in any way with
```

#### html2text {}

```diff
@@ -10,11 +10,12 @@
 speed up your scripts ## Installation It is recommended to install FastF1 using
 `pip`: ```commandline pip install fastf1 ``` Note that Python 3.8 or higher is
 required. Alternatively, a wheel or a source distribution can be downloaded
 from Pypi. You can also install using `conda`: ```commandline conda install -
 c conda-forge fastf1 ``` ## Documentation The official documentation can be
 found here: [docs.fastf1.dev](https://docs.fastf1.dev) ## Supporting the
 Project If you want to support the continuous development of FastF1, you can
-buy me a coffee. [Buy_Me_A_Coffee] ## Notice FastF1 and this website are
-unofficial and are not associated in any way with the Formula 1 companies. F1,
-FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD CHAMPIONSHIP, GRAND PRIX and
-related marks are trade marks of Formula One Licensing B.V.
+sponsor me on GitHub or buy me a coffee. https://github.com/sponsors/theOehrly
+[Buy_Me_A_Coffee] ## Notice FastF1 and this website are unofficial and are not
+associated in any way with the Formula 1 companies. F1, FORMULA ONE, FORMULA 1,
+FIA FORMULA ONE WORLD CHAMPIONSHIP, GRAND PRIX and related marks are trade
+marks of Formula One Licensing B.V.
```

### Comparing `fastf1-3.0.3/fastf1/__init__.py` & `fastf1-3.0.4/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/_api.py` & `fastf1-3.0.4/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/api.py` & `fastf1-3.0.4/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/core.py` & `fastf1-3.0.4/fastf1/core.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/ergast/interface.py` & `fastf1-3.0.4/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/ergast/legacy.py` & `fastf1-3.0.4/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/ergast/sphinx.py` & `fastf1-3.0.4/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/ergast/structure.py` & `fastf1-3.0.4/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/events.py` & `fastf1-3.0.4/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/legacy.py` & `fastf1-3.0.4/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/livetiming/__init__.py` & `fastf1-3.0.4/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/livetiming/__main__.py` & `fastf1-3.0.4/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/livetiming/client.py` & `fastf1-3.0.4/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/livetiming/data.py` & `fastf1-3.0.4/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/logger.py` & `fastf1-3.0.4/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/plotting.py` & `fastf1-3.0.4/fastf1/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 COMPOUND_COLORS: Dict[str, str] = {
     "SOFT": "#da291c",
     "MEDIUM": "#ffd12e",
     "HARD": "#f0f0ec",
     "INTERMEDIATE": "#43b02a",
     "WET": "#0067ad",
     "UNKNOWN": "#00ffff",
+    "TEST-UNKNOWN": "#434649"
 }
 """Mapping of tyre compound names to compound colors (hex color codes).
 (current season only)"""
 
 COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
                             '#FFB86C', '#FF5555', '#F1FA8C']
 """The default color palette for matplotlib plot lines in fastf1's color
```

### Comparing `fastf1-3.0.3/fastf1/req.py` & `fastf1-3.0.4/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/signalr_aio/_connection.py` & `fastf1-3.0.4/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.0.4/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.0.4/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.0.4/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1/utils.py` & `fastf1-3.0.4/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/fastf1.egg-info/PKG-INFO` & `fastf1-3.0.4/fastf1.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
         
@@ -49,16 +49,18 @@
         
         The official documentation can be found here:
         [docs.fastf1.dev](https://docs.fastf1.dev)
         
         
         ## Supporting the Project
         
-        If you want to support the continuous development of FastF1, you can buy me
-        a coffee.
+        If you want to support the continuous development of FastF1, you can sponsor me
+        on GitHub or buy me a coffee.
+        
+        https://github.com/sponsors/theOehrly
         
         <a href="https://www.buymeacoffee.com/fastf1" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         
         ## Notice
         
         FastF1 and this website are unofficial and are not associated in any way with
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.3 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.4 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
@@ -13,13 +13,14 @@
 caching for all API requests to speed up your scripts ## Installation It is
 recommended to install FastF1 using `pip`: ```commandline pip install fastf1
 ``` Note that Python 3.8 or higher is required. Alternatively, a wheel or a
 source distribution can be downloaded from Pypi. You can also install using
 `conda`: ```commandline conda install -c conda-forge fastf1 ``` ##
 Documentation The official documentation can be found here: [docs.fastf1.dev]
 (https://docs.fastf1.dev) ## Supporting the Project If you want to support the
-continuous development of FastF1, you can buy me a coffee. [Buy_Me_A_Coffee] ##
-Notice FastF1 and this website are unofficial and are not associated in any way
-with the Formula 1 companies. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD
+continuous development of FastF1, you can sponsor me on GitHub or buy me a
+coffee. https://github.com/sponsors/theOehrly [Buy_Me_A_Coffee] ## Notice
+FastF1 and this website are unofficial and are not associated in any way with
+the Formula 1 companies. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD
 CHAMPIONSHIP, GRAND PRIX and related marks are trade marks of Formula One
 Licensing B.V. Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-
 Type: text/markdown
```

### Comparing `fastf1-3.0.3/fastf1.egg-info/SOURCES.txt` & `fastf1-3.0.4/fastf1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.3/setup.cfg` & `fastf1-3.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	requests-cache>=0.8.0
 	pandas>=1.2.4,<3.0.0
 	numpy>=1.20.3,<2.0.0
 	scipy>=1.6.3,<2.0.0
 	thefuzz
 	matplotlib>=3.4.2,<4.0.0
 	python-dateutil
-	timple>=0.1.2
+	timple>=0.1.6
 	requests>=2.28.0
 	websockets>=8.1
 
 [build_sphinx]
 project = Fast F1
 source-dir = ./docs
 build-dir = ./docs/_build
```

