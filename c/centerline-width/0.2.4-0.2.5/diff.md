# Comparing `tmp/centerline-width-0.2.4.tar.gz` & `tmp/centerline-width-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.2.4.tar", last modified: Sat Jun  3 01:11:41 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.2.5.tar", last modified: Sat Jun  3 01:23:41 2023, max compression
```

## Comparing `centerline-width-0.2.4.tar` & `centerline-width-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/
--rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:11:41.553426 centerline-width-0.2.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32073 2023-06-03 00:59:35.000000 centerline-width-0.2.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.4/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22474 2023-06-01 21:57:25.000000 centerline-width-0.2.4/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.4/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.4/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-01 21:30:40.000000 centerline-width-0.2.4/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.2.4/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.4/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.4/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.4/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.4/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.4/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     5221 2023-06-01 22:13:28.000000 centerline-width-0.2.4/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-03 01:11:41.553426 centerline-width-0.2.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-06-03 00:59:56.000000 centerline-width-0.2.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/
+-rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:23:41.188273 centerline-width-0.2.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32073 2023-06-03 00:59:35.000000 centerline-width-0.2.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.5/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22521 2023-06-03 01:17:56.000000 centerline-width-0.2.5/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.5/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.5/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-01 21:30:40.000000 centerline-width-0.2.5/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.2.5/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.5/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.5/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.5/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.5/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.5/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5221 2023-06-01 22:13:28.000000 centerline-width-0.2.5/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-03 01:23:41.188273 centerline-width-0.2.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-06-03 01:22:11.000000 centerline-width-0.2.5/setup.py
```

### Comparing `centerline-width-0.2.4/PKG-INFO` & `centerline-width-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.4.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.5.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
```

### Comparing `centerline-width-0.2.4/README.md` & `centerline-width-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/__init__.py` & `centerline-width-0.2.5/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/centerline.py` & `centerline-width-0.2.5/centerline_width/centerline.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,16 @@
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
 	# recreate the centerline with evenly spaced points
 	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineVoronoi,
 																			number_of_fixed_points=river_object.interpolate_n_centerpoints)
 	if apply_smoothing:
-		defined_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineVoronoi,
+		defined_centerline_coordinates = centerline_width.smoothedCoordinates(river_object=river_object,
+																				centerline_coordinates=river_object.centerlineVoronoi,
 																				interprolate_num=river_object.interpolate_n_centerpoints)
 	# if using smoothing, replace left/right coordinates with the smoothed variation
 	right_width_coord, left_width_coord, _ = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																								centerline_coordinates=defined_centerline_coordinates,
 																								transect_span_distance=transect_span_distance,
 																								remove_intersections=remove_intersections)
```

### Comparing `centerline-width-0.2.4/centerline_width/error_handling.py` & `centerline-width-0.2.5/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/getCoordinatesKML.py` & `centerline-width-0.2.5/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/plotDiagrams.py` & `centerline-width-0.2.5/centerline_width/plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/preprocessing.py` & `centerline-width-0.2.5/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/pytests/test_centerline.py` & `centerline-width-0.2.5/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.2.5/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.2.5/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.2.5/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.2.5/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width/riverCenterlineClass.py` & `centerline-width-0.2.5/centerline_width/riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.2.5/centerline_width.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.4.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.5.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
```

### Comparing `centerline-width-0.2.4/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.2.5/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.4/setup.py` & `centerline-width-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.2.4"
+VERSION="0.2.5"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

