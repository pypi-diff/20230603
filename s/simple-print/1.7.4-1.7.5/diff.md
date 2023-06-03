# Comparing `tmp/simple_print-1.7.4-py3-none-any.whl.zip` & `tmp/simple_print-1.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 7787 bytes, number of entries: 11
+Zip file size: 9000 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       51 b- defN 23-Apr-28 06:49 simple_print/__init__.py
 -rw-rw-r--  2.0 unx     4467 b- defN 22-Dec-04 17:59 simple_print/broker.py
--rw-rw-r--  2.0 unx     4538 b- defN 23-May-17 07:41 simple_print/sprint.py
+-rw-rw-r--  2.0 unx     4716 b- defN 23-Jun-03 06:28 simple_print/sprint.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-21 11:16 test/__init__.py
 -rw-rw-r--  2.0 unx      220 b- defN 22-Dec-04 18:00 test/test_broker.py
 -rw-rw-r--  2.0 unx     1861 b- defN 23-Feb-27 07:48 test/test_print.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-May-17 07:44 simple_print-1.7.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2605 b- defN 23-May-17 07:44 simple_print-1.7.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 07:44 simple_print-1.7.4.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       18 b- defN 23-May-17 07:44 simple_print-1.7.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      868 b- defN 23-May-17 07:44 simple_print-1.7.4.dist-info/RECORD
-11 files, 15814 bytes uncompressed, 6319 bytes compressed:  60.0%
+-rw-rw-r--  2.0 unx     1960 b- defN 23-Jun-03 06:11 test/test_sprint.py
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jun-03 06:34 test/test_sprint_err.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-03 06:37 simple_print-1.7.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2580 b- defN 23-Jun-03 06:37 simple_print-1.7.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 06:37 simple_print-1.7.5.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       18 b- defN 23-Jun-03 06:37 simple_print-1.7.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-03 06:37 simple_print-1.7.5.dist-info/RECORD
+13 files, 18473 bytes uncompressed, 7296 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -12,23 +12,29 @@
 
 Filename: test/test_broker.py
 Comment: 
 
 Filename: test/test_print.py
 Comment: 
 
-Filename: simple_print-1.7.4.dist-info/LICENSE
+Filename: test/test_sprint.py
 Comment: 
 
-Filename: simple_print-1.7.4.dist-info/METADATA
+Filename: test/test_sprint_err.py
 Comment: 
 
-Filename: simple_print-1.7.4.dist-info/WHEEL
+Filename: simple_print-1.7.5.dist-info/LICENSE
 Comment: 
 
-Filename: simple_print-1.7.4.dist-info/top_level.txt
+Filename: simple_print-1.7.5.dist-info/METADATA
 Comment: 
 
-Filename: simple_print-1.7.4.dist-info/RECORD
+Filename: simple_print-1.7.5.dist-info/WHEEL
+Comment: 
+
+Filename: simple_print-1.7.5.dist-info/top_level.txt
+Comment: 
+
+Filename: simple_print-1.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_print/sprint.py

```diff
@@ -106,17 +106,18 @@
             s = s[:-1]
         return s
 
     if DEBUG:
         stack = traceback.extract_stack()
         filename, lineno, function_name, code = stack[-3]
 
-        cprint(f"\nSprintErr. filename={filename} lineno={lineno} [ START OK ]", color="green")
+        cprint(f"░░░░░░░░░░ SprintErr. f_name={filename} lineno={lineno} [ ENTER ]", color="green")
         try:
             yield 
         except Exception as e:
+            cprint(f"░░░░░░░░░░ SprintErr. f_name={filename} lineno={lineno} [ ERRORS FOUND ]\n", color="red")
             ei = sys.exc_info()
             print(format_exception(ei))
         finally:
-            cprint(f"SprintErr. filename={filename} lineno={lineno} [ FINISH OK ]\n", color="yellow")
+            cprint(f"░░░░░░░░░░ SprintErr. f_name={filename} lineno={lineno} [ EXIT ]\n", color="green")
```

## Comparing `simple_print-1.7.4.dist-info/LICENSE` & `simple_print-1.7.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simple_print-1.7.4.dist-info/METADATA` & `simple_print-1.7.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-print
-Version: 1.7.4
+Version: 1.7.5
 Summary: Powerful debugging tool for Python.
 Home-page: https://github.com/Sobolev5/simple-print/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -91,11 +91,11 @@
 Always show path to file:  
 ```sh
 export SIMPLE_PRINT_SHOW_PATH_TO_FILE=True
 ```
 
 ### Test 
 ```sh
-pytest test/test_print.py -s
+tox
 ```
```

