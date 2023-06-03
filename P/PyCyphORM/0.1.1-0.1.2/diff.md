# Comparing `tmp/PyCyphORM-0.1.1-py3-none-any.whl.zip` & `tmp/PyCyphORM-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,9 @@
-Zip file size: 5807 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       22 b- defN 23-Mar-08 20:36 bin/__init__.py
--rw-rw-r--  2.0 unx     1390 b- defN 23-Jun-03 00:29 bin/pycyphorm.py
--rw-rw-r--  2.0 unx     1326 b- defN 23-Mar-10 01:14 bin/pyorm.py
--rw-rw-r--  2.0 unx       53 b- defN 23-Mar-08 23:57 lib/__init__.py
--rw-rw-r--  2.0 unx     1836 b- defN 23-Mar-12 11:31 lib/adapter.py
--rw-rw-r--  2.0 unx     5212 b- defN 23-Mar-08 21:52 lib/orm.py
--rw-rw-r--  2.0 unx     1031 b- defN 23-Jun-03 00:47 PyCyphORM-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 00:47 PyCyphORM-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Jun-03 00:47 PyCyphORM-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-03 00:47 PyCyphORM-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-03 00:47 PyCyphORM-0.1.1.dist-info/RECORD
-11 files, 11840 bytes uncompressed, 4429 bytes compressed:  62.6%
+Zip file size: 2755 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       91 b- defN 23-Jun-03 01:40 src/__init__.py
+-rw-rw-r--  2.0 unx     1394 b- defN 23-Jun-03 01:39 src/cli.py
+-rw-rw-r--  2.0 unx     1130 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      539 b- defN 23-Jun-03 01:46 PyCyphORM-0.1.2.dist-info/RECORD
+7 files, 3288 bytes uncompressed, 1795 bytes compressed:  45.4%
```

## zipnote {}

```diff
@@ -1,34 +1,22 @@
-Filename: bin/__init__.py
+Filename: src/__init__.py
 Comment: 
 
-Filename: bin/pycyphorm.py
+Filename: src/cli.py
 Comment: 
 
-Filename: bin/pyorm.py
+Filename: PyCyphORM-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: lib/__init__.py
+Filename: PyCyphORM-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: lib/adapter.py
+Filename: PyCyphORM-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: lib/orm.py
+Filename: PyCyphORM-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: PyCyphORM-0.1.1.dist-info/METADATA
-Comment: 
-
-Filename: PyCyphORM-0.1.1.dist-info/WHEEL
-Comment: 
-
-Filename: PyCyphORM-0.1.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: PyCyphORM-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: PyCyphORM-0.1.1.dist-info/RECORD
+Filename: PyCyphORM-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bin/pycyphorm.py` & `src/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,14 @@
                 "SALT": b16encode(urandom(16)).decode("utf-8"),
                 "PASSWORD": b16encode(bytes(random_password(), "utf-8")).decode("utf-8")
             }))
 
     elif args['decrypt']:
         if path.exists(path.abspath(args['decrypt'])):
             
-            from lib.adapter import decrypt_cdb, load_config
+            from src.lib.adapter import decrypt_cdb, load_config
             
             cnf = load_config(".pyorm")
             decrypt_cdb(path.abspath(args['decrypt']), cnf["PASSWORD"], cnf["SALT"])
 
 
 if __name__ == "__main__": cli()
```

