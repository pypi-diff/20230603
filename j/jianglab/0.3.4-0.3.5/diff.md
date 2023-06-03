# Comparing `tmp/jianglab-0.3.4.tar.gz` & `tmp/jianglab-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.4.tar", last modified: Sat Jun  3 11:41:16 2023, max compression
+gzip compressed data, was "jianglab-0.3.5.tar", last modified: Sat Jun  3 12:23:23 2023, max compression
```

## Comparing `jianglab-0.3.4.tar` & `jianglab-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 11:41:16.389363 jianglab-0.3.4/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 11:41:16.389056 jianglab-0.3.4/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.4/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 11:41:16.386109 jianglab-0.3.4/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.4/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    17693 2023-06-03 11:39:58.000000 jianglab-0.3.4/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.4/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 11:41:16.388382 jianglab-0.3.4/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 11:41:16.000000 jianglab-0.3.4/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-03 11:41:16.000000 jianglab-0.3.4/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-03 11:41:16.000000 jianglab-0.3.4/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-03 11:41:16.000000 jianglab-0.3.4/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-03 11:41:16.000000 jianglab-0.3.4/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-03 11:41:16.389491 jianglab-0.3.4/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-03 11:41:11.000000 jianglab-0.3.4/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.181008 jianglab-0.3.5/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:23:23.180711 jianglab-0.3.5/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.5/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.178048 jianglab-0.3.5/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.5/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    18104 2023-06-03 12:23:04.000000 jianglab-0.3.5/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.5/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.180154 jianglab-0.3.5/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-03 12:23:23.181111 jianglab-0.3.5/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-03 12:23:09.000000 jianglab-0.3.5/setup.py
```

### Comparing `jianglab-0.3.4/PKG-INFO` & `jianglab-0.3.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.4/README.md` & `jianglab-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.4/jianglab/common_functions.py` & `jianglab-0.3.5/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,11 +382,16 @@
     clean_data = remove_bad_lanes(lowpass_data, bad_lanes)
     clean_centers = clean_centers_all_process(clean_data, 
                                               neighbour_size = neighbour_size)
 
     return clean_centers, clean_data
 
 
-    
+def get_ssvf_center_waveform(lp_data, centers, pre_center_margin = 100, post_center_margin = 800):
+    center_waveform = []
+    for center in centers:
+        if (center[0] > pre_center_margin) and (center[0] < (lp_data.shape[0]-post_center_margin)):
+            center_waveform.append(lp_data[(center[0]-pre_center_margin):(center[0]+post_center_margin), center[1], center[2]])
+    return np.array(center_waveform)
 
 def func3():
     pass
```

### Comparing `jianglab-0.3.4/jianglab.egg-info/PKG-INFO` & `jianglab-0.3.5/jianglab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.4/setup.py` & `jianglab-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.4',
+    version='0.3.5',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

