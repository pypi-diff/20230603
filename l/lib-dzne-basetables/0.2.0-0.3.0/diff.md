# Comparing `tmp/lib-dzne-basetables-0.2.0.tar.gz` & `tmp/lib-dzne-basetables-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-basetables-0.2.0.tar", last modified: Mon May 29 12:56:27 2023, max compression
+gzip compressed data, was "lib-dzne-basetables-0.3.0.tar", last modified: Fri Jun  2 22:17:33 2023, max compression
```

## Comparing `lib-dzne-basetables-0.2.0.tar` & `lib-dzne-basetables-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.2.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       22 2023-05-29 09:10:54.000000 lib-dzne-basetables-0.2.0/README.md
--rw-r--r--   0 base      (1001) base      (1001)      528 2023-05-29 12:56:17.000000 lib-dzne-basetables-0.2.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.472574 lib-dzne-basetables-0.2.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.472574 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/
--rw-r--r--   0 base      (1001) base      (1001)       54 2023-05-29 12:54:38.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     2363 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/baseconv.py
--rw-r--r--   0 base      (1001) base      (1001)      675 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/common.py
--rw-rw-r--   0 base      (1001) base      (1001)     1241 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/data.py
--rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/pattern.py
--rw-r--r--   0 base      (1001) base      (1001)     7732 2023-05-29 12:54:58.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/table.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      482 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       22 2023-05-29 09:10:54.000000 lib-dzne-basetables-0.3.0/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      528 2023-06-02 22:16:56.000000 lib-dzne-basetables-0.3.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/
+-rw-r--r--   0 base      (1001) base      (1001)       88 2023-06-02 22:16:04.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/__init__.py
+-rw-rw-r--   0 base      (1001) base      (1001)     1732 2023-06-02 22:17:06.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/_data.py
+-rw-r--r--   0 base      (1001) base      (1001)     2363 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/baseconv.py
+-rw-r--r--   0 base      (1001) base      (1001)      675 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/common.py
+-rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/pattern.py
+-rw-r--r--   0 base      (1001) base      (1001)     7732 2023-05-29 12:54:58.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/table.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      483 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/top_level.txt
```

### Comparing `lib-dzne-basetables-0.2.0/LICENSE` & `lib-dzne-basetables-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.2.0/PKG-INFO` & `lib-dzne-basetables-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.2.0
+Version: 0.3.0
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-basetables-0.2.0/pyproject.toml` & `lib-dzne-basetables-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-basetables"
-version = "0.2.0"
+version = "0.3.0"
 description = "Libary for basetables. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/baseconv.py` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/baseconv.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/common.py` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/common.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/data.py` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,58 @@
-import lib_dzne_basetable as _bt
+import lib_dzne_basetable.baseconv as _baseconv
+import lib_dzne_basetable.table as _table
 import lib_dzne_tsv as _tsv
+import pandas as _pd
 
 
 class BASEData(_tsv.TSVData):
+    _ext = None
     @classmethod
     def basetype(cls):
+        if cls._ext is None:
+            return None
         if cls._ext.startswith("."):
             raise ValueError()
         if cls._ext.startswith("base"):
             raise ValueError()
         return cls._ext[1:-4]
     @classmethod
     def _load(cls, /, file, **kwargs):
         ans = super().load(file, **kwargs).dataFrame
-        ans = _bt.table.make(ans, basetype=cls.basetype())
+        ans = _table.make(ans, basetype=cls.basetype())
         return ans
     def _save(self, /, file):
-        data = _bt.table.make(data, basetype=self.basetype())
+        data = _table.make(data, basetype=self.basetype())
         super().save(string, data)
     @classmethod
     def _default(cls):
-        return _bt.table.make(basetype=cls.basetype())
+        return _table.make(basetype=cls.basetype())
     @classmethod
     def from_file(cls, file, /):
         return super().from_file(file, ABASEData, CBASEData, DBASEData, MBASEData, YBASEData)
     @classmethod
     def clone_data(cls, data, /):
         data = super().clone_data(data)
-        return _bt.table.make(data, basetype=cls.basetype())
+        return _table.make(data, basetype=cls.basetype())
+    @classmethod
+    def concat(cls, *args):
+        args = [cls(x).data for x in args]
+        fulltable = _pd.concat(args, axis=0, ignore_index=True)
+        return cls(fulltable)
+
+
 class ABASEData(BASEData):
     _ext = ".abase"
+    @property
+    def dBASE(self):
+        return DBASEData(_baseconv.a2d(self.data))
 class CBASEData(BASEData):
     _ext = ".cbase"
 class DBASEData(BASEData):
     _ext = ".dbase"
 class MBASEData(BASEData):
     _ext = ".mbase"
 class YBASEData(BASEData):
-    _ext = ".ybase"
+    _ext = ".ybase"
+    @property
+    def cBASE(self):
+        return CBASEData(_baseconv.y2c(self.data))
```

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/pattern.py` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/pattern.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/table.py` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/table.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/PKG-INFO` & `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.2.0
+Version: 0.3.0
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

