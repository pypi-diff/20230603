# Comparing `tmp/stemdiff-5.0.2.tar.gz` & `tmp/stemdiff-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemdiff-5.0.2.tar", last modified: Wed May 10 12:48:05 2023, max compression
+gzip compressed data, was "stemdiff-5.0.4.tar", last modified: Sat Jun  3 07:57:49 2023, max compression
```

## Comparing `stemdiff-5.0.2.tar` & `stemdiff-5.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:48:05.914051 stemdiff-5.0.2/
--rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-5.0.2/CITATION
--rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-5.0.2/LICENCE
--rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-5.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3491 2023-05-10 12:48:05.914051 stemdiff-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2940 2023-05-10 12:40:34.000000 stemdiff-5.0.2/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 12:48:05.914051 stemdiff-5.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-10 12:47:28.000000 stemdiff-5.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:48:05.812627 stemdiff-5.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:48:05.898534 stemdiff-5.0.2/src/stemdiff/
--rw-rw-rw-   0        0        0      794 2023-05-10 12:45:01.000000 stemdiff-5.0.2/src/stemdiff/__init__.py
--rw-rw-rw-   0        0        0     5224 2023-05-02 21:01:54.000000 stemdiff-5.0.2/src/stemdiff/dbase.py
--rw-rw-rw-   0        0        0     5441 2023-05-08 14:22:33.000000 stemdiff-5.0.2/src/stemdiff/detectors.py
--rw-rw-rw-   0        0        0     4437 2023-04-30 15:34:56.000000 stemdiff-5.0.2/src/stemdiff/gvars.py
--rw-rw-rw-   0        0        0    27878 2023-05-06 23:36:48.000000 stemdiff-5.0.2/src/stemdiff/io.py
--rw-rw-rw-   0        0        0    14357 2023-05-07 11:24:49.000000 stemdiff-5.0.2/src/stemdiff/psf.py
--rw-rw-rw-   0        0        0    15600 2023-05-07 10:59:16.000000 stemdiff-5.0.2/src/stemdiff/sum.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:48:05.914051 stemdiff-5.0.2/src/stemdiff.egg-info/
--rw-rw-rw-   0        0        0     3491 2023-05-10 12:48:05.000000 stemdiff-5.0.2/src/stemdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-10 12:48:05.000000 stemdiff-5.0.2/src/stemdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:48:05.000000 stemdiff-5.0.2/src/stemdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-10 12:48:05.000000 stemdiff-5.0.2/src/stemdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 12:48:05.000000 stemdiff-5.0.2/src/stemdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 07:57:49.409022 stemdiff-5.0.4/
+-rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-5.0.4/CITATION
+-rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-5.0.4/LICENCE
+-rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-5.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3455 2023-06-03 07:57:49.409022 stemdiff-5.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-06-02 10:53:50.000000 stemdiff-5.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 07:57:49.409022 stemdiff-5.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-10 12:47:28.000000 stemdiff-5.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:57:49.377140 stemdiff-5.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 07:57:49.394515 stemdiff-5.0.4/src/stemdiff/
+-rw-rw-rw-   0        0        0      794 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/__init__.py
+-rw-rw-rw-   0        0        0     5544 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/dbase.py
+-rw-rw-rw-   0        0        0     7864 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/detectors.py
+-rw-rw-rw-   0        0        0     4437 2023-04-30 15:34:56.000000 stemdiff-5.0.4/src/stemdiff/gvars.py
+-rw-rw-rw-   0        0        0    35244 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/io.py
+-rw-rw-rw-   0        0        0       92 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/mcore.py
+-rw-rw-rw-   0        0        0    14639 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/psf.py
+-rw-rw-rw-   0        0        0    16326 2023-06-02 10:53:50.000000 stemdiff-5.0.4/src/stemdiff/sum.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:57:49.409022 stemdiff-5.0.4/src/stemdiff.egg-info/
+-rw-rw-rw-   0        0        0     3455 2023-06-03 07:57:49.000000 stemdiff-5.0.4/src/stemdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-03 07:57:49.000000 stemdiff-5.0.4/src/stemdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 07:57:49.000000 stemdiff-5.0.4/src/stemdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-03 07:57:49.000000 stemdiff-5.0.4/src/stemdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 07:57:49.000000 stemdiff-5.0.4/src/stemdiff.egg-info/top_level.txt
```

### Comparing `stemdiff-5.0.2/LICENCE` & `stemdiff-5.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.2/PKG-INFO` & `stemdiff-5.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 5.0.2
+Version: 5.0.4
 Summary: Convert 4D-STEM data to 2D-powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
 Classifier: Programming Language :: Python :: 3
@@ -50,28 +50,28 @@
 * [GitHub](https://github.com/mirekslouf/stemdiff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/stemdiff)
   with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
-* Version 2.0 = like v1.0 + post-processing in Jupyter
+* Version 2.0 = like v.1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
 	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
-* Version 4.2 = like v4.0 + a few important improvements, such as:
+* Version 4.2 = like v.4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
-* Version 5.0 = complete rewrite of v4.2
-	* all key features of v4.2 (summation, filtering, deconvolution)
-	* plus several generalizations and improvements, namely:
+* Version 5.0 = complete rewrite of v.4.2
+	* all key features of v.4.2 (summation, filtering, deconvolution)
+	* conversion *2D-diffractogram &rarr; 1D-profile* moved to package EDIFF
+	* several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
 		- better filtering (including estimated number of diffractions)
 		- more types of deconvolution algorithms
-	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to a sister package EDIFF
+
```

### Comparing `stemdiff-5.0.2/README.md` & `stemdiff-5.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 * [GitHub](https://github.com/mirekslouf/stemdiff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/stemdiff)
   with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
-* Version 2.0 = like v1.0 + post-processing in Jupyter
+* Version 2.0 = like v.1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
 	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
-* Version 4.2 = like v4.0 + a few important improvements, such as:
+* Version 4.2 = like v.4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
-* Version 5.0 = complete rewrite of v4.2
-	* all key features of v4.2 (summation, filtering, deconvolution)
-	* plus several generalizations and improvements, namely:
+* Version 5.0 = complete rewrite of v.4.2
+	* all key features of v.4.2 (summation, filtering, deconvolution)
+	* conversion *2D-diffractogram &rarr; 1D-profile* moved to package EDIFF
+	* several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
 		- better filtering (including estimated number of diffractions)
 		- more types of deconvolution algorithms
-	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to a sister package EDIFF
+
```

### Comparing `stemdiff-5.0.2/setup.py` & `stemdiff-5.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.2/src/stemdiff/__init__.py` & `stemdiff-5.0.4/src/stemdiff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     - 2D-NBD's = monocrystalline-like nanobeam diffraction patterns.
 * Output = 2D-powder diffraction pattern
     - A 2D-powder diffraction pattern is calculated from a 4D-STEM dataset.
     - The calculation is basically a specific summation of 2D-NBD patterns.
     - In other words, a 4D-STEM dataset is reduced to a 2D-diffraction pattern.
     - The whole method (and final pattern) is called 4D-STEM/PNBD (powder NBD).
 '''
-__version__ = "5.0.2"
+__version__ = "5.0.4"
```

### Comparing `stemdiff-5.0.2/src/stemdiff/dbase.py` & `stemdiff-5.0.4/src/stemdiff/dbase.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,38 +32,43 @@
     Returns
     -------
     df : pandas DataFrame object
         Database contains [filename, xc, yc, MaxInt, NumPeaks, S]
         for each datafile in the dataset.
     """
     # Prepare variables before we run for-cycle to go through datafiles
-    # Initialize coordinates of the center = intensity center = primary beam
+    # (initialize coordinates of the center + rescale/upscale coefficient
     xc,yc = (None,None)
+    R = SDATA.detector.upscale
     # Initialize list of datafiles
     # (appending to lists is more efficient than appending to np/pd-structures
     list_of_datafiles = []
     # Pre-calculate additional variables
     # (it would be wasteful to calculate them in each for-cycle loop
     # half_of_csquare = round(DIFFIMAGES.csquare/2)
     neighborhood_matrix = np.ones((DIFFIMAGES.peak_dist,DIFFIMAGES.peak_dist))
     # Go through datafiles and calculated their entropy
     for datafile in SDATA.filenames:
         # a) Read datafile
         arr = stemdiff.io.Datafiles.read(SDATA,datafile)
         # b) Get datafile name
         datafile_name = datafile.relative_to(SDATA.data_dir)
-        # c) Calculate center (of intensity)
+        # c) Calculate intensity center
+        # (to get high precision
+        # (the center must be determined for rescaled/upscaled array
         if DIFFIMAGES.ctype == 2:
             xc,yc = stemdiff.io.Arrays.find_center(
-                arr, DIFFIMAGES.csquare, DIFFIMAGES.cintensity)
+                stemdiff.io.Arrays.rescale(arr, R, order=3),  # rescaled array
+                DIFFIMAGES.csquare*R, DIFFIMAGES.cintensity)  # central region
         elif (DIFFIMAGES.ctype == 1) and (xc == None):
             xc,yc = stemdiff.io.Array.find_center(
-                arr, DIFFIMAGES.csquare, DIFFIMAGES.cintensity)
+                stemdiff.io.Arrays.rescale(arr, R, order=3),  # rescaled array
+                DIFFIMAGES.csquare*R, DIFFIMAGES.cintensity)  # central region
         elif (DIFFIMAGES.ctype == 0) and (xc == None):
-            geometric_center = round(SDATA.detector.detector_size/2)
+            geometric_center = round(SDATA.detector.detector_size*R/2)
             xc,yc = (geometric_center,geometric_center)
         # d) Determine maximum intensity
         max_intensity = np.max(arr)
         # e) Estimate number of peaks (local maxima)
         no_of_maxima = stemdiff.io.Arrays.number_of_peaks(arr,
             peak_height = DIFFIMAGES.peak_height, 
             neighborhood_matrix=neighborhood_matrix)
```

### Comparing `stemdiff-5.0.2/src/stemdiff/gvars.py` & `stemdiff-5.0.4/src/stemdiff/gvars.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.2/src/stemdiff/io.py` & `stemdiff-5.0.4/src/stemdiff/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 
 Three types of stemdiff.io objects
 
 * Datafiles = files on disk, saved directly from a 2D-STEM detector.
 * Arrays = the datafiles converted to numpy array objects.
 * Images = the datafiles converted to PNG files.
 
-General strategy of stemdiff.io package
+General strategy for working with stemdiff.io objects
     
 * Datafiles and Images are usually
   not used directly, but just converted to Array objects.
 * All data manipulation (showing, scaling, saving ...)
   is done within Array objects.
 * Datafiles and Images have (intentionally) just a limited amount of methods,
   the most important of which is read - this method simply reads
   Datafile/Image to an array.
 
+Additional stemdiff.io utilities
+
+* These are stored directly in the package, without any subclassing.
+* Mostly general routines for more convenient I/O within stemdiff package.
+
 Examples how to use Datafiles, Arrays and Images
 
 >>> # Show a datafile
 >>> # (basic operation => there is Datafiles.function for it
 >>> stemdiff.io.Datafiles.show(SDATA, filename)
 
 >>> # Read a datafile to array
@@ -30,25 +35,125 @@
 >>> arr = stemdiff.io.Datafiles.read(SDATA, filename)
 
 >>> # Describe AND show the datafile
 >>> # (more complex operation:
 >>> # (1) read datafile to array - using Datafiles.read
 >>> # (2) do what you need (here: describe, show) - using Arrays.functions
 >>> arr = stemdiff.io.Datafiles.read(SDATA, datafile)
->>> stemdiff.io.Arrays.describe(arr, central_square=20)
+>>> stemdiff.io.Arrays.describe(arr, csquare=20)
 >>> stemdiff.io.Arrays.show(arr, icut=1000, cmap='gray')
 '''
 
 
 import numpy as np
 import matplotlib.pyplot as plt
 from PIL import Image
 from skimage import transform, measure, morphology
 
 
+def set_plot_parameters(size=(12,9), dpi=75, fontsize=10, my_rcParams=None):
+    '''
+    Set global plot parameters (mostly for plotting in Jupyter).
+
+    Parameters
+    ----------
+    size : tuple of two floats, optional, the default is (12,9)
+        Size of the figure (width, height) in [cm].
+    dpi : int, optional, the defalut is 75
+        DPI of the figure.
+    fontsize : int, optional, the default is 10
+        Size of the font used in figure labels etc.
+    my_rcParams : dict, optional, default is None
+        Dictionary in plt.rcParams format
+        containing any other allowed global plot parameters.
+
+    Returns
+    -------
+    None; the result is a modification of the global plt.rcParams variable.
+    '''
+    if size:  # Figure size
+        # Convert size in [cm] to required size in [inch]
+        size = (size[0]/2.54, size[1]/2.54)
+        plt.rcParams.update({'figure.figsize' : size})
+    if dpi:  # Figure dpi
+        plt.rcParams.update({'figure.dpi' : dpi})
+    if fontsize:  # Global font size
+        plt.rcParams.update({'font.size' : fontsize})
+    if my_rcParams:  # Other possible rcParams in the form of dictionary
+        plt.rcParams.update(my_rcParams)
+
+
+def plot_2d_diffractograms(data_to_plot,
+                           icut=None, cmap='viridis',
+                           output_file=None, dpi=300):
+    '''
+    Plot a few selected 2D diffraction patterns in a row one-by-one.
+
+    Parameters
+    ----------
+    data_to_plot : list of lists
+        This object is a list of lists.
+        The number of rows = the number of plotted diffractograms.
+        Each row contains two elements:
+        (i) data for diffractogram to plot and (ii) title of the plot.
+        The data (first element of each row) can be:
+        (i) PNG-file or (ii) 2D-array containing the 2D diffractogram. 
+    integer, optional, default is None
+        Cut of intensity;
+        if icut = 300, all image intensities > 300 will be equal to 300.
+    cmap : str - matplotlib.colormap name, optional, the default is 'viridis'
+        Matplotlib colormap for plotting of the diffractogram.
+        Other interesting or high-contrast options:
+        'gray', 'plasma', 'magma', ...
+        The full list of matplotlib colormaps:
+        `matplotlib.pyplot.colormaps()` 
+    output_file : str, optional, default is None
+        If this argument is given,
+        the plot is also saved in *output_file* image
+        with *dpi* resolution (dpi is specified by the following argument).
+    dpi : int, optional, default is 300
+        The (optional) argument gives resolution of (optional) output image. 
+
+    Returns
+    -------
+    None.
+    The output is the plot of the diffraction patterns on the screen.
+    If argument *ouput_file* is given, the plot is also saved as an image. 
+    '''
+    # Initialize
+    n = len(data_to_plot)
+    diffs = data_to_plot
+    fig,ax = plt.subplots(nrows=1, ncols=n)
+    # Plot 2D-diffractograms
+    for i in range(n):
+        # Read data to plot
+        data = diffs[i][0]
+        if type(data) == str:  # Datafile
+            if data.lower().endswith('.png'):  # ....PNG file, 2D-diffractogram
+                # we read image as '16bit'
+                # in this case, it works for 8bit images as well    
+                arr = Images.read(data, itype='16bit')
+            else:  # .......some other string not ending on PNG => unknown data
+                print('Unknown type of data to plot!')
+        elif type(data) == np.ndarray:  # Numpy array
+            if data.shape[0] == data.shape[1]:  # sqare array, 2D-diffractogram
+                arr = data
+            else: # .....some other, non-square array => nonstandard array size
+                print('Non-standard array for plotting!')
+        # Read plot parameters
+        my_title = diffs[i][1]
+        # Plot i-th datafile/array
+        ax[i].imshow(arr, vmax=icut, cmap=cmap)
+        ax[i].set_title(my_title)
+    # Finalize plot
+    for i in range(n): ax[i].axis('off')
+    fig.tight_layout()
+    if output_file: fig.savefig(output_file, dpi=dpi)
+
+    
 class Datafiles:
     
 
     def read(SDATA, filename):
         '''
         Read a datafile from STEM detector to an array.
         
@@ -66,15 +171,15 @@
         '''
         arr = SDATA.detector.read_datafile(filename)
         return(arr)
     
 
     def show(SDATA, filename,
              icut=None, itype='8bit', R=None, cmap='gray',
-             center=False, central_square=20, cintensity=0.8):
+             center=False, csquare=20, cintensity=0.8):
         '''
         Show datafile/diffractogram with basic characteristics.
         
         Parameters
         ----------
         SDATA : stemdiff.gvars.SourceData object
             The object describes source data (detector, data_dir, filenames).
@@ -88,21 +193,24 @@
             If itype equals None or '16-bit' the image is treated as 16-bit.
         R : integer, optional, default is None
             Rescale coefficient;
             the input array is rescaled (usually upscaled) R-times.
             For typical 2D-STEM detector with size 256x256 pixels,
             the array should be processed with R=4
             in order to get sufficiently large image for further processing.
-        cmap : str, name of colormap, optional, default is 'gray'
-            Colormap for plotting of the array.
-            Other options: 'viridis', 'plasma' etc.; more info in www.
+        cmap : str - matplotlib.colormap name, optional, the default is 'gray'
+            Matplotlib colormap for plotting of the array.
+            Other interesting or high-contrast options:
+            'viridis', 'plasma', 'magma' ...
+            The full list of matplotlib colormaps:
+            `matplotlib.pyplot.colormaps()`
         center : bool, optional, default is False
             If True, intensity center is drawn in the final image.
-        central_square : integer, optional, default is 20
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is 20
+            Edge of a central square, from which the center will be determined.
             Ignored if center == False.
         cintensity : float in interval 0--1, optional, default is 0.8
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
             Ignored if center == False.
             
         Returns
@@ -115,21 +223,21 @@
         This function just combines Datafiles.read + Arrays.show functions.
         '''
         # Read datafile to array
         arr = Datafiles.read(SDATA, filename)
         # Describe datafile/array
         Arrays.show(arr,
             icut, itype, R, cmap,
-            center, central_square, cintensity)
+            center, csquare, cintensity)
 
 
     def show_from_disk(SDATA,
                        interactive=True, max_files=None,
                        icut=1000, itype=None, R=None, cmap='gray',
-                       center=True, central_square=20, cintensity=0.8,
+                       center=True, csquare=20, cintensity=0.8,
                        peak_height=100, peak_distance=9):
         '''
         Show datafiles (stored in a disk) from 2D-STEM detector. 
         
         Parameters
         ----------
         SDATA : stemdiff.gvars.SourceData object
@@ -149,21 +257,24 @@
             If itype equals None or '16-bit' the image is treated as 16-bit.
         R : integer, optional, default is None
             Rescale coefficient;
             the input array is rescaled (usually upscaled) R-times.
             For typical 2D-STEM detector with size 256x256 pixels,
             the array should be processed with R=4
             in order to get sufficiently large image for further processing.
-        cmap : str, name of colormap, optional, default is 'gray'
-            Colormap for plotting of the array.
-            Other options: 'viridis', 'plasma' etc.; more info in www.
+        cmap : str - matplotlib.colormap name, optional, the default is 'gray'
+            Matplotlib colormap for plotting of the array.
+            Other interesting or high-contrast options:
+            'viridis', 'plasma', 'magma', ...
+            The full list of matplotlib colormaps:
+            `matplotlib.pyplot.colormaps()`
         center : bool, optional, default is False
             If True, intensity center is drawn in the final image.
-        central_square : integer, optional, default is 20
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is 20
+            Edge of a central square, from which the center will be determined.
             Ignored if center == False.
         cintensity : float in interval 0--1, optional, default is 0.8
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
             Ignored if center == False.
         peak_height : int, optional, default is 100
             Minimal height of the peak to be detected.
@@ -186,33 +297,33 @@
             # Read datafile from disk to array
             arr = Datafiles.read(SDATA, datafile)
             # Print datafile name
             datafile_name = datafile.relative_to(SDATA.data_dir)
             print('Datafile:', datafile_name)
             # Describe the datafile/array
             Arrays.describe(arr,
-                central_square, cintensity, peak_height, peak_distance)
+                csquare, cintensity, peak_height, peak_distance)
             # Show the datafile/array
             Arrays.show(arr,
                 icut, itype, R, cmap,
-                center, central_square, cintensity)
+                center, csquare, cintensity)
             # Decide if we should stop the show
             if interactive:
                 # Wait for keyboard input...
                 choice = str(input('[Enter] to show next, [q] to quit...\n'))
                 # Break if 'q' was pressed and continue otherwise...
                 if choice == 'q': break
             elif max_files:
                 file_counter += 1
                 if file_counter >= max_files: break
 
     
     def show_from_database(SDATA, df,
                            interactive=True, max_files=None,
-                           icut=1000, itype='8bit', R=None, cmap='gray'):
+                           icut=1000, itype='8bit', cmap='gray'):
         '''
         Show datafiles (pre-selected in a database) from 2D-STEM detector.
 
         Parameters
         ----------
         SDATA : TYPE
             DESCRIPTION.
@@ -226,30 +337,29 @@
             show files non-interactively = in one run, until
             number of files is less than max_files limit.
         icut : integer, optional, default is None
             Cut of intensity;
             if icut = 300, all image intensities > 300 will be equal to 300.
         itype : string, optional, '8bit' or '16bit', default is '8bit'
             Type of the image - 8 or 16 bit grayscale.   
-        R : integer, optional, default is None
-            Rescale coefficient;
-            the input array is rescaled (usually upscaled) R-times.
-        cmap : str, name of colormap, optional, default is 'gray'
-            Colormap for plotting of the array.
-            Other options: 'viridis', 'plasma' etc.; more info in www.
+        cmap : str - matplotlib.colormap name, optional, the default is 'gray'
+            Matplotlib colormap for plotting of the array.
+            Other interesting or high-contrast options:
+            'viridis', 'plasma', 'magma', ...
+            The full list of matplotlib colormaps:
+            `matplotlib.pyplot.colormaps()`
 
         Returns
         -------
         Nothing
             The output are the files and their characteristics on the screen.
         
         Technical note
         --------------
-        This function uses Datafiles.read function
-        and it reads data from database.
+        This function uses Datafiles.read function to read data from database.
         As it uses database data, it cannot use standard Arrays functions. 
         '''
         # Initialize file counter
         file_counter = 0
         # Show the files and their characteristics saved in the database
         for index,datafile in df.iterrows():
             # Read datafile
@@ -262,32 +372,36 @@
             print(f'Maximum intensity: {datafile.MaxInt}')
             print(f'Number of peaks: {datafile.Peaks}')
             print(f'Shannon entropy: {datafile.S}')
             # Show datafile (and draw XY-center from the database data)
             arr = np.where(arr>icut, icut, arr)
             plt.imshow(arr, cmap=cmap)
             # Draw center
-            # (if the image is rescaled, the center should be rescaled as well
-            if R == None: R = 1
+            # (we read data from database
+            # (files are shown without any rescaling
+            # (but database contains Xcenter,Ycenter from upscaled images
+            # (=> we have to divide Xcenter,Ycenter by rescale coefficient!
+            R = SDATA.detector.upscale
             plt.plot(
-                datafile.Ycenter * R,
-                datafile.Xcenter * R,
+                datafile.Ycenter/R,
+                datafile.Xcenter/R,
                 'r+', markersize=20)
             plt.show()
             # Increase file counter & stop if max_files limit was reached
             file_counter += 1
             if file_counter >= max_files: break
 
 
 class Arrays:
 
 
     def show(arr,
-             icut=None, itype=None, R=None, cmap='gray',
-             center=False, central_square=20, cintensity=0.8):
+             icut=None, itype=None, R=None, cmap=None,
+             center=False, csquare=20, cintensity=0.8,
+             plt_type='2D', plt_size=None, colorbar=False):
         '''
         Show 2D-array as an image.
         
         Parameters
         ----------
         arr : 2D numpy array
             Array to show.
@@ -299,56 +413,105 @@
             If itype equals None or '16-bit' the image is treated as 16-bit.
         R : integer, optional, default is None
             Rescale coefficient;
             the input array is rescaled (usually upscaled) R-times.
             For typical 2D-STEM detector with size 256x256 pixels,
             the array should be processed with R=4
             in order to get sufficiently large image for further processing.
-        cmap : str, name of colormap, optional, default is 'gray'
-            Colormap for plotting of the array.
-            Other options: 'viridis', 'plasma' etc.; more info in www.
+        cmap : str - matplotlib.colormap name, optional, the default is None
+            Matplotlib colormap for plotting of the array.
+            Interesting or high-contrast options:
+            'gray', 'viridis', 'plasma', 'magma', ...
+            The full list of matplotlib colormaps:
+            `matplotlib.pyplot.colormaps()`
         center : bool, optional, default is False
             If True, intensity center is drawn in the final image.
-        central_square : integer, optional, default is 20
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is 20
+            Edge of a central square, from which the center will be determined.
             Ignored if center == False.
         cintensity : float in interval 0--1, optional, default is 0.8
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
             Ignored if center == False.
+        plt_type : str, '2D' or '3D', optional, default is '2D'
+            Type of the plot: 2D-dimensional or 3D-dimensional/surface plot.
+        plt_size : int, optional, default is not
+            If given, we plot only the central region with size = *plt_size*.
+            For central region we use a geometric center - see Technical notes.
+        colorbar : bool, optional, the default is False
+            If True, a colorbar is added to the plot.
     
         Returns
         -------
         Nothing
             The output is the array shown as an image on the screen.
+        
+        Technical notes
+        ---------------
+        * In this function, we *do not* center the image/array.
+          Center can be drawn to 2D-image, but array *is not centered*.
+        * Edges can be removed (using plt_size argument),
+          but only only with respect to the geometrical center,
+          which means that the function shows a *non-cenered central region*.
+        * If you need to show *centered central region* of an array,
+          combine Arrays.find_center + Arrays.remove_edges + Arrays.show
         '''        
         # Prepare array for saving
         arr = Arrays.prepare_for_show_or_save(arr, icut, itype, R)
+        # Remove edges of the plot, if requested
+        # (just simple removal of edges based on geometrical center!
+        # (reason: simplicity; for centering/edge removal we have other funcs
+        if plt_size:
+            Xsize,Ysize = arr.shape
+            xc,yc = (int(Xsize/2),int(Ysize/2))
+            if plt_size:
+                arr = Arrays.remove_edges(arr,plt_size,xc,yc)    
         # Plot array as image
-        plt.imshow(arr, cmap=cmap)
-        # If center argument was given, add intensity center to the plot
-        if center==True:
-            xc,yc = Arrays.find_center(arr,central_square, cintensity)
-            plt.plot(yc,xc, 'r+', markersize=20)
-        # Show the plot
+        # (a) Prepare 2D plot (default)
+        if plt_type=='2D':  
+            if cmap==None:  # if cmap not selected, set default for 2D maps
+                cmap='viridis'
+            plt.imshow(arr, cmap=cmap)
+            if colorbar:  # Add colorbar
+                plt.colorbar()
+            if center==True:  # Mark intensity center in the plot
+                xc,yc = Arrays.find_center(arr,csquare, cintensity)
+                plt.plot(yc,xc, 'r+', markersize=20)
+        # (b) Prepare 3D plot (option; if plt_type is not the default '2D')
+        else:  
+            if cmap==None:  # if cmap not selected, set default for 3D maps
+                cmap='coolwarm'
+            # Prepare meshgrid for 3D-plotting
+            Xsize,Ysize = arr.shape
+            X = np.arange(Xsize)
+            Y = np.arange(Ysize)
+            Xm,Ym = np.meshgrid(X,Y)
+            # Create 3D-plot
+            from mpl_toolkits.mplot3d import Axes3D
+            fig = plt.figure()
+            ax = fig.add_subplot(111, projection='3d')
+            ax.plot_surface(
+                Xm,Ym,arr, cmap=cmap, linewidth=0, antialiased=False)
+            plt.tight_layout()
+        # (c) Show the plot
         plt.show()
 
 
     def describe(arr,
-                 central_square=20, cintensity=0.8,
+                 csquare=20, cintensity=0.8,
                  peak_height=100, peak_distance=5):
         '''
         Describe 2D-array = print XY-center, MaxIntensity, Peaks, Sh-entropy.
 
         Parameters
         ----------
         arr : 2D numpy array
             Array to describe.
-        central_square : integer, optional, default is None
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is None
+            Edge of a central square, from which the center will be determined.
         cintensity : float in interval 0--1, optional, default is None
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
         peak_height : int, optional, default is 100
             Minimal height of the peak to be detected.
         peak_distance : int, optional, default is 5
             Minimal distance between two peaks so that they were separated.
@@ -361,68 +524,68 @@
         Technical note
         --------------
         This function is just a wrapper
         around several np.functions and Arrays.functions.
         To get the values, use the individual functions instead.
         '''
         # Determine center (of intensity)
-        x,y = Arrays.find_center(arr, central_square, cintensity)
+        x,y = Arrays.find_center(arr, csquare, cintensity)
         print(f'Center (x,y): ({x:.1f},{y:.1f})')
         # Determine maximum intensity
         max_intensity = np.max(arr)
         print(f'Maximum intensity = {max_intensity:d}')
         # Estimate number of peaks (local maxima)
         no_of_maxima = Arrays.number_of_peaks(arr, peak_height, peak_distance)
         print(f'Number of peaks = {no_of_maxima}')
         # Calculate Shannon entropy of the datafile
         entropy_value = measure.shannon_entropy(arr)
         print(f'Shannon entropy = {entropy_value:.2f}')
             
 
-    def find_center(arr, central_square=None, cintensity=None):
+    def find_center(arr, csquare=None, cintensity=None):
         '''
         Determine center of mass for 2D numpy array.
         Array center = mass/intensity center ~ position of central spot.
         Warning: In most cases, geometric center is NOT mass/intensity center.
     
         Parameters
         ----------
         arr : numpy 2D array
             Numpy 2D array, whose center (of mass ~ intensity) we want to get.
-        central_square : integer, optional, default is None
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is None
+            Edge of a central square, from which the center will be determined.
         cintensity : float in interval 0--1, optional, default is None
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
             
         Returns
         -------
         xc,yc : integers
             Coordinates of the intesity center = position of the primary beam.
         '''
         # Calculate center of array
-        if central_square:
-            # If central_square was given,
+        if csquare:
+            # If csquare was given,
             # calculate center only for the square in the center,
             # in which we set background intensity = 0 to get correct results.
             # a) Calculate array corresponding to central square
             xsize,ysize = arr.shape
-            xborder = (xsize - central_square) // 2
-            yborder = (ysize - central_square) // 2
+            xborder = (xsize - csquare) // 2
+            yborder = (ysize - csquare) // 2
             arr2 = arr[xborder:-xborder,yborder:-yborder].copy()
             # b) Set intensity lower than maximum*coeff to 0 (background removal)
             coeff = cintensity or 0.8
             arr2 = np.where(arr2>np.max(arr2)*coeff, arr2, 0)
             # c) Calculate center of intensity (and add borders at the end)
             M = measure.moments(arr2,1)
             (xc,yc) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
             (xc,yc) = (xc+xborder,yc+yborder)
             (xc,yc) = np.round([xc,yc],2)
         else:
-            # If central_square was not given,
+            # If csquare was not given,
             # calculate center for the whole array.
             # => Wrong position of central spot for non-centrosymmetric images!
             M = measure.moments(arr,1)
             (xc,yc) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
             (xc,yc) = np.round([xc,yc],2)
         # Return final values            
         return(xc,yc)
@@ -629,15 +792,15 @@
         else:
             arr = np.asarray(img, dtype=np.uint16)
         return(arr)
     
 
     def show(image_name,
              icut=None, itype='8bit', R=None, cmap='gray',
-             center=False, central_square=20, cintensity=0.8):
+             center=False, csquare=20, cintensity=0.8):
         '''
         Read and display image from disk.
         
         Parameters
         ----------
         image_name : str or path-like object
             Name of image to read.
@@ -648,31 +811,34 @@
             Type of the image - 8 or 16 bit grayscale.   
         R : integer, optional, default is None
             Rescale coefficient;
             the input array is rescaled (usually upscaled) R-times.
             For typical 2D-STEM detector with size 256x256 pixels,
             the array should be processed with R=4
             in order to get sufficiently large image for further processing.
-        cmap : str, name of colormap, optional, default is 'gray'
-            Colormap for plotting of the array.
-            Other options: 'viridis', 'plasma' etc.; more info in www.
+        cmap : str - matplotlib.colormap name, optional, the default is 'gray'
+            Matplotlib colormap for plotting of the array.
+            Other interesting or high-contrast options:
+            'viridis', 'plasma', 'magma', ...
+            The full list of matplotlib colormaps:
+            `matplotlib.pyplot.colormaps()`
         center : bool, optional, default is False
             If True, intensity center is drawn in the final image.
-        central_square : integer, optional, default is 20
-            Edge of a central_square, from which the center will be determined.
+        csquare : integer, optional, default is 20
+            Edge of a central square, from which the center will be determined.
             Ignored if center == False.
         cintensity : float in interval 0--1, optional, default is 0.8
             The intensity < maximum_intensity * cintensity is regarded as 0
             (a simple temporary background removal in the central square).
             Ignored if center == False.
         
         Returns
         -------
         Nothing
             The output is *image_name* shown on the screen.
         '''
         # Read Image to array.
-        arr = Images.read_image(image_name, itype=itype)
+        arr = Images.read(image_name, itype=itype)
         # Show the array using pre-defined stemdiff.io.Array.show function.
         Arrays.show(arr,
                     icut, itype, R, cmap,
-                    center, central_square, cintensity)
+                    center, csquare, cintensity)
```

### Comparing `stemdiff-5.0.2/src/stemdiff/psf.py` & `stemdiff-5.0.4/src/stemdiff/psf.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             arr = stemdiff.io.Datafiles.read(SDATA, file_to_read)
             file_counter += 1
             # (b) Rescale array
             arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
             # (c) Remove edges if psf_size is given
             if psf_size:
                 xc,yc = stemdiff.io.Arrays.find_center(arr,
-                    central_square = DIFFIMAGES.csquare*R,
+                    csquare = DIFFIMAGES.csquare*R,
                     cintensity = DIFFIMAGES.cintensity)
                 arr = stemdiff.io.Arrays.remove_edges(arr,
                     rsize = psf_size*R, xc=round(xc), yc=round(yc))
                 psf += arr
             else:
                 psf += arr
         # (3) Calculate final experimental PSF
@@ -283,30 +283,34 @@
         # (they are very dangerous, leading to unwanted side-effects and errors
         psf = np.where(psf < 0, 0, psf)
         # Return final PSF
         return(psf)
 
 class PSFtype3:
         
-    def get_psf(arr, psf_size, cake, subtract = False):
+    def get_psf(arr, psf_size=100, cake=30, subtract=False):
         '''
         Get PSF of type3 = individual PSF based on cake-method.
 
         Parameters
         ----------
         arr : 2D-numpy array
             The array/datafile, from which the PSF is to be determined.
             The array is a square with geometrical center = intensity center.
             See *Technical notes* below for more details and consequences.
-        psf_size : int
+        psf_size : int, optional, default
             The size/diameter of PSF function to be determined.
         cake : int
             Size of cake-piece in degrees.
         subtract : bool, optional, default is False
             If True, prepare PSF with the same size as scattering pattern.
+            In fact, this function *does not* subtract anything.
+            It can *prepare PSF suitable for subtracting* if required.
+            The trick is that a PSF suitable for subtracting
+            must have the the same size as the original image = arr.
             
         Returns
         -------
         psf : 2D-numpy array
             The array represents estimate of experimental PSF.
 
         Technical notes
@@ -342,15 +346,15 @@
         # Pixels selection without peak 
         for i in range(arr.shape[0]):
             for ii in range(arr.shape[1]):
                 sig_sorted = np.sort(psf_multilevel[i,ii,:], axis=None)
                 # Prepared for np.mean and interval [0:x]
                 psf[i,ii] = np.median(sig_sorted[:]) 
         
-        # XXX: Important safety insertion
+        # Important safety insertion
         # (due to various recalcs and roundings, psf may go below 0
         # (negative psf values result in many unwanted side effects and errors!
         psf = np.where(psf < 0, 0, psf)
         
         return(psf)
 
 class PSFtype4:
```

### Comparing `stemdiff-5.0.2/src/stemdiff/sum.py` & `stemdiff-5.0.4/src/stemdiff/sum.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,35 +85,37 @@
         - The parameters are transferred from the sum_files function
 '''
     # Prepare variables
     n = 0  # number of summed datafiles
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     # Prepare array for summation
-    # (for summation without deconvolution array size = detector size
-    # (we will sum original datafiles, just without the borders/edges  
-    # (rescaling to higher resolution can be done AFTER the summation
-    sum_arr   = np.zeros((img_size,img_size), dtype=np.float32)
+    # (for the precise center determination, we must sum upscaled arrays
+    sum_arr   = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     for index,datafile in df.iterrows():
         # Read datafile to array
         datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
         arr = stemdiff.io.Datafiles.read(SDATA, datafile_name)
-        # Reduce array size = cut borders, keep just central region
-        # (some border region is ALWAYS cut, due to detector edge artifacts
+        # Rescale/upscale datafile and THEN remove border region
+        # (i) the accurate image center must be taken from the upscaled image
+        # (ii) then the borders can be removed with respect to the center
+        # (This procedure is necessary to center the images precisely.
+        # (The accurate centers from upscaled images are saved in database.
+        # (Some border region should ALWAYS be cut, for two reasons:
+        # (i) weak/zero diffractions at edges and (ii) detector edge artifacts
+        arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
         xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size*R,xc,yc)
         # Add current datafile/array to summation
         sum_arr += arr
         # Update n = number of summed arrays
         n += 1
-    # Prepare final array:
-    # (1) normalize summation, 2) rescale to higher res, 3) convert to final
+    # Prepare final array = (1) normalize summation and (2) convert to final
     sum_arr = sum_arr/n
-    sum_arr = stemdiff.io.Arrays.rescale(sum_arr, R, order=3)
     final_arr = np.round(sum_arr).astype(np.uint16)
     # Return the final array
     return(final_arr)
 
 def sum_with_deconvolution_type1(SDATA, DIFFIMAGES, df, psf, iterate):
     '''
     Sum datafiles with 2D-PSF deconvolution of type1.
@@ -130,50 +132,51 @@
         - The parameters are transferred from the sum_files function
     '''
     # Prepare variables .......................................................
     n = 0
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     # Prepare array for summation
-    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    # (for better precision, we use deconvolution on rescaled/upscaled array
     sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     # (we sum datafiles cut, rescaled, and deconvoluted
     # (rescaling DURING the summation => smoother deconvolution function
     # Sum with deconvolution, external PSF from low-diffracting files .........
     for index,datafile in df.iterrows():
         # (0) Simple progress indicator
         print('.', end='')
         # (1) Read datafile
         datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
-        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
-        # (2) Remove edges
-        # (reason: edges usually contain weak or neglibible difractions
-        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
-        # (3) Upscale array
-        # (reason: deconvolution should be performed at higher resolution
-        # ( -logically, more pixels means smoother PSF => better deconvolution
-        # ( -surprisingly, upscaling increases real final resolution
+        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name)
+        # (2) Rescale/upscale datafile and THEN remove border region
+        # (i) the accurate image center must be taken from the upscaled image
+        # (ii) then the borders can be removed with respect to the center
+        # (This procedure is necessary to center the images precisely.
+        # (The accurate centers from upscaled images are saved in database.
+        # (Some border region should ALWAYS be cut, for two reasons:
+        # (i) weak/zero diffractions at edges and (ii) detector edge artifacts
         arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
-        # (4) Deconvolute using the external PSF
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size*R,xc,yc)        
+        # (3) Deconvolute using the external PSF
         # (a) save np.max, normalize
         # (reason: deconvolution algorithm requires normalized arrays...
         # (...and we save original max.intensity to re-normalize the result
         norm_const = np.max(arr)
         arr_norm = arr/np.max(arr)
         psf_norm = psf/np.max(psf)
         # (b) perform the deconvolution
         arr_deconv = restoration.richardson_lucy(
             arr_norm, psf_norm, num_iter=iterate)
         # (c) restore original range of intensities = re-normalize
         arr = arr_deconv * norm_const
-        # (6) Add rescaled and deconvoluted array to summation
+        # (4) Add rescaled and deconvoluted array to summation
         sum_arr += arr
-        # (7) Updated n = number of summed arrays
+        # (5) Updated n = number of summed arrays
         n += 1
     # Finalize and return result ..............................................
     # (a) terminate simple progress indicator
     print('End')
     # (b) normalize the final array
     sum_arr = sum_arr/n
     # (c) convert to final array with integer values
@@ -199,52 +202,53 @@
     '''
     # Prepare variables .......................................................
     n = 0
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     psf_size = DIFFIMAGES.psfsize
     # Prepare array for summation
-    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    # (for better precision, we use deconvolution on rescaled/upscaled array
     sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     # (we sum datafiles cut, rescaled, and deconvoluted
     # (rescaling DURING the summation => smoother deconvolution function
     # Sum with deconvolution, PSF from center of image ........................
     for index,datafile in df.iterrows():
         # (0) Simple progress indicator
         print('.', end='')
         # (1) Read datafile
         datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
         arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
-        # (2) Remove edges
-        # (reason: edges usually contain weak or neglibible difractions
-        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
-        # (3) Upscale array
-        # (reason: deconvolution should be performed at higher resolution
-        # ( -logically, more pixels means smoother PSF => better deconvolution
-        # ( -surprisingly, upscaling increases real final resolution
+        # (2) Rescale/upscale datafile and THEN remove border region
+        # (i) the accurate image center must be taken from the upscaled image
+        # (ii) then the borders can be removed with respect to the center
+        # (This procedure is necessary to center the images precisely.
+        # (The accurate centers from upscaled images are saved in database.
+        # (Some border region should ALWAYS be cut, for two reasons:
+        # (i) weak/zero diffractions at edges and (ii) detector edge artifacts
         arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
-        # (4) Prepare PSF from the center of given array
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size*R,xc,yc)        
+        # (3) Prepare PSF from the center of given array
         psf = stemdiff.psf.PSFtype2.get_psf(arr, psf_size, circular=True)
-        # (5) Deconvolute
+        # (4) Deconvolute
         # (a) save np.max, normalize
         # (reason: deconvolution algorithm requires normalized arrays...
         # (...and we save original max.intensity to re-normalize the result
         norm_const = np.max(arr)
         arr_norm = arr/np.max(arr)
         psf_norm = psf/np.max(psf)
         # (b) perform the deconvolution
         arr_deconv = restoration.richardson_lucy(
             arr_norm, psf_norm, num_iter=iterate)
         # (c) restore original range of intensities = re-normalize
         arr = arr_deconv * norm_const
-        # (6) Add rescaled and deconvoluted array to summation
+        # (5) Add rescaled and deconvoluted array to summation
         sum_arr += arr
-        # (7) Updated n = number of summed arrays
+        # (6) Updated n = number of summed arrays
         n += 1
     # Finalize and return result ..............................................
     # (a) terminate simple progress indicator
     print('End')
     # (b) normalize the final array
     sum_arr = sum_arr/n
     # (c) convert to final array with integer values
@@ -266,63 +270,64 @@
         - This function is usually called from stemdiff.sum.sum_files.
         - The parameters are transferred from the sum_files function
     '''
     
     # Prepare variables .......................................................
     n = 0
     R = SDATA.detector.upscale
-    # !!! img_size and psf_size must by multiplied by R wherever relevant
+    # ! img_size and psf_size must by multiplied by R wherever relevant
     img_size = DIFFIMAGES.imgsize 
     psf_size = DIFFIMAGES.psfsize
     # Prepare array for summation
-    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    # (for better precision, we use deconvolution on rescaled/upscaled array
     sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     # (we sum datafiles cut, rescaled, and deconvoluted
     # (rescaling DURING the summation => smoother deconvolution function
     # Sum with deconvolution, PSF from center of image ........................
     for index,datafile in df.iterrows():
         # (0) Simple progress indicator
         print('.', end='')
         # (1) Read datafile
         datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
         arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
-        # (2) Remove edges
-        # (reason: edges usually contain weak or neglibible difractions
-        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
-        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
-        # (3) Upscale array
-        # (reason: deconvolution should be performed at higher resolution
-        # ( -logically, more pixels means smoother PSF => better deconvolution
-        # ( -surprisingly, upscaling increases real final resolution
+        # (2) Rescale/upscale datafile and THEN remove border region
+        # (i) the accurate image center must be taken from the upscaled image
+        # (ii) then the borders can be removed with respect to the center
+        # (This procedure is necessary to center the images precisely.
+        # (The accurate centers from upscaled images are saved in database.
+        # (Some border region should ALWAYS be cut, for two reasons:
+        # (i) weak/zero diffractions at edges and (ii) detector edge artifacts
         arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
-        # (4) Prepare PSF from the center of given array
-        # !!! psf_size must by multiplied by R
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size*R,xc,yc)        
+        # (3) Prepare PSF from the center of given array
+        # ! psf_size must by multiplied by R
         psf = stemdiff.psf.PSFtype3.get_psf(arr, psf_size*R, cake, subtract)   
         if subtract:    
             # Individual background (PSF) subtraction
             arr = arr - psf
             # All negative values shoud go to zero!
             # (the negative values have result in many side effects and errors!
             arr = np.where(arr < 0, 0, arr)
-        # (5) Deconvolute
+        # (4) Deconvolute
         # (a) save np.max, normalize
         # (reason: deconvolution algorithm requires normalized arrays...
         # (...and we save original max.intensity to re-normalize the result
         norm_const = np.max(arr)
         arr_norm = arr/np.max(arr)
         psf_norm = psf/np.max(psf)
         # (b) perform the deconvolution
         arr_deconv = restoration.richardson_lucy(
             arr_norm, psf_norm, num_iter=iterate)
         # (c) restore original range of intensities = re-normalize
         arr = arr_deconv * norm_const
-        # (6) Add rescaled and deconvoluted array to summation
+        # (5) Add rescaled and deconvoluted array to summation
         sum_arr += arr
-        # (7) Updated n = number of summed arrays
+        # (6) Updated n = number of summed arrays
         n += 1
     # Finalize and return result ..............................................
     # (a) terminate simple progress indicator
     print('End')
     # (b) normalize the final array
     sum_arr = sum_arr/n
     # (c) convert to final array with integer values
```

### Comparing `stemdiff-5.0.2/src/stemdiff.egg-info/PKG-INFO` & `stemdiff-5.0.4/src/stemdiff.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 5.0.2
+Version: 5.0.4
 Summary: Convert 4D-STEM data to 2D-powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
 Classifier: Programming Language :: Python :: 3
@@ -50,28 +50,28 @@
 * [GitHub](https://github.com/mirekslouf/stemdiff) repository.
 * [GitHub Pages](https://mirekslouf.github.io/stemdiff)
   with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
-* Version 2.0 = like v1.0 + post-processing in Jupyter
+* Version 2.0 = like v.1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
 	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
-* Version 4.2 = like v4.0 + a few important improvements, such as:
+* Version 4.2 = like v.4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
-* Version 5.0 = complete rewrite of v4.2
-	* all key features of v4.2 (summation, filtering, deconvolution)
-	* plus several generalizations and improvements, namely:
+* Version 5.0 = complete rewrite of v.4.2
+	* all key features of v.4.2 (summation, filtering, deconvolution)
+	* conversion *2D-diffractogram &rarr; 1D-profile* moved to package EDIFF
+	* several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
 		- better filtering (including estimated number of diffractions)
 		- more types of deconvolution algorithms
-	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to a sister package EDIFF
+
```

