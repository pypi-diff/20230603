# Comparing `tmp/tidytcells-1.8.2.tar.gz` & `tmp/tidytcells-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.2.tar", last modified: Fri Jun  2 22:33:51 2023, max compression
+gzip compressed data, was "tidytcells-1.8.3.tar", last modified: Sat Jun  3 17:33:19 2023, max compression
```

## Comparing `tidytcells-1.8.2.tar` & `tidytcells-1.8.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.2/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.2/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-02 22:33:51.014972 tidytcells-1.8.2/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-02 21:45:08.000000 tidytcells-1.8.2/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-02 22:30:44.000000 tidytcells-1.8.2/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-02 22:33:51.014972 tidytcells-1.8.2/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-02 22:32:49.000000 tidytcells-1.8.2/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.010972 tidytcells-1.8.2/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.011972 tidytcells-1.8.2/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-02 22:22:53.000000 tidytcells-1.8.2/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4225 2023-06-02 16:09:52.000000 tidytcells-1.8.2/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    11289 2023-06-02 16:08:36.000000 tidytcells-1.8.2/src/tidytcells/_utils/gene_standardizers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-02 16:10:03.000000 tidytcells-1.8.2/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-02 16:10:51.000000 tidytcells-1.8.2/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-02 16:10:30.000000 tidytcells-1.8.2/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-02 16:11:27.000000 tidytcells-1.8.2/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-02 16:11:13.000000 tidytcells-1.8.2/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-02 16:45:57.000000 tidytcells-1.8.2/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-02 16:38:32.000000 tidytcells-1.8.2/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-02 16:06:36.000000 tidytcells-1.8.2/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-02 16:40:17.000000 tidytcells-1.8.2/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.011972 tidytcells-1.8.2/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-06-02 16:02:49.000000 tidytcells-1.8.2/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-06-02 16:02:49.000000 tidytcells-1.8.2/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-02 16:38:32.000000 tidytcells-1.8.2/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8118 2023-06-02 16:39:27.000000 tidytcells-1.8.2/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.794156 tidytcells-1.8.3/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.3/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.3/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-03 17:33:19.794156 tidytcells-1.8.3/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-03 13:18:28.000000 tidytcells-1.8.3/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-03 17:28:40.000000 tidytcells-1.8.3/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-03 17:33:19.794156 tidytcells-1.8.3/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-03 13:18:28.000000 tidytcells-1.8.3/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.788156 tidytcells-1.8.3/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.789156 tidytcells-1.8.3/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.8.3/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.791156 tidytcells-1.8.3/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.792156 tidytcells-1.8.3/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.8.3/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4092 2023-06-03 16:23:43.000000 tidytcells-1.8.3/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.8.3/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-03 17:26:54.000000 tidytcells-1.8.3/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.792156 tidytcells-1.8.3/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.790156 tidytcells-1.8.3/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.794156 tidytcells-1.8.3/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-03-11 19:32:17.000000 tidytcells-1.8.3/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-03-11 19:32:17.000000 tidytcells-1.8.3/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-03 15:14:45.000000 tidytcells-1.8.3/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8447 2023-06-03 17:26:54.000000 tidytcells-1.8.3/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.2/LICENSE.txt` & `tidytcells-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/PKG-INFO` & `tidytcells-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.2
+Version: 1.8.3
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.2/README.md` & `tidytcells-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/setup.py` & `tidytcells-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/__init__.py` & `tidytcells-1.8.3/src/tidytcells/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977689488163589%*

 * *Differences: {"'HLA-A'": "{'01': {'428': OrderedDict(), '429': OrderedDict(), '430': OrderedDict(), '431': "*

 * *            "OrderedDict()}, '02': {'1090': OrderedDict(), '1091': OrderedDict(), '1092': "*

 * *            "OrderedDict(), '1093': OrderedDict(), '1094': OrderedDict(), '1095': OrderedDict(), "*

 * *            "'1096': OrderedDict(), '1097': OrderedDict(), '1098': OrderedDict(), '1099': "*

 * *            "OrderedDict()}, '03': {'247P': OrderedDict(), '459': OrderedDict(), '460': "*

 * *            "OrderedDict()}, '11': {'403':  […]*

```diff
@@ -388,15 +388,19 @@
             "421": {},
             "422": {},
             "423": {},
             "424": {},
             "425": {},
             "426": {},
             "427": {},
+            "428": {},
+            "429": {},
             "43": {},
+            "430": {},
+            "431": {},
             "44": {},
             "45": {},
             "46": {},
             "47": {},
             "48": {},
             "49": {},
             "50": {},
@@ -586,14 +590,24 @@
             "1084": {},
             "1085": {},
             "1086": {},
             "1087": {},
             "1088": {},
             "1089": {},
             "109": {},
+            "1090": {},
+            "1091": {},
+            "1092": {},
+            "1093": {},
+            "1094": {},
+            "1095": {},
+            "1096": {},
+            "1097": {},
+            "1098": {},
+            "1099": {},
             "10P": {},
             "11": {
                 "01G": {}
             },
             "110": {},
             "111": {},
             "112": {},
@@ -1830,14 +1844,15 @@
             "241": {},
             "242": {},
             "243": {},
             "244": {},
             "245": {},
             "246": {},
             "247": {},
+            "247P": {},
             "248": {},
             "249": {},
             "25": {},
             "250": {},
             "251": {},
             "252": {},
             "253": {},
@@ -2065,15 +2080,17 @@
             "452": {},
             "453": {},
             "454": {},
             "455": {},
             "456": {},
             "457": {},
             "458": {},
+            "459": {},
             "46": {},
+            "460": {},
             "47": {},
             "48": {},
             "49": {},
             "50": {},
             "51": {},
             "51P": {},
             "52": {},
@@ -2497,15 +2514,17 @@
             "397": {},
             "398": {},
             "399": {},
             "40": {},
             "400": {},
             "401": {},
             "402": {},
-            "403": {},
+            "403": {
+                "01G": {}
+            },
             "404": {},
             "405": {},
             "406": {},
             "407": {},
             "408": {},
             "409": {},
             "41": {},
@@ -2526,25 +2545,34 @@
             "423": {},
             "424": {},
             "425": {},
             "426": {},
             "427": {},
             "428": {},
             "429": {},
-            "43": {},
+            "43": {
+                "01G": {}
+            },
             "430": {},
             "431": {},
             "432": {},
             "433": {},
             "434": {},
             "435": {},
             "436": {},
             "437": {},
             "438": {},
+            "439": {},
+            "43P": {},
             "44": {},
+            "440": {},
+            "441": {},
+            "442": {},
+            "443": {},
+            "444": {},
             "45": {},
             "46": {},
             "47": {},
             "48": {},
             "49": {},
             "50": {},
             "51": {},
@@ -2646,14 +2674,15 @@
             "124": {},
             "125": {},
             "126": {},
             "127": {},
             "128": {},
             "129": {},
             "13": {},
+            "130": {},
             "14": {},
             "14P": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
@@ -2783,24 +2812,29 @@
             "114": {},
             "115": {},
             "116": {},
             "117": {},
             "118": {},
             "119": {},
             "120": {},
-            "121": {},
+            "121": {
+                "01G": {}
+            },
+            "121P": {},
             "122": {},
             "123": {},
             "124": {},
             "125": {},
             "126": {},
             "127": {},
             "128": {},
             "129": {},
-            "13": {},
+            "13": {
+                "02G": {}
+            },
             "130": {},
             "131": {},
             "132": {},
             "133": {},
             "134": {},
             "135": {},
             "135P": {},
@@ -2971,14 +3005,15 @@
             "268": {},
             "269": {},
             "26P": {},
             "27": {},
             "270": {},
             "271": {},
             "272": {},
+            "272P": {},
             "273": {},
             "274": {},
             "275": {},
             "276": {},
             "277": {},
             "278": {},
             "279": {},
@@ -3328,15 +3363,26 @@
             "584": {},
             "585": {},
             "586": {},
             "587": {},
             "588": {},
             "589": {},
             "59": {},
+            "590": {},
+            "591": {},
+            "592": {},
+            "593": {},
+            "594": {},
+            "595": {},
+            "596": {},
+            "597": {},
+            "598": {},
+            "599": {},
             "60": {},
+            "600": {},
             "61": {},
             "62": {},
             "63": {},
             "64": {},
             "66": {},
             "67": {},
             "68": {},
@@ -3459,22 +3505,25 @@
             "77": {},
             "78": {},
             "79": {},
             "80": {},
             "81": {},
             "82": {},
             "83": {},
-            "84": {}
+            "84": {},
+            "85": {}
         },
         "26": {
             "01": {
                 "01G": {}
             },
             "01P": {},
-            "02": {},
+            "02": {
+                "01G": {}
+            },
             "02P": {},
             "03": {
                 "01G": {}
             },
             "03P": {},
             "04": {},
             "05": {},
@@ -3634,14 +3683,17 @@
             "224": {},
             "225": {},
             "226": {},
             "227": {},
             "228": {},
             "229": {},
             "23": {},
+            "230": {},
+            "231": {},
+            "232": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
@@ -3814,14 +3866,17 @@
             "167": {},
             "168": {},
             "169": {},
             "17": {},
             "170": {},
             "171": {},
             "172": {},
+            "173": {},
+            "174": {},
+            "175": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
             "23": {},
             "24": {},
@@ -4039,14 +4094,17 @@
             "200": {},
             "201": {},
             "202": {},
             "203": {},
             "204": {},
             "205": {},
             "206": {},
+            "207": {},
+            "208": {},
+            "209": {},
             "22": {},
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
@@ -4272,14 +4330,15 @@
             "214": {},
             "215": {},
             "216": {},
             "217": {},
             "218": {},
             "219": {},
             "22": {},
+            "220": {},
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
@@ -4448,14 +4507,15 @@
             "168": {},
             "169": {},
             "17": {},
             "170": {},
             "171": {},
             "172": {},
             "173": {},
+            "174": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
             "23": {},
             "24": {},
@@ -4702,15 +4762,23 @@
             "229": {},
             "23": {},
             "230": {},
             "231": {},
             "232": {},
             "233": {},
             "234": {},
+            "235": {},
+            "236": {},
+            "237": {},
+            "238": {},
+            "239": {},
             "24": {},
+            "240": {},
+            "241": {},
+            "242": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
             "31": {},
@@ -4816,15 +4884,16 @@
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
-            "30": {}
+            "30": {},
+            "31": {}
         },
         "36": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -5163,15 +5232,17 @@
             "292": {},
             "293": {},
             "294": {},
             "295": {},
             "296": {},
             "297": {},
             "298": {},
+            "299": {},
             "30": {},
+            "300": {},
             "31": {},
             "32": {},
             "33": {},
             "34": {},
             "35": {
                 "01G": {}
             },
@@ -5785,14 +5856,18 @@
             "469": {},
             "47": {},
             "470": {},
             "471": {},
             "472": {},
             "473": {},
             "474": {},
+            "475": {},
+            "476": {},
+            "477": {},
+            "478": {},
             "48": {},
             "49": {},
             "50": {},
             "51": {},
             "52": {},
             "53": {},
             "54": {},
@@ -6091,14 +6166,16 @@
             "300": {},
             "301": {},
             "302": {},
             "303": {},
             "304": {},
             "305": {},
             "306": {},
+            "307": {},
+            "308": {},
             "31": {},
             "32": {},
             "33": {},
             "34": {},
             "35": {},
             "36": {},
             "37": {},
@@ -6270,14 +6347,17 @@
             "170": {},
             "171": {},
             "172": {},
             "173": {},
             "174": {},
             "175": {},
             "176": {},
+            "177": {},
+            "178": {},
+            "179": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
             "22P": {},
             "23": {},
@@ -6391,14 +6471,17 @@
             "110": {},
             "111": {},
             "112": {},
             "113": {},
             "114": {},
             "115": {},
             "116": {},
+            "117": {},
+            "118": {},
+            "119": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
@@ -7206,15 +7289,28 @@
             "648": {},
             "649": {},
             "64P": {},
             "65": {},
             "650": {},
             "651": {},
             "652": {},
+            "653": {},
+            "654": {},
+            "655": {},
+            "656": {},
+            "657": {},
+            "658": {},
+            "659": {},
             "66": {},
+            "660": {},
+            "661": {},
+            "662": {},
+            "663": {},
+            "664": {},
+            "665": {},
             "67": {},
             "68": {},
             "69": {},
             "70": {},
             "71": {},
             "72": {},
             "73": {
@@ -7427,15 +7523,20 @@
             "220": {},
             "221": {},
             "222": {},
             "223": {},
             "224": {},
             "225": {},
             "226": {},
+            "227": {},
+            "228": {},
+            "229": {},
             "23": {},
+            "230": {},
+            "231": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
@@ -8410,14 +8511,17 @@
             "57": {},
             "570": {},
             "571": {},
             "572": {},
             "573": {},
             "574": {},
             "575": {},
+            "576": {},
+            "577": {},
+            "578": {},
             "58": {},
             "59": {},
             "59P": {},
             "60": {},
             "61": {},
             "61P": {},
             "62": {},
@@ -8595,14 +8699,17 @@
             "09": {},
             "10": {},
             "100": {},
             "101": {},
             "102": {},
             "103": {},
             "104": {},
+            "105": {},
+            "106": {},
+            "107": {},
             "11": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "160": {},
@@ -8848,14 +8955,15 @@
             "189": {},
             "19": {},
             "190": {},
             "191": {},
             "192": {},
             "193": {},
             "194": {},
+            "195": {},
             "19P": {},
             "20": {},
             "22": {},
             "23": {},
             "24": {},
             "24P": {},
             "25": {},
@@ -9482,15 +9590,25 @@
             "522": {},
             "523": {},
             "524": {},
             "525": {},
             "526": {},
             "527": {},
             "528": {},
+            "529": {},
             "53": {},
+            "530": {},
+            "531": {},
+            "532": {},
+            "533": {},
+            "534": {},
+            "535": {},
+            "536": {},
+            "537": {},
+            "538": {},
             "54": {},
             "55": {},
             "56": {},
             "57": {},
             "58": {},
             "59": {},
             "60": {},
@@ -9622,15 +9740,17 @@
             "72": {},
             "73": {},
             "74": {},
             "75": {},
             "76": {},
             "77": {},
             "78": {},
-            "79": {}
+            "79": {},
+            "80": {},
+            "81": {}
         },
         "42": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {
@@ -9664,15 +9784,16 @@
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
             "31": {},
             "32": {},
-            "33": {}
+            "33": {},
+            "34": {}
         },
         "44": {
             "02": {
                 "01G": {}
             },
             "02P": {},
             "03": {
@@ -10003,15 +10124,23 @@
             "36": {},
             "360": {},
             "361": {},
             "362": {},
             "363": {},
             "364": {},
             "365": {},
+            "366": {},
+            "367": {},
+            "368": {},
+            "369": {},
             "37": {},
+            "370": {},
+            "371": {},
+            "372": {},
+            "373": {},
             "37P": {},
             "38": {},
             "39": {},
             "40": {},
             "41": {},
             "41P": {},
             "42": {},
@@ -10065,22 +10194,24 @@
             "476": {},
             "477": {},
             "478": {},
             "479": {},
             "48": {},
             "480": {},
             "481": {},
+            "481P": {},
             "482": {},
             "483": {},
             "484": {},
             "485": {},
             "486": {},
             "487": {},
             "488": {},
             "489": {},
+            "48P": {},
             "49": {},
             "490": {},
             "491": {},
             "492": {},
             "493": {},
             "494": {},
             "495": {},
@@ -10502,15 +10633,17 @@
             "71": {},
             "72": {},
             "73": {},
             "74": {},
             "75": {},
             "76": {},
             "77": {},
-            "78": {}
+            "78": {},
+            "79": {},
+            "80": {}
         },
         "50": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {
@@ -10931,15 +11064,19 @@
             "371": {},
             "372": {},
             "373": {},
             "374": {},
             "375": {},
             "376": {},
             "377": {},
+            "378": {},
+            "379": {},
             "38": {},
+            "380": {},
+            "381": {},
             "39": {},
             "40": {},
             "40P": {},
             "41": {},
             "42": {
                 "01G": {}
             },
@@ -11034,14 +11171,16 @@
             "107": {},
             "108": {},
             "109": {},
             "10P": {},
             "11": {},
             "110": {},
             "111": {},
+            "112": {},
+            "113": {},
             "11P": {},
             "12": {},
             "13": {},
             "14": {},
             "14P": {},
             "15": {},
             "16": {},
@@ -11313,15 +11452,14 @@
             "128": {},
             "129": {},
             "13": {},
             "130": {},
             "131": {},
             "132": {},
             "133": {},
-            "134": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
@@ -11504,15 +11642,17 @@
             "84": {},
             "85": {},
             "86": {},
             "87": {},
             "88": {},
             "89": {},
             "90": {},
-            "91": {}
+            "91": {},
+            "92": {},
+            "93": {}
         },
         "57": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {
@@ -11600,14 +11740,16 @@
             "16": {},
             "160": {},
             "161": {},
             "162": {},
             "163": {},
             "164": {},
             "165": {},
+            "166": {},
+            "167": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
             "23": {},
@@ -11748,14 +11890,17 @@
             "135": {},
             "136": {},
             "137": {},
             "138": {},
             "139": {},
             "14": {},
             "140": {},
+            "141": {},
+            "142": {},
+            "143": {},
             "15": {},
             "16": {},
             "16P": {},
             "17": {},
             "18": {},
             "19": {
                 "01G": {}
@@ -12113,14 +12258,15 @@
             "241": {},
             "242": {},
             "243": {},
             "244": {},
             "245": {},
             "246": {},
             "247": {},
+            "248": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
             "31": {},
@@ -12353,15 +12499,18 @@
             "211": {},
             "212": {},
             "213": {},
             "214": {},
             "215": {},
             "216": {},
             "217": {},
+            "218": {},
+            "219": {},
             "22": {},
+            "220": {},
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "26P": {},
             "27": {},
             "27P": {},
@@ -13093,15 +13242,24 @@
             "621": {},
             "622": {},
             "623": {},
             "624": {},
             "625": {},
             "626": {},
             "627": {},
+            "628": {},
+            "629": {},
             "63": {},
+            "630": {},
+            "631": {},
+            "632": {},
+            "633": {},
+            "634": {},
+            "635": {},
+            "636": {},
             "64": {},
             "64P": {},
             "65": {},
             "66": {},
             "67": {},
             "68": {},
             "69": {},
@@ -13131,14 +13289,15 @@
             "91": {},
             "91P": {},
             "92": {},
             "93": {},
             "94": {},
             "95": {},
             "96": {},
+            "96P": {},
             "97": {},
             "98": {}
         },
         "04": {
             "01": {
                 "01G": {},
                 "76G": {}
@@ -13619,15 +13778,26 @@
             "489": {},
             "49": {},
             "490": {},
             "491": {},
             "492": {},
             "493": {},
             "494": {},
+            "495": {},
+            "496": {},
+            "497": {},
+            "498": {},
+            "499": {},
             "50": {},
+            "500": {},
+            "501": {
+                "01G": {}
+            },
+            "501P": {},
+            "502": {},
             "51": {},
             "52": {},
             "53": {},
             "54": {},
             "54P": {},
             "55": {},
             "56": {},
@@ -13903,15 +14073,19 @@
             "271": {},
             "272": {},
             "273": {},
             "274": {},
             "275": {},
             "276": {},
             "277": {},
+            "278": {},
+            "279": {},
             "28": {},
+            "280": {},
+            "281": {},
             "29": {},
             "29P": {},
             "30": {},
             "31": {},
             "32": {},
             "33": {},
             "34": {},
@@ -14265,14 +14439,15 @@
             "317": {},
             "318": {},
             "319": {},
             "32": {},
             "320": {},
             "321": {},
             "322": {},
+            "322P": {},
             "323": {},
             "324": {},
             "325": {},
             "326": {},
             "327": {},
             "328": {},
             "329": {},
@@ -14313,14 +14488,15 @@
             "357": {},
             "358": {},
             "359": {},
             "36": {},
             "360": {},
             "361": {},
             "362": {},
+            "363": {},
             "37": {},
             "38": {},
             "39": {},
             "40": {},
             "41": {},
             "42": {},
             "42P": {},
@@ -14473,15 +14649,26 @@
             "1049": {},
             "105": {},
             "1050": {},
             "1051": {},
             "1052": {},
             "1053": {},
             "1054": {},
+            "1055": {},
+            "1056": {},
+            "1057": {},
+            "1058": {},
+            "1059": {},
             "106": {},
+            "1060": {},
+            "1061": {},
+            "1062": {},
+            "1063": {},
+            "1064": {},
+            "1065": {},
             "107": {},
             "108": {},
             "108P": {},
             "109": {},
             "109P": {},
             "11": {},
             "110": {},
@@ -15720,14 +15907,15 @@
             "201": {},
             "202": {},
             "203": {},
             "204": {},
             "205": {},
             "206": {},
             "207": {},
+            "207P": {},
             "208": {},
             "209": {},
             "21": {},
             "210": {},
             "211": {},
             "212": {},
             "213": {},
@@ -15780,14 +15968,17 @@
             "256": {},
             "257": {},
             "258": {},
             "259": {},
             "26": {},
             "260": {},
             "261": {},
+            "262": {},
+            "263": {},
+            "264": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
             "31": {},
             "32": {},
             "33": {},
@@ -16191,15 +16382,23 @@
             "370": {},
             "371": {},
             "372": {},
             "373": {},
             "374": {},
             "375": {},
             "376": {},
+            "377": {},
+            "378": {},
+            "379": {},
             "38": {},
+            "380": {},
+            "381": {},
+            "382": {},
+            "383": {},
+            "384": {},
             "39": {},
             "40": {},
             "41": {},
             "42": {},
             "43": {},
             "44": {},
             "45": {},
@@ -16329,14 +16528,15 @@
             "145": {},
             "146": {},
             "147": {},
             "148": {},
             "149": {},
             "15": {},
             "150": {},
+            "151": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
@@ -16430,15 +16630,16 @@
             "02P": {},
             "03": {},
             "04": {
                 "01G": {}
             },
             "04P": {},
             "05": {
-                "01G": {}
+                "01G": {},
+                "20G": {}
             },
             "05P": {},
             "06": {
                 "01G": {}
             },
             "06P": {},
             "07": {
@@ -16623,14 +16824,16 @@
             "25": {},
             "250": {},
             "251": {},
             "252": {},
             "253": {},
             "254": {},
             "255": {},
+            "256": {},
+            "257": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
             "31": {},
             "32": {},
@@ -16835,14 +17038,16 @@
             "198": {},
             "20": {},
             "200": {},
             "201": {},
             "202": {},
             "203": {},
             "204": {},
+            "205": {},
+            "206": {},
             "21": {},
             "22": {},
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
@@ -16991,15 +17196,17 @@
             "62": {},
             "63": {},
             "64": {},
             "65": {},
             "66": {},
             "67": {},
             "68": {},
-            "69": {}
+            "69": {},
+            "70": {},
+            "71": {}
         },
         "18": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -17014,15 +17221,16 @@
             "11": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
-            "18": {}
+            "18": {},
+            "19": {}
         }
     },
     "HLA-DMA": {
         "01": {
             "01": {
                 "01G": {}
             },
@@ -17109,15 +17317,17 @@
     },
     "HLA-DPA1": {
         "01": {
             "03": {
                 "01G": {}
             },
             "03P": {},
-            "04": {},
+            "04": {
+                "01G": {}
+            },
             "04P": {},
             "05": {
                 "01G": {}
             },
             "05P": {},
             "06": {},
             "06P": {},
@@ -17136,15 +17346,17 @@
             "108": {},
             "109": {},
             "11": {},
             "110": {},
             "111": {},
             "112": {},
             "113": {},
-            "114": {},
+            "114": {
+                "01G": {}
+            },
             "115": {},
             "116": {},
             "117": {},
             "118": {},
             "119": {},
             "11P": {},
             "12": {},
@@ -17174,15 +17386,25 @@
             "140": {},
             "141": {},
             "142": {},
             "143": {},
             "144": {},
             "145": {},
             "146": {},
+            "147": {},
+            "148": {},
+            "149": {},
             "15": {},
+            "150": {},
+            "151": {},
+            "152": {},
+            "153": {},
+            "154": {},
+            "155": {},
+            "156": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
@@ -17292,25 +17514,31 @@
             "10": {},
             "100": {},
             "101": {},
             "102": {},
             "103": {},
             "104": {},
             "105": {},
+            "106": {},
+            "107": {},
+            "108": {},
+            "109": {},
             "11": {},
+            "110": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {
+                "01G": {},
                 "03G": {}
             },
             "21P": {},
             "22": {},
             "22P": {},
             "23": {},
             "24": {},
@@ -17417,15 +17645,16 @@
             "08": {},
             "09": {},
             "10": {},
             "11": {},
             "12": {},
             "13": {},
             "14": {},
-            "15": {}
+            "15": {},
+            "16": {}
         },
         "04": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -17503,15 +17732,18 @@
         "10": {
             "01": {
                 "01G": {}
             },
             "01P": {}
         },
         "100": {
-            "01": {}
+            "01": {
+                "01G": {}
+            },
+            "01P": {}
         },
         "1000": {
             "01": {}
         },
         "1001": {
             "01": {}
         },
@@ -19038,23 +19270,110 @@
         },
         "1453": {
             "01": {}
         },
         "1454": {
             "01": {}
         },
+        "1455": {
+            "01": {}
+        },
+        "1456": {
+            "01": {}
+        },
+        "1457": {
+            "01": {}
+        },
+        "1458": {
+            "01": {}
+        },
+        "1459": {
+            "01": {}
+        },
         "146": {
             "01": {}
         },
+        "1460": {
+            "01": {}
+        },
+        "1461": {
+            "01": {}
+        },
+        "1462": {
+            "01": {}
+        },
+        "1463": {
+            "01": {}
+        },
+        "1464": {
+            "01": {}
+        },
+        "1465": {
+            "01": {}
+        },
+        "1466": {
+            "01": {}
+        },
+        "1467": {
+            "01": {}
+        },
+        "1468": {
+            "01": {}
+        },
+        "1469": {
+            "01": {}
+        },
         "147": {
             "01": {}
         },
+        "1470": {
+            "01": {}
+        },
+        "1471": {
+            "01": {}
+        },
+        "1472": {
+            "01": {}
+        },
+        "1473": {
+            "01": {}
+        },
+        "1474": {
+            "01": {}
+        },
+        "1475": {
+            "01": {}
+        },
+        "1476": {
+            "01": {}
+        },
+        "1477": {
+            "01": {}
+        },
+        "1478": {
+            "01": {}
+        },
+        "1479": {
+            "01": {}
+        },
         "148": {
             "01": {}
         },
+        "1480": {
+            "01": {}
+        },
+        "1481": {
+            "01": {}
+        },
+        "1482": {
+            "01": {}
+        },
+        "1483": {
+            "01": {}
+        },
         "149": {
             "01": {}
         },
         "15": {
             "01": {
                 "01G": {}
             },
@@ -19424,15 +19743,18 @@
         "248": {
             "01": {}
         },
         "249": {
             "01": {}
         },
         "25": {
-            "01": {}
+            "01": {
+                "01G": {}
+            },
+            "01P": {}
         },
         "250": {
             "01": {}
         },
         "251": {
             "01": {}
         },
@@ -22040,14 +22362,19 @@
             "106": {},
             "107": {},
             "108": {},
             "109": {},
             "11": {},
             "110": {},
             "111": {},
+            "112": {},
+            "113": {},
+            "114": {},
+            "115": {},
+            "116": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
@@ -22162,15 +22489,17 @@
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
             "29": {},
             "30": {},
-            "31": {}
+            "31": {},
+            "32": {},
+            "33": {}
         },
         "03": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -22211,15 +22540,19 @@
             "37": {},
             "38": {},
             "39": {},
             "40": {},
             "41": {},
             "42": {},
             "43": {},
-            "44": {}
+            "44": {},
+            "45": {},
+            "46": {},
+            "47": {},
+            "48": {}
         },
         "04": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -22315,15 +22648,19 @@
             "67": {},
             "68": {},
             "69": {},
             "70": {},
             "71": {},
             "72": {},
             "73": {},
-            "74": {}
+            "74": {},
+            "75": {},
+            "76": {},
+            "77": {},
+            "78": {}
         },
         "06": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -22345,15 +22682,16 @@
             "10": {},
             "11": {}
         }
     },
     "HLA-DQB1": {
         "02": {
             "01": {
-                "01G": {}
+                "01G": {},
+                "38G": {}
             },
             "01P": {},
             "02": {},
             "03": {},
             "03P": {},
             "04": {},
             "05": {},
@@ -22490,14 +22828,15 @@
             "206": {},
             "207": {},
             "208": {},
             "209": {},
             "21": {},
             "210": {},
             "211": {},
+            "212": {},
             "22": {},
             "23": {},
             "24": {},
             "25": {},
             "26": {},
             "27": {},
             "28": {},
@@ -22917,15 +23256,17 @@
             "373": {},
             "374": {},
             "375": {},
             "376": {},
             "377": {},
             "378": {},
             "379": {},
-            "38": {},
+            "38": {
+                "01G": {}
+            },
             "380": {},
             "381": {},
             "382": {},
             "383": {},
             "384": {},
             "385": {},
             "386": {},
@@ -23063,14 +23404,15 @@
             "504": {},
             "505": {},
             "506": {},
             "507": {},
             "508": {},
             "509": {},
             "51": {},
+            "510": {},
             "52": {},
             "53": {},
             "54": {},
             "55": {},
             "56": {},
             "57": {},
             "58": {},
@@ -23215,15 +23557,16 @@
             "88": {},
             "89": {},
             "90": {},
             "91": {},
             "92": {},
             "93": {},
             "94": {},
-            "95": {}
+            "95": {},
+            "96": {}
         },
         "05": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {
@@ -23484,15 +23827,18 @@
             "312": {},
             "313": {},
             "314": {},
             "315": {},
             "316": {},
             "317": {},
             "318": {},
+            "319": {},
             "32": {},
+            "320": {},
+            "321": {},
             "33": {},
             "34": {},
             "35": {},
             "36": {},
             "37": {},
             "38": {},
             "39": {},
@@ -24011,16 +24357,21 @@
             "460": {},
             "461": {},
             "462": {},
             "463": {},
             "464": {},
             "465": {},
             "466": {},
+            "467": {},
+            "468": {},
+            "469": {},
             "46P": {},
             "47": {},
+            "470": {},
+            "471": {},
             "48": {},
             "48P": {},
             "49": {},
             "50": {},
             "51": {},
             "51P": {},
             "52": {},
@@ -24087,15 +24438,17 @@
             "01": {},
             "02": {},
             "03": {},
             "04": {},
             "05": {},
             "06": {},
             "07": {},
-            "08": {}
+            "08": {},
+            "09": {},
+            "10": {}
         }
     },
     "HLA-DRA": {
         "01": {
             "01": {
                 "01G": {}
             },
@@ -24170,14 +24523,16 @@
             "136": {},
             "137": {},
             "138": {},
             "139": {},
             "14": {},
             "140": {},
             "141": {},
+            "142": {},
+            "143": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "18P": {},
             "19": {},
             "20": {},
@@ -24407,14 +24762,16 @@
             "20": {},
             "200": {},
             "201": {},
             "202": {},
             "203": {},
             "204": {},
             "205": {},
+            "206": {},
+            "207": {},
             "21": {},
             "22": {},
             "23": {},
             "24": {},
             "25": {},
             "25P": {},
             "26": {},
@@ -24829,14 +25186,18 @@
             "356": {},
             "357": {},
             "358": {},
             "359": {},
             "36": {},
             "360": {},
             "361": {},
+            "362": {},
+            "363": {},
+            "364": {},
+            "365": {},
             "37": {},
             "38": {
                 "01G": {}
             },
             "38P": {},
             "39": {},
             "40": {},
@@ -24968,14 +25329,17 @@
             "140": {},
             "141": {},
             "142": {},
             "143": {},
             "144": {},
             "145": {},
             "146": {},
+            "147": {},
+            "148": {},
+            "149": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
@@ -25106,14 +25470,15 @@
             "115": {},
             "116": {},
             "117": {},
             "118": {},
             "119": {},
             "11P": {},
             "12": {},
+            "120": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
@@ -25255,15 +25620,16 @@
             "45": {},
             "46": {},
             "47": {},
             "48": {},
             "49": {},
             "50": {},
             "51": {},
-            "52": {}
+            "52": {},
+            "53": {}
         },
         "10": {
             "01": {
                 "01G": {}
             },
             "01P": {},
             "02": {},
@@ -25305,15 +25671,16 @@
             "38": {},
             "39": {},
             "40": {},
             "41": {},
             "42": {},
             "43": {},
             "44": {},
-            "45": {}
+            "45": {},
+            "46": {}
         },
         "11": {
             "01": {
                 "01G": {},
                 "02G": {}
             },
             "01P": {},
@@ -25610,14 +25977,18 @@
             "307": {},
             "308": {},
             "309": {},
             "31": {},
             "310": {},
             "311": {},
             "312": {},
+            "313": {},
+            "314": {},
+            "315": {},
+            "316": {},
             "32": {},
             "33": {},
             "34": {},
             "35": {},
             "36": {},
             "37": {},
             "37P": {},
@@ -26124,14 +26495,18 @@
             "33": {},
             "330": {},
             "331": {},
             "332": {},
             "333": {},
             "334": {},
             "335": {},
+            "336": {},
+            "337": {},
+            "338": {},
+            "339": {},
             "33P": {},
             "34": {},
             "35": {},
             "36": {},
             "37": {},
             "38": {},
             "39": {},
@@ -26419,14 +26794,16 @@
             "249": {},
             "24P": {},
             "25": {
                 "01G": {}
             },
             "250": {},
             "251": {},
+            "252": {},
+            "253": {},
             "25P": {},
             "26": {},
             "27": {},
             "27P": {},
             "28": {},
             "29": {},
             "30": {},
@@ -26551,14 +26928,15 @@
             "112": {},
             "113": {},
             "114": {},
             "115": {},
             "116": {},
             "117": {},
             "118": {},
+            "118P": {},
             "119": {},
             "11P": {},
             "12": {},
             "120": {},
             "121": {},
             "122": {},
             "123": {},
@@ -26867,14 +27245,16 @@
             "107": {},
             "108": {},
             "109": {},
             "11": {},
             "110": {},
             "111": {},
             "112": {},
+            "113": {},
+            "114": {},
             "12": {},
             "13": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
@@ -27077,14 +27457,15 @@
             "185": {},
             "186": {},
             "187": {},
             "188": {},
             "189": {},
             "19": {},
             "190": {},
+            "191": {},
             "20": {},
             "21": {},
             "22": {},
             "22P": {},
             "23": {},
             "24": {},
             "25": {},
@@ -27228,15 +27609,16 @@
             "54": {},
             "55": {},
             "56": {},
             "57": {},
             "58": {},
             "59": {},
             "60": {},
-            "61": {}
+            "61": {},
+            "62": {}
         }
     },
     "HLA-DRB4": {
         "01": {
             "01": {
                 "01G": {}
             },
@@ -27321,15 +27703,20 @@
             "161": {},
             "162": {},
             "163": {},
             "164": {},
             "165": {},
             "166": {},
             "167": {},
+            "168": {},
+            "169": {},
             "17": {},
+            "170": {},
+            "171": {},
+            "172": {},
             "18": {},
             "19": {},
             "20": {},
             "21": {},
             "22": {},
             "23": {},
             "24": {},
@@ -27470,14 +27857,16 @@
             "125": {},
             "126": {},
             "127": {},
             "128": {},
             "129": {},
             "13": {},
             "130": {},
+            "131": {},
+            "132": {},
             "14": {},
             "15": {},
             "16": {},
             "17": {},
             "18": {},
             "19": {},
             "20": {},
```

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.3/src/tidytcells/_utils/abstract_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,28 +41,22 @@
     species = "".join(species.split()).lower()
 
     if not species in standardizer_dict:
         if not suppress_warnings:
             warn_unsupported_species(species, gene_type)
         return gene
 
-    original_input = gene
-
-    gene = "".join(gene.split())
-    gene = gene.replace("&nbsp;", "")
-    gene = gene.upper()
-
     standardized = standardizer_dict[species](gene)
 
     invalid_reason = standardized.invalid(enforce_functional)
     if invalid_reason:
         if not suppress_warnings:
             warn_failure(
                 reason_for_failure=invalid_reason,
-                original_input=original_input,
+                original_input=gene,
                 attempted_fix=standardized.compile("allele"),
                 species=species,
             )
         return None
 
     return standardized.compile(precision)
```

### Comparing `tidytcells-1.8.2/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.3/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/_utils/gene_standardizers.py` & `tidytcells-1.8.3/src/tidytcells/_utils/gene_standardizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 
 
 class GeneStandardizer(ABC):
     """
     Abstract base standardizer class.
     """
 
-    @abstractmethod
     def __init__(self, gene: str) -> None:
         """
-        Init method for the standardizer objects. Should expect a whitespace-
-        cleaned, uppercased string to be supplied to the 'gene' parameter.
+        Init method for the standardizer objects.
         """
+        gene = "".join(gene.split())
+        gene = gene.replace("&nbsp;", "")
+        gene = gene.replace("&ndash;", "-")
+        gene = gene.upper()
+
+        self.gene = gene
 
     def valid(self, enforce_functional: bool = False) -> bool:
         """
         Taking into account whether enforcing functionality or not, returns
         True if the gene/allele is valid in its current state. Returns False
         otherwise.
         """
@@ -62,67 +66,99 @@
     TCR standardizer base class.
     """
 
     ref_dict = None
     syn_dict = None
 
     def __init__(self, gene: str) -> None:
-        self.parse_gene_str(gene)
+        super().__init__(gene)
+        self.parse_gene_str()
         self.resolve_errors()
 
-    def parse_gene_str(self, gene: str) -> None:
-        parse_attempt = re.match(r"^([A-Z0-9\-\.\(\)\/]+)(\*(\d+))?", gene)
+    def parse_gene_str(self) -> None:
+        parse_attempt = re.match(r"^([A-Z0-9\-\.\(\)\/]+)(\*(\d+))?", self.gene)
 
         if parse_attempt:
             self.gene = parse_attempt.group(1)
             self.allele_designation = (
                 None
                 if parse_attempt.group(3) is None
                 else f"{int(parse_attempt.group(3)):02}"
             )
             return
 
-        self.gene = gene
         self.allele_designation = None
 
-    def resolve_errors(self) -> None:
+    def resolve_errors(self, try_dash1: bool = True) -> None:
         if self.valid():
             return  # No resolution necessary
 
         # If a synonym, correct to currently approved name
         if self.syn_dict and self.gene in self.syn_dict:
             self.gene = self.syn_dict[self.gene]
             return
 
         # Fix common errors
+        self.gene = self.gene.replace("TCR", "TR")
+        self.gene = self.gene.replace("S", "-")
+        self.gene = self.gene.replace(".", "-")
         self.gene = re.sub(r"(?<!TR)(?<!\/)DV", "/DV", self.gene)
         self.gene = re.sub(r"(?<!\d)0", "", self.gene)
-        self.gene = self.gene.replace("TCR", "TR")
         if self.valid():
             return
 
         # Make sure gene starts with 'TR'
         if not self.gene.startswith("TR"):
             self.gene = "TR" + self.gene
             if self.valid():
                 return
 
         # Resolve DV designation from AV if necessary
         if self.gene.startswith("TRAV") and "DV" not in self.gene:
-            for valid_gene in self.ref_dict:
-                if valid_gene.startswith(self.gene + "/DV"):
-                    self.gene = valid_gene
+            if "/" in self.gene:
+                split_gene = self.gene.split("/")
+                dv = "DV" + split_gene.pop()
+                self.gene = "/".join([*split_gene, dv])
+                if self.valid():
                     return
+            else:
+                for valid_gene in self.ref_dict:
+                    if valid_gene.startswith(self.gene + "/DV"):
+                        self.gene = valid_gene
+                        return
 
         # Resolve AV designation from DV is necessary
-        if self.gene.startswith("TRDV"):
-            for valid_gene in self.ref_dict:
-                if re.match(rf"^TRAV\d+(-\d)?\/{self.gene[2:]}$", valid_gene):
-                    self.gene = valid_gene
+        if "DV" in self.gene:
+            if self.gene.startswith("TRDV"):
+                for valid_gene in self.ref_dict:
+                    if re.match(rf"^TRAV\d+(-\d)?\/{self.gene[2:]}$", valid_gene):
+                        self.gene = valid_gene
+                        return
+            else:
+                parse_attempt = re.match(r"^TR([\d-]+)\/(DV[\d-]+)$", self.gene)
+                if parse_attempt:
+                    self.gene = f"TRAV{parse_attempt.group(1)}/{parse_attempt.group(2)}"
+                    if self.valid():
+                        return
+
+        # Try adding or removing "-1" to the end of the gene name
+        if try_dash1:
+            if "-1" in self.gene:
+                orig = self.gene
+                self.gene = self.gene.replace("-1", "")
+                self.resolve_errors(try_dash1=False)
+                if self.valid():
+                    return
+                self.gene = orig
+            else:
+                self.gene += "-1"
+                self.resolve_errors(try_dash1=False)
+                if self.valid():
                     return
+                self.gene = self.gene.replace("-1", "")
 
     def invalid(self, enforce_functional: bool = False) -> bool:
         if not self.gene in self.ref_dict:
             return "unrecognised gene name"
 
         if self.allele_designation:
             allele_valid = self.allele_designation in self.ref_dict[self.gene]
@@ -150,38 +186,38 @@
         return self.gene
 
 
 class HomoSapiensTCRStandardizer(TCRStandardizer):
     ref_dict = HOMOSAPIENS_TCR
     syn_dict = HOMOSAPIENS_TCR_SYNONYMS
 
-    def resolve_errors(self) -> None:
-        super().resolve_errors()
-
+    def resolve_errors(self, *args, **kwargs) -> None:
         # Fix common errors
         self.gene = re.sub(r"(?<!\/)OR", "/OR", self.gene)
+        super().resolve_errors(*args, **kwargs)
 
 
 class MusMusculusTCRStandardizer(TCRStandardizer):
     ref_dict = MUSMUSCULUS_TCR
 
 
 class HLAStandardizer(GeneStandardizer):
     def __init__(self, gene: str) -> None:
-        self.parse_gene(gene)
+        super().__init__(gene)
+        self.parse_gene()
         self.resolve_errors()
 
-    def parse_gene(self, gene: str) -> None:
-        if gene == "B2M":
+    def parse_gene(self) -> None:
+        if self.gene == "B2M":
             self.gene = "B2M"
             self.allele_designation = []
             return
 
         # If period between digits, replace with colon
-        gene = re.sub(r"(?<=\d)\.(?=\d)", ":", gene)
+        gene = re.sub(r"(?<=\d)\.(?=\d)", ":", self.gene)
 
         def listify_allele_designation(allele_designation) -> list:
             if allele_designation is None:
                 return []
 
             return [
                 f"{int(d):02}" if d.isdigit() else d
@@ -308,30 +344,30 @@
                 return f'{self.gene}*{":".join(self.allele_designation[:2])}'
 
         return self.gene
 
 
 class MusMusculusMHCStandardizer(GeneStandardizer):
     def __init__(self, gene: str) -> None:
-        self.parse_gene(gene)
+        super().__init__(gene)
+        self.parse_gene()
         self.resolve_errors()
 
-    def parse_gene(self, gene: str) -> None:
-        parse_attempt = re.match(r"^([A-Z0-9\-\.\(\)\/]+)(\*(\d+))?", gene)
+    def parse_gene(self) -> None:
+        parse_attempt = re.match(r"^([A-Z0-9\-\.\(\)\/]+)(\*(\d+))?", self.gene)
 
         if parse_attempt:
             self.gene = parse_attempt.group(1)
             self.allele_designation = (
                 None
                 if parse_attempt.group(3) is None
                 else f"{int(parse_attempt.group(3)):02}"
             )
             return
 
-        self.gene = gene
         self.allele_designation = None
 
     def resolve_errors(self) -> None:
         if self.valid():
             return  # No resolution needed
 
         # If a synonym, correct to currently approved name
```

### Comparing `tidytcells-1.8.2/src/tidytcells/aa/_main.py` & `tidytcells-1.8.3/src/tidytcells/aa/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/junction/_main.py` & `tidytcells-1.8.3/src/tidytcells/junction/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/mhc/__init__.py` & `tidytcells-1.8.3/src/tidytcells/mhc/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.3/src/tidytcells/mhc/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.3/src/tidytcells/tcr/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.3/src/tidytcells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.2
+Version: 1.8.3
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.2/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.3/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/tests/test_aa.py` & `tidytcells-1.8.3/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/tests/test_junction.py` & `tidytcells-1.8.3/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.2/tests/test_mhc.py` & `tidytcells-1.8.3/tests/test_mhc.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
 
 class TestQuery:
     @pytest.mark.filterwarnings("ignore:tidytcells is not.+aware")
     @pytest.mark.parametrize(
         ("species", "precision", "expected_len", "expected_in", "expected_not_in"),
         (
-            ("homosapiens", "allele", 22475, "HLA-DRB3*03:04", "HLA-DRB3*03:04P"),
+            ("homosapiens", "allele", 22768, "HLA-DRB3*03:04", "HLA-DRB3*03:04P"),
             ("homosapiens", "gene", 45, "HLA-B", "HLA-FOO"),
             ("musmusculus", "allele", 70, "MH1-M10-1", "HLA-A"),
             ("musmusculus", "gene", 70, "MH1-Q8", "H2-Aa"),
         ),
     )
     def test_query_all(
         self, species, precision, expected_len, expected_in, expected_not_in
```

### Comparing `tidytcells-1.8.2/tests/test_tcr.py` & `tidytcells-1.8.3/tests/test_tcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,22 @@
         (
             ("TRAV14DV4", "TRAV14/DV4"),
             ("TRBV20OR9-2", "TRBV20/OR9-2"),
             ("TRBV01", "TRBV1"),
             ("TCRBV1", "TRBV1"),
             ("TRAV14", "TRAV14/DV4"),
             ("TRDV4", "TRAV14/DV4"),
+            ("TCRAV13S2", "TRAV13-2"),
+            ("TCRAV38S2", "TRAV38-2/DV8"),
+            ("TCRAV30-1", "TRAV30"),
+            ("TCRDV01-01*01", "TRDV1*01"),
+            ("TCRAV14/4", "TRAV14/DV4"),
+            ("TCRAV36-01*01", "TRAV36/DV7*01"),
+            ("29/DV5*01", "TRAV29/DV5*01"),
+            ("TCRBJ2.7", "TRBJ2-7"),
         ),
     )
     def test_various_typos(self, gene, expected):
         result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
@@ -126,15 +134,15 @@
 class TestStandardizeMusMusculus:
     @pytest.mark.parametrize("gene", MUSMUSCULUS_TCR)
     def test_already_correctly_formatted(self, gene):
         result = tcr.standardize(gene=gene, species="musmusculus")
 
         assert result == gene
 
-    @pytest.mark.parametrize("gene", ("foobar", "TRAV3*01"))
+    @pytest.mark.parametrize("gene", ("foobar", "noice"))
     def test_inivalid_tcr(self, gene):
         with pytest.warns(UserWarning, match="Failed to standardize"):
             result = tcr.standardize(gene=gene, species="musmusculus")
 
         assert result == None
```

