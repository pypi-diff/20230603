# Comparing `tmp/samplics-0.4.7.tar.gz` & `tmp/samplics-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samplics-0.4.7.tar", max compression
+gzip compressed data, was "samplics-0.4.8.tar", max compression
```

## Comparing `samplics-0.4.7.tar` & `samplics-0.4.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     9504 2022-11-18 16:37:14.052836 samplics-0.4.7/README.md
--rw-r--r--   0        0        0     2055 2023-06-02 08:35:51.319620 samplics-0.4.7/pyproject.toml
--rwxr-xr-x   0        0        0     2442 2023-06-02 08:36:08.411611 samplics-0.4.7/src/samplics/__init__.py
--rw-r--r--   0        0        0      177 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/categorical/__init__.py
--rw-r--r--   0        0        0    17506 2022-11-22 17:33:15.855653 samplics-0.4.7/src/samplics/categorical/comparison.py
--rw-r--r--   0        0        0    28691 2023-02-17 13:27:25.371149 samplics-0.4.7/src/samplics/categorical/tabulation.py
--rw-r--r--   0        0        0      573 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/datasets/__init__.py
--rw-r--r--   0        0        0     2575 2021-04-19 23:27:02.000000 samplics-0.4.7/src/samplics/datasets/data/auto.csv
--rw-r--r--   0        0        0    11931 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/birth.csv
--rw-r--r--   0        0        0      951 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/countycrop.csv
--rw-r--r--   0        0        0      461 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/countycrop_means.csv
--rw-r--r--   0        0        0     1236 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/expenditure_on_milk.csv
--rw-r--r--   0        0        0   243781 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/nhanes2.csv
--rw-r--r--   0        0        0   200898 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/nhanes2brr_subset.csv
--rw-r--r--   0        0        0   318640 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/nhanes2jk_subset.csv
--rw-r--r--   0        0        0   221603 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/nmihs_subset.csv
--rw-r--r--   0        0        0     1676 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/psu_frame.csv
--rw-r--r--   0        0        0      335 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/psu_sample.csv
--rw-r--r--   0        0        0     4986 2021-04-19 19:46:20.000000 samplics-0.4.7/src/samplics/datasets/data/ssu_sample.csv
--rw-r--r--   0        0        0     5884 2022-09-17 09:54:59.584836 samplics-0.4.7/src/samplics/datasets/datasets.py
--rwxr-xr-x   0        0        0      175 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/estimation/__init__.py
--rw-r--r--   0        0        0      960 2022-11-01 16:01:56.283535 samplics-0.4.7/src/samplics/estimation/calibration.py
--rwxr-xr-x   0        0        0    39689 2022-11-22 18:36:03.306764 samplics-0.4.7/src/samplics/estimation/expansion.py
--rw-r--r--   0        0        0    20703 2022-11-22 03:17:50.704502 samplics-0.4.7/src/samplics/estimation/replication.py
--rw-r--r--   0        0        0       68 2020-05-24 01:54:43.000000 samplics-0.4.7/src/samplics/py.typed
--rw-r--r--   0        0        0       72 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/regression/__init__.py
--rw-r--r--   0        0        0     3625 2022-11-23 00:11:38.571578 samplics-0.4.7/src/samplics/regression/glm.py
--rw-r--r--   0        0        0      301 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/sae/__init__.py
--rw-r--r--   0        0        0    26914 2022-11-19 01:05:01.264773 samplics-0.4.7/src/samplics/sae/eb_unit_model.py
--rw-r--r--   0        0        0    20341 2023-05-26 18:03:02.682778 samplics-0.4.7/src/samplics/sae/eblup_area_model.py
--rw-r--r--   0        0        0    22790 2022-11-19 01:12:00.459101 samplics-0.4.7/src/samplics/sae/eblup_unit_model.py
--rw-r--r--   0        0        0    19440 2022-11-19 01:05:01.261193 samplics-0.4.7/src/samplics/sae/robust_unit_model.py
--rw-r--r--   0        0        0    13780 2022-09-17 09:54:59.587353 samplics-0.4.7/src/samplics/sae/sae_core_functions.py
--rwxr-xr-x   0        0        0      876 2022-11-20 03:10:58.335741 samplics-0.4.7/src/samplics/sampling/__init__.py
--rw-r--r--   0        0        0    12991 2022-11-19 01:13:31.225123 samplics-0.4.7/src/samplics/sampling/power_functions.py
--rw-r--r--   0        0        0    33695 2023-06-02 08:25:35.578892 samplics-0.4.7/src/samplics/sampling/selection.py
--rw-r--r--   0        0        0    34921 2023-03-17 07:43:07.886958 samplics-0.4.7/src/samplics/sampling/size.py
--rw-r--r--   0        0        0    17936 2022-11-19 01:16:07.524103 samplics-0.4.7/src/samplics/sampling/size_functions.py
--rw-r--r--   0        0        0      584 2022-11-22 19:20:12.473575 samplics-0.4.7/src/samplics/utils/__init__.py
--rw-r--r--   0        0        0     9255 2022-11-22 01:44:42.359380 samplics-0.4.7/src/samplics/utils/basic_functions.py
--rw-r--r--   0        0        0     3273 2022-11-19 01:05:01.275256 samplics-0.4.7/src/samplics/utils/checks.py
--rw-r--r--   0        0        0      472 2022-11-22 19:19:11.336637 samplics-0.4.7/src/samplics/utils/errors.py
--rw-r--r--   0        0        0     6987 2022-11-22 17:56:51.550307 samplics-0.4.7/src/samplics/utils/formats.py
--rw-r--r--   0        0        0     6813 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/utils/hadamard.py
--rw-r--r--   0        0        0     1403 2022-11-20 05:53:29.545084 samplics-0.4.7/src/samplics/utils/types.py
--rwxr-xr-x   0        0        0      161 2021-11-29 11:21:45.000000 samplics-0.4.7/src/samplics/weighting/__init__.py
--rw-r--r--   0        0        0    24814 2022-11-19 01:05:01.273917 samplics-0.4.7/src/samplics/weighting/adjustment.py
--rw-r--r--   0        0        0    13745 2022-11-19 01:05:01.277558 samplics-0.4.7/src/samplics/weighting/replicates.py
--rw-r--r--   0        0        0    10895 1970-01-01 00:00:00.000000 samplics-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     9504 2022-11-18 16:37:14.052836 samplics-0.4.8/README.md
+-rw-r--r--   0        0        0     2055 2023-06-03 08:58:20.522018 samplics-0.4.8/pyproject.toml
+-rwxr-xr-x   0        0        0     2442 2023-06-03 08:58:34.884171 samplics-0.4.8/src/samplics/__init__.py
+-rw-r--r--   0        0        0      177 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/categorical/__init__.py
+-rw-r--r--   0        0        0    17506 2022-11-22 17:33:15.855653 samplics-0.4.8/src/samplics/categorical/comparison.py
+-rw-r--r--   0        0        0    28691 2023-02-17 13:27:25.371149 samplics-0.4.8/src/samplics/categorical/tabulation.py
+-rw-r--r--   0        0        0      573 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/datasets/__init__.py
+-rw-r--r--   0        0        0     2575 2021-04-19 23:27:02.000000 samplics-0.4.8/src/samplics/datasets/data/auto.csv
+-rw-r--r--   0        0        0    11931 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/birth.csv
+-rw-r--r--   0        0        0      951 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/countycrop.csv
+-rw-r--r--   0        0        0      461 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/countycrop_means.csv
+-rw-r--r--   0        0        0     1236 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/expenditure_on_milk.csv
+-rw-r--r--   0        0        0   243781 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/nhanes2.csv
+-rw-r--r--   0        0        0   200898 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/nhanes2brr_subset.csv
+-rw-r--r--   0        0        0   318640 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/nhanes2jk_subset.csv
+-rw-r--r--   0        0        0   221603 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/nmihs_subset.csv
+-rw-r--r--   0        0        0     1676 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/psu_frame.csv
+-rw-r--r--   0        0        0      335 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/psu_sample.csv
+-rw-r--r--   0        0        0     4986 2021-04-19 19:46:20.000000 samplics-0.4.8/src/samplics/datasets/data/ssu_sample.csv
+-rw-r--r--   0        0        0     5884 2022-09-17 09:54:59.584836 samplics-0.4.8/src/samplics/datasets/datasets.py
+-rwxr-xr-x   0        0        0      175 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/estimation/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-01 16:01:56.283535 samplics-0.4.8/src/samplics/estimation/calibration.py
+-rwxr-xr-x   0        0        0    39689 2022-11-22 18:36:03.306764 samplics-0.4.8/src/samplics/estimation/expansion.py
+-rw-r--r--   0        0        0    20703 2022-11-22 03:17:50.704502 samplics-0.4.8/src/samplics/estimation/replication.py
+-rw-r--r--   0        0        0       68 2020-05-24 01:54:43.000000 samplics-0.4.8/src/samplics/py.typed
+-rw-r--r--   0        0        0       72 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/regression/__init__.py
+-rw-r--r--   0        0        0     3625 2022-11-23 00:11:38.571578 samplics-0.4.8/src/samplics/regression/glm.py
+-rw-r--r--   0        0        0      301 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/sae/__init__.py
+-rw-r--r--   0        0        0    26914 2022-11-19 01:05:01.264773 samplics-0.4.8/src/samplics/sae/eb_unit_model.py
+-rw-r--r--   0        0        0    20341 2023-05-26 18:03:02.682778 samplics-0.4.8/src/samplics/sae/eblup_area_model.py
+-rw-r--r--   0        0        0    22790 2022-11-19 01:12:00.459101 samplics-0.4.8/src/samplics/sae/eblup_unit_model.py
+-rw-r--r--   0        0        0    19440 2022-11-19 01:05:01.261193 samplics-0.4.8/src/samplics/sae/robust_unit_model.py
+-rw-r--r--   0        0        0    13780 2022-09-17 09:54:59.587353 samplics-0.4.8/src/samplics/sae/sae_core_functions.py
+-rwxr-xr-x   0        0        0      876 2022-11-20 03:10:58.335741 samplics-0.4.8/src/samplics/sampling/__init__.py
+-rw-r--r--   0        0        0    12991 2022-11-19 01:13:31.225123 samplics-0.4.8/src/samplics/sampling/power_functions.py
+-rw-r--r--   0        0        0    33763 2023-06-03 09:05:06.512644 samplics-0.4.8/src/samplics/sampling/selection.py
+-rw-r--r--   0        0        0    34921 2023-03-17 07:43:07.886958 samplics-0.4.8/src/samplics/sampling/size.py
+-rw-r--r--   0        0        0    17936 2022-11-19 01:16:07.524103 samplics-0.4.8/src/samplics/sampling/size_functions.py
+-rw-r--r--   0        0        0      584 2022-11-22 19:20:12.473575 samplics-0.4.8/src/samplics/utils/__init__.py
+-rw-r--r--   0        0        0     9255 2022-11-22 01:44:42.359380 samplics-0.4.8/src/samplics/utils/basic_functions.py
+-rw-r--r--   0        0        0     3273 2022-11-19 01:05:01.275256 samplics-0.4.8/src/samplics/utils/checks.py
+-rw-r--r--   0        0        0      472 2022-11-22 19:19:11.336637 samplics-0.4.8/src/samplics/utils/errors.py
+-rw-r--r--   0        0        0     6987 2022-11-22 17:56:51.550307 samplics-0.4.8/src/samplics/utils/formats.py
+-rw-r--r--   0        0        0     6813 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/utils/hadamard.py
+-rw-r--r--   0        0        0     1403 2022-11-20 05:53:29.545084 samplics-0.4.8/src/samplics/utils/types.py
+-rwxr-xr-x   0        0        0      161 2021-11-29 11:21:45.000000 samplics-0.4.8/src/samplics/weighting/__init__.py
+-rw-r--r--   0        0        0    24814 2022-11-19 01:05:01.273917 samplics-0.4.8/src/samplics/weighting/adjustment.py
+-rw-r--r--   0        0        0    13745 2022-11-19 01:05:01.277558 samplics-0.4.8/src/samplics/weighting/replicates.py
+-rw-r--r--   0        0        0    10693 1970-01-01 00:00:00.000000 samplics-0.4.8/PKG-INFO
```

### Comparing `samplics-0.4.7/README.md` & `samplics-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/pyproject.toml` & `samplics-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Mamadou S Diallo <msdiallo@samplics.org>"]
 description = "Select, weight and analyze complex sample data"
 license = "MIT"
 name = "samplics"
-version = "0.4.7"
+version = "0.4.8"
 
 readme = "README.md"
 
 documentation = "https://samplics-org.github.io/samplics/"
 homepage = "https://samplics-org.github.io/samplics//"
 repository = "https://github.com/survey-methods/samplics"
```

### Comparing `samplics-0.4.7/src/samplics/__init__.py` & `samplics-0.4.8/src/samplics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,8 +99,8 @@
     "CertaintyError",
     "DimensionError",
     "MethodError",
     "ProbError",
     "SinglePSUError",
 ]
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
```

### Comparing `samplics-0.4.7/src/samplics/categorical/comparison.py` & `samplics-0.4.8/src/samplics/categorical/comparison.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/categorical/tabulation.py` & `samplics-0.4.8/src/samplics/categorical/tabulation.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/__init__.py` & `samplics-0.4.8/src/samplics/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/auto.csv` & `samplics-0.4.8/src/samplics/datasets/data/auto.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/birth.csv` & `samplics-0.4.8/src/samplics/datasets/data/birth.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/countycrop.csv` & `samplics-0.4.8/src/samplics/datasets/data/countycrop.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/expenditure_on_milk.csv` & `samplics-0.4.8/src/samplics/datasets/data/expenditure_on_milk.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/nhanes2.csv` & `samplics-0.4.8/src/samplics/datasets/data/nhanes2.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/nhanes2brr_subset.csv` & `samplics-0.4.8/src/samplics/datasets/data/nhanes2brr_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/nhanes2jk_subset.csv` & `samplics-0.4.8/src/samplics/datasets/data/nhanes2jk_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/nmihs_subset.csv` & `samplics-0.4.8/src/samplics/datasets/data/nmihs_subset.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/psu_frame.csv` & `samplics-0.4.8/src/samplics/datasets/data/psu_frame.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/data/ssu_sample.csv` & `samplics-0.4.8/src/samplics/datasets/data/ssu_sample.csv`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/datasets/datasets.py` & `samplics-0.4.8/src/samplics/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/estimation/calibration.py` & `samplics-0.4.8/src/samplics/estimation/calibration.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/estimation/expansion.py` & `samplics-0.4.8/src/samplics/estimation/expansion.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/estimation/replication.py` & `samplics-0.4.8/src/samplics/estimation/replication.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/regression/glm.py` & `samplics-0.4.8/src/samplics/regression/glm.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sae/eb_unit_model.py` & `samplics-0.4.8/src/samplics/sae/eb_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sae/eblup_area_model.py` & `samplics-0.4.8/src/samplics/sae/eblup_area_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sae/eblup_unit_model.py` & `samplics-0.4.8/src/samplics/sae/eblup_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sae/robust_unit_model.py` & `samplics-0.4.8/src/samplics/sae/robust_unit_model.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sae/sae_core_functions.py` & `samplics-0.4.8/src/samplics/sae/sae_core_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sampling/__init__.py` & `samplics-0.4.8/src/samplics/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sampling/power_functions.py` & `samplics-0.4.8/src/samplics/sampling/power_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sampling/selection.py` & `samplics-0.4.8/src/samplics/sampling/selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,18 +649,18 @@
             sample, hits = self._sys_selection_method(samp_unit, samp_size_n, samp_rate_n)
 
         return sample, hits
 
     def inclusion_probs(
         self,
         samp_unit: np.ndarray,
-        samp_size: Union[DictStrInt, int],
-        stratum: np.ndarray,
-        mos: np.ndarray,
-        samp_rate: Union[DictStrFloat, float],
+        samp_size: Optional[Union[DictStrInt, int]] = None,
+        stratum: Optional[np.ndarray] = None,
+        mos: Optional[np.ndarray] = None,
+        samp_rate: Optional[Union[DictStrFloat, float]] = None,
     ) -> np.ndarray:
 
         samp_unit = sample_units(samp_unit, unique=True)
 
         samp_size_temp: Union[DictStrInt, int]
         if stratum is not None:
             stratum = numpy_array(stratum)
```

### Comparing `samplics-0.4.7/src/samplics/sampling/size.py` & `samplics-0.4.8/src/samplics/sampling/size.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/sampling/size_functions.py` & `samplics-0.4.8/src/samplics/sampling/size_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/__init__.py` & `samplics-0.4.8/src/samplics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/basic_functions.py` & `samplics-0.4.8/src/samplics/utils/basic_functions.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/checks.py` & `samplics-0.4.8/src/samplics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/formats.py` & `samplics-0.4.8/src/samplics/utils/formats.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/hadamard.py` & `samplics-0.4.8/src/samplics/utils/hadamard.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/utils/types.py` & `samplics-0.4.8/src/samplics/utils/types.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/weighting/adjustment.py` & `samplics-0.4.8/src/samplics/weighting/adjustment.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/src/samplics/weighting/replicates.py` & `samplics-0.4.8/src/samplics/weighting/replicates.py`

 * *Files identical despite different names*

### Comparing `samplics-0.4.7/PKG-INFO` & `samplics-0.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samplics
-Version: 0.4.7
+Version: 0.4.8
 Summary: Select, weight and analyze complex sample data
 Home-page: https://samplics-org.github.io/samplics//
 License: MIT
 Keywords: sampling,sample,weighting,estimation,survey
 Author: Mamadou S Diallo
 Author-email: msdiallo@samplics.org
 Requires-Python: >=3.8,<3.12
@@ -12,18 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: matplotlib (>=3.4,<4.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: statsmodels (>=0.13,<0.14)
```

