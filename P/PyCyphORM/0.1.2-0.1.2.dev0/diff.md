# Comparing `tmp/PyCyphORM-0.1.2-py3-none-any.whl.zip` & `tmp/PyCyphORM-0.1.2.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,7 @@
-Zip file size: 2755 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       91 b- defN 23-Jun-03 01:40 src/__init__.py
--rw-rw-r--  2.0 unx     1394 b- defN 23-Jun-03 01:39 src/cli.py
--rw-rw-r--  2.0 unx     1130 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       38 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      539 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/RECORD
-7 files, 3288 bytes uncompressed, 1795 bytes compressed:  45.4%
+Zip file size: 1785 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx     1135 b- defN 23-Jun-03 02:03 PyCyphORM-0.1.2.dev0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 02:03 PyCyphORM-0.1.2.dev0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-03 02:03 PyCyphORM-0.1.2.dev0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-Jun-03 02:03 PyCyphORM-0.1.2.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-03 02:03 PyCyphORM-0.1.2.dev0.dist-info/RECORD
+5 files, 1696 bytes uncompressed, 977 bytes compressed:  42.4%
```

## zipnote {}

```diff
@@ -1,22 +1,16 @@
-Filename: src/__init__.py
+Filename: PyCyphORM-0.1.2.dev0.dist-info/METADATA
 Comment: 
 
-Filename: src/cli.py
+Filename: PyCyphORM-0.1.2.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: PyCyphORM-0.1.2.dist-info/METADATA
+Filename: PyCyphORM-0.1.2.dev0.dist-info/entry_points.txt
 Comment: 
 
-Filename: PyCyphORM-0.1.2.dist-info/WHEEL
+Filename: PyCyphORM-0.1.2.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: PyCyphORM-0.1.2.dist-info/entry_points.txt
-Comment: 
-
-Filename: PyCyphORM-0.1.2.dist-info/top_level.txt
-Comment: 
-
-Filename: PyCyphORM-0.1.2.dist-info/RECORD
+Filename: PyCyphORM-0.1.2.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `PyCyphORM-0.1.2.dist-info/METADATA` & `PyCyphORM-0.1.2.dev0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCyphORM
-Version: 0.1.2
+Version: 0.1.2.dev0
 Summary: A Minimalistic SQLite InMemory Encrypted ORM
 Author: jafrmartins
 Author-email: j.afr.martins@outlook.pt
 Keywords: sqlite encrypted inmemory orm
 Description-Content-Type: text/markdown
 
 # PyCyphOrm
```

