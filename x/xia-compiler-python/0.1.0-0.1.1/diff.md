# Comparing `tmp/xia_compiler_python-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.1-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 155741 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-03 19:04 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx   397312 b- defN 23-Jun-03 19:07 xia_compiler_python/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-03 19:07 xia_compiler_python-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-03 19:07 xia_compiler_python-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-03 19:07 xia_compiler_python-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 19:07 xia_compiler_python-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      641 b- defN 23-Jun-03 19:07 xia_compiler_python-0.1.0.dist-info/RECORD
-7 files, 399013 bytes uncompressed, 154585 bytes compressed:  61.3%
+Zip file size: 128183 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-03 19:05 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx   339752 b- defN 23-Jun-03 19:05 xia_compiler_python/compiler.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-03 19:05 xia_compiler_python-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      637 b- defN 23-Jun-03 19:05 xia_compiler_python-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-03 19:05 xia_compiler_python-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 19:05 xia_compiler_python-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      645 b- defN 23-Jun-03 19:05 xia_compiler_python-0.1.1.dist-info/RECORD
+7 files, 341429 bytes uncompressed, 127021 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
-Filename: xia_compiler_python/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_python/compiler.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_compiler_python-0.1.0.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.0.dist-info/METADATA
+Filename: xia_compiler_python-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.0.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.0.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.0.dist-info/RECORD
+Filename: xia_compiler_python-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

