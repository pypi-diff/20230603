# Comparing `tmp/ediff-0.1.0.tar.gz` & `tmp/ediff-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediff-0.1.0.tar", last modified: Tue May  9 16:20:15 2023, max compression
+gzip compressed data, was "ediff-0.1.2.tar", last modified: Sat Jun  3 08:00:54 2023, max compression
```

## Comparing `ediff-0.1.0.tar` & `ediff-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.346619 ediff-0.1.0/
--rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 ediff-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     2010 2023-05-09 16:20:15.345621 ediff-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2023-05-09 15:48:32.000000 ediff-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 16:20:15.346619 ediff-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1258 2021-12-09 19:48:00.000000 ediff-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.308198 ediff-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.337655 ediff-0.1.0/src/ediff/
--rw-rw-rw-   0        0        0      173 2023-05-09 06:50:36.000000 ediff-0.1.0/src/ediff/__init__.py
--rw-rw-rw-   0        0        0      888 2022-09-12 12:23:00.000000 ediff-0.1.0/src/ediff/background.py
--rw-rw-rw-   0        0        0     2570 2023-05-09 07:17:18.000000 ediff-0.1.0/src/ediff/center.py
--rw-rw-rw-   0        0        0      718 2023-04-21 18:14:14.000000 ediff-0.1.0/src/ediff/io.py
--rw-rw-rw-   0        0        0    28913 2022-10-01 22:10:28.000000 ediff-0.1.0/src/ediff/pxrd.py
--rw-rw-rw-   0        0        0     4956 2023-04-21 18:14:46.000000 ediff-0.1.0/src/ediff/radial.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.344624 ediff-0.1.0/src/ediff.egg-info/
--rw-rw-rw-   0        0        0     2010 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 08:00:54.553764 ediff-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:53.000000 ediff-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     2141 2023-06-03 08:00:54.553764 ediff-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1603 2023-06-02 10:40:26.000000 ediff-0.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 08:00:54.553764 ediff-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2021-12-09 19:47:58.000000 ediff-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:00:54.472092 ediff-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 08:00:54.534808 ediff-0.1.2/src/ediff/
+-rw-rw-rw-   0        0        0      173 2023-05-26 18:40:17.000000 ediff-0.1.2/src/ediff/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-05-30 17:09:06.000000 ediff-0.1.2/src/ediff/background.py
+-rw-rw-rw-   0        0        0     2570 2023-05-09 07:17:17.000000 ediff-0.1.2/src/ediff/center.py
+-rw-rw-rw-   0        0        0     6340 2023-05-27 10:43:46.000000 ediff-0.1.2/src/ediff/io.py
+-rw-rw-rw-   0        0        0    28933 2023-05-27 10:59:24.000000 ediff-0.1.2/src/ediff/pxrd.py
+-rw-rw-rw-   0        0        0     3455 2023-05-18 10:21:52.000000 ediff-0.1.2/src/ediff/radial.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:00:54.553764 ediff-0.1.2/src/ediff.egg-info/
+-rw-rw-rw-   0        0        0     2141 2023-06-03 08:00:54.000000 ediff-0.1.2/src/ediff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-03 08:00:54.000000 ediff-0.1.2/src/ediff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 08:00:54.000000 ediff-0.1.2/src/ediff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 08:00:54.000000 ediff-0.1.2/src/ediff.egg-info/top_level.txt
```

### Comparing `ediff-0.1.0/LICENCE` & `ediff-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ediff-0.1.0/PKG-INFO` & `ediff-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.1.0
+Version: 0.1.2
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 Quick start
 -----------
 
 * See how it works:
 	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/pzio12tdj4j2c5v8usi5o/h?dl=0&rlkey=szpwqmvrdp5yeeiarfr2a5ab7).
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
 	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
@@ -46,7 +46,9 @@
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1.0 = 1st semi-complete version with basic documentation
+* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
+* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
```

### Comparing `ediff-0.1.0/README.md` & `ediff-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Quick start
 -----------
 
 * See how it works:
 	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/pzio12tdj4j2c5v8usi5o/h?dl=0&rlkey=szpwqmvrdp5yeeiarfr2a5ab7).
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
 	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
@@ -30,7 +30,9 @@
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1.0 = 1st semi-complete version with basic documentation
+* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
+* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
```

### Comparing `ediff-0.1.0/setup.py` & `ediff-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ediff-0.1.0/src/ediff/background.py` & `ediff-0.1.2/src/ediff/background.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # The module just imports key objects from external bground module.
 # This is a formal incorporation of bground module to ediff.background module.
 
 # How it works? = comment to the next two import commands:
 # The 1st import command = all modules from bground.ui to THIS module
 #  => now ediff.background knows the same modules as bground.ui
 #  => but NOT yet the classes withing bground.ui - these are imported next
-# The 2nd import ommand = three key classes from bground.ui to THIS module
+# The 2nd import command = three key classes from bground.ui to THIS module
 #  => now ediff.bacground contains the three objects from bground.ui
 #  => THIS module now contains InputData, PlotParams...
 #  => OTHER files can do: import bground.ui; DATA = bground.ui.InputData ...
 
 import bground.ui
 from bground.ui import InputData, PlotParams, InteractivePlot
```

### Comparing `ediff-0.1.0/src/ediff/center.py` & `ediff-0.1.2/src/ediff/center.py`

 * *Files identical despite different names*

### Comparing `ediff-0.1.0/src/ediff/pxrd.py` & `ediff-0.1.2/src/ediff/pxrd.py`

 * *Files 7% similar despite different names*

```diff
@@ -184,77 +184,29 @@
     title : str
         Title of the plot.
     x_axis : str, 'TwoTheta','S','q' or 'dhkl', optional, default is 'q'
         Quantity for X-axis.
     rcParams : dict; optional, the default is empty dictionary {}
         The dictionary should have the format of mathplotlib.pyplot.rcParams.
         The argmument is passed to matplotlib.pyplot.rcParams.update.
-        The initialization procedure creates some default rcParams.
-        This argument can override the pre-defined parameters,
-        which means that the default is created anyway
-        and then it can be adjusted here by rcParams argument.
+        This enables to override current rcParams, if necessary.
     '''
     
     def __init__(self, title=None, x_axis='q', xlim=None, rcParams={}):
         '''
         * Initialize PlotParameters object.
         * The parameters are described above in class definition.
         '''
         
         # Initialize basic parameters
         self.title = title
         self.x_axis = x_axis
         self.xlim = xlim
-        self.rcParams = rcParams
-        # Set global plot settings using rcParams
-        self.set_default_rcParams(rcParams)
-
-    @staticmethod
-    def set_default_rcParams(my_rcParams={}):
-        '''
-        A class method defining global plot parameters (plt.rcParams).
-        
-        Parameters
-        ----------
-        my_rcParams : dictionary
-            containing selected plt.rcParams keys)
-            DESCRIPTION. The default is {}.
-
-        Returns
-        -------
-        None, BUT it redefines global variable plt.rcParams!
-
-        Notes:
-        ------
-        * This is a @classmethod (because it is used within the whole class)
-          but it could be a @staticmethod as well (because it does not use
-          cls variable in fact).
-        * The method is employed in two ways:
-            - standard usage of MCREEP package: default rcParams are used
-              (and possibly modified) in objects of PlotParameters class
-            - special usage of MCREEP (more figures, multiplots): default
-              rcParams are used when definining the axes of (multiple)figures
-        '''
-        # (1) Set default rcParams
-        # (Hardcoded, suitable default for standard plots
-        plt.rcParams.update({
-            'figure.figsize'     : (8/2.54,6/2.54),
-            'figure.dpi'         : 500,
-            'font.size'          : 7,
-            'lines.linewidth'    : 0.8,
-            'axes.linewidth'     : 0.6,
-            'xtick.major.width'  : 0.6,
-            'ytick.major.width'  : 0.6,
-            'grid.linewidth'     : 0.6,
-            'grid.linestyle'     : ':'})
-        # (2) Update default with argument rcParams, if it was given
-        # (User-defined in the main program, if necessary
-        # (Useful namely for multiplots
-        plt.rcParams.update(my_rcParams)
-
+        if rcParams: plt.rcParams.update(rcParams)
+       
 class PeakProfiles:
     '''
     Define profile of diffraction peaks.
 
     * This class is employed only as a namespace.
     * It contains three functions/definitions of diffratction peak profiles.
     '''
@@ -539,14 +491,15 @@
         ---------------
         * The code below uses (sligthly modified) PyMatGen functions.
         * Reason: PyMatGen plotting works well with diffraction indexes.
           Re-programing of indexed plots would be difficult and useless...
         '''
         # (0) Redefine plot parameters
         # (so that they were optimized for the interactive plot
+        original_rcParams = plt.rcParams
         plt.rcParams.update({
             'figure.figsize'  : (12/2.54,4/2.54),
             'figure.dpi'      : 200,
             'font.size'       : 6})
         # (1) Calculate diffractions
         # (re-calculation in order to get the original PyMatGen xrd object
         # (the xrd object can be employed to plot diffractions with indexes
@@ -573,14 +526,16 @@
         # Trick #2: minor ticks => import special class for them
         ax.xaxis.set_major_locator(plt.MaxNLocator(15, steps=[1,2,5,10] ))
         from matplotlib.ticker import AutoMinorLocator
         ax.xaxis.set_minor_locator(AutoMinorLocator(5))
         # (5) Final adjustments
         fig.tight_layout()
         fig.show()
+        # (6) Revert to original rcParams.
+        plt.rcParams.update(original_rcParams)
         
     def print_diffractogram(self):
         self.print_diffractions()
         print('-----')
         print('* Just diffraction intensities, not the whole pattern.')
         print('* Reason: the whole diffraction pattern is too long.')
         print('* Note: save_diffractogram save the pattern to TXT-file.')
@@ -609,25 +564,47 @@
         if outfile != None: 
             plt.savefig(outfile) 
         else:
             plt.show()
         
     @staticmethod    
     def diffractions_to_dframe(intensities):
+        # Prepare hkl indexes
         h = []; k = []; l = []
-        for i in intensities.hkls:
-            h.append(i[0]['hkl'][0])
-            k.append(i[0]['hkl'][1])
-            l.append(i[0]['hkl'][2])
-        df = pd.DataFrame( 
-            np.transpose(
-                [intensities.x, h, k, l, intensities.d_hkls, intensities.y]),
-            columns=['TwoTheta','h','k','l','dhkl','Ihkl'])
-        df.insert(loc=5, column='S', value=1/df.dhkl)
-        df.insert(loc=6, column='q', value=2*np.pi*df.S)
+        # Test if the structure is hexagonal
+        hexagonal = (len(intensities.hkls[0][0]['hkl']) == 4)
+        # ...and if the structure is hexagonal, prepare i-index (hkl) -> (hkil)
+        if hexagonal: i = []
+        # Fill in hkl (or hkil) indexes
+        for ints in intensities.hkls:
+            h.append(ints[0]['hkl'][0])
+            k.append(ints[0]['hkl'][1])
+            if not(hexagonal):
+                l.append(ints[0]['hkl'][2])
+            else:    
+                i.append(ints[0]['hkl'][2])
+                l.append(ints[0]['hkl'][3])
+        # Create DataFrame from all values
+        # (again, we have to consider hexagonal structures => hkil indexes
+        if not(hexagonal):
+            df = pd.DataFrame( 
+                np.transpose(
+                    [intensities.x,
+                     h, k, l, intensities.d_hkls, intensities.y]),
+                columns=['TwoTheta','h','k','l','dhkl','Ihkl'])
+            df.insert(loc=5, column='S', value=1/df.dhkl)
+            df.insert(loc=6, column='q', value=2*np.pi*df.S)
+        else:
+            df = pd.DataFrame( 
+                np.transpose(
+                    [intensities.x,
+                     h, k, i, l, intensities.d_hkls, intensities.y]),
+                columns=['TwoTheta','h','k','i', 'l','dhkl','Ihkl'])
+            df.insert(loc=6, column='S', value=1/df.dhkl)
+            df.insert(loc=7, column='q', value=2*np.pi*df.S)
         return(df)
     
     @staticmethod
     def dframe_to_table(dframe):
         # POZOR: parametr formatters je zaludny!
         # * musi to byt sada funkci, takze...
         #   NEfunguji string-formaty '%.3f' - nejsou to funkce
@@ -638,26 +615,42 @@
         #       {}, {nazev_pole}, {nazev_pole:specifikace_formatu} ...
         #       pricemz v nasem pripade mame {:specifikace_formatu}
         #       takze odtud se tam vezme ta zdanlive mysticka dvojtecka
         #   trik #1: float M.N-format je bez carky '{:8.3f}'.format
         #       ale: float  .N-format je s carkou  '{:,.3f}'.format
         #   trik #2: NElze naformatovat obecny typ jako integer
         #     takze: pro obecne cislo misto NEfunkcniho {:3d} nutno {:3.0f}
-        table = dframe.to_string(
-            formatters={
-                'TwoTheta' : '{:8.3f}'.format,
-                'h'        : '{:3.0f}'.format,
-                'k'        : '{:3.0f}'.format,
-                'l'        : '{:3.0f}'.format,
-                'dhkl'     : '{:7.3f}'.format,
-                'S'        : '{:7.3f}'.format,
-                'q'        : '{:7.3f}'.format,
-                'Ihkl'     : '{:9.3f}'.format
-            }
-        )
+        # ------
+        # Test if the structure is hexagonal
+        hexagonal = (len(dframe.columns) == 9)
+        if not(hexagonal):
+            # (a) Non-hexagonal structure => hkl indexes (standard)
+            table = dframe.to_string(
+                formatters={
+                    'TwoTheta' : '{:8.3f}'.format,
+                    'h'        : '{:3.0f}'.format,
+                    'k'        : '{:3.0f}'.format,
+                    'l'        : '{:3.0f}'.format,
+                    'dhkl'     : '{:7.3f}'.format,
+                    'S'        : '{:7.3f}'.format,
+                    'q'        : '{:7.3f}'.format,
+                    'Ihkl'     : '{:9.3f}'.format})
+        else:
+            # (b) Hexagonal structure => hkil indexes (four, non-standard)
+            table = dframe.to_string(
+                formatters={
+                    'TwoTheta' : '{:8.3f}'.format,
+                    'h'        : '{:3.0f}'.format,
+                    'k'        : '{:3.0f}'.format,
+                    'i'        : '{:3.0f}'.format,
+                    'l'        : '{:3.0f}'.format,
+                    'dhkl'     : '{:7.3f}'.format,
+                    'S'        : '{:7.3f}'.format,
+                    'q'        : '{:7.3f}'.format,
+                    'Ihkl'     : '{:9.3f}'.format})
         return(table)
 
     def add_diffraction_vectors_to_diffractogram(self, df):
         # Prepare wavelenght (just shortcut for convenience)
         wavelength = self.experiment.wavelength
         # Insert a column with the calculated values of diffration vector S
         df.insert(loc = 1,
```

### Comparing `ediff-0.1.0/src/ediff/radial.py` & `ediff-0.1.2/src/ediff/radial.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 Module ediff.radial
 -------------------
 The conversion of a 2D powder diffraction pattern
 to a 1D powder diffraction pattern = radially averaged intensity distribution.
 '''
 
 import numpy as np
-import matplotlib.pyplot as plt
 from skimage import measure
 
-def calc_radial_distribution(arr):
+def calc_radial_distribution(arr, output_file=None):
     """
-    Calculate 1D-radially averaged distrubution profile
-    from 2D-PNBD diffraction pattern.
+    Calculate 1D radially averaged distrubution profile
+    from 2D diffraction pattern.
 
     Parameters
     ----------
     arr : 2D-numpy array
         The numpy array which contains the 2D-PNBD pattern.
+    output_file : str, optional, default is None
+        Name of the output file.
+        If given, the calculated 1D profile is saved to *output_file*.
 
     Returns
     -------
-    radial_distance, intensity : 1D numpy arrays
-        * radial_distance = distances from the center of 2D-PNBD [pixels]
-        * intensity = intensities at given distances [arbitrary units]
-    
-    Note
-    ----
-    * The plot of [radial_distance, intensity] = 1D-radial profile
-      corresponding to the input 2D-PNBD diffraction pattern.
+    profile : 2D numpy array containing two rows [R,I]
+        * R = radial_distance = dist. from the diffractogram center [pixels]
+        * I = intensity = intensities at given distances [arbitrary units]
     """
     # 1) Find center
     # (We employ function from skimage.measure (not from stemdiff.io),
     # (because we want float/non-integer values from the whole array.
     M =  measure.moments(arr,1)
     (xc,yc) = (M[1,0]/M[0,0], M[0,1]/M[0,0])
     # 2) Get image dimensions
@@ -52,37 +49,37 @@
     # (in circles with increasing distance from the center 
     # (trick 2: to create the circles, we will employ mask from trick 1
     for i in radial_distance:
         mask = np.greater(R, i - bin_size/2) & np.less(R, i + bin_size/2)
         values = arr[mask]
         intensity[index] = np.mean(values)
         index += 1 
-    # 6) Return the profile
-    return(radial_distance,intensity)
+    # 6) Save profile to array, save it to file if requested, and return it
+    profile = np.array([radial_distance, intensity])
+    if output_file: save_radial_distribution(profile, output_file)
+    return(profile)
 
-def save_radial_distribution(arr,filename):
+def save_radial_distribution(profile, output_file):
     """
-    Save 1D-radially averaged distrubution profile,
-    which is calculated from 2D-PNBD diffraction pattern, as a TXT-file.
+    Save 1D radially averaged distrubution profile to output_file.
 
     Parameters
     ----------
-    arr : 2D-numpy array
-        The numpy array which contains the 2D-PNBD pattern.
+    profile : 2D numpy array containing two rows [R,I]
+        * R = radial_distance = dist. from the diffractogram center [pixels]
+        * I = intensity = intensities at given distances [arbitrary units]
     filename : str
         Name of the output file.
 
     Returns
     -------
     None.
         The output is the radial distribution saved in a file with *filename*. 
     """
-    R,I = calc_radial_distribution(arr)
-    arr2 = np.array([R,I]).transpose()
-    np.savetxt(filename, arr2, fmt='%3d %8.1f')
+    np.savetxt(output_file, np.transpose(profile), fmt='%3d %8.1f')
 
 def read_radial_distribution(filename):
     """
     Read 1D-radially averaged distrubution profile from a TXT-file.
 
     Parameters
     ----------
@@ -93,55 +90,7 @@
     Returns
     -------
     arr : 2D-numpy array
         The array containing two columns: distance, intensity.
     """
     arr = np.loadtxt(filename, unpack=True)
     return(arr)
-    
-def plot_radial_distributions(
-        radial_distribution_files, xlimit, ylimit, output=None):
-    """
-    Plot several 1D-radial distrubution files in one graph.
-
-    Parameters
-    ----------
-    radial_distribution_files : 2D-list 
-        * list with several rows containing [filename, plot-style, name]
-        * filename = name of the TXT-file to plot
-        * plot-style = matplotlib.pyplot style, such as 'r-' (red line)
-        * name = name of the data, which will appear in the plot legend
-    xlimit : int
-        maximum of the X-axis
-    ylimit : int
-        maximum of the Y-axis
-    output : int, optional, default=None
-        Name of the output file;
-        if the *output* argument is given,
-        the plot is not only shown on screen, but also saved in *output* file. 
-
-    Returns
-    -------
-    Nothing
-        The output is the plot on screen
-        (and in *output* file if the *output* argument was given).
-    """
-    # Read radial distribution files
-    n = len(radial_distribution_files)
-    rdist = radial_distribution_files
-    # Plot radial distribution files
-    for i in range(n):
-        R,I     = read_radial_distribution(rdist[i][0])
-        myls    = rdist[i][1]
-        mylabel = rdist[i][2]
-        plt.plot(R,I, myls, label=mylabel)
-    # ...adjust plot
-    plt.xlabel('Radial distance [pixel]')
-    plt.ylabel('Intensity [grayscale]')
-    plt.xlim(0,xlimit)
-    plt.ylim(0,ylimit)
-    plt.legend()
-    plt.grid()
-    # ...save plot as PNG (only if argument [output] was given)
-    if output: plt.savefig(output, dpi=300)
-    # ...show plot
-    plt.show()
```

### Comparing `ediff-0.1.0/src/ediff.egg-info/PKG-INFO` & `ediff-0.1.2/src/ediff.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.1.0
+Version: 0.1.2
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 Quick start
 -----------
 
 * See how it works:
 	- Look at [worked example](https://mirekslouf.github.io/ediff/docs/examples/ex1_ediff.nb.html)
       in Jupyter.
 * Try it yourself:
-	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/pzio12tdj4j2c5v8usi5o/h?dl=0&rlkey=szpwqmvrdp5yeeiarfr2a5ab7).
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/nmsvdtef7xtmb7r2ku5aa/h?dl=0&rlkey=2evadkk009wp248rp2c3ij2nj).
 	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
 * [PyPI](https://pypi.org/project/ediff) repository.
 * [GitHub](https://github.com/mirekslouf/ediff) repository.
@@ -46,7 +46,9 @@
 -----------------
 
 * Version 0.0.1 = just draft
 * Version 0.0.2 = pxrd module works
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1.0 = 1st semi-complete version with basic documentation
+* Version 0.1.1 = v.0.1.0 + improved/simplified outputs
+* Version 0.1.2 = v.0.1.1 + small improvements of code and documentation
```

