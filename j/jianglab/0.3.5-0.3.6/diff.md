# Comparing `tmp/jianglab-0.3.5.tar.gz` & `tmp/jianglab-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.5.tar", last modified: Sat Jun  3 12:23:23 2023, max compression
+gzip compressed data, was "jianglab-0.3.6.tar", last modified: Sat Jun  3 12:39:56 2023, max compression
```

## Comparing `jianglab-0.3.5.tar` & `jianglab-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.181008 jianglab-0.3.5/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:23:23.180711 jianglab-0.3.5/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.5/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.178048 jianglab-0.3.5/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.5/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    18104 2023-06-03 12:23:04.000000 jianglab-0.3.5/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.5/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:23:23.180154 jianglab-0.3.5/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-03 12:23:23.000000 jianglab-0.3.5/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-03 12:23:23.181111 jianglab-0.3.5/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-03 12:23:09.000000 jianglab-0.3.5/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:39:56.437513 jianglab-0.3.6/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:39:56.437217 jianglab-0.3.6/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.6/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:39:56.434611 jianglab-0.3.6/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.6/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    19149 2023-06-03 12:39:36.000000 jianglab-0.3.6/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.6/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-03 12:39:56.436731 jianglab-0.3.6/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-03 12:39:56.000000 jianglab-0.3.6/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-03 12:39:56.000000 jianglab-0.3.6/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-03 12:39:56.000000 jianglab-0.3.6/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-03 12:39:56.000000 jianglab-0.3.6/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-03 12:39:56.000000 jianglab-0.3.6/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-03 12:39:56.437642 jianglab-0.3.6/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-03 12:39:44.000000 jianglab-0.3.6/setup.py
```

### Comparing `jianglab-0.3.5/PKG-INFO` & `jianglab-0.3.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.5/README.md` & `jianglab-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.5/jianglab/common_functions.py` & `jianglab-0.3.6/jianglab/common_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -389,9 +389,30 @@
 def get_ssvf_center_waveform(lp_data, centers, pre_center_margin = 100, post_center_margin = 800):
     center_waveform = []
     for center in centers:
         if (center[0] > pre_center_margin) and (center[0] < (lp_data.shape[0]-post_center_margin)):
             center_waveform.append(lp_data[(center[0]-pre_center_margin):(center[0]+post_center_margin), center[1], center[2]])
     return np.array(center_waveform)
 
+def ssvf_full_analysis(file_list, 
+                       show_plot = True,
+                       save_data = True,
+                       kernel_size = 51, 
+                       pre_resample_rate = 100, 
+                       post_resample_rate = 10, 
+                       neighbour_size = (6,6,6)):
+    for filepath in file_list:
+        print(filepath)
+        centers, lp_data = clean_cmcr_data(filepath,
+                                           kernel_size = kernel_size,
+                                           pre_resample_rate = pre_resample_rate,
+                                           post_resample_rate = post_resample_rate,
+                                           neighbour_size = neighbour_size)
+        center_waveform = get_ssvf_center_waveform(lp_data, centers)
+        data_dict = {"centers":centers, "lp_data":lp_data, "center_waveform":center_waveform}
+        if save_data:
+            save_instance(filepath[:-5]+".pkl", data_dict)
+        if show_plot:
+            plt.plot(center_waveform.mean(axis=0))
+
 def func3():
     pass
```

### Comparing `jianglab-0.3.5/jianglab.egg-info/PKG-INFO` & `jianglab-0.3.6/jianglab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.5/setup.py` & `jianglab-0.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.5',
+    version='0.3.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

