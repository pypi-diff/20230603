# Comparing `tmp/centerline-width-0.2.3.tar.gz` & `tmp/centerline-width-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.2.3.tar", last modified: Fri May 26 07:16:36 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.2.4.tar", last modified: Sat Jun  3 01:11:41 2023, max compression
```

## Comparing `centerline-width-0.2.3.tar` & `centerline-width-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.414115 centerline-width-0.2.3/
--rw-rw-r--   0 user      (1000) user      (1000)    33829 2023-05-26 07:16:36.410114 centerline-width-0.2.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    28771 2023-05-26 07:15:14.000000 centerline-width-0.2.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.3/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    21536 2023-05-26 06:59:06.000000 centerline-width-0.2.3/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.3/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.3/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     7421 2023-05-26 06:06:57.000000 centerline-width-0.2.3/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6750 2023-05-24 20:32:04.000000 centerline-width-0.2.3/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.3/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.3/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.3/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.3/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.3/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     5202 2023-05-26 07:01:19.000000 centerline-width-0.2.3/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33829 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-26 07:16:36.414115 centerline-width-0.2.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-26 07:15:41.000000 centerline-width-0.2.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/
+-rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:11:41.553426 centerline-width-0.2.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32073 2023-06-03 00:59:35.000000 centerline-width-0.2.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.4/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22474 2023-06-01 21:57:25.000000 centerline-width-0.2.4/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.4/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.4/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-01 21:30:40.000000 centerline-width-0.2.4/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.2.4/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.4/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.4/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.4/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.4/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.4/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5221 2023-06-01 22:13:28.000000 centerline-width-0.2.4/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:11:41.553426 centerline-width-0.2.4/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-03 01:11:41.000000 centerline-width-0.2.4/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-03 01:11:41.553426 centerline-width-0.2.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-06-03 00:59:56.000000 centerline-width-0.2.4/setup.py
```

### Comparing `centerline-width-0.2.3/PKG-INFO` & `centerline-width-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,500 +1,507 @@
-Metadata-Version: 2.1
-Name: centerline-width
-Version: 0.2.3
-Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
-Home-page: https://github.com/cyschneck/centerline-width
-Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
-License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.3.tar.gz
-Description: # Centerline-Width
-        ![PyPi](https://img.shields.io/pypi/v/centerline-width)
-        ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
-        [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
-        [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
-        
-        Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
-        
-        * **Convert raw data from Google Earth Pro to CSV**
-        	* extractPointsToTextFile()
-        	* convertColumnsToCSV()
-        * **Find centerline and width of river**
-        	* plotCenterline()
-        	* plotCenterlineWidth()
-        	* riverWidthFromCenterline()
-        	* saveCenterlineCSV()
-        	* centerlineVoronoi
-        	* centerlineEvenlySpaced
-        	* centerlineSmoothed
-        	* centerlineLength
-        	* rightBankLength
-        	* leftBankLength
-        
-        | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
-        | ------------- | ------------- |
-        | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
-        
-        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
-        
-        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
-        
-        ## Requirements
-        Currently running on Python 3.7+
-        
-        ```
-        pip install -r requirements.txt
-        ```
-        Requirements will also be downloaded as part of the pip download
-        
-        ## Install
-        PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
-        
-        ```
-        pip install centerline-width
-        ```
-        ## Quickstart: centerline-width
-        
-        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
-        
-        ```python
-        import centerline_width
-        centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
-        					right_kml="right_bank.kml",
-        					text_output_name="river_coordinates_output.txt")
-        centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
-        ```
-        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
-        
-        ```python
-        river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
-        ```
-        
-        To plot the centerline, run the `plotCenterline()` function from `river_object` created
-        ```python
-        river_object.plotCenterline()
-        ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
-        
-        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
-        
-        While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
-        ```python
-        river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-        ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
-        
-        ## Preprocessing
-        ### Convert KML files to Text File
-        
-        Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
-        
-        ```
-        extractPointsToTextFile(left_kml=None,
-        			right_kml=None,
-        			text_output_name=None)
-        ```
-        
-        * **[REQUIRED]** left_kml (string): File location of the kml file for left bank
-        * **[REQUIRED]** right_kml (string): File location of the kml file for right bank
-        * **[REQUIRED]** text_output_name (string): Output file name (and location)
-        
-        ```python
-        import centerline_width
-        centerline_width.extractPointsToTextFile(left_kml="leftbank.kml",
-        					right_kml="rightbank.kml",
-        					text_output_name="data/river_coords_output.txt")
-        ```
-        Output: The text file `data/river_coords_output.txt` with the headers `llat, llon, rlat, rlon` (for the left latitude, left longitude, right latitude, and right longitude)
-        
-        Example:
-        ```
-             llat       llon      rlat       rlon
-        30.037581 -92.868569 30.119804 -92.907933
-        30.037613 -92.868549 30.119772 -92.907924
-        30.037648 -92.868546 30.119746 -92.907917
-        30.037674 -92.868536 30.119721 -92.907909
-        30.037702 -92.868533 30.119706 -92.907905
-        ```
-        
-        ### Converted Text File to CSV
-        
-        Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
-        
-        ```
-        convertColumnsToCSV(text_file=None, flipBankDirection=False)
-        ```
-        * **[REQUIRED]** text_file (string): File location of the text file to convert
-        * [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
-        
-        Scripts expects data as a list of point for left and right banks:
-        - Header: llat, llon, rlat, rlon
-        
-        ```python
-        import centerline_width
-        centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
-        				flipBankDirection=True)
-        ```
-        Converts text file:
-        ```
-             llat       llon      rlat       rlon
-        30.037581 -92.868569 30.037441 -92.867476
-        30.037613 -92.868549 30.037448 -92.867474
-        30.037648 -92.868546 30.037482 -92.867449
-        30.037674 -92.868536 30.037506 -92.867432
-        30.037702 -92.868533 30.037525 -92.867430
-        ```
-        To a CSV file:
-        ```
-        llat,llon,rlat,rlon
-        30.037581,-92.868569,30.037441,-92.867476
-        30.037613,-92.868549,30.037448,-92.867474
-        30.037648,-92.868546,30.037482,-92.867449
-        30.037674,-92.868536,30.037506,-92.867432
-        30.037702,-92.868533,30.037525,-92.867430
-        ```
-        Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
-        
-        ## Centerline and Width
-        ### River Object
-        First, generate a river object to contain river data and available transformations
-        ```
-        centerline_width.riverCenterline(csv_data=None,
-        				optional_cutoff=None,
-        				interpolate_data=False,
-        				interpolate_n=5)
-        ```
-        * **[REQUIRED]** csv_data (string): File location of the text file to convert
-        * [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
-        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
-        * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
-        
-        Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
-        
-        Object (class) useful attributes:
-        
-        * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
-        * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
-        * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
-        * centerlineLength (float): Length of the centerline of the river (in km)
-        * rightBankLength (float): Length of the right bank of the river (in km)
-        * leftBankLength (float): Length of the left bank of the river (in km)
-        
-        Object (class) additional atttributes:
-        
-        * river_name (string): name of object, set to the csv_data string
-        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
-        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
-        * df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
-        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
-        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
-        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
-        * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
-        * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
-        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
-        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
-        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-        * interpolate_data (bool): if interpolating between existing data, defaults to False
-        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
-        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
-        
-        
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        ```
-        
-        ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longitude coordinates of the centerline based on the left and right banks
-        
-        **Types of Centerlines**
-        There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
-        - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
-        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
-        - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
-        
-        Centerline coordinates are formed by the Voronoi vertices
-        ```
-        river_object.centerlineVoronoi
-        ```
-        
-        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
-        ```
-        river_object.centerlineEvenlySpaced
-        ```
-        
-        Centerline coordinates are formed from Smoothed Voronoi vertices
-        ```
-        river_object.centerlineSmoothed
-        ```
-        
-        Example:
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
-        river_centerline_coordinates = river_object.centerlineVoronoi
-        ```
-        Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
-        
-        ### Save Centerline Coordinates to a CSV
-        Save the centerline coordinates to a csv file with columns for latitude and longitude
-        
-        ```
-        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
-        ```
-        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
-        
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
-        ```
-        
-        Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
-        
-        ### Return Length of Centerline
-        Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
-        ```
-        river_object.centerlineLength
-        ```
-        Length returned in kilometers
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
-        river_centerline_length = river_object.centerlineLength
-        ```
-        The length of the river centerline returns `215.34700589636674` km
-        
-        ## Plot Centerline in Matplotlib
-        Plot the centerline created from a list of right and left banks with Voronoi vertices
-        
-        ```
-        plotCenterline(display_all_possible_paths=False, 
-        		plot_title=None, 
-        		save_plot_name=None, 
-        		display_voronoi=False)
-        ```
-        * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging)
-        * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
-        * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
-        * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline
-        
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
-        ```
-        Output:
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
-        
-        ## Plot Centerline Width Lines in Matplotlib
-        ### Plot the Centerline Width Lines
-        Plot the width of the river based on the centerline
-        
-        Display Centerline at even intervals from the Voronoi generated centerline
-        ```
-        plotCenterlineWidth(plot_title=None, 
-        		save_plot_name=None, 
-        		display_true_centerline=True,
-        		transect_span_distance=3,
-        		apply_smoothing=False,
-        		flag_intersections=True,
-        		remove_intersections=False)
-        ```
-        * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
-        * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
-        * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-        * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
-        
-        **apply_smoothing**
-        
-        apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
-        
-        | apply_smoothing=False | apply_smoothing=True |
-        | ------------- | ------------- |
-        | ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
-        
-        **transect_span_distance**
-        
-        Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
-        
-        ![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
-        | transect_span_distance=6 | transect_span_distance=30 |
-        | ------------- | ------------- |
-        | ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
-        
-        **remove_intersections**
-        
-        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
-        
-        Intersecting lines are flagged in red by default (flag_intersections=True)
-        
-        | remove_intersections=False | remove_intersections=True |
-        | ------------- | ------------- |
-        | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
-        
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-        ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
-        
-        ### Return Width of River
-        
-        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
-        
-        ```
-        riverWidthFromCenterline(transect_span_distance=3,
-        			apply_smoothing=True,
-        			remove_intersections=False,
-        			units="km",
-        			save_to_csv=None)
-        ```
-        * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
-        * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
-        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
-        
-        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
-        
-        ```python
-        import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
-        							apply_smoothing=True,
-        							units="km",
-        							remove_intersections=True)
-        ```
-        Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
-        
-        ## Documentation and Algorithm to Determine Centerline
-        
-        The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
-        
-        ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example1.png)
-        
-        ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example2.png)
-        
-        ### Generate a Voronoi based on the points along the river banks
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
-        
-        ### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
-        
-        ### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
-        With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
-        
-        ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
-        | Points on River Bank | NetworkX Graph of Points on River Bank |
-        | ------------- | ------------- |
-        | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
-        
-        ### Display the centerline found by connecting the starting/ending node with the shortest path
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example8.png)
-        
-        This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed and no gaps exist in the centerline
-        
-        Points that only have one connection are removed, but by limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
-        
-        **All vertices:**
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
-        
-        **Vertices that have at least two connections (that would create gaps):**
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
-        
-        ## Debugging, Error Handling, and Edge Cases
-        ### Wide Start/End of River
-        If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
-        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
-        
-        ### Invalid Polygon
-        A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
-        
-        A polygon is invalid if it overlaps within itself:
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
-        In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
-        
-        With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
-        
-        ### Invalid Centerline
-        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
-        
-        `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
-        Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
-        
-        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
-        Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
-        
-        If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
-        
-        If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
-        
-        This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
-        
-        ### Fix Gaps and Jagged Centerlines
-        Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
-        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
-        Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
-        ```python
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
-        ```
-        | interpolate_data = False | interpolate_data = True |
-        | ------------- | ------------- |
-        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
-        
-        The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
-        
-        ## Developer Notes: Tech Debt and Bug Fixes
-        * Fix legend overlapping on graph, replace doc_examples that have an overlapping
-        * Verify that smoothing filter option does not produce a line that goes outside of the polygon
-        
-        ## Citations
-        Based on work written in R (Golly et al. 2017):
-        
-        >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
-        
-        [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
-        
-         <p align="center">
-          <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
-          <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
-          <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
-        </p>
-        
-        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
-        
-        ## Bug and Feature Request
-        
-        Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
-        
-Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+# Centerline-Width
+ <p align="center">
+  <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
+</p>
+
+![PyPi](https://img.shields.io/pypi/v/centerline-width)
+![license](https://img.shields.io/github/license/cyschneck/centerline-width)
+[![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+[![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
+
+Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
+
+* **Convert raw data from Google Earth Pro to CSV**
+	* extractPointsToTextFile()
+	* convertColumnsToCSV()
+* **Find centerline and width of river**
+	* plotCenterline()
+	* plotCenterlineWidth()
+	* riverWidthFromCenterline()
+	* saveCenterlineCSV()
+	* centerlineVoronoi
+	* centerlineEvenlySpaced
+	* centerlineSmoothed
+	* centerlineLength
+	* rightBankLength
+	* leftBankLength
+
+| River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
+| ------------- | ------------- |
+| ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
+
+Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
+
+NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
+
+## Install
+PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
+
+```
+pip install centerline-width
+```
+
+## Requirements
+Currently running on Python 3.7+
+
+```
+pip install -r requirements.txt
+```
+Requirements will also be downloaded as part of the pip download
+
+## Quickstart: centerline-width
+
+The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+
+```python
+import centerline_width
+centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
+					right_kml="right_bank.kml",
+					text_output_name="river_coordinates_output.txt")
+centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
+```
+Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+
+```python
+river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
+```
+
+To plot the centerline, run the `plotCenterline()` function from `river_object` created
+```python
+river_object.plotCenterline()
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
+
+To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
+
+While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
+```python
+river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+
+## Preprocessing
+### Convert KML files to Text File
+
+Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
+
+```
+extractPointsToTextFile(left_kml=None,
+			right_kml=None,
+			text_output_name=None)
+```
+
+* **[REQUIRED]** left_kml (string): File location of the kml file for left bank
+* **[REQUIRED]** right_kml (string): File location of the kml file for right bank
+* **[REQUIRED]** text_output_name (string): Output file name (and location)
+
+```python
+import centerline_width
+centerline_width.extractPointsToTextFile(left_kml="leftbank.kml",
+					right_kml="rightbank.kml",
+					text_output_name="data/river_coords_output.txt")
+```
+Output: The text file `data/river_coords_output.txt` with the headers `llat, llon, rlat, rlon` (for the left latitude, left longitude, right latitude, and right longitude)
+
+Example:
+```
+     llat       llon      rlat       rlon
+30.037581 -92.868569 30.119804 -92.907933
+30.037613 -92.868549 30.119772 -92.907924
+30.037648 -92.868546 30.119746 -92.907917
+30.037674 -92.868536 30.119721 -92.907909
+30.037702 -92.868533 30.119706 -92.907905
+```
+
+### Converted Text File to CSV
+
+Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
+
+```
+convertColumnsToCSV(text_file=None, flipBankDirection=False)
+```
+* **[REQUIRED]** text_file (string): File location of the text file to convert
+* [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+
+Scripts expects data as a list of point for left and right banks:
+- Header: llat, llon, rlat, rlon
+
+```python
+import centerline_width
+centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
+				flipBankDirection=True)
+```
+Converts text file:
+```
+     llat       llon      rlat       rlon
+30.037581 -92.868569 30.037441 -92.867476
+30.037613 -92.868549 30.037448 -92.867474
+30.037648 -92.868546 30.037482 -92.867449
+30.037674 -92.868536 30.037506 -92.867432
+30.037702 -92.868533 30.037525 -92.867430
+```
+To a CSV file:
+```
+llat,llon,rlat,rlon
+30.037581,-92.868569,30.037441,-92.867476
+30.037613,-92.868549,30.037448,-92.867474
+30.037648,-92.868546,30.037482,-92.867449
+30.037674,-92.868536,30.037506,-92.867432
+30.037702,-92.868533,30.037525,-92.867430
+```
+Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
+
+## Centerline and Width
+### River Object
+First, generate a river object to contain river data and available transformations
+```
+centerline_width.riverCenterline(csv_data=None,
+				optional_cutoff=None,
+				interpolate_data=False,
+				interpolate_n=5,
+				interpolate_n_centerpoints=None)
+```
+* **[REQUIRED]** csv_data (string): File location of the text file to convert
+* [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
+* [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+* [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+* [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
+
+**Solutions for sparse data:**
+
+`interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+
+`interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
+
+| interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
+
+**Object (class) useful attributes:**
+
+* centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+* centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+* centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
+* centerlineLength (float): Length of the centerline of the river (in km)
+* rightBankLength (float): Length of the right bank of the river (in km)
+* leftBankLength (float): Length of the left bank of the river (in km)
+
+**Object (class) additional atttributes:**
+
+* river_name (string): name of object, set to the csv_data string
+* left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+* right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+* df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
+* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+* top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
+* bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+* starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+* ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
+* bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+* x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
+* y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+* interpolate_data (bool): if interpolating between existing data, defaults to False
+* interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+* interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
+
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+```
+
+### Return Latitude/Longitude Coordinates of Centerline
+Return the latitude/longitude coordinates of the centerline based on the left and right banks
+
+**Types of Centerlines**
+
+There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+
+- **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
+- **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
+- **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
+
+Centerline coordinates are formed by the Voronoi vertices
+```
+river_object.centerlineVoronoi
+```
+
+Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+```
+river_object.centerlineEvenlySpaced
+```
+
+Centerline coordinates are formed from Smoothed Voronoi vertices
+```
+river_object.centerlineSmoothed
+```
+
+Example:
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
+river_centerline_coordinates = river_object.centerlineVoronoi
+```
+Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
+
+### Save Centerline Coordinates to a CSV
+Save the centerline coordinates to a csv file with columns for latitude and longitude
+
+```
+saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+```
+* **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
+* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
+```
+
+Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
+
+### Return Length of Centerline
+Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
+```
+river_object.centerlineLength
+```
+Length returned in kilometers
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
+river_centerline_length = river_object.centerlineLength
+```
+The length of the river centerline returns `215.34700589636674` km
+
+## Plot Centerline in Matplotlib
+Plot the centerline created from a list of right and left banks with Voronoi vertices
+
+```
+plotCenterline(display_all_possible_paths=False, 
+		plot_title=None, 
+		save_plot_name=None, 
+		display_voronoi=False)
+```
+* [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
+* [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.plotCenterline()
+```
+Output:
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
+
+## Plot Centerline Width Lines in Matplotlib
+### Plot the Centerline Width Lines
+Plot the width of the river based on the centerline
+
+Display Centerline at even intervals from the Voronoi generated centerline
+```
+plotCenterlineWidth(plot_title=None, 
+		save_plot_name=None, 
+		display_true_centerline=True,
+		transect_span_distance=3,
+		apply_smoothing=False,
+		flag_intersections=True,
+		remove_intersections=False)
+```
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
+* [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
+* [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
+* [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
+* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
+
+**apply_smoothing**
+
+apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
+
+| apply_smoothing=False | apply_smoothing=True |
+| ------------- | ------------- |
+| ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
+
+**transect_span_distance**
+
+Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
+
+![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
+| transect_span_distance=6 | transect_span_distance=30 |
+| ------------- | ------------- |
+| ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
+
+**remove_intersections**
+
+remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
+
+Intersecting lines are flagged in red by default (flag_intersections=True)
+
+| remove_intersections=False | remove_intersections=True |
+| ------------- | ------------- |
+| ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+
+### Return Width of River
+
+Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
+
+```
+riverWidthFromCenterline(transect_span_distance=3,
+			apply_smoothing=True,
+			remove_intersections=False,
+			units="km",
+			save_to_csv=None)
+```
+* [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
+* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+* [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
+* [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+
+Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
+							apply_smoothing=True,
+							units="km",
+							remove_intersections=True)
+```
+Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
+
+## Documentation and Algorithm to Determine Centerline
+
+The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
+
+### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
+
+### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
+
+### Generate a Voronoi based on the points along the riverbanks
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
+
+### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+
+### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
+
+### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
+| Points on River Bank | NetworkX Graph of Points on River Bank |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
+
+### Display the centerline found by connecting the starting/ending node with the shortest path
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
+
+This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
+
+Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
+
+**All vertices:**
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+
+**Vertices that have at least two connections (that would create gaps):**
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
+
+## Debugging, Error Handling, and Edge Cases
+### Wide Start/End of River
+If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
+Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
+
+### Invalid Polygon
+A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
+
+A polygon is invalid if it overlaps within itself:
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
+In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
+
+With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
+
+### Invalid Centerline
+If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
+
+`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
+Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
+
+### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+
+If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+
+If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+
+This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+
+### Invalid Smoothed Centerline
+The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+
+Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
+
+By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
+
+`interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
+
+| interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
+
+
+### Fix Gaps and Jagged Centerlines
+Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
+Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
+```python
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
+```
+| interpolate_data = False | interpolate_data = True |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
+
+The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
+
+## Developer Notes: Tech Debt and Bug Fixes
+* Fix legend overlapping on graph, replace doc_examples that have an overlapping
+* Verify that smoothing filter option does not produce a line that goes outside of the polygon
+
+## Citations
+Based on work written in R (Golly et al. 2017):
+
+>Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
+
+[Github - CMGO](https://github.com/AntoniusGolly/cmgo)
+
+ <p align="center">
+  <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
+  <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
+  <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
+</p>
+
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
+
+## Bug and Feature Request
+
+Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-0.2.3/README.md` & `centerline-width-0.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,475 +1,532 @@
-# Centerline-Width
-![PyPi](https://img.shields.io/pypi/v/centerline-width)
-![license](https://img.shields.io/github/license/cyschneck/centerline-width)
-[![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
-[![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
-
-Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
-
-* **Convert raw data from Google Earth Pro to CSV**
-	* extractPointsToTextFile()
-	* convertColumnsToCSV()
-* **Find centerline and width of river**
-	* plotCenterline()
-	* plotCenterlineWidth()
-	* riverWidthFromCenterline()
-	* saveCenterlineCSV()
-	* centerlineVoronoi
-	* centerlineEvenlySpaced
-	* centerlineSmoothed
-	* centerlineLength
-	* rightBankLength
-	* leftBankLength
-
-| River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
-| ------------- | ------------- |
-| ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
-
-Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
-
-NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
-
-## Requirements
-Currently running on Python 3.7+
-
-```
-pip install -r requirements.txt
-```
-Requirements will also be downloaded as part of the pip download
-
-## Install
-PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
-
-```
-pip install centerline-width
-```
-## Quickstart: centerline-width
-
-The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
-
-```python
-import centerline_width
-centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
-					right_kml="right_bank.kml",
-					text_output_name="river_coordinates_output.txt")
-centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
-```
-Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
-
-```python
-river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
-```
-
-To plot the centerline, run the `plotCenterline()` function from `river_object` created
-```python
-river_object.plotCenterline()
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
-
-To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
-
-While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
-```python
-river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
-
-## Preprocessing
-### Convert KML files to Text File
-
-Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
-
-```
-extractPointsToTextFile(left_kml=None,
-			right_kml=None,
-			text_output_name=None)
-```
-
-* **[REQUIRED]** left_kml (string): File location of the kml file for left bank
-* **[REQUIRED]** right_kml (string): File location of the kml file for right bank
-* **[REQUIRED]** text_output_name (string): Output file name (and location)
-
-```python
-import centerline_width
-centerline_width.extractPointsToTextFile(left_kml="leftbank.kml",
-					right_kml="rightbank.kml",
-					text_output_name="data/river_coords_output.txt")
-```
-Output: The text file `data/river_coords_output.txt` with the headers `llat, llon, rlat, rlon` (for the left latitude, left longitude, right latitude, and right longitude)
-
-Example:
-```
-     llat       llon      rlat       rlon
-30.037581 -92.868569 30.119804 -92.907933
-30.037613 -92.868549 30.119772 -92.907924
-30.037648 -92.868546 30.119746 -92.907917
-30.037674 -92.868536 30.119721 -92.907909
-30.037702 -92.868533 30.119706 -92.907905
-```
-
-### Converted Text File to CSV
-
-Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
-
-```
-convertColumnsToCSV(text_file=None, flipBankDirection=False)
-```
-* **[REQUIRED]** text_file (string): File location of the text file to convert
-* [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
-
-Scripts expects data as a list of point for left and right banks:
-- Header: llat, llon, rlat, rlon
-
-```python
-import centerline_width
-centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
-				flipBankDirection=True)
-```
-Converts text file:
-```
-     llat       llon      rlat       rlon
-30.037581 -92.868569 30.037441 -92.867476
-30.037613 -92.868549 30.037448 -92.867474
-30.037648 -92.868546 30.037482 -92.867449
-30.037674 -92.868536 30.037506 -92.867432
-30.037702 -92.868533 30.037525 -92.867430
-```
-To a CSV file:
-```
-llat,llon,rlat,rlon
-30.037581,-92.868569,30.037441,-92.867476
-30.037613,-92.868549,30.037448,-92.867474
-30.037648,-92.868546,30.037482,-92.867449
-30.037674,-92.868536,30.037506,-92.867432
-30.037702,-92.868533,30.037525,-92.867430
-```
-Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
-
-## Centerline and Width
-### River Object
-First, generate a river object to contain river data and available transformations
-```
-centerline_width.riverCenterline(csv_data=None,
-				optional_cutoff=None,
-				interpolate_data=False,
-				interpolate_n=5)
-```
-* **[REQUIRED]** csv_data (string): File location of the text file to convert
-* [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
-* [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
-* [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
-
-Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
-
-Object (class) useful attributes:
-
-* centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
-* centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
-* centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
-* centerlineLength (float): Length of the centerline of the river (in km)
-* rightBankLength (float): Length of the right bank of the river (in km)
-* leftBankLength (float): Length of the left bank of the river (in km)
-
-Object (class) additional atttributes:
-
-* river_name (string): name of object, set to the csv_data string
-* left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
-* right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
-* df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
-* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
-* top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
-* bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
-* starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
-* ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
-* bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
-* x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
-* y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-* interpolate_data (bool): if interpolating between existing data, defaults to False
-* interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
-* interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
-
-
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-```
-
-### Return Latitude/Longitude Coordinates of Centerline
-Return the latitude/longitude coordinates of the centerline based on the left and right banks
-
-**Types of Centerlines**
-There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
-- **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
-- **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
-- **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
-
-Centerline coordinates are formed by the Voronoi vertices
-```
-river_object.centerlineVoronoi
-```
-
-Centerline coordinates are formed by Evenly Spaced Voronoi vertices
-```
-river_object.centerlineEvenlySpaced
-```
-
-Centerline coordinates are formed from Smoothed Voronoi vertices
-```
-river_object.centerlineSmoothed
-```
-
-Example:
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
-river_centerline_coordinates = river_object.centerlineVoronoi
-```
-Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
-
-### Save Centerline Coordinates to a CSV
-Save the centerline coordinates to a csv file with columns for latitude and longitude
-
-```
-saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
-```
-* **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
-
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
-```
-
-Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
-
-### Return Length of Centerline
-Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
-```
-river_object.centerlineLength
-```
-Length returned in kilometers
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
-river_centerline_length = river_object.centerlineLength
-```
-The length of the river centerline returns `215.34700589636674` km
-
-## Plot Centerline in Matplotlib
-Plot the centerline created from a list of right and left banks with Voronoi vertices
-
-```
-plotCenterline(display_all_possible_paths=False, 
-		plot_title=None, 
-		save_plot_name=None, 
-		display_voronoi=False)
-```
-* [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging)
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
-* [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
-* [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline
-
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
-```
-Output:
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
-
-## Plot Centerline Width Lines in Matplotlib
-### Plot the Centerline Width Lines
-Plot the width of the river based on the centerline
-
-Display Centerline at even intervals from the Voronoi generated centerline
-```
-plotCenterlineWidth(plot_title=None, 
-		save_plot_name=None, 
-		display_true_centerline=True,
-		transect_span_distance=3,
-		apply_smoothing=False,
-		flag_intersections=True,
-		remove_intersections=False)
-```
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
-* [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
-* [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-* [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-* [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
-* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
-
-**apply_smoothing**
-
-apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
-
-| apply_smoothing=False | apply_smoothing=True |
-| ------------- | ------------- |
-| ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
-
-**transect_span_distance**
-
-Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
-
-![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
-| transect_span_distance=6 | transect_span_distance=30 |
-| ------------- | ------------- |
-| ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
-
-**remove_intersections**
-
-remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
-
-Intersecting lines are flagged in red by default (flag_intersections=True)
-
-| remove_intersections=False | remove_intersections=True |
-| ------------- | ------------- |
-| ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
-
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
-
-### Return Width of River
-
-Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
-
-```
-riverWidthFromCenterline(transect_span_distance=3,
-			apply_smoothing=True,
-			remove_intersections=False,
-			units="km",
-			save_to_csv=None)
-```
-* [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
-* [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
-* [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
-
-Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
-
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
-							apply_smoothing=True,
-							units="km",
-							remove_intersections=True)
-```
-Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
-
-## Documentation and Algorithm to Determine Centerline
-
-The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
-
-### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example1.png)
-
-### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example2.png)
-
-### Generate a Voronoi based on the points along the river banks
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
-
-### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
-
-### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
-With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
-
-### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
-| Points on River Bank | NetworkX Graph of Points on River Bank |
-| ------------- | ------------- |
-| ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
-
-### Display the centerline found by connecting the starting/ending node with the shortest path
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example8.png)
-
-This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed and no gaps exist in the centerline
-
-Points that only have one connection are removed, but by limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
-
-**All vertices:**
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
-
-**Vertices that have at least two connections (that would create gaps):**
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
-
-## Debugging, Error Handling, and Edge Cases
-### Wide Start/End of River
-If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
-Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
-
-### Invalid Polygon
-A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
-
-A polygon is invalid if it overlaps within itself:
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
-In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
-
-With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
-
-### Invalid Centerline
-If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
-
-`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
-Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
-
-### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
-Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
-
-If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
-
-If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
-
-This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
-
-### Fix Gaps and Jagged Centerlines
-Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
-Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
-```python
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
-```
-| interpolate_data = False | interpolate_data = True |
-| ------------- | ------------- |
-| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
-
-The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
-
-## Developer Notes: Tech Debt and Bug Fixes
-* Fix legend overlapping on graph, replace doc_examples that have an overlapping
-* Verify that smoothing filter option does not produce a line that goes outside of the polygon
-
-## Citations
-Based on work written in R (Golly et al. 2017):
-
->Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
-
-[Github - CMGO](https://github.com/AntoniusGolly/cmgo)
-
- <p align="center">
-  <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
-  <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
-  <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
-</p>
-
-This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
-
-## Bug and Feature Request
-
-Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
+Metadata-Version: 2.1
+Name: centerline-width
+Version: 0.2.4
+Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
+Home-page: https://github.com/cyschneck/centerline-width
+Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
+License: MIT
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.4.tar.gz
+Description: # Centerline-Width
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
+        </p>
+        
+        ![PyPi](https://img.shields.io/pypi/v/centerline-width)
+        ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
+        [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+        [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
+        
+        Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
+        
+        * **Convert raw data from Google Earth Pro to CSV**
+        	* extractPointsToTextFile()
+        	* convertColumnsToCSV()
+        * **Find centerline and width of river**
+        	* plotCenterline()
+        	* plotCenterlineWidth()
+        	* riverWidthFromCenterline()
+        	* saveCenterlineCSV()
+        	* centerlineVoronoi
+        	* centerlineEvenlySpaced
+        	* centerlineSmoothed
+        	* centerlineLength
+        	* rightBankLength
+        	* leftBankLength
+        
+        | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
+        | ------------- | ------------- |
+        | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
+        
+        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
+        
+        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
+        
+        ## Install
+        PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
+        
+        ```
+        pip install centerline-width
+        ```
+        
+        ## Requirements
+        Currently running on Python 3.7+
+        
+        ```
+        pip install -r requirements.txt
+        ```
+        Requirements will also be downloaded as part of the pip download
+        
+        ## Quickstart: centerline-width
+        
+        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+        
+        ```python
+        import centerline_width
+        centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
+        					right_kml="right_bank.kml",
+        					text_output_name="river_coordinates_output.txt")
+        centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
+        ```
+        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+        
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
+        ```
+        
+        To plot the centerline, run the `plotCenterline()` function from `river_object` created
+        ```python
+        river_object.plotCenterline()
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
+        
+        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
+        
+        While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
+        ```python
+        river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+        
+        ## Preprocessing
+        ### Convert KML files to Text File
+        
+        Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
+        
+        ```
+        extractPointsToTextFile(left_kml=None,
+        			right_kml=None,
+        			text_output_name=None)
+        ```
+        
+        * **[REQUIRED]** left_kml (string): File location of the kml file for left bank
+        * **[REQUIRED]** right_kml (string): File location of the kml file for right bank
+        * **[REQUIRED]** text_output_name (string): Output file name (and location)
+        
+        ```python
+        import centerline_width
+        centerline_width.extractPointsToTextFile(left_kml="leftbank.kml",
+        					right_kml="rightbank.kml",
+        					text_output_name="data/river_coords_output.txt")
+        ```
+        Output: The text file `data/river_coords_output.txt` with the headers `llat, llon, rlat, rlon` (for the left latitude, left longitude, right latitude, and right longitude)
+        
+        Example:
+        ```
+             llat       llon      rlat       rlon
+        30.037581 -92.868569 30.119804 -92.907933
+        30.037613 -92.868549 30.119772 -92.907924
+        30.037648 -92.868546 30.119746 -92.907917
+        30.037674 -92.868536 30.119721 -92.907909
+        30.037702 -92.868533 30.119706 -92.907905
+        ```
+        
+        ### Converted Text File to CSV
+        
+        Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
+        
+        ```
+        convertColumnsToCSV(text_file=None, flipBankDirection=False)
+        ```
+        * **[REQUIRED]** text_file (string): File location of the text file to convert
+        * [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+        
+        Scripts expects data as a list of point for left and right banks:
+        - Header: llat, llon, rlat, rlon
+        
+        ```python
+        import centerline_width
+        centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
+        				flipBankDirection=True)
+        ```
+        Converts text file:
+        ```
+             llat       llon      rlat       rlon
+        30.037581 -92.868569 30.037441 -92.867476
+        30.037613 -92.868549 30.037448 -92.867474
+        30.037648 -92.868546 30.037482 -92.867449
+        30.037674 -92.868536 30.037506 -92.867432
+        30.037702 -92.868533 30.037525 -92.867430
+        ```
+        To a CSV file:
+        ```
+        llat,llon,rlat,rlon
+        30.037581,-92.868569,30.037441,-92.867476
+        30.037613,-92.868549,30.037448,-92.867474
+        30.037648,-92.868546,30.037482,-92.867449
+        30.037674,-92.868536,30.037506,-92.867432
+        30.037702,-92.868533,30.037525,-92.867430
+        ```
+        Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
+        
+        ## Centerline and Width
+        ### River Object
+        First, generate a river object to contain river data and available transformations
+        ```
+        centerline_width.riverCenterline(csv_data=None,
+        				optional_cutoff=None,
+        				interpolate_data=False,
+        				interpolate_n=5,
+        				interpolate_n_centerpoints=None)
+        ```
+        * **[REQUIRED]** csv_data (string): File location of the text file to convert
+        * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
+        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+        * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+        * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
+        
+        **Solutions for sparse data:**
+        
+        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+        
+        `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
+        
+        | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
+        
+        **Object (class) useful attributes:**
+        
+        * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+        * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
+        * centerlineLength (float): Length of the centerline of the river (in km)
+        * rightBankLength (float): Length of the right bank of the river (in km)
+        * leftBankLength (float): Length of the left bank of the river (in km)
+        
+        **Object (class) additional atttributes:**
+        
+        * river_name (string): name of object, set to the csv_data string
+        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
+        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+        * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+        * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
+        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
+        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+        * interpolate_data (bool): if interpolating between existing data, defaults to False
+        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
+        
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        ```
+        
+        ### Return Latitude/Longitude Coordinates of Centerline
+        Return the latitude/longitude coordinates of the centerline based on the left and right banks
+        
+        **Types of Centerlines**
+        
+        There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+        
+        - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
+        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
+        - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
+        
+        Centerline coordinates are formed by the Voronoi vertices
+        ```
+        river_object.centerlineVoronoi
+        ```
+        
+        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+        ```
+        river_object.centerlineEvenlySpaced
+        ```
+        
+        Centerline coordinates are formed from Smoothed Voronoi vertices
+        ```
+        river_object.centerlineSmoothed
+        ```
+        
+        Example:
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
+        river_centerline_coordinates = river_object.centerlineVoronoi
+        ```
+        Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
+        
+        ### Save Centerline Coordinates to a CSV
+        Save the centerline coordinates to a csv file with columns for latitude and longitude
+        
+        ```
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+        ```
+        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
+        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
+        ```
+        
+        Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
+        
+        ### Return Length of Centerline
+        Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
+        ```
+        river_object.centerlineLength
+        ```
+        Length returned in kilometers
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
+        river_centerline_length = river_object.centerlineLength
+        ```
+        The length of the river centerline returns `215.34700589636674` km
+        
+        ## Plot Centerline in Matplotlib
+        Plot the centerline created from a list of right and left banks with Voronoi vertices
+        
+        ```
+        plotCenterline(display_all_possible_paths=False, 
+        		plot_title=None, 
+        		save_plot_name=None, 
+        		display_voronoi=False)
+        ```
+        * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
+        * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+        * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
+        * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.plotCenterline()
+        ```
+        Output:
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
+        
+        ## Plot Centerline Width Lines in Matplotlib
+        ### Plot the Centerline Width Lines
+        Plot the width of the river based on the centerline
+        
+        Display Centerline at even intervals from the Voronoi generated centerline
+        ```
+        plotCenterlineWidth(plot_title=None, 
+        		save_plot_name=None, 
+        		display_true_centerline=True,
+        		transect_span_distance=3,
+        		apply_smoothing=False,
+        		flag_intersections=True,
+        		remove_intersections=False)
+        ```
+        * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+        * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
+        * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
+        * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
+        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
+        
+        **apply_smoothing**
+        
+        apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
+        
+        | apply_smoothing=False | apply_smoothing=True |
+        | ------------- | ------------- |
+        | ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
+        
+        **transect_span_distance**
+        
+        Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
+        
+        ![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
+        | transect_span_distance=6 | transect_span_distance=30 |
+        | ------------- | ------------- |
+        | ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
+        
+        **remove_intersections**
+        
+        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
+        
+        Intersecting lines are flagged in red by default (flag_intersections=True)
+        
+        | remove_intersections=False | remove_intersections=True |
+        | ------------- | ------------- |
+        | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+        
+        ### Return Width of River
+        
+        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
+        
+        ```
+        riverWidthFromCenterline(transect_span_distance=3,
+        			apply_smoothing=True,
+        			remove_intersections=False,
+        			units="km",
+        			save_to_csv=None)
+        ```
+        * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+        * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
+        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+        
+        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
+        							apply_smoothing=True,
+        							units="km",
+        							remove_intersections=True)
+        ```
+        Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
+        
+        ## Documentation and Algorithm to Determine Centerline
+        
+        The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
+        
+        ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
+        
+        ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
+        
+        ### Generate a Voronoi based on the points along the riverbanks
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
+        
+        ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+        
+        ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
+        
+        ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
+        | Points on River Bank | NetworkX Graph of Points on River Bank |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
+        
+        ### Display the centerline found by connecting the starting/ending node with the shortest path
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
+        
+        This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
+        
+        Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
+        
+        **All vertices:**
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+        
+        **Vertices that have at least two connections (that would create gaps):**
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
+        
+        ## Debugging, Error Handling, and Edge Cases
+        ### Wide Start/End of River
+        If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
+        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
+        
+        ### Invalid Polygon
+        A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
+        
+        A polygon is invalid if it overlaps within itself:
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
+        In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
+        
+        With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
+        
+        ### Invalid Centerline
+        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
+        
+        `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
+        Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
+        
+        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+        Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+        
+        If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+        
+        If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+        
+        This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+        
+        ### Invalid Smoothed Centerline
+        The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+        
+        Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
+        
+        By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
+        
+        `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
+        
+        | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
+        
+        
+        ### Fix Gaps and Jagged Centerlines
+        Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
+        Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
+        ```
+        | interpolate_data = False | interpolate_data = True |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
+        
+        The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
+        
+        ## Developer Notes: Tech Debt and Bug Fixes
+        * Fix legend overlapping on graph, replace doc_examples that have an overlapping
+        * Verify that smoothing filter option does not produce a line that goes outside of the polygon
+        
+        ## Citations
+        Based on work written in R (Golly et al. 2017):
+        
+        >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
+        
+        [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
+        
+         <p align="center">
+          <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
+          <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
+          <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
+        </p>
+        
+        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
+        
+        ## Bug and Feature Request
+        
+        Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
+        
+Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
```

### Comparing `centerline-width-0.2.3/centerline_width/__init__.py` & `centerline-width-0.2.4/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/centerline.py` & `centerline-width-0.2.4/centerline_width/centerline.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,42 @@
 	nx_graphs, largest_subgraph_nodes = generateNXGraph(start_end_points_dict)
 
 	x_ridge_point = [] # X position on path
 	y_ridge_point = [] # Y poistion on path
 	starting_node = None # starting position at the top of the river
 	ending_node = None # ending position at the bottom of the river
 	for start_point, end_point_list in start_end_points_dict.items():
-			if len(end_point_list) > 0: # TESTING TESTING: Show only the end points that have multiple connections (set to 0 during production)
-				# Find the starting and ending node based on distance from the top and bottom of the polygon
-				if starting_node is None: 
-					starting_node = start_point
-				else:
-					if start_point in largest_subgraph_nodes: # Only include if node is on the largest subgraph (that represents the centerline)
-						if Point(start_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
-							starting_node = start_point
-				for end_point in end_point_list:
-					if start_point in largest_subgraph_nodes: # Only include if node is on the largest subgraph (that represents the centerline)
-						if Point(end_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
-							starting_node = end_point
-						if ending_node is None: 
+		if len(end_point_list) > 0: # TESTING TESTING: Show only the end points that have multiple connections (set to 0 during production)
+			# Find the starting and ending node based on distance from the top and bottom of the polygon
+			if starting_node is None: 
+				starting_node = start_point
+			else:
+				# Only include if starting point node is on the largest subgraph (that represents the centerline)
+				if start_point in largest_subgraph_nodes: 
+					# if start_point is closer to the top of the polygon than the current starting_node
+					if Point(start_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
+						starting_node = start_point
+			for end_point in end_point_list:
+				if ending_node is None: 
+					ending_node = end_point
+				# Only include if starting point node is on the largest subgraph (that represents the centerline)
+				if start_point in largest_subgraph_nodes:
+					# if the end_point is closer to the top of the polygon than the current starting_node
+					if Point(end_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
+						starting_node = end_point
+					else:
+						# if start_point is closer to the bottom than current ending_node
+						if Point(start_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
+							ending_node = start_point
+						# if end_point is closer to the bottom than current ending_node
+						if Point(end_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
 							ending_node = end_point
-						else:
-							if Point(start_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
-								ending_node = start_point
-							if Point(end_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
-								ending_node = end_point
-					# Save all starting and end positions for all possible paths
-					x_ridge_point.append((start_point[0], end_point[0]))
-					y_ridge_point.append((start_point[1], end_point[1]))
+				# Save all starting and end positions for all possible paths
+				x_ridge_point.append((start_point[0], end_point[0]))
+				y_ridge_point.append((start_point[1], end_point[1]))
 
 	if starting_node is None:
 		logger.critical("\nCRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.")
 		shortest_path_points = None
 	else:
 		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
 
@@ -118,15 +124,15 @@
 	# Convert Shapley Points to a List of Tuples (coordinates)
 	interpolated_centerline_coordinates = []
 	for point in points_evenly_spaced:
 		interpolated_centerline_coordinates.append((point.x, point.y))
 
 	return interpolated_centerline_coordinates
 
-def smoothedCoordinates(centerline_coordinates=None, interprolate_num=None):
+def smoothedCoordinates(river_object=None, centerline_coordinates=None, interprolate_num=None):
 	# return a list coordinates after applying b-spline (smoothing)
 	if centerline_coordinates is None:
 		return None
 
 	x_coordinates = []
 	y_coordinates = []
 
@@ -140,14 +146,22 @@
 	tck, *rest = interpolate.splprep([x_coordinates, y_coordinates], s=0.000001) # spline prep, tck = knots - coefficeinets - degree
 	u = np.linspace(0, 1, interprolate_num) # number of steps between each point (to determine smoothness)
 	x_smoothed, y_smoothed =  interpolate.splev(u, tck) # interpolated list of points
 
 	x_smoothed, y_smoothed = x_smoothed.tolist(), y_smoothed.tolist() # convert array to list
 	smoothed_coordinates = list(zip(x_smoothed, y_smoothed))
 
+	# Check if smoothed centerline lies outside polygon
+	points_outside_polygon = 0
+	for centerline_point in smoothed_coordinates:
+		if not river_object.bank_polygon.contains(Point(centerline_point)):
+			points_outside_polygon += 1
+	if points_outside_polygon > 2:
+		logger.critical("\nWARNING: Partially invalid smoothed centerline due to sparse centerline data ({0} points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to {1}+\n".format(points_outside_polygon, round(len(centerline_coordinates)*2.5)))
+
 	return smoothed_coordinates
 
 def riverWidthFromCenterlineCoordinates(river_object=None,
 										centerline_coordinates=None,
 										transect_span_distance=3,
 										remove_intersections=False,
 										save_to_csv=None):
```

### Comparing `centerline-width-0.2.3/centerline_width/error_handling.py` & `centerline-width-0.2.4/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/getCoordinatesKML.py` & `centerline-width-0.2.4/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/plotDiagrams.py` & `centerline-width-0.2.4/centerline_width/plotDiagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 			y.append(v)
 		#plt.scatter(x, y, c="black", label="Centerline Coordinates", s=8)
 		if display_true_centerline:
 			plt.plot(*zip(*river_object.centerlineVoronoi), c="black", label="Centerline")
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
-			plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
-			plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
+		plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
+		plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
 
 	return fig, ax, valid_path_through
 
 def plotCenterline(river_object=None,
 					display_all_possible_paths=False, 
 					plot_title=None, 
 					save_plot_name=None, 
@@ -136,17 +136,18 @@
 			else:
 				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
 																														remove_intersections=remove_intersections)
 
+			# Display the evenly spaced centerline
 			#x = []
 			#y = []
-			#for k, v in evenly_spaced_centerline_coordinates:
+			#for k, v in river_object.centerlineEvenlySpaced:
 			#	x.append(k)
 			#	y.append(v)
 			#plt.scatter(x, y, c="plum", label="Evenly Spaced Centerline Coordinates", s=8)
 			#plt.plot(*zip(*evenly_spaced_centerline_coordinates), "--", c="thistle", label="Evenly Spaced Centerline")
 
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
```

### Comparing `centerline-width-0.2.3/centerline_width/preprocessing.py` & `centerline-width-0.2.4/centerline_width/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 	top_river = LineString([Point(left_bank_lst[::-1][0][0],left_bank_lst[::-1][0][1]), Point(right_bank_lst[::-1][0][0], right_bank_lst[::-1][0][1])])
 	bottom_river = LineString([Point(right_bank_lst[0][0], right_bank_lst[0][1]), Point(left_bank_lst[0][0], left_bank_lst[0][1])])
 
 	if not river_polygon.is_valid and not recursion_check:
 		logger.critical("[FAILED]  Invalid Polygon may need to be corrected")
 		polygon_check, _, _ = generatePolygon(left_bank_lst, right_bank_lst[::-1], recursion_check=True) # only run once with recursion_check set (just to check if reverse banks fixes issue)
 		if polygon_check.is_valid:
-			logger.critical("\nInvalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)\n")
+			logger.critical("\nWARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)\n")
 	if river_polygon.is_valid and not recursion_check:
 		logger.info("[SUCCESS] Valid polygon generated")
 
 	return river_polygon, top_river, bottom_river
 
 def generateVoronoi(left_bank_lst, right_bank_lst):
 	# Generate a Voronoi shape based on the left/right bank points
```

### Comparing `centerline-width-0.2.3/centerline_width/pytests/test_centerline.py` & `centerline-width-0.2.4/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.2.4/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.2.4/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.2.4/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.2.4/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/centerline_width/riverCenterlineClass.py` & `centerline-width-0.2.4/centerline_width/riverCenterlineClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
 		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
 		# Centerline coordinates
 		self.centerlineVoronoi = shortest_path_coordinates
 		self.centerlineEvenlySpaced = centerline_width.evenlySpacedCenterline(centerline_coordinates=self.centerlineVoronoi,
 																						number_of_fixed_points=self.interpolate_n_centerpoints)
-		self.centerlineSmoothed = centerline_width.smoothedCoordinates(centerline_coordinates=self.centerlineEvenlySpaced,
+		self.centerlineSmoothed = centerline_width.smoothedCoordinates(river_object=self, centerline_coordinates=self.centerlineEvenlySpaced,
 																						interprolate_num=self.interpolate_n_centerpoints)
 
 		# Right/Length Bank Length
 		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
 		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
 
 		# Centerline length
```

### Comparing `centerline-width-0.2.3/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.2.4/centerline_width.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.3.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.4.tar.gz
 Description: # Centerline-Width
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
+        </p>
+        
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
-        Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
+        Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
         
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
@@ -25,36 +29,37 @@
         	* centerlineVoronoi
         	* centerlineEvenlySpaced
         	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
         
-        | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
+        | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
         
         Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
         
         NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
         
+        ## Install
+        PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
+        
+        ```
+        pip install centerline-width
+        ```
+        
         ## Requirements
         Currently running on Python 3.7+
         
         ```
         pip install -r requirements.txt
         ```
         Requirements will also be downloaded as part of the pip download
         
-        ## Install
-        PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
-        
-        ```
-        pip install centerline-width
-        ```
         ## Quickstart: centerline-width
         
         The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
         
         ```python
         import centerline_width
         centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
@@ -68,23 +73,23 @@
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
         To plot the centerline, run the `plotCenterline()` function from `river_object` created
         ```python
         river_object.plotCenterline()
         ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
         
         To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
         
         While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
@@ -156,67 +161,79 @@
         ## Centerline and Width
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
         				interpolate_data=False,
-        				interpolate_n=5)
+        				interpolate_n=5,
+        				interpolate_n_centerpoints=None)
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
-        * [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
+        * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+        * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         
-        Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
+        **Solutions for sparse data:**
         
-        Object (class) useful attributes:
+        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+        
+        `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
+        
+        | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
+        
+        **Object (class) useful attributes:**
         
         * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
-        Object (class) additional atttributes:
+        **Object (class) additional atttributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
-        * df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
+        * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
         * interpolate_data (bool): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
-        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
+        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
         
         **Types of Centerlines**
-        There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
+        
+        There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+        
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
         - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
         ```
         
         Centerline coordinates are formed by Evenly Spaced Voronoi vertices
@@ -272,26 +289,26 @@
         
         ```
         plotCenterline(display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False)
         ```
-        * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging)
+        * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
-        * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline
+        * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
+        river_object.plotCenterline()
         ```
         Output:
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
         
         ## Plot Centerline Width Lines in Matplotlib
         ### Plot the Centerline Width Lines
         Plot the width of the river based on the centerline
         
         Display Centerline at even intervals from the Voronoi generated centerline
         ```
@@ -302,15 +319,15 @@
         		apply_smoothing=False,
         		flag_intersections=True,
         		remove_intersections=False)
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-        * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+        * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
@@ -339,34 +356,34 @@
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         ### Return Width of River
         
         Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
         			units="km",
         			save_to_csv=None)
         ```
-        * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
+        * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
+        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
         * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
         
-        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
+        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
         							units="km",
@@ -375,91 +392,106 @@
         Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
         
         ## Documentation and Algorithm to Determine Centerline
         
         The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
         
         ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example1.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
         
         ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example2.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
         
-        ### Generate a Voronoi based on the points along the river banks
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
+        ### Generate a Voronoi based on the points along the riverbanks
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
         
-        ### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
+        ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
         
-        ### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
-        With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
+        ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
         | Points on River Bank | NetworkX Graph of Points on River Bank |
         | ------------- | ------------- |
-        | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
         
         ### Display the centerline found by connecting the starting/ending node with the shortest path
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example8.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
         
-        This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed and no gaps exist in the centerline
+        This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
         
-        Points that only have one connection are removed, but by limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
+        Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
         
         **All vertices:**
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
         
         **Vertices that have at least two connections (that would create gaps):**
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
         
         ## Debugging, Error Handling, and Edge Cases
         ### Wide Start/End of River
         If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
         Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
         A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
         
         A polygon is invalid if it overlaps within itself:
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
         
         With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
         
         ### Invalid Centerline
         If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
         
         `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
         ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
-        Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+        Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
         
-        If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+        If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
         This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+        
+        ### Invalid Smoothed Centerline
+        The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+        
+        Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
+        
+        By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
+        
+        `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
+        
+        | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
+        
         
         ### Fix Gaps and Jagged Centerlines
         Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
         Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
         ```python
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
         ```
         | interpolate_data = False | interpolate_data = True |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
         * Verify that smoothing filter option does not produce a line that goes outside of the polygon
```

### Comparing `centerline-width-0.2.3/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.2.4/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.3/setup.py` & `centerline-width-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.2.3"
+VERSION="0.2.4"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

