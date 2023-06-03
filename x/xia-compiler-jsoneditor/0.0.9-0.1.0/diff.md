# Comparing `tmp/xia_compiler_jsoneditor-0.0.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_jsoneditor-0.1.0-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 167163 bytes, number of entries: 7
--rw-r--r--  2.0 unx      135 b- defN 23-Mar-30 19:50 xia_compiler_jsoneditor/__init__.py
--rw-r--r--  2.0 unx   442368 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      687 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/RECORD
-7 files, 444134 bytes uncompressed, 165951 bytes compressed:  62.6%
+Zip file size: 138231 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor/__init__.py
+-rw-r--r--  2.0 unx   386136 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor/compiler.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      650 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      673 b- defN 23-Jun-03 15:43 xia_compiler_jsoneditor-0.1.0.dist-info/RECORD
+7 files, 387877 bytes uncompressed, 137013 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_jsoneditor/__init__.py
 Comment: 
 
-Filename: xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_jsoneditor/compiler.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt
+Filename: xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.9.dist-info/METADATA
+Filename: xia_compiler_jsoneditor-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL
+Filename: xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt
+Filename: xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.9.dist-info/RECORD
+Filename: xia_compiler_jsoneditor-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_jsoneditor/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_jsoneditor.compiler import XiaCompilerJsoneditor
 
 
 __all__ = [
     "XiaCompilerJsoneditor",
 ]
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
```

## Comparing `xia_compiler_jsoneditor-0.0.9.dist-info/METADATA` & `xia_compiler_jsoneditor-0.1.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-compiler-jsoneditor
-Version: 0.0.9
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.0.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-api
 
 .. image:: https://img.shields.io/pypi/v/xia-compiler-jsoneditor.svg?color=blue
    :alt: PyPI-Server
@@ -26,9 +24,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

## Comparing `xia_compiler_jsoneditor-0.0.9.dist-info/RECORD` & `xia_compiler_jsoneditor-0.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_jsoneditor/__init__.py,sha256=dLz-GHzknjgWl5WE4Gl5Qqv7LDMCKzO_rr82cZST9ZM,135
-xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=_K9J2sZS7j4JjfHAgz5O-lm6hNXVY1OTTHyuhY51Ypg,442368
-xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
-xia_compiler_jsoneditor-0.0.9.dist-info/METADATA,sha256=hBLUogY3Pa1mkhCQFye-w68MUtyhcd2FXWvo3xl6PVM,687
-xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
-xia_compiler_jsoneditor-0.0.9.dist-info/RECORD,,
+xia_compiler_jsoneditor/__init__.py,sha256=VVoUNP-ZaWiuh8MgDo4H1bvEiaZPypokL9YW-vc4B34,135
+xia_compiler_jsoneditor/compiler.cpython-310-darwin.so,sha256=0H_Pgxk9IuOu3qDAJlSXrEKNweTf_U136kzDDnw5osc,386136
+xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt,sha256=uYnvfTF5TW6hakbLwlmA14uetnfEmRohRS_PHhU5dY4,151
+xia_compiler_jsoneditor-0.1.0.dist-info/METADATA,sha256=p9Dm8AMkbl-ruG4bN3WfIBo0RoTSqqPSUYZxPi3X1Ac,650
+xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
+xia_compiler_jsoneditor-0.1.0.dist-info/RECORD,,
```

