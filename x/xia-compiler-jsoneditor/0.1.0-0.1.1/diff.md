# Comparing `tmp/xia_compiler_jsoneditor-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_jsoneditor-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 171514 bytes, number of entries: 7
--rw-r--r--  2.0 unx      135 b- defN 23-Jun-03 15:42 xia_compiler_jsoneditor/__init__.py
--rw-r--r--  2.0 unx   454656 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      687 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Jun-03 15:46 xia_compiler_jsoneditor-0.1.0.dist-info/RECORD
-7 files, 456421 bytes uncompressed, 170302 bytes compressed:  62.7%
+Zip file size: 171431 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-03 20:10 xia_compiler_jsoneditor/__init__.py
+-rw-r--r--  2.0 unx   454656 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      687 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Jun-03 20:13 xia_compiler_jsoneditor-0.1.1.dist-info/RECORD
+7 files, 456421 bytes uncompressed, 170219 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_jsoneditor/__init__.py
 Comment: 
 
 Filename: xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt
+Filename: xia_compiler_jsoneditor-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.0.dist-info/METADATA
+Filename: xia_compiler_jsoneditor-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL
+Filename: xia_compiler_jsoneditor-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt
+Filename: xia_compiler_jsoneditor-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.0.dist-info/RECORD
+Filename: xia_compiler_jsoneditor-0.1.1.dist-info/RECORD
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
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_compiler_jsoneditor-0.1.0.dist-info/METADATA` & `xia_compiler_jsoneditor-0.1.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-jsoneditor
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_jsoneditor-0.1.0.dist-info/RECORD` & `xia_compiler_jsoneditor-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_jsoneditor/__init__.py,sha256=VVoUNP-ZaWiuh8MgDo4H1bvEiaZPypokL9YW-vc4B34,135
-xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=rZuhfb7a88y4nHA3FL0wnDK4qIGu_QY0oukcjJ1bcVQ,454656
-xia_compiler_jsoneditor-0.1.0.dist-info/LICENSE.txt,sha256=uYnvfTF5TW6hakbLwlmA14uetnfEmRohRS_PHhU5dY4,151
-xia_compiler_jsoneditor-0.1.0.dist-info/METADATA,sha256=qmvAPSnL6jtu0vovzaGMLT3X-5RaDz2s1AzAa2syygo,687
-xia_compiler_jsoneditor-0.1.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_jsoneditor-0.1.0.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
-xia_compiler_jsoneditor-0.1.0.dist-info/RECORD,,
+xia_compiler_jsoneditor/__init__.py,sha256=V-XpNNbUGY4OWqJuh1lPV3jY4vVvvfi5uPNHZfCJgB4,135
+xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=8ACVcH9Y-G8RINxS17ff0eQiCItxbPG2YItAaev5FPw,454656
+xia_compiler_jsoneditor-0.1.1.dist-info/LICENSE.txt,sha256=uYnvfTF5TW6hakbLwlmA14uetnfEmRohRS_PHhU5dY4,151
+xia_compiler_jsoneditor-0.1.1.dist-info/METADATA,sha256=axzMoJgdb37BPb5OVZV-uN_ENDWcm6SZtodgfPErqmk,687
+xia_compiler_jsoneditor-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_jsoneditor-0.1.1.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
+xia_compiler_jsoneditor-0.1.1.dist-info/RECORD,,
```

