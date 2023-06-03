# Comparing `tmp/colablib-0.1.6.tar.gz` & `tmp/colablib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.6.tar", last modified: Fri Jun  2 07:31:39 2023, max compression
+gzip compressed data, was "colablib-0.1.7.tar", last modified: Sat Jun  3 09:25:08 2023, max compression
```

## Comparing `colablib-0.1.6.tar` & `colablib-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/
--rw-rw-rw-   0        0        0      213 2023-06-02 07:31:39.142990 colablib-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.123374 colablib-0.1.6/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.6/colablib/colored_print.py
-drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/colablib/sd_models/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/sd_models/__init__.py
--rw-rw-rw-   0        0        0     3752 2023-06-02 05:08:40.000000 colablib-0.1.6/colablib/sd_models/downloader.py
--rw-rw-rw-   0        0        0     9083 2023-06-02 06:32:59.000000 colablib-0.1.6/colablib/sd_models/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/colablib/utils/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/utils/__init__.py
--rw-rw-rw-   0        0        0     2416 2023-06-02 07:15:23.000000 colablib-0.1.6/colablib/utils/git_utils.py
--rw-rw-rw-   0        0        0     3338 2023-06-02 07:15:25.000000 colablib-0.1.6/colablib/utils/py_utils.py
--rw-rw-rw-   0        0        0     1180 2023-06-02 03:58:41.000000 colablib-0.1.6/colablib/utils/ubuntu_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.134917 colablib-0.1.6/colablib.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-06-02 07:31:39.000000 colablib-0.1.6/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 07:31:39.142990 colablib-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-06-02 07:31:30.000000 colablib-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:25:08.759241 colablib-0.1.7/
+-rw-rw-rw-   0        0        0      213 2023-06-03 09:25:08.758231 colablib-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 09:25:08.721456 colablib-0.1.7/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.7/colablib/__init__.py
+-rw-rw-rw-   0        0        0     3668 2023-06-03 03:17:55.000000 colablib-0.1.7/colablib/colored_print.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:25:08.751227 colablib-0.1.7/colablib/sd_models/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.7/colablib/sd_models/__init__.py
+-rw-rw-rw-   0        0        0     6084 2023-06-03 09:13:54.000000 colablib-0.1.7/colablib/sd_models/downloader.py
+-rw-rw-rw-   0        0        0     9083 2023-06-02 06:32:59.000000 colablib-0.1.7/colablib/sd_models/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:25:08.756595 colablib-0.1.7/colablib/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.7/colablib/utils/__init__.py
+-rw-rw-rw-   0        0        0    12009 2023-06-03 08:44:00.000000 colablib-0.1.7/colablib/utils/git_utils.py
+-rw-rw-rw-   0        0        0     3336 2023-06-03 08:45:32.000000 colablib-0.1.7/colablib/utils/py_utils.py
+-rw-rw-rw-   0        0        0     1355 2023-06-03 08:51:03.000000 colablib-0.1.7/colablib/utils/ubuntu_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:25:08.747757 colablib-0.1.7/colablib.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-03 09:25:08.000000 colablib-0.1.7/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-03 09:25:08.000000 colablib-0.1.7/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:25:08.000000 colablib-0.1.7/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-03 09:25:08.000000 colablib-0.1.7/colablib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 09:25:08.000000 colablib-0.1.7/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:25:08.759241 colablib-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      430 2023-06-03 09:23:35.000000 colablib-0.1.7/setup.py
```

### Comparing `colablib-0.1.6/colablib/sd_models/validators.py` & `colablib-0.1.7/colablib/sd_models/validators.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.6/colablib/utils/py_utils.py` & `colablib-0.1.7/colablib/utils/py_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     elapsed_time = int(end_time - start_time)
 
     if elapsed_time < 60:
         return f"{elapsed_time} sec"
     else:
         mins, secs = divmod(elapsed_time, 60)
         return f"{mins} mins {secs} sec"
-
     
 def get_filename(url):
     """
     Extracts the filename from the given URL.
 
     Args:
         url (str): The URL to extract the filename from.
```

### Comparing `colablib-0.1.6/colablib/utils/ubuntu_utils.py` & `colablib-0.1.7/colablib/utils/ubuntu_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import zipfile
-import subprocess
 import requests
 import shutil
 from .py_utils import get_filename
 from tqdm import tqdm
 from ..colored_print import cprint
 
 def ubuntu_deps(url, dst, desc=None):
@@ -20,20 +19,26 @@
     
     response = requests.get(url, stream=True)
     response.raise_for_status()
     
     with open(filename, 'wb') as file:
         for chunk in response.iter_content(chunk_size=8192):
             file.write(chunk)
-            
-    with zipfile.ZipFile(filename, "r") as deps:
-        deps.extractall(dst)
 
-    if desc is None:
-        desc = cprint("Installing...", color="green", tqdm_desc=True)
+    if filename.endswith(".zip"):
+        with zipfile.ZipFile(filename, "r") as deps:
+            deps.extractall(dst)
+
+        if desc is None:
+            desc = cprint("Installing...", color="green", tqdm_desc=True)
 
-    deb_files = [os.path.join(dst, f) for f in os.listdir(dst) if f.endswith('.deb')]
-    for deb_file in tqdm(deb_files, desc=desc):
+        deb_files = [os.path.join(dst, f) for f in os.listdir(dst) if f.endswith('.deb')]
+        for deb_file in tqdm(deb_files, desc=desc):
+            os.system(f'dpkg -i {deb_file}')
+            
+        os.remove(filename)
+        shutil.rmtree(dst)
+
+    elif filename.endswith(".deb"):
+        deb_file = os.path.join(dst, filename)
         os.system(f'dpkg -i {deb_file}')
-        
-    os.remove(filename)
-    shutil.rmtree(dst)
+
```

