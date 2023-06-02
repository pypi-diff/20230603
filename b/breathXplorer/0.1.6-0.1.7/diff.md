# Comparing `tmp/breathXplorer-0.1.6.tar.gz` & `tmp/breathXplorer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breathXplorer-0.1.6.tar", last modified: Thu Jun  1 18:46:03 2023, max compression
+gzip compressed data, was "breathXplorer-0.1.7.tar", last modified: Fri Jun  2 22:26:40 2023, max compression
```

## Comparing `breathXplorer-0.1.6.tar` & `breathXplorer-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.228761 breathXplorer-0.1.6/
--rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.6/LICENSE
--rw-r--r--   0 wangyk     (501) staff       (20)     6822 2023-06-01 18:46:03.228546 breathXplorer-0.1.6/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)     6141 2023-06-01 18:38:02.000000 breathXplorer-0.1.6/README.md
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.226377 breathXplorer-0.1.6/breathXplorer/
--rw-r--r--   0 wangyk     (501) staff       (20)       85 2023-06-01 18:11:03.000000 breathXplorer-0.1.6/breathXplorer/__init__.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.6/breathXplorer/cluster.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2763 2023-05-31 22:39:26.000000 breathXplorer-0.1.6/breathXplorer/container.py
--rw-r--r--   0 wangyk     (501) staff       (20)     1939 2023-05-30 23:11:26.000000 breathXplorer-0.1.6/breathXplorer/extract.py
--rw-r--r--   0 wangyk     (501) staff       (20)     5589 2023-05-30 23:09:12.000000 breathXplorer-0.1.6/breathXplorer/file_io.py
--rw-r--r--   0 wangyk     (501) staff       (20)     6081 2023-06-01 18:11:03.000000 breathXplorer-0.1.6/breathXplorer/find_peak.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2392 2023-05-04 19:00:37.000000 breathXplorer-0.1.6/breathXplorer/utils.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.227748 breathXplorer-0.1.6/breathXplorer.egg-info/
--rw-r--r--   0 wangyk     (501) staff       (20)     6822 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)      410 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/requires.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/top_level.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-06-01 18:46:03.228828 breathXplorer-0.1.6/setup.cfg
--rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-05-31 00:33:00.000000 breathXplorer-0.1.6/setup.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.227920 breathXplorer-0.1.6/tests/
--rw-r--r--   0 wangyk     (501) staff       (20)      523 2023-06-01 18:32:19.000000 breathXplorer-0.1.6/tests/test_extract.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-02 22:26:40.777725 breathXplorer-0.1.7/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.7/LICENSE
+-rw-r--r--   0 wangyk     (501) staff       (20)     9209 2023-06-02 22:26:40.777521 breathXplorer-0.1.7/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)     8528 2023-06-02 22:23:05.000000 breathXplorer-0.1.7/README.md
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-02 22:26:40.775712 breathXplorer-0.1.7/breathXplorer/
+-rw-r--r--   0 wangyk     (501) staff       (20)       85 2023-06-01 18:11:03.000000 breathXplorer-0.1.7/breathXplorer/__init__.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.7/breathXplorer/cluster.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     4884 2023-06-02 21:16:45.000000 breathXplorer-0.1.7/breathXplorer/container.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     1967 2023-06-02 21:22:51.000000 breathXplorer-0.1.7/breathXplorer/extract.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     5301 2023-06-02 21:22:51.000000 breathXplorer-0.1.7/breathXplorer/file_io.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     6081 2023-06-01 18:11:03.000000 breathXplorer-0.1.7/breathXplorer/find_peak.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2392 2023-05-04 19:00:37.000000 breathXplorer-0.1.7/breathXplorer/utils.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-02 22:26:40.776850 breathXplorer-0.1.7/breathXplorer.egg-info/
+-rw-r--r--   0 wangyk     (501) staff       (20)     9209 2023-06-02 22:26:40.000000 breathXplorer-0.1.7/breathXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)      410 2023-06-02 22:26:40.000000 breathXplorer-0.1.7/breathXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-06-02 22:26:40.000000 breathXplorer-0.1.7/breathXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-06-02 22:26:40.000000 breathXplorer-0.1.7/breathXplorer.egg-info/requires.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-06-02 22:26:40.000000 breathXplorer-0.1.7/breathXplorer.egg-info/top_level.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-06-02 22:26:40.777785 breathXplorer-0.1.7/setup.cfg
+-rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-06-02 21:22:51.000000 breathXplorer-0.1.7/setup.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-02 22:26:40.777041 breathXplorer-0.1.7/tests/
+-rw-r--r--   0 wangyk     (501) staff       (20)      523 2023-06-01 18:32:19.000000 breathXplorer-0.1.7/tests/test_extract.py
```

### Comparing `breathXplorer-0.1.6/LICENSE` & `breathXplorer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.6/PKG-INFO` & `breathXplorer-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,28 @@
-Metadata-Version: 2.1
-Name: breathXplorer
-Version: 0.1.6
-Summary: A toolkit for breath metabolomics analysis
-Home-page: https://github.com/wykswr/breathXplorer
-Author: wykswr
-Author-email: bifocal.above.0y@icloud.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # breathXplorer
 
 [![PyPI](https://img.shields.io/pypi/pyversions/breathXplorer)](https://pypi.org/project/breathXplorer/)
 [![Python package](https://github.com/wykswr/breathXplorer/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/wykswr/breathXplorer/actions/workflows/python-package.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <!-- TOC -->
-
 * [breathXplorer](#breathxplorer)
-    * [Introduction](#introduction)
-    * [Quick start](#quick-start)
-        * [Installation](#installation)
-        * [File format](#file-format)
-        * [Feature extraction](#feature-extraction)
-        * [Feature alignment](#feature-alignment)
-    * [Utilities](#utilities)
-        * [MS/MS spectra export](#msms-spectra-export)
-        * [Peak recognition](#peak-recognition)
-    * [Citation](#citation)
-
+  * [Introduction](#introduction)
+  * [Quick start](#quick-start)
+    * [Installation](#installation)
+    * [File format](#file-format)
+      * [Feature table CSV](#feature-table-csv)
+      * [Aligned feature table CSV](#aligned-feature-table-csv)
+      * [MS/MS spectra MGF](#msms-spectra-mgf)
+    * [Feature extraction](#feature-extraction)
+    * [Feature alignment](#feature-alignment)
+  * [Utilities](#utilities)
+    * [MS/MS spectra export](#msms-spectra-export)
+    * [Peak recognition](#peak-recognition)
+  * [Citation](#citation)
 <!-- TOC -->
 
 ## Introduction
 
 BreathXplorer is a swiss army knife for breath analysis. It provides a set of tools for breath analysis, including
 feature extraction, feature alignment, and breath recognition.
 
@@ -52,34 +34,79 @@
 It's recommended to install the package in a virtual environment or a conda environment,
 after activating the environment, run the following command to install the package:
 
 `pip install breathXplorer`
 
 ### File format
 
-The input file should be in mzML format. For the output, the single or aligned feature table can be exported as csv
-file.
+The input file should be in mzML or mzXML format (Perhaps more in the future). For the output, 
+the single or aligned feature table can be exported as csv file.
 The related MS/MS spectra can be exported in an mgf file.
 
+#### Feature table CSV
+
+|                   | intensity          | 0.0072552628 | 0.026703197   | 0.043871898 |
+|-------------------|--------------------|--------------|---------------|-------------|
+| 70.00432621552620 | 42831.928564484600 | 90863.234375 | 34955.3671875 | 0.0         |
+| 70.06507751535940 | 7697202.355213430  | 6714245.5    | 6476909.5     | 6479075.5   |
+| 70.07309580891320 | 18459.317394976800 | 0.0          | 0.0           | 0.0         |
+| 70.12570290061420 | 65085.35662117530  | 0.33127435   | 0.34847233    | 0.36571398  |
+
+The index of the table is the m/z value of the features, and the 1st column is the total intensity of the feature.
+The other columns are the intensity of the feature over time, the time is the name of the corresponding column.
+
+#### Aligned feature table CSV
+
+|                   | S01_Before        | S02_Before         | S03_Before         |
+|-------------------|-------------------|--------------------|--------------------|
+| 70.06522594212220 | 8400258.455035770 | 3229242.0293803000 | 8472742.497544320  |
+| 71.0489436673768  | 449896.521925234  | 11058.402315007400 | 413906.96622934300 |
+| 71.06833464948300 | 386030.8760258960 | 12110.036064627900 | 398033.1097357460  |
+
+The index of the table is the m/z value of the features, and each column is the total intensity of the feature in a sample (
+experiment of a subject). The name of the column is the sample name.
+
+#### MS/MS spectra MGF
+
+```
+BEGIN IONS
+PEPMASS=70.004
+MSLEVEL=2
+50.630638335563866 1466.3514404296875
+50.63166334943464 2041.7808837890625
+END IONS
+
+BEGIN IONS
+PEPMASS=70.064993720777
+MSLEVEL=2
+53.00126253392352 1509.3829345703125
+71.06273290316524 27731.6875
+71.06506220434123 870.4231567382812
+END IONS
+```
+
+The file contains the MS/MS spectra of the features, each feature has a PEPMASS (precursor mass) and MSLEVEL field, and the following
+pairs are the m/z and intensity of the MS/MS spectra.
+
 ### Feature extraction
 
 Feature extraction is used to find the volatile organic compound (VOC) in the breath sample.
-The feature extraction is performed using the `find_feature` function. The function takes the path to an mzMl file
+The feature extraction is performed using the `find_feature` function. The function takes the path to an mzMl/mzXML file
 as input, and returns an object containing the extracted feature table:
 
 ```python
 from breathXplorer import find_feature
 
 fs = find_feature("sample.mzML", False, .8, "Topological", 6)
 ```
 
 The `False` indicates that the input file is not a line spectrum, and the `.8` controls the quality of the extracted
 features, higher value means higher quality. The `"Topological"` indicates the algorithm used for feature extraction,
 the other option is `"Gaussian"`. The `6` is the prior knowledge of the number of breath in an experiment (only used
-for Gaussian algorithm).
+for Gaussian algorithm, and you don't need to impute it if using Topological).
 
 The `fs` is a FeatureSet object, it contains the following information:
 
 ```python
 fs.mz  # m/z values of the extracted features
 fs.scan_time  # scan time of the experiment
 fs.intensity  # the total intensity of each feature (calculated by integrating the intensity over scan time)
@@ -98,19 +125,23 @@
 The `merge_feature` function takes as input a list of FeatureSet objects, and returns a Sample object. It aligns the
 features with the similar m/z value from different samples, and calculate the total intensity of each feature in each
 sample. To use the function, you can do the following:
 
 ```python
 from breathXplorer import merge_result, find_feature
 
-fss = [find_feature(f, False, .8, "Gaussian", 6) for f in ["sample1.mzML", "sample2.mzML", "sample3.mzML"]]
+fss = [find_feature(f, False, .8, "Gaussian", 6) for f in ["sample1.mzML", "sample2.mzXML", "sample3.mzML"]]
 sample = merge_result(fss, ["sample1", "sample2", "sample3"])
 ```
 
-The first statement creates a list of FeatureSet objects, the second statement aligns those FeatureSet objects.
+The first statement creates a list of FeatureSet objects.
+One thing very cool is the function can deal with different file formats in one line of code (though it's not 
+recommended to do so, because we usually want to keep our experiment data in a more consistent way).
+
+The second statement aligns those FeatureSet objects using `merge_result`.
 The `fss` is a list of FeatureSet objects, the `["sample1", "sample2", "sample3"]` is the customizable names assigned
 to each sample.
 
 Just like the FeatureSet object, the Sample object contains the following information:
 
 ```python
 sample.mz  # m/z values of the extracted features
@@ -130,20 +161,17 @@
 from breathXplorer import retrieve_tandem
 
 tandem = retrieve_tandem("sample.mzML", fs, 0.005)
 tandem.to_mgf("ms2.mgf")
 ```
 
 The file `sample.mzML` contains tandem MS data. The `fs` object represents either a FeatureSet or a Sample, from which
-the
-m/z values are extracted. These m/z values are then used to obtain the corresponding MS/MS spectra. A tolerance
-of `0.005`
-is applied to the m/z values. Any MS/MS spectra with a difference smaller than `0.005` between the precursor m/z value
-and
-the feature's m/z value will be retrieved.
+the m/z values are extracted. These m/z values are then used to obtain the corresponding MS/MS spectra. A tolerance
+of `0.005`is applied to the m/z values. Any MS/MS spectra with a difference smaller than `0.005` between the precursor 
+m/z value and the feature's m/z value will be retrieved.
 
 ### Peak recognition
 
 The total ion current (TIC) of mass spectral data from breath analysis exhibits two key properties that preclude the use
 of existing peak detection methods but facilitate the development of specialized breath analysis algorithms:
 
 1. Breath peaks are characteristically irregular and contain a substantial number of subsidiary peaks.
```

### Comparing `breathXplorer-0.1.6/breathXplorer/cluster.py` & `breathXplorer-0.1.7/breathXplorer/cluster.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.6/breathXplorer/extract.py` & `breathXplorer-0.1.7/breathXplorer/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .file_io import cluster_ms, gen_df
 from .utils import score, time_union, interpolate_time
 
 
 # a single task
 def find_feature(ms: Union[Path, str], line: bool, quantity: float, method: str, n_peak: int = 1) -> FeatureSet:
     """
-    Calculate the feature table of a single mzML file.
+    Calculate the feature table of a single MS file (mzML or mzXML).
     :param ms:  Path of the mzML file.
     :param line:  Whether to use line mode.
     :param quantity: control the quality of peak
     :param method:  The method used to find peaks ('Topological' or 'Gaussian').
     :param n_peak:  Number of peaks to be picked
     :return:  Feature table
     """
@@ -28,15 +28,15 @@
         scores = score(scanned)
     return FeatureSet(gen_df(scanned, [('intensity', scores)]))
 
 
 # merge all the result files of single tasks in the target folder
 def merge_result(tbs: Sequence[FeatureSet], names: List[str]) -> Sample:
     """
-    Merge the feature tables of multiple mzML files.
+    Merge the feature tables of multiple MS files (mzML or mzXML).
     :param tbs:  Feature tables
     :param names:  Names of the mzML files
     :return:  Merged feature table
     """
     sub_results = [dict(zip(tb.mz, tb.intensity)) for tb in tbs]
     result = cluster_merge(sub_results)
     return Sample(pd.DataFrame(data=list(result.values()), index=list(result.keys()), columns=names))
```

### Comparing `breathXplorer-0.1.6/breathXplorer/file_io.py` & `breathXplorer-0.1.7/breathXplorer/file_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from functools import reduce
 from pathlib import Path
 from typing import Tuple, List, Union
 
 import numpy as np
 import pandas as pd
-from pyteomics import mzml
 from scipy import signal, sparse
 
 from .cluster import cluster_mz, __drop_zero_near
-from .container import FeatureSet, TandemMS
+from .container import FeatureSet, TandemMS, Source
 from .find_peak import time_with_peak
 
 
 def __purify(mz: np.ndarray, ints: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """
     Filter the m/z values and intensities by removing noise.
     :param mz: m/z values
@@ -22,78 +21,79 @@
     peaks = signal.argrelmax(ints)[0]
     peaks = peaks[ints[peaks] > ints.max() / 1000]
     return mz[peaks], ints[peaks]
 
 
 def __scan_mz(file: str, line: bool) -> np.ndarray:
     """
-    Read all m/z values at any time from an mzML file.
-    :param file: mzML file path
+    Read all m/z values at any time from an MS file (mzML or mzXML).
+    :param file: MS file (mzML or mzXML) path
     :param line: Whether the spectra are line spectra
     :return: Unique m/z values
     """
     concat_func = lambda x, y: np.concatenate([x, y])
-    with mzml.read(file) as handle:
-        all_mz = reduce(concat_func, [sp['m/z array'] for sp in handle if sp['ms level'] == 1]) if line else \
-            reduce(concat_func,
-                   [__purify(sp['m/z array'], sp['intensity array'])[0] for sp in handle if sp['ms level'] == 1])
+    source = Source(file)
+    all_mz = reduce(concat_func, [sp.mz for sp in source if sp.level == 1]) if line else \
+        reduce(concat_func, [__purify(sp.mz, sp.intensity)[0] for sp in source if sp.level == 1])
+
     return np.unique(all_mz)
 
 
 def __scan_time(file: str) -> np.ndarray:
     """
-    Read all scan times in an mzML file, usually in minutes.
-    :param file: mzML file path
+    Read all scan times in an MS file (mzML or mzXML), usually in minutes.
+    :param file: MS file (mzML or mzXML) path
     :return: Scan times
     """
-    with mzml.read(file) as handle:
-        all_time = [sp['scanList']['scan'][0]['scan start time'] for sp in handle if sp['ms level'] == 1]
+    source = Source(file)
+    all_time = [sp.scan_start_time for sp in source if sp.level == 1]
     return np.array(all_time)
 
 
 def __scan_tic(file: str) -> np.ndarray:
     """
     Get the total ion current (TIC) at each rotation time.
-    :param file: mzML file path
+    :param file: MS file (mzML or mzXML) path
     :return: TIC values
     """
-    with mzml.read(file) as handle:
-        tic = [sp['total ion current'] for sp in handle if sp['ms level'] == 1]
+    source = Source(file)
+    tic = [sp.tic for sp in source if sp.level == 1]
     return np.array(tic)
 
 
 def read_sparse(file: str, line: bool) -> pd.DataFrame:
     """
-    Read all information of an mzML file, with rows as unique m/z values and columns as time.
-    :param file: mzML file path
+    Read all information of an MS file (mzML or mzXML), with rows as unique m/z values and columns as time.
+    :param file: MS file (mzML or mzXML) path
     :param line: Whether the spectra are line spectra
     :return: Sparse DataFrame
     """
     times = __scan_time(file)
     times = pd.Series(index=times, data=np.arange(times.size))
     mzs = __scan_mz(file, line)
     mzs = pd.Series(index=mzs, data=np.arange(mzs.size))
     data = sparse.lil_matrix((times.size, mzs.size))
-    with mzml.read(file) as handle:
-        for sp in handle:
-            if sp['ms level'] == 2:
-                continue
-            mz_arr, ints_arr = (sp['m/z array'], sp['intensity array']) if line else __purify(sp['m/z array'],
-                                                                                              sp['intensity array'])
-            data[times[sp['scanList']['scan'][0]['scan start time']], mzs[mz_arr]] = ints_arr
+
+    source = Source(file)
+    for sp in source:
+        if sp.level == 2:
+            continue
+        mz_arr, ints_arr = (sp.mz, sp.intensity) if line else __purify(sp.mz, sp.intensity)
+        data[times[sp.scan_start_time], mzs[mz_arr]] = ints_arr
+
     tb = pd.DataFrame.sparse.from_spmatrix(data.transpose())
     tb.index = mzs.index
     tb.columns = times.index
     return tb
 
 
 def cluster_ms(ms: str, line: bool, dense: float, method: str, n_peak=1) -> dict:
     """
-    Find all bars in the time to m/z heatmap.:param ms: mzML file path
-    :param line: Whether the mzML file is a line spectra mzML
+    Find all bars in the time to m/z heatmap.:param ms: MS file (mzML or mzXML) path
+    :param line: Whether the MS file (mzML or mzXML) is a line spectra mzML
     :param dense: Control the quality of peak
     :param method: Peak picking method
     :param n_peak: Number of peaks
     :return: Dictionary with time, intensities, TIC, and peak time information
     """
     tb = read_sparse(ms, line)
     times = tb.columns.values
@@ -125,19 +125,17 @@
         ntb = pd.DataFrame({name: list(ndc.values())}, index=list(ndc.keys()))
         otb = pd.concat([ntb, otb], axis='columns', ignore_index=False)
     return otb
 
 
 def retrieve_tandem(file: Union[str, Path], feature: FeatureSet, radium: float) -> TandemMS:
     """
-    Retrieve tandem MS information from an zML mzML.
+    Retrieve tandem MS information from an MS file (mzML or mzXML).
 
-    :param file: mzML file path
+    :param file: MS file (mzML or mzXML) path
     :param feature: result FeatureSet
     :param radium: Radium of the feature
     :return: TandemMS object
     """
-    file = Path(file)
     tandem = TandemMS(feature.mz)
-    with mzml.read(str(file.absolute())) as handle:
-        tandem.build(handle, radium)
+    tandem.build(Source(file), radium)
     return tandem
```

### Comparing `breathXplorer-0.1.6/breathXplorer/find_peak.py` & `breathXplorer-0.1.7/breathXplorer/find_peak.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.6/breathXplorer/utils.py` & `breathXplorer-0.1.7/breathXplorer/utils.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.6/breathXplorer.egg-info/PKG-INFO` & `breathXplorer-0.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breathXplorer
-Version: 0.1.6
+Version: 0.1.7
 Summary: A toolkit for breath metabolomics analysis
 Home-page: https://github.com/wykswr/breathXplorer
 Author: wykswr
 Author-email: bifocal.above.0y@icloud.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,27 +20,28 @@
 # breathXplorer
 
 [![PyPI](https://img.shields.io/pypi/pyversions/breathXplorer)](https://pypi.org/project/breathXplorer/)
 [![Python package](https://github.com/wykswr/breathXplorer/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/wykswr/breathXplorer/actions/workflows/python-package.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <!-- TOC -->
-
 * [breathXplorer](#breathxplorer)
-    * [Introduction](#introduction)
-    * [Quick start](#quick-start)
-        * [Installation](#installation)
-        * [File format](#file-format)
-        * [Feature extraction](#feature-extraction)
-        * [Feature alignment](#feature-alignment)
-    * [Utilities](#utilities)
-        * [MS/MS spectra export](#msms-spectra-export)
-        * [Peak recognition](#peak-recognition)
-    * [Citation](#citation)
-
+  * [Introduction](#introduction)
+  * [Quick start](#quick-start)
+    * [Installation](#installation)
+    * [File format](#file-format)
+      * [Feature table CSV](#feature-table-csv)
+      * [Aligned feature table CSV](#aligned-feature-table-csv)
+      * [MS/MS spectra MGF](#msms-spectra-mgf)
+    * [Feature extraction](#feature-extraction)
+    * [Feature alignment](#feature-alignment)
+  * [Utilities](#utilities)
+    * [MS/MS spectra export](#msms-spectra-export)
+    * [Peak recognition](#peak-recognition)
+  * [Citation](#citation)
 <!-- TOC -->
 
 ## Introduction
 
 BreathXplorer is a swiss army knife for breath analysis. It provides a set of tools for breath analysis, including
 feature extraction, feature alignment, and breath recognition.
 
@@ -52,34 +53,79 @@
 It's recommended to install the package in a virtual environment or a conda environment,
 after activating the environment, run the following command to install the package:
 
 `pip install breathXplorer`
 
 ### File format
 
-The input file should be in mzML format. For the output, the single or aligned feature table can be exported as csv
-file.
+The input file should be in mzML or mzXML format (Perhaps more in the future). For the output, 
+the single or aligned feature table can be exported as csv file.
 The related MS/MS spectra can be exported in an mgf file.
 
+#### Feature table CSV
+
+|                   | intensity          | 0.0072552628 | 0.026703197   | 0.043871898 |
+|-------------------|--------------------|--------------|---------------|-------------|
+| 70.00432621552620 | 42831.928564484600 | 90863.234375 | 34955.3671875 | 0.0         |
+| 70.06507751535940 | 7697202.355213430  | 6714245.5    | 6476909.5     | 6479075.5   |
+| 70.07309580891320 | 18459.317394976800 | 0.0          | 0.0           | 0.0         |
+| 70.12570290061420 | 65085.35662117530  | 0.33127435   | 0.34847233    | 0.36571398  |
+
+The index of the table is the m/z value of the features, and the 1st column is the total intensity of the feature.
+The other columns are the intensity of the feature over time, the time is the name of the corresponding column.
+
+#### Aligned feature table CSV
+
+|                   | S01_Before        | S02_Before         | S03_Before         |
+|-------------------|-------------------|--------------------|--------------------|
+| 70.06522594212220 | 8400258.455035770 | 3229242.0293803000 | 8472742.497544320  |
+| 71.0489436673768  | 449896.521925234  | 11058.402315007400 | 413906.96622934300 |
+| 71.06833464948300 | 386030.8760258960 | 12110.036064627900 | 398033.1097357460  |
+
+The index of the table is the m/z value of the features, and each column is the total intensity of the feature in a sample (
+experiment of a subject). The name of the column is the sample name.
+
+#### MS/MS spectra MGF
+
+```
+BEGIN IONS
+PEPMASS=70.004
+MSLEVEL=2
+50.630638335563866 1466.3514404296875
+50.63166334943464 2041.7808837890625
+END IONS
+
+BEGIN IONS
+PEPMASS=70.064993720777
+MSLEVEL=2
+53.00126253392352 1509.3829345703125
+71.06273290316524 27731.6875
+71.06506220434123 870.4231567382812
+END IONS
+```
+
+The file contains the MS/MS spectra of the features, each feature has a PEPMASS (precursor mass) and MSLEVEL field, and the following
+pairs are the m/z and intensity of the MS/MS spectra.
+
 ### Feature extraction
 
 Feature extraction is used to find the volatile organic compound (VOC) in the breath sample.
-The feature extraction is performed using the `find_feature` function. The function takes the path to an mzMl file
+The feature extraction is performed using the `find_feature` function. The function takes the path to an mzMl/mzXML file
 as input, and returns an object containing the extracted feature table:
 
 ```python
 from breathXplorer import find_feature
 
 fs = find_feature("sample.mzML", False, .8, "Topological", 6)
 ```
 
 The `False` indicates that the input file is not a line spectrum, and the `.8` controls the quality of the extracted
 features, higher value means higher quality. The `"Topological"` indicates the algorithm used for feature extraction,
 the other option is `"Gaussian"`. The `6` is the prior knowledge of the number of breath in an experiment (only used
-for Gaussian algorithm).
+for Gaussian algorithm, and you don't need to impute it if using Topological).
 
 The `fs` is a FeatureSet object, it contains the following information:
 
 ```python
 fs.mz  # m/z values of the extracted features
 fs.scan_time  # scan time of the experiment
 fs.intensity  # the total intensity of each feature (calculated by integrating the intensity over scan time)
@@ -98,19 +144,23 @@
 The `merge_feature` function takes as input a list of FeatureSet objects, and returns a Sample object. It aligns the
 features with the similar m/z value from different samples, and calculate the total intensity of each feature in each
 sample. To use the function, you can do the following:
 
 ```python
 from breathXplorer import merge_result, find_feature
 
-fss = [find_feature(f, False, .8, "Gaussian", 6) for f in ["sample1.mzML", "sample2.mzML", "sample3.mzML"]]
+fss = [find_feature(f, False, .8, "Gaussian", 6) for f in ["sample1.mzML", "sample2.mzXML", "sample3.mzML"]]
 sample = merge_result(fss, ["sample1", "sample2", "sample3"])
 ```
 
-The first statement creates a list of FeatureSet objects, the second statement aligns those FeatureSet objects.
+The first statement creates a list of FeatureSet objects.
+One thing very cool is the function can deal with different file formats in one line of code (though it's not 
+recommended to do so, because we usually want to keep our experiment data in a more consistent way).
+
+The second statement aligns those FeatureSet objects using `merge_result`.
 The `fss` is a list of FeatureSet objects, the `["sample1", "sample2", "sample3"]` is the customizable names assigned
 to each sample.
 
 Just like the FeatureSet object, the Sample object contains the following information:
 
 ```python
 sample.mz  # m/z values of the extracted features
@@ -130,20 +180,17 @@
 from breathXplorer import retrieve_tandem
 
 tandem = retrieve_tandem("sample.mzML", fs, 0.005)
 tandem.to_mgf("ms2.mgf")
 ```
 
 The file `sample.mzML` contains tandem MS data. The `fs` object represents either a FeatureSet or a Sample, from which
-the
-m/z values are extracted. These m/z values are then used to obtain the corresponding MS/MS spectra. A tolerance
-of `0.005`
-is applied to the m/z values. Any MS/MS spectra with a difference smaller than `0.005` between the precursor m/z value
-and
-the feature's m/z value will be retrieved.
+the m/z values are extracted. These m/z values are then used to obtain the corresponding MS/MS spectra. A tolerance
+of `0.005`is applied to the m/z values. Any MS/MS spectra with a difference smaller than `0.005` between the precursor 
+m/z value and the feature's m/z value will be retrieved.
 
 ### Peak recognition
 
 The total ion current (TIC) of mass spectral data from breath analysis exhibits two key properties that preclude the use
 of existing peak detection methods but facilitate the development of specialized breath analysis algorithms:
 
 1. Breath peaks are characteristically irregular and contain a substantial number of subsidiary peaks.
```

### Comparing `breathXplorer-0.1.6/setup.py` & `breathXplorer-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirement.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="breathXplorer",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=required_packages,
     author="wykswr",
     author_email="bifocal.above.0y@icloud.com",
     description="A toolkit for breath metabolomics analysis",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `breathXplorer-0.1.6/tests/test_extract.py` & `breathXplorer-0.1.7/tests/test_extract.py`

 * *Files identical despite different names*

