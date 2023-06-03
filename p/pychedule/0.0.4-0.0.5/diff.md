# Comparing `tmp/pychedule-0.0.4-py3-none-any.whl.zip` & `tmp/pychedule-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 2476 bytes, number of entries: 8
+Zip file size: 2940 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       47 b- defN 23-Jun-01 14:12 packageTest/__init__.py
 -rw-r--r--  2.0 unx      459 b- defN 23-Jun-01 16:31 packageTest/packageTest.py
--rw-r--r--  2.0 unx       83 b- defN 23-Jun-03 16:08 test/__init__.py
+-rwxr-xr-x  2.0 unx     1029 b- defN 23-Jun-03 16:02 pychedule-0.0.5.data/scripts/test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 16:21 test/__init__.py
 -rw-r--r--  2.0 unx     1029 b- defN 23-Jun-03 16:02 test/test.py
--rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      604 b- defN 23-Jun-03 16:09 pychedule-0.0.4.dist-info/RECORD
-8 files, 2909 bytes uncompressed, 1420 bytes compressed:  51.2%
+-rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      696 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/RECORD
+9 files, 3947 bytes uncompressed, 1736 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: packageTest/__init__.py
 Comment: 
 
 Filename: packageTest/packageTest.py
 Comment: 
 
+Filename: pychedule-0.0.5.data/scripts/test.py
+Comment: 
+
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test.py
 Comment: 
 
-Filename: pychedule-0.0.4.dist-info/METADATA
+Filename: pychedule-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pychedule-0.0.4.dist-info/WHEEL
+Filename: pychedule-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pychedule-0.0.4.dist-info/top_level.txt
+Filename: pychedule-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pychedule-0.0.4.dist-info/RECORD
+Filename: pychedule-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test/__init__.py

```diff
@@ -1,6 +0,0 @@
-00000000: 6672 6f6d 202e 7465 7374 2069 6d70 6f72  from .test impor
-00000010: 7420 2a0a 6672 6f6d 202e 2069 6d70 6f72  t *.from . impor
-00000020: 7420 5f5f 616c 6c5f 5f0a 0a5f 5f76 6572  t __all__..__ver
-00000030: 7369 6f6e 5f5f 203d 2027 302e 302e 3427  sion__ = '0.0.4'
-00000040: 0a5f 5f61 6c6c 5f5f 203d 205b 2774 6573  .__all__ = ['tes
-00000050: 7427 5d                                  t']
```

## Comparing `pychedule-0.0.4.dist-info/METADATA` & `pychedule-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychedule
-Version: 0.0.4
+Version: 0.0.5
 Summary: Scheduler for Python
 Home-page: https://github.com/wklee610/pychedule
 Author: wklee610
 Author-email: wklee610@gmail.com
 License: UNKNOWN
 Keywords: scheduler,wklee610,python
 Platform: UNKNOWN
```

