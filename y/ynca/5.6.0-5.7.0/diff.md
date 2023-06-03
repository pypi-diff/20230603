# Comparing `tmp/ynca-5.6.0.tar.gz` & `tmp/ynca-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynca-5.6.0.tar", last modified: Fri Apr 14 19:25:52 2023, max compression
+gzip compressed data, was "ynca-5.7.0.tar", last modified: Sat Jun  3 09:37:32 2023, max compression
```

## Comparing `ynca-5.6.0.tar` & `ynca-5.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 19:25:41.000000 ynca-5.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 19:25:41.000000 ynca-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 19:25:52.607591 ynca-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-14 19:25:41.000000 ynca-5.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 19:25:52.607591 ynca-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 19:25:41.000000 ynca-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.603591 ynca-5.6.0/ynca/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/modelinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/ynca/subunits/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/airplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/bt.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/dab.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/ipod.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/ipodusb.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/napster.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/netradio.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/pandora.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/pc.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/rhap.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/sirius.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/uaw.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/ynca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:37:32.537238 ynca-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-03 09:37:23.000000 ynca-5.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-03 09:37:23.000000 ynca-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-03 09:37:32.537238 ynca-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-03 09:37:23.000000 ynca-5.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 09:37:32.541238 ynca-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-03 09:37:23.000000 ynca-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:37:32.537238 ynca-5.7.0/ynca/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/modelinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:37:32.537238 ynca-5.7.0/ynca/subunits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/airplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/bt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/dab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/ipod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/ipodusb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/napster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/netradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/rhap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/sirius.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/uaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/subunits/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-03 09:37:23.000000 ynca-5.7.0/ynca/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:37:32.537238 ynca-5.7.0/ynca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-03 09:37:32.000000 ynca-5.7.0/ynca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-03 09:37:32.000000 ynca-5.7.0/ynca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:37:32.000000 ynca-5.7.0/ynca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 09:37:32.000000 ynca-5.7.0/ynca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 09:37:32.000000 ynca-5.7.0/ynca.egg-info/top_level.txt
```

### Comparing `ynca-5.6.0/LICENSE.txt` & `ynca-5.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/PKG-INFO` & `ynca-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.6.0
+Version: 5.7.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-According to reports of users and info found on the internet the following receivers should work (not all tested).
+According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
```

### Comparing `ynca-5.6.0/README.md` & `ynca-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-According to reports of users and info found on the internet the following receivers should work (not all tested).
+According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
```

### Comparing `ynca-5.6.0/setup.py` & `ynca-5.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="ynca",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="5.6.0",
+    version="5.7.0",
     description="Package to control Yamaha receivers that support the YNCA protocol.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/mvdwetering/ynca",
     # Author details
     author="Michel van de Wetering",
```

### Comparing `ynca-5.6.0/ynca/__init__.py` & `ynca-5.7.0/ynca/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .enums import (
     Avail,
     AdaptiveDrc,
     BandDab,
     BandTun,
     Enhancer,
     HdmiOut,
+    HdmiOutOnOff,
     InitVolLvl,
     InitVolMode,
     Input,
     Mute,
     Party,
     PartyMute,
     Playback,
```

### Comparing `ynca-5.6.0/ynca/api.py` & `ynca-5.7.0/ynca/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     def _get_subunit_class(self, subunit_id):
         subunit_classes = all_subclasses(SubunitBase)
         for subunit_class in subunit_classes:
             try:
                 if subunit_class.id == subunit_id:
                     return subunit_class
-            except AttributeError:
+            except AttributeError:   # pragma: no cover
                 # Intermediate Subunit classes like ZoneBase don't have an ID
                 pass
 
     def _initialize_available_subunits(self, connection: YncaConnection):
         # Every receiver has a System subunit
         # It also does not respond to AVAIL=? so it will not end up in _available_subunits
         system = System(connection)
```

### Comparing `ynca-5.6.0/ynca/connection.py` & `ynca-5.7.0/ynca/connection.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/constants.py` & `ynca-5.7.0/ynca/constants.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/converters.py` & `ynca-5.7.0/ynca/converters.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/enums.py` & `ynca-5.7.0/ynca/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,26 @@
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
+class HdmiOutOnOff(Enum):
+    ON = "On"
+    OFF = "Off"
+
+    @classmethod
+    def _missing_(cls, value):
+        logger.warning("Unknown value '%s' in %s", value, cls.__name__)
+        return cls.UNKNOWN
+
+    UNKNOWN = UNKNOWN_STRING
+    """Unknown values in the enum are mapped to UNKNOWN"""
+
 
 class InitVolLvl(str, Enum):
     MUTE = "Mute"
     OFF = "Off"
     """Only some receivers report Off, most seem to use InitVolMode to indicate On/Off"""
 
     @classmethod
```

### Comparing `ynca-5.6.0/ynca/errors.py` & `ynca-5.7.0/ynca/errors.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/function.py` & `ynca-5.7.0/ynca/function.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/helpers.py` & `ynca-5.7.0/ynca/helpers.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/modelinfo.py` & `ynca-5.7.0/ynca/modelinfo.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/server.py` & `ynca-5.7.0/ynca/server.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunit.py` & `ynca-5.7.0/ynca/subunit.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/__init__.py` & `ynca-5.7.0/ynca/subunits/__init__.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/dab.py` & `ynca-5.7.0/ynca/subunits/dab.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/pandora.py` & `ynca-5.7.0/ynca/subunits/pandora.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/sirius.py` & `ynca-5.7.0/ynca/subunits/sirius.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/system.py` & `ynca-5.7.0/ynca/subunits/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
 
 from ..constants import Subunit
 from ..converters import StrConverter
 from ..function import Cmd, EnumFunction, FunctionBase, StrFunction
-from ..enums import Party, PartyMute, Pwr
+from ..enums import HdmiOutOnOff, Party, PartyMute, Pwr
 from ..subunit import SubunitBase
 
 logger = logging.getLogger(__name__)
 
 
 class System(SubunitBase):
     id = Subunit.SYS
 
+    hdmiout1 = EnumFunction[HdmiOutOnOff]("HDMIOUT1", HdmiOutOnOff)
+    hdmiout2 = EnumFunction[HdmiOutOnOff]("HDMIOUT2", HdmiOutOnOff)
+    hdmiout3 = EnumFunction[HdmiOutOnOff]("HDMIOUT3", HdmiOutOnOff)
     inpnameaudio1 = StrFunction("INPNAMEAUDIO1", Cmd.GET, init="INPNAME")
     inpnameaudio2 = StrFunction("INPNAMEAUDIO2", Cmd.GET, init="INPNAME")
     inpnameaudio3 = StrFunction("INPNAMEAUDIO3", Cmd.GET, init="INPNAME")
     inpnameaudio4 = StrFunction("INPNAMEAUDIO4", Cmd.GET, init="INPNAME")
     inpnameav1 = StrFunction("INPNAMEAV1", Cmd.GET, init="INPNAME")
     inpnameav2 = StrFunction("INPNAMEAV2", Cmd.GET, init="INPNAME")
     inpnameav3 = StrFunction("INPNAMEAV3", Cmd.GET, init="INPNAME")
```

### Comparing `ynca-5.6.0/ynca/subunits/tun.py` & `ynca-5.7.0/ynca/subunits/tun.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/subunits/zone.py` & `ynca-5.7.0/ynca/subunits/zone.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca/terminal.py` & `ynca-5.7.0/ynca/terminal.py`

 * *Files identical despite different names*

### Comparing `ynca-5.6.0/ynca.egg-info/PKG-INFO` & `ynca-5.7.0/ynca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.6.0
+Version: 5.7.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-According to reports of users and info found on the internet the following receivers should work (not all tested).
+According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
```

### Comparing `ynca-5.6.0/ynca.egg-info/SOURCES.txt` & `ynca-5.7.0/ynca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

