# Comparing `tmp/dpivsoft-0.2.5.tar.gz` & `tmp/dpivsoft-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpivsoft-0.2.5.tar", last modified: Sat Jan 14 17:06:09 2023, max compression
+gzip compressed data, was "dpivsoft-0.2.6.tar", last modified: Sat Jun  3 13:41:54 2023, max compression
```

## Comparing `dpivsoft-0.2.5.tar` & `dpivsoft-0.2.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.504064 dpivsoft-0.2.5/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    35150 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/LICENSE.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       79 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/MANIFEST.in
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     3196 2023-01-14 17:06:09.504064 dpivsoft-0.2.5/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2577 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/README.md
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.496064 dpivsoft-0.2.5/dpivsoft/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    27256 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/Cl_DPIV.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11533 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/Classes.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    40654 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/DPIV.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.496064 dpivsoft-0.2.5/dpivsoft/Examples/
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.496064 dpivsoft-0.2.5/dpivsoft/Examples/CFD/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)  2160128 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/Examples/CFD/Mixing_Flow.npy
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5235 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/Examples/Performance.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/Examples/Performance_parameters.yaml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5292 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/Examples/Tutorial_1.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/Examples/Tutorial_1_parameters.yaml
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.504064 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-10-24 10:54:01.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.Jacobian.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-06 11:16:20.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.deform_image.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:46:07.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:05:39.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 10:54:56.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2022-11-26 15:22:43.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swn
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2021-10-15 18:39:27.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swo
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    20480 2021-10-14 10:16:50.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-10 16:30:18.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1004 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Jacobian.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      497 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Normalize_Img.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      573 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Slice.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      686 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/SubMean.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      689 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Weighting.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      496 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/box_blur.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2567 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/deform_image.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2090 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/directCorrelation.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6179 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/find_peak.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4341 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/find_peak_direct.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      976 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/gaussian_filter.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      271 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/ini_index.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      707 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/interpolation.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4001 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/median_filter.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      214 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/GPU_Kernels/multiply_them.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    12471 2023-01-14 17:00:20.000000 dpivsoft-0.2.5/dpivsoft/SyIm.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        0 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8617 2022-12-03 15:03:54.000000 dpivsoft-0.2.5/dpivsoft/meshTools.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-01-14 17:06:09.496064 dpivsoft-0.2.5/dpivsoft.egg-info/
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)     3196 2023-01-14 17:06:09.000000 dpivsoft-0.2.5/dpivsoft.egg-info/PKG-INFO
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)     1437 2023-01-14 17:06:09.000000 dpivsoft-0.2.5/dpivsoft.egg-info/SOURCES.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)        1 2023-01-14 17:06:09.000000 dpivsoft-0.2.5/dpivsoft.egg-info/dependency_links.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)      151 2023-01-14 17:06:09.000000 dpivsoft-0.2.5/dpivsoft.egg-info/requires.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)        9 2023-01-14 17:06:09.000000 dpivsoft-0.2.5/dpivsoft.egg-info/top_level.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2023-01-14 17:06:09.504064 dpivsoft-0.2.5/setup.cfg
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1268 2023-01-14 17:03:29.000000 dpivsoft-0.2.5/setup.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    35150 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/LICENSE.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       79 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/MANIFEST.in
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     3247 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2577 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/README.md
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    27256 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Cl_DPIV.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    11533 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Classes.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    40654 2023-06-03 13:34:49.000000 dpivsoft-0.2.6/dpivsoft/DPIV.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/Examples/
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/Examples/CFD/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)  2160128 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/CFD/Mixing_Flow.npy
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5235 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/Performance.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Examples/Performance_parameters.yaml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5292 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1_parameters.yaml
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-10-24 10:54:01.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.Jacobian.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-06 11:16:20.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.deform_image.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:46:07.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:05:39.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 10:54:56.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2022-11-26 15:22:43.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swn
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2021-10-15 18:39:27.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swo
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    20480 2021-10-14 10:16:50.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-10 16:30:18.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1004 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Jacobian.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      497 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Normalize_Img.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      573 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Slice.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      686 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/SubMean.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      689 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Weighting.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      496 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/box_blur.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2567 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/deform_image.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2090 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/directCorrelation.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6179 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4341 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak_direct.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      976 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/gaussian_filter.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      271 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/ini_index.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      707 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/interpolation.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4001 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/median_filter.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      214 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/multiply_them.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    12471 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/SyIm.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        0 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8617 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/meshTools.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft.egg-info/
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)     3247 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/PKG-INFO
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)     1437 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)        1 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)      159 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/requires.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)        9 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/top_level.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/setup.cfg
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1326 2023-06-03 13:34:49.000000 dpivsoft-0.2.6/setup.py
```

### Comparing `dpivsoft-0.2.5/LICENSE.txt` & `dpivsoft-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/PKG-INFO` & `dpivsoft-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dpivsoft
-Version: 0.2.5
+Version: 0.2.6
 Summary: UNKNOWN
 Home-page: https://gitlab.com/jacabello/dpivsoft_python
 Author: Jorge Aguilar-Cabello
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `dpivsoft-0.2.5/README.md` & `dpivsoft-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/Cl_DPIV.py` & `dpivsoft-0.2.6/dpivsoft/Cl_DPIV.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/Classes.py` & `dpivsoft-0.2.6/dpivsoft/Classes.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/DPIV.py` & `dpivsoft-0.2.6/dpivsoft/DPIV.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             u_1, v_1 = check_mask(u_1, v_1, grid.mask_1)
 
         # Calculates the jacobian matrix onto de grid
         du_dx, du_dy, dv_dx, dv_dy = jacobian_matrix(u_1, v_1, x_1, y_1,
                 no_boxes_1_x, no_boxes_1_y)
 
         for j in range(0,no_boxes_1_y):
-            for i in range(0,no_boxes_1_y):
+            for i in range(0,no_boxes_1_x):
 
                 # Obtain deformed image.
                 SubImg1, SubImg2, u_index, v_index = deform_image(Img1, Img2,
                         Width, Height, box_origin_x, box_origin_y, i_matrix,
                         j_matrix, box_size_x, box_size_y, u_1, v_1, du_dx,
                         du_dy, dv_dx, dv_dy, i, j)
```

### Comparing `dpivsoft-0.2.5/dpivsoft/Examples/CFD/Mixing_Flow.npy` & `dpivsoft-0.2.6/dpivsoft/Examples/CFD/Mixing_Flow.npy`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/Examples/Performance.py` & `dpivsoft-0.2.6/dpivsoft/Examples/Performance.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/Examples/Tutorial_1.py` & `dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.Jacobian.cl.swp` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.Jacobian.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.deform_image.cl.swp` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.deform_image.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swn` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swn`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swo` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swo`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.find_peak.cl.swp` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Jacobian.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Jacobian.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Slice.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Slice.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/SubMean.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/SubMean.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/Weighting.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Weighting.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/deform_image.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/deform_image.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/directCorrelation.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/directCorrelation.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/find_peak.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/find_peak_direct.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak_direct.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/gaussian_filter.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/gaussian_filter.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/interpolation.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/interpolation.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/GPU_Kernels/median_filter.cl` & `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/median_filter.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/SyIm.py` & `dpivsoft-0.2.6/dpivsoft/SyIm.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft/meshTools.py` & `dpivsoft-0.2.6/dpivsoft/meshTools.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/dpivsoft.egg-info/PKG-INFO` & `dpivsoft-0.2.6/dpivsoft.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dpivsoft
-Version: 0.2.5
+Version: 0.2.6
 Summary: UNKNOWN
 Home-page: https://gitlab.com/jacabello/dpivsoft_python
 Author: Jorge Aguilar-Cabello
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `dpivsoft-0.2.5/dpivsoft.egg-info/SOURCES.txt` & `dpivsoft-0.2.6/dpivsoft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.5/setup.py` & `dpivsoft-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "dpivsoft",
-    version="0.2.5",
+    version="0.2.6",
     url="https://gitlab.com/jacabello/dpivsoft_python",
     author = "Jorge Aguilar-Cabello",
     python_requires=">=3.7",
     packages = find_packages(),
     include_package_data = True,
     long_description = long_description,
     long_description_content_type = "text/markdown",
     setup_requires=[
         'setuptools',
     ],
     install_requires = [
-        'numpy>=1.2',
+        'numpy>=1.3,<1.24.0',
         'reikna>=0.7.6',
         'scipy>=1.5',
         'opencv-python>=4.5',
         'matplotlib>=3',
         'PyYAML>=5.4',
         'pyopencl>=2021',
         'Shapely>=1.7',
@@ -33,14 +33,15 @@
         ],
     },
     classifiers=[
          # Sublist of all supported Python versions.
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
 
         #Miscelaneous metadata
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
     ],
 )
```

