# Comparing `tmp/pychedule-0.0.5-py3-none-any.whl.zip` & `tmp/pychedule-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2940 bytes, number of entries: 9
+Zip file size: 2959 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       47 b- defN 23-Jun-01 14:12 packageTest/__init__.py
 -rw-r--r--  2.0 unx      459 b- defN 23-Jun-01 16:31 packageTest/packageTest.py
--rwxr-xr-x  2.0 unx     1029 b- defN 23-Jun-03 16:02 pychedule-0.0.5.data/scripts/test.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 16:21 test/__init__.py
+-rwxr-xr-x  2.0 unx     1029 b- defN 23-Jun-03 16:02 pychedule-0.0.6.data/scripts/test.py
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-03 16:26 test/__init__.py
 -rw-r--r--  2.0 unx     1029 b- defN 23-Jun-03 16:02 test/test.py
--rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      696 b- defN 23-Jun-03 16:22 pychedule-0.0.5.dist-info/RECORD
-9 files, 3947 bytes uncompressed, 1736 bytes compressed:  56.0%
+-rw-r--r--  2.0 unx      590 b- defN 23-Jun-03 16:27 pychedule-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 16:27 pychedule-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-03 16:27 pychedule-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      697 b- defN 23-Jun-03 16:27 pychedule-0.0.6.dist-info/RECORD
+9 files, 3967 bytes uncompressed, 1755 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: packageTest/__init__.py
 Comment: 
 
 Filename: packageTest/packageTest.py
 Comment: 
 
-Filename: pychedule-0.0.5.data/scripts/test.py
+Filename: pychedule-0.0.6.data/scripts/test.py
 Comment: 
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test.py
 Comment: 
 
-Filename: pychedule-0.0.5.dist-info/METADATA
+Filename: pychedule-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pychedule-0.0.5.dist-info/WHEEL
+Filename: pychedule-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pychedule-0.0.5.dist-info/top_level.txt
+Filename: pychedule-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pychedule-0.0.5.dist-info/RECORD
+Filename: pychedule-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 7465 7374 2069 6d70 6f72  from .test impor
+00000010: 7420 2a                                  t *
```

## Comparing `pychedule-0.0.5.data/scripts/test.py` & `pychedule-0.0.6.data/scripts/test.py`

 * *Files identical despite different names*

## Comparing `pychedule-0.0.5.dist-info/METADATA` & `pychedule-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychedule
-Version: 0.0.5
+Version: 0.0.6
 Summary: Scheduler for Python
 Home-page: https://github.com/wklee610/pychedule
 Author: wklee610
 Author-email: wklee610@gmail.com
 License: UNKNOWN
 Keywords: scheduler,wklee610,python
 Platform: UNKNOWN
```

