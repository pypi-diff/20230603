# Comparing `tmp/clevertable-3.0.1.tar.gz` & `tmp/clevertable-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-3.0.1.tar", last modified: Tue May 30 06:15:42 2023, max compression
+gzip compressed data, was "clevertable-3.0.3.tar", last modified: Sat Jun  3 10:24:27 2023, max compression
```

## Comparing `clevertable-3.0.1.tar` & `clevertable-3.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.807304 clevertable-3.0.1/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-3.0.1/LICENSE
--rw-rw-rw-   0        0        0    35991 2023-05-30 06:15:42.807304 clevertable-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    34221 2023-05-29 18:29:05.000000 clevertable-3.0.1/README.md
--rw-rw-rw-   0        0        0     1292 2023-05-30 06:14:55.000000 clevertable-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 06:15:42.807304 clevertable-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.744286 clevertable-3.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.791663 clevertable-3.0.1/src/clevertable/
--rw-rw-rw-   0        0        0     3518 2023-05-29 17:24:28.000000 clevertable-3.0.1/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3765 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4367 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0     1018 2023-05-29 18:08:53.000000 clevertable-3.0.1/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      291 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3297 2023-05-30 06:09:36.000000 clevertable-3.0.1/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      896 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4976 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      213 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      369 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3063 2023-05-30 06:02:41.000000 clevertable-3.0.1/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      398 2023-05-29 17:11:23.000000 clevertable-3.0.1/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1566 2023-05-29 18:13:39.000000 clevertable-3.0.1/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1558 2023-05-29 17:59:47.000000 clevertable-3.0.1/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1830 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2877 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     9269 2023-05-29 17:50:54.000000 clevertable-3.0.1/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      843 2023-05-29 17:51:55.000000 clevertable-3.0.1/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3576 2023-05-29 17:18:36.000000 clevertable-3.0.1/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      991 2023-05-29 17:52:36.000000 clevertable-3.0.1/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1194 2023-05-29 17:18:36.000000 clevertable-3.0.1/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2769 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-30 06:14:55.000000 clevertable-3.0.1/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2501 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.807304 clevertable-3.0.1/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    35991 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.869383 clevertable-3.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-01 10:04:41.000000 clevertable-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0    36138 2023-06-03 10:24:27.868050 clevertable-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    34368 2023-06-01 10:06:41.000000 clevertable-3.0.3/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-03 10:23:46.000000 clevertable-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 10:24:27.869383 clevertable-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-06-01 10:04:41.000000 clevertable-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.716666 clevertable-3.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.820853 clevertable-3.0.3/src/clevertable/
+-rw-rw-rw-   0        0        0     3518 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3765 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4367 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0     1018 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      291 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3297 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      896 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4976 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      369 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3087 2023-06-03 10:16:43.000000 clevertable-3.0.3/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      398 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1566 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1558 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1830 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2877 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     9272 2023-06-03 09:39:39.000000 clevertable-3.0.3/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      843 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3576 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      991 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1194 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2769 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-06-03 10:23:46.000000 clevertable-3.0.3/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2501 2023-06-01 10:04:41.000000 clevertable-3.0.3/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:24:27.852384 clevertable-3.0.3/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    36138 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 10:24:27.000000 clevertable-3.0.3/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-3.0.1/LICENSE` & `clevertable-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/PKG-INFO` & `clevertable-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.1
+Version: 3.0.3
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # CleverTable
+![Pytest](https://github.com/tom-mohr/clevertable/actions/workflows/pytest.yml/badge.svg)
 
 Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
@@ -114,15 +115,15 @@
   ```
 - Send multiple columns into one converter:
   ```python
   profile["Column 1", "Column 2"] = max
   ```
 - Send nested columns into one converter:
   ```python
-  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  profile[("Column A", "Column B"), "Column C"] = [Parallel(max, floor), min]  # min(max(A, B), floor(C))
   ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
@@ -367,15 +368,15 @@
 | [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
 | Special:                              |                                                                                     |           |                                                                 |
 | [`Id()`](#id)                         |                                                                                     |           |                                                                 |
 | [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
 | [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
 | [`Label()`](#label)                   |                                                                                     |           |                                                                 |
 | Dimensionality:                       |                                                                                     |           |                                                                 |
-| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a tuple of tuples into a single tuple. This is often needed after `ForEach()` or `Parallel()`. |           |                                                                 |
 | [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
 | Arbitrary Functions:                  |                                                                                     |           |                                                                 |
 | [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
 | [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
```

### Comparing `clevertable-3.0.1/README.md` & `clevertable-3.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # CleverTable
+![Pytest](https://github.com/tom-mohr/clevertable/actions/workflows/pytest.yml/badge.svg)
 
 Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
@@ -77,15 +78,15 @@
   ```
 - Send multiple columns into one converter:
   ```python
   profile["Column 1", "Column 2"] = max
   ```
 - Send nested columns into one converter:
   ```python
-  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  profile[("Column A", "Column B"), "Column C"] = [Parallel(max, floor), min]  # min(max(A, B), floor(C))
   ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
@@ -330,15 +331,15 @@
 | [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
 | Special:                              |                                                                                     |           |                                                                 |
 | [`Id()`](#id)                         |                                                                                     |           |                                                                 |
 | [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
 | [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
 | [`Label()`](#label)                   |                                                                                     |           |                                                                 |
 | Dimensionality:                       |                                                                                     |           |                                                                 |
-| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a tuple of tuples into a single tuple. This is often needed after `ForEach()` or `Parallel()`. |           |                                                                 |
 | [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
 | Arbitrary Functions:                  |                                                                                     |           |                                                                 |
 | [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
 | [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
```

### Comparing `clevertable-3.0.1/pyproject.toml` & `clevertable-3.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "3.0.1"
+version = "3.0.3"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,24 +19,24 @@
     "numpy",
     "pandas",
     "openpyxl",  # needed for xlsx support
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["bumpver", "twine", "pytest"]
+dev = ["bumpver", "build", "twine", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "3.0.1"
+current_version = "3.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-3.0.1/src/clevertable/Binary.py` & `clevertable-3.0.3/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/ConversionProfile.py` & `clevertable-3.0.3/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Converter.py` & `clevertable-3.0.3/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/DataFrameProfile.py` & `clevertable-3.0.3/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Enumerate.py` & `clevertable-3.0.3/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Float.py` & `clevertable-3.0.3/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/ForEach.py` & `clevertable-3.0.3/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Function.py` & `clevertable-3.0.3/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Infer.py` & `clevertable-3.0.3/src/clevertable/Infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         :raises ValueError: if no converter can be inferred and ignore_uninferrable is False
         """
         try:
             self.inferred = _infer_converter_from_data(rows)
         except ValueError as e:
             if self.ignore_uninferrable:
                 self.inferred = Ignore()
+                return
             raise e
         self.inferred.fit(rows)
 
     def labels(self, labels: tuple) -> tuple:
         return self.inferred.labels(labels)
 
     def transform(self, row: tuple) -> tuple:
```

### Comparing `clevertable-3.0.1/src/clevertable/List.py` & `clevertable-3.0.3/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Map.py` & `clevertable-3.0.3/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/OneHot.py` & `clevertable-3.0.3/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Parallel.py` & `clevertable-3.0.3/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Pipeline.py` & `clevertable-3.0.3/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/RecordProfile.py` & `clevertable-3.0.3/src/clevertable/RecordProfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             else:
                 rows = [
                     (d[key],)  # wrap single element (row needs to be a tuple)
                     for d in dicts
                     if key in d
                 ]
             if not rows:
-                raise ValueError(f"Not a single value for key {repr(key)} present int fit()!"
+                raise ValueError(f"Not a single value for key {repr(key)} present during fit()!"
                                  f" You must at least provide one value to fit() for this key.")
                 pass
 
             try:
                 conv.fit(rows)
             except Exception as e:
                 # add helpful context to error message
```

### Comparing `clevertable-3.0.1/src/clevertable/Split.py` & `clevertable-3.0.3/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/StrictFunction.py` & `clevertable-3.0.3/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Strip.py` & `clevertable-3.0.3/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Transpose.py` & `clevertable-3.0.3/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/Try.py` & `clevertable-3.0.3/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/__init__.py` & `clevertable-3.0.3/src/clevertable/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-3.0.1/src/clevertable/__main__.py` & `clevertable-3.0.3/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable/_utils.py` & `clevertable-3.0.3/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.1/src/clevertable.egg-info/PKG-INFO` & `clevertable-3.0.3/src/clevertable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.1
+Version: 3.0.3
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # CleverTable
+![Pytest](https://github.com/tom-mohr/clevertable/actions/workflows/pytest.yml/badge.svg)
 
 Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
@@ -114,15 +115,15 @@
   ```
 - Send multiple columns into one converter:
   ```python
   profile["Column 1", "Column 2"] = max
   ```
 - Send nested columns into one converter:
   ```python
-  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  profile[("Column A", "Column B"), "Column C"] = [Parallel(max, floor), min]  # min(max(A, B), floor(C))
   ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
@@ -367,15 +368,15 @@
 | [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
 | Special:                              |                                                                                     |           |                                                                 |
 | [`Id()`](#id)                         |                                                                                     |           |                                                                 |
 | [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
 | [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
 | [`Label()`](#label)                   |                                                                                     |           |                                                                 |
 | Dimensionality:                       |                                                                                     |           |                                                                 |
-| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a tuple of tuples into a single tuple. This is often needed after `ForEach()` or `Parallel()`. |           |                                                                 |
 | [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
 | Arbitrary Functions:                  |                                                                                     |           |                                                                 |
 | [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
 | [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
```

### Comparing `clevertable-3.0.1/src/clevertable.egg-info/SOURCES.txt` & `clevertable-3.0.3/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

