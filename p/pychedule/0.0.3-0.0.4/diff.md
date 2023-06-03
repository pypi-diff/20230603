# Comparing `tmp/pychedule-0.0.3-py3-none-any.whl.zip` & `tmp/pychedule-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2447 bytes, number of entries: 8
+Zip file size: 2476 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       47 b- defN 23-Jun-01 14:12 packageTest/__init__.py
 -rw-r--r--  2.0 unx      459 b- defN 23-Jun-01 16:31 packageTest/packageTest.py
--rw-r--r--  2.0 unx       40 b- defN 23-Jun-03 15:54 test/__init__.py
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-03 16:08 test/__init__.py
 -rw-r--r--  2.0 unx     1029 b- defN 23-Jun-03 16:02 test/test.py
--rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:03 pychedule-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:03 pychedule-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:03 pychedule-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      604 b- defN 23-Jun-03 16:03 pychedule-0.0.3.dist-info/RECORD
-8 files, 2866 bytes uncompressed, 1391 bytes compressed:  51.5%
+-rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      604 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/RECORD
+8 files, 2909 bytes uncompressed, 1420 bytes compressed:  51.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test.py
 Comment: 
 
-Filename: pychedule-0.0.3.dist-info/METADATA
+Filename: pychedule-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pychedule-0.0.3.dist-info/WHEEL
+Filename: pychedule-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pychedule-0.0.3.dist-info/top_level.txt
+Filename: pychedule-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pychedule-0.0.3.dist-info/RECORD
+Filename: pychedule-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test/__init__.py

```diff
@@ -1,2 +1,5 @@
-__version__ = '0.0.3'
+from .test import *
+from . import __all__
+
+__version__ = '0.0.4'
 __all__ = ['test']
```

## Comparing `pychedule-0.0.3.dist-info/METADATA` & `pychedule-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychedule
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scheduler for Python
 Home-page: https://github.com/wklee610/pychedule
 Author: wklee610
 Author-email: wklee610@gmail.com
 License: UNKNOWN
 Keywords: scheduler,wklee610,python
 Platform: UNKNOWN
```

## Comparing `pychedule-0.0.3.dist-info/RECORD` & `pychedule-0.0.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 packageTest/__init__.py,sha256=4XJPInAaL0j-GGxbL8zGuID0kDxBiAsKuSEQ6suiIMw,47
 packageTest/packageTest.py,sha256=KRNuCWYDdao46Xve_QucF6JBd9e8h1Au6rScqaOUPS4,459
-test/__init__.py,sha256=uhqJRNU1OuZggkNtXYN9nE0XZIQY5mDzGN3VS8O9q_8,40
+test/__init__.py,sha256=UFR2shYxZUNmPIAAeXgSSJ_MuQeVHRk0UzkEeHlBP_w,83
 test/test.py,sha256=fwTDRsE-dw0zL8ivrAdU3gPslx_RCOL-5gYfy0TEUuc,1029
-pychedule-0.0.3.dist-info/METADATA,sha256=BvfOPuTilatdrHfpxGs1fwQc3hHP94apNOmnKwIVdpI,590
-pychedule-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pychedule-0.0.3.dist-info/top_level.txt,sha256=8sobtsfpB9Btr-Roflefznazfk6Tt2BQItpS5szCb9I,5
-pychedule-0.0.3.dist-info/RECORD,,
+pychedule-0.0.4.dist-info/METADATA,sha256=DOhbcrcF6Z1FbX9d8WbqCbMZEekkZH_-Oyf50Pxyybs,590
+pychedule-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pychedule-0.0.4.dist-info/top_level.txt,sha256=8sobtsfpB9Btr-Roflefznazfk6Tt2BQItpS5szCb9I,5
+pychedule-0.0.4.dist-info/RECORD,,
```

