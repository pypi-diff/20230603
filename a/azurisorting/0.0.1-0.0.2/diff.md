# Comparing `tmp/azurisorting-0.0.1.tar.gz` & `tmp/azurisorting-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurisorting-0.0.1.tar", last modified: Wed May 31 12:26:28 2023, max compression
+gzip compressed data, was "azurisorting-0.0.2.tar", last modified: Sat Jun  3 12:35:08 2023, max compression
```

## Comparing `azurisorting-0.0.1.tar` & `azurisorting-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-05-31 12:26:27.999401 azurisorting-0.0.1/
--rw-r--r--   0 azure     (1000) azure     (1000)      863 2023-05-31 12:26:27.992401 azurisorting-0.0.1/PKG-INFO
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-05-31 12:26:27.976401 azurisorting-0.0.1/azurisorting/
--rw-r--r--   0 azure     (1000) azure     (1000)     1013 2023-05-31 12:08:43.000000 azurisorting-0.0.1/azurisorting/ACS.py
--rw-r--r--   0 azure     (1000) azure     (1000)     1148 2023-05-31 12:08:51.000000 azurisorting-0.0.1/azurisorting/AFS.py
--rw-r--r--   0 azure     (1000) azure     (1000)     1785 2023-05-31 12:08:52.000000 azurisorting-0.0.1/azurisorting/AS.py
--rw-r--r--   0 azure     (1000) azure     (1000)       96 2023-05-31 12:12:51.000000 azurisorting-0.0.1/azurisorting/__init__.py
-drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-05-31 12:26:27.991401 azurisorting-0.0.1/azurisorting.egg-info/
--rw-r--r--   0 azure     (1000) azure     (1000)      863 2023-05-31 12:26:27.000000 azurisorting-0.0.1/azurisorting.egg-info/PKG-INFO
--rw-r--r--   0 azure     (1000) azure     (1000)      236 2023-05-31 12:26:27.000000 azurisorting-0.0.1/azurisorting.egg-info/SOURCES.txt
--rw-r--r--   0 azure     (1000) azure     (1000)        1 2023-05-31 12:26:27.000000 azurisorting-0.0.1/azurisorting.egg-info/dependency_links.txt
--rw-r--r--   0 azure     (1000) azure     (1000)       13 2023-05-31 12:26:27.000000 azurisorting-0.0.1/azurisorting.egg-info/top_level.txt
--rw-r--r--   0 azure     (1000) azure     (1000)       38 2023-05-31 12:26:27.999401 azurisorting-0.0.1/setup.cfg
--rw-r--r--   0 azure     (1000) azure     (1000)     1335 2023-05-31 12:21:27.000000 azurisorting-0.0.1/setup.py
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.617834 azurisorting-0.0.2/
+-rw-r--r--   0 azure     (1000) azure     (1000)      940 2023-06-03 12:35:08.615834 azurisorting-0.0.2/PKG-INFO
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.610834 azurisorting-0.0.2/azurisorting/
+-rw-r--r--   0 azure     (1000) azure     (1000)     1013 2023-05-31 12:08:43.000000 azurisorting-0.0.2/azurisorting/ACS.py
+-rw-r--r--   0 azure     (1000) azure     (1000)     1299 2023-06-03 12:31:42.000000 azurisorting-0.0.2/azurisorting/AFS.py
+-rw-r--r--   0 azure     (1000) azure     (1000)     1785 2023-05-31 12:08:52.000000 azurisorting-0.0.2/azurisorting/AS.py
+-rw-r--r--   0 azure     (1000) azure     (1000)       52 2023-06-03 12:32:15.000000 azurisorting-0.0.2/azurisorting/__init__.py
+drwxr-xr-x   0 azure     (1000) azure     (1000)        0 2023-06-03 12:35:08.614834 azurisorting-0.0.2/azurisorting.egg-info/
+-rw-r--r--   0 azure     (1000) azure     (1000)      940 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/PKG-INFO
+-rw-r--r--   0 azure     (1000) azure     (1000)      236 2023-06-03 12:35:08.000000 azurisorting-0.0.2/azurisorting.egg-info/SOURCES.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)        1 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/dependency_links.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)       13 2023-06-03 12:35:07.000000 azurisorting-0.0.2/azurisorting.egg-info/top_level.txt
+-rw-r--r--   0 azure     (1000) azure     (1000)       38 2023-06-03 12:35:08.617834 azurisorting-0.0.2/setup.cfg
+-rw-r--r--   0 azure     (1000) azure     (1000)     1405 2023-06-03 12:34:11.000000 azurisorting-0.0.2/setup.py
```

### Comparing `azurisorting-0.0.1/azurisorting/ACS.py` & `azurisorting-0.0.2/azurisorting/ACS.py`

 * *Files identical despite different names*

### Comparing `azurisorting-0.0.1/azurisorting/AFS.py` & `azurisorting-0.0.2/azurisorting/AS.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 '''
-AZURI FAST SORTER
+AZURI SORTER
 
-This sorting algorithm is faster than the default sorter.
-It only sorts once and is optimized for speed.
+This sorting algorithm is the default sorter.
+It sorts twice to correct any errors.
 
-Useful for small datasets.
+Useful for medium sized datasets.
 '''
-class AzuriFastSorter:
+class AzuriSorter:
+    #Default sorter for Azuri
+    def __init__(self):
+        pass
+    
+    def loadset(self, file):
+        #Return a dataset
+        with open(file, 'r') as f:
+            return f.read()
+    
     def sort(self, data):
+        #Sort the data
         data = list(data)
-        self._quick_sort(data, 0, len(data) - 1)
+        data = self._first_pass_sort(data)
+        data = self._second_pass_sort(data)
         data = ''.join(data)
         return data
-
-    def _quick_sort(self, data, low, high):
-        if low < high:
-            pivot_index = self._partition(data, low, high)
-            self._quick_sort(data, low, pivot_index - 1)
-            self._quick_sort(data, pivot_index + 1, high)
-
-    def _partition(self, data, low, high):
-        pivot = data[high]
-        i = low - 1
-        for j in range(low, high):
-            if self._sort_key(data[j]) <= self._sort_key(pivot):
-                i += 1
-                data[i], data[j] = data[j], data[i]
-        data[i + 1], data[high] = data[high], data[i + 1]
-        return i + 1
-
+    
+    def _first_pass_sort(self, data):
+        # First run through of sorting
+        for i in range(len(data)):
+            for j in range(i + 1, len(data)):
+                try:
+                    if self._sort_key(data[i]) > self._sort_key(data[j]):
+                        data[i], data[j] = data[j], data[i]
+                except ValueError as e:
+                    print(f"Unknown character encountered at position {i}:", e)
+        return data
+    
+    def _second_pass_sort(self, data):
+        # Second run through of sorting
+        for i in range(len(data)):
+            for j in range(i + 1, len(data)):
+                try:
+                    if self._sort_key(data[i]) == self._sort_key(data[j]) and data[i] > data[j]:
+                        data[i], data[j] = data[j], data[i]
+                except ValueError as e:
+                    print(f"Unknown character encountered at position {i}:", e)
+        return data
+    
     def _sort_key(self, item):
+        # Sort based on ASCII Key
         if isinstance(item, (float, int)):
-            return item
+            return item, item
         elif isinstance(item, str):
-            return ord(item)
+            return ord(item), item
         else:
             raise ValueError("Unknown character")
```

### Comparing `azurisorting-0.0.1/setup.py` & `azurisorting-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'This sorter is used to sort datasets based on their ASCII Position.'
-LONG_DESCRIPTION = "These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy."
+LONG_DESCRIPTION = "These sorters are based on speed with 3 options: AzuriSorter is the default sorter used. AzuriFastSorter is meant for small datasets, it doesn't perform any corrections. AzuriCorrectiveSorter is a sorter that runs through the data as many times specified it sacrifices speed for accuracy.\nFixes: Fixed Major error in which causes the package to be unusable."
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="azurisorting", 
         version=VERSION,
         author="Nathan Hornby",
```

