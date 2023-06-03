# Comparing `tmp/knapsack-0.0.7-py3-none-any.whl.zip` & `tmp/knapsack-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2785 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1096 b- defN 80-Jan-01 00:00 knapsack/__init__.py
--rw-r--r--  2.0 unx     1070 b- defN 80-Jan-01 00:00 knapsack-0.0.7.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 knapsack-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1300 b- defN 16-Jan-01 00:00 knapsack-0.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx      375 b- defN 16-Jan-01 00:00 knapsack-0.0.7.dist-info/RECORD
-5 files, 3924 bytes uncompressed, 2091 bytes compressed:  46.7%
+Zip file size: 5893 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1103 b- defN 80-Jan-01 00:00 knapsack/__init__.py
+-rw-r--r--  2.0 unx    10758 b- defN 80-Jan-01 00:00 knapsack-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1272 b- defN 80-Jan-01 00:00 knapsack-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 knapsack-0.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      376 b- defN 16-Jan-01 00:00 knapsack-0.1.0.dist-info/RECORD
+5 files, 13597 bytes uncompressed, 5199 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: knapsack/__init__.py
 Comment: 
 
-Filename: knapsack-0.0.7.dist-info/LICENSE
+Filename: knapsack-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: knapsack-0.0.7.dist-info/WHEEL
+Filename: knapsack-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: knapsack-0.0.7.dist-info/METADATA
+Filename: knapsack-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: knapsack-0.0.7.dist-info/RECORD
+Filename: knapsack-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## knapsack/__init__.py

```diff
@@ -23,15 +23,15 @@
     knapsack.knapsack(size, weight).solve(capacity)
     """
 
     def __init__(self, size, weight):
         self.size = size
         self.weight = weight
 
-    @lru_cache(maxsize=4096)
+    @lru_cache(maxsize=4096 * 4096)
     def solve(self, cap, i=0):
         if cap < 0:
             return -sum(self.weight), []
         if i == len(self.size):
             return 0, []
         res1 = self.solve(cap, i + 1)
         res2 = self.solve(cap - self.size[i], i + 1)
```

## Comparing `knapsack-0.0.7.dist-info/METADATA` & `knapsack-0.1.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: knapsack
-Version: 0.0.7
+Version: 0.1.0
 Summary: `knapsack` is a package for for solving knapsack problem.
 Home-page: https://github.com/SaitoTsutomu/knapsack
-License: MIT
+License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst
 
 `knapsack` is a package for solving knapsack problem.
 Maximize sum of selected weight.
 Sum of selected size is les than capacity.
```

