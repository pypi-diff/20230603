# Comparing `tmp/p0_script-1.0.2-py3-none-any.whl.zip` & `tmp/p0_script-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1660133 bytes, number of entries: 916
+Zip file size: 1660134 bytes, number of entries: 916
 -rw-rw-rw-  2.0 fat     4293 b- defN 23-Jun-03 03:51 application/CommandBus.py
 -rw-rw-rw-  2.0 fat     1400 b- defN 23-Jun-03 03:51 application/CommandBusHistory.py
 -rw-rw-rw-  2.0 fat    11970 b- defN 23-Jun-03 03:51 application/Container.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-Jun-03 03:51 application/ContainerInterface.py
 -rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-03 04:05 application/Protocol0.py
 -rw-rw-rw-  2.0 fat     1880 b- defN 23-Jun-03 03:51 application/Protocol0Midi.py
 -rw-rw-rw-  2.0 fat       50 b- defN 22-Oct-29 15:31 application/ScriptDisconnectedEvent.py
@@ -906,13 +906,13 @@
 -rw-rw-rw-  2.0 fat      658 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/saveopts.py
 -rw-rw-rw-  2.0 fat     6711 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/sdist.py
 -rw-rw-rw-  2.0 fat     5085 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/setopt.py
 -rw-rw-rw-  2.0 fat     9214 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/test.py
 -rw-rw-rw-  2.0 fat     1172 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/upload.py
 -rw-rw-rw-  2.0 fat     7311 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/command/upload_docs.py
 -rw-rw-rw-  2.0 fat     2499 b- defN 23-Jun-03 03:42 venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-03 04:06 p0_script-1.0.2.dist-info/LICENSE.rst
--rw-rw-rw-  2.0 fat     8190 b- defN 23-Jun-03 04:06 p0_script-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 04:06 p0_script-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-03 04:06 p0_script-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    96277 b- defN 23-Jun-03 04:07 p0_script-1.0.2.dist-info/RECORD
-916 files, 5568108 bytes uncompressed, 1501195 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/LICENSE.rst
+-rw-rw-rw-  2.0 fat     8190 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    96277 b- defN 23-Jun-03 04:11 p0_script-1.1.0.dist-info/RECORD
+916 files, 5568108 bytes uncompressed, 1501196 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -2727,23 +2727,23 @@
 
 Filename: venv/Lib/site-packages/setuptools/command/upload_docs.py
 Comment: 
 
 Filename: venv/Lib/site-packages/setuptools/extern/__init__.py
 Comment: 
 
-Filename: p0_script-1.0.2.dist-info/LICENSE.rst
+Filename: p0_script-1.1.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: p0_script-1.0.2.dist-info/METADATA
+Filename: p0_script-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: p0_script-1.0.2.dist-info/WHEEL
+Filename: p0_script-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: p0_script-1.0.2.dist-info/top_level.txt
+Filename: p0_script-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: p0_script-1.0.2.dist-info/RECORD
+Filename: p0_script-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `p0_script-1.0.2.dist-info/LICENSE.rst` & `p0_script-1.1.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `p0_script-1.0.2.dist-info/METADATA` & `p0_script-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p0-script
-Version: 1.0.2
+Version: 1.1.0
 Summary: Protocol0 ableton remote script
 Author-email: Thibault Lebrun <thibaultlebrun@live.fr>
 License: MIT License
         
         Copyright (c) 2023 Thibault Lebrun
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `p0_script-1.0.2.dist-info/RECORD` & `p0_script-1.1.0.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -905,12 +905,12 @@
 venv/Lib/site-packages/setuptools/command/saveopts.py,sha256=za7QCBcQimKKriWcoCcbhxPjUz30gSB74zuTL47xpP4,658
 venv/Lib/site-packages/setuptools/command/sdist.py,sha256=obDTe2BmWt2PlnFPZZh7e0LWvemEsbCCO9MzhrTZjm8,6711
 venv/Lib/site-packages/setuptools/command/setopt.py,sha256=NTWDyx-gjDF-txf4dO577s7LOzHVoKR0Mq33rFxaRr8,5085
 venv/Lib/site-packages/setuptools/command/test.py,sha256=MeBAcXUePGjPKqjz4zvTrHatLvNsjlPFcagt3XnFYdk,9214
 venv/Lib/site-packages/setuptools/command/upload.py,sha256=i1gfItZ3nQOn5FKXb8tLC2Kd7eKC8lWO4bdE6NqGpE4,1172
 venv/Lib/site-packages/setuptools/command/upload_docs.py,sha256=oXiGplM_cUKLwE4CWWw98RzCufAu8tBhMC97GegFcms,7311
 venv/Lib/site-packages/setuptools/extern/__init__.py,sha256=2eKMsBMwsZqolIcYBtLZU3t96s6xSTP4PTaNfM5P-I0,2499
-p0_script-1.0.2.dist-info/LICENSE.rst,sha256=Y0J4NqzCszO_UmU8AsJ7mkpcUWrFT5vJS5Pst7GmXhA,1091
-p0_script-1.0.2.dist-info/METADATA,sha256=_9moV2oabTGZU4D7CY_pmrazoMYKAR1qr-7inT1v84c,8190
-p0_script-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-p0_script-1.0.2.dist-info/top_level.txt,sha256=BiJEocJxVkGNfPLQUhIBhXXbuzHOiYjFyZCuEg9rebY,43
-p0_script-1.0.2.dist-info/RECORD,,
+p0_script-1.1.0.dist-info/LICENSE.rst,sha256=Y0J4NqzCszO_UmU8AsJ7mkpcUWrFT5vJS5Pst7GmXhA,1091
+p0_script-1.1.0.dist-info/METADATA,sha256=luh53OdBYxIWMSXyywOwQ-ustwOAF7IyvgB0hlIVq3g,8190
+p0_script-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+p0_script-1.1.0.dist-info/top_level.txt,sha256=BiJEocJxVkGNfPLQUhIBhXXbuzHOiYjFyZCuEg9rebY,43
+p0_script-1.1.0.dist-info/RECORD,,
```

