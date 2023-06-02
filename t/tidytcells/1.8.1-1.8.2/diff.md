# Comparing `tmp/tidytcells-1.8.1.tar.gz` & `tmp/tidytcells-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.1.tar", last modified: Fri Jun  2 16:52:54 2023, max compression
+gzip compressed data, was "tidytcells-1.8.2.tar", last modified: Fri Jun  2 22:33:51 2023, max compression
```

## Comparing `tidytcells-1.8.1.tar` & `tidytcells-1.8.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.1/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.1/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-06-02 16:52:54.677380 tidytcells-1.8.1/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-06-02 16:02:49.000000 tidytcells-1.8.1/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-02 16:49:12.000000 tidytcells-1.8.1/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-02 16:52:54.677380 tidytcells-1.8.1/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-06-02 16:02:49.000000 tidytcells-1.8.1/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.660380 tidytcells-1.8.1/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.662380 tidytcells-1.8.1/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.675380 tidytcells-1.8.1/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1283 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4225 2023-06-02 16:09:52.000000 tidytcells-1.8.1/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    11289 2023-06-02 16:08:36.000000 tidytcells-1.8.1/src/tidytcells/_utils/gene_standardizers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-02 16:10:03.000000 tidytcells-1.8.1/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-02 16:10:51.000000 tidytcells-1.8.1/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-02 16:10:30.000000 tidytcells-1.8.1/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-02 16:11:27.000000 tidytcells-1.8.1/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-02 16:11:13.000000 tidytcells-1.8.1/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-02 16:45:57.000000 tidytcells-1.8.1/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-02 16:38:32.000000 tidytcells-1.8.1/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-02 16:06:36.000000 tidytcells-1.8.1/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-02 16:40:17.000000 tidytcells-1.8.1/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.662380 tidytcells-1.8.1/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-06-02 16:02:49.000000 tidytcells-1.8.1/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-06-02 16:02:49.000000 tidytcells-1.8.1/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-02 16:38:32.000000 tidytcells-1.8.1/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8118 2023-06-02 16:39:27.000000 tidytcells-1.8.1/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.2/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.2/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-02 22:33:51.014972 tidytcells-1.8.2/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-02 21:45:08.000000 tidytcells-1.8.2/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-02 22:30:44.000000 tidytcells-1.8.2/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-02 22:33:51.014972 tidytcells-1.8.2/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-02 22:32:49.000000 tidytcells-1.8.2/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.010972 tidytcells-1.8.2/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.011972 tidytcells-1.8.2/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-02 22:22:53.000000 tidytcells-1.8.2/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.2/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4225 2023-06-02 16:09:52.000000 tidytcells-1.8.2/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-02 16:02:49.000000 tidytcells-1.8.2/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    11289 2023-06-02 16:08:36.000000 tidytcells-1.8.2/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-02 16:10:03.000000 tidytcells-1.8.2/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-02 16:10:51.000000 tidytcells-1.8.2/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-02 16:10:30.000000 tidytcells-1.8.2/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.013972 tidytcells-1.8.2/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-02 16:11:27.000000 tidytcells-1.8.2/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-02 16:11:13.000000 tidytcells-1.8.2/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-02 16:45:57.000000 tidytcells-1.8.2/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-02 16:38:32.000000 tidytcells-1.8.2/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-02 16:06:36.000000 tidytcells-1.8.2/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-02 16:40:17.000000 tidytcells-1.8.2/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.011972 tidytcells-1.8.2/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-02 22:33:51.000000 tidytcells-1.8.2/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 22:33:51.014972 tidytcells-1.8.2/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-06-02 16:02:49.000000 tidytcells-1.8.2/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-06-02 16:02:49.000000 tidytcells-1.8.2/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-02 16:38:32.000000 tidytcells-1.8.2/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8118 2023-06-02 16:39:27.000000 tidytcells-1.8.2/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.1/LICENSE.txt` & `tidytcells-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/PKG-INFO` & `tidytcells-1.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.1
+Version: 1.8.2
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tidytcells
 
 ![Tests](https://github.com/yutanagano/tidytcells/actions/workflows/tests.yaml/badge.svg)
 ![Docs](https://readthedocs.org/projects/tidytcells/badge/?version=latest)
 ![License](https://img.shields.io/badge/license-MIT-blue)
 
-`tidytcells` is a lightweight python package that cleans and standardises T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
-The main purpose of the package is to solve the problem of parsing and collating together non-standardised TCR datasets.
+`tidytcells` is a lightweight python package that cleans and standardizes T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
+The main purpose of the package is to solve the problem of parsing and collating together non-standardized TCR datasets.
 It is often difficult to compile TCR data from multiple sources because the formats/nomenclature of how each dataset encodes TCR and MHC gene names are slightly different, or even inconsistent within themselves.
-`tidytcells` can ameliorate this issue by auto-correcting and auto-standardising your data!
+`tidytcells` can ameliorate this issue by auto-correcting and auto-standardizing your data!
+Check out the [documentation page](https://tidytcells.readthedocs.io).
 
 ## Installation
 
 ### Via [PyPI](https://pypi.org/project/tidytcells/) (recommended)
 
 `tidytcells` can be installed using `pip`:
```

### Comparing `tidytcells-1.8.1/README.md` & `tidytcells-1.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # tidytcells
 
 ![Tests](https://github.com/yutanagano/tidytcells/actions/workflows/tests.yaml/badge.svg)
 ![Docs](https://readthedocs.org/projects/tidytcells/badge/?version=latest)
 ![License](https://img.shields.io/badge/license-MIT-blue)
 
-`tidytcells` is a lightweight python package that cleans and standardises T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
-The main purpose of the package is to solve the problem of parsing and collating together non-standardised TCR datasets.
+`tidytcells` is a lightweight python package that cleans and standardizes T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
+The main purpose of the package is to solve the problem of parsing and collating together non-standardized TCR datasets.
 It is often difficult to compile TCR data from multiple sources because the formats/nomenclature of how each dataset encodes TCR and MHC gene names are slightly different, or even inconsistent within themselves.
-`tidytcells` can ameliorate this issue by auto-correcting and auto-standardising your data!
+`tidytcells` can ameliorate this issue by auto-correcting and auto-standardizing your data!
+Check out the [documentation page](https://tidytcells.readthedocs.io).
 
 ## Installation
 
 ### Via [PyPI](https://pypi.org/project/tidytcells/) (recommended)
 
 `tidytcells` can be installed using `pip`:
```

### Comparing `tidytcells-1.8.1/setup.py` & `tidytcells-1.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,34 @@
     version=VERSION,
     description="Standardise TCR/MHC data.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Yuta Nagano",
     author_email="yutanagano51@proton.me",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="immunology, bioinformatics, TCR, MHC, HLA, T cell, IMGT",
     package_dir={"": "src"},
     packages=find_packages("src"),
     package_data={"tidytcells": ["_resources/*"]},
-    python_requires=">=3.9",
+    python_requires=">=3.7",
     extras_require={
         "dev": [
             "build",
             "odfpy>=1.4.1",
             "pandas>=1.1.5",
             "pip",
             "pytest>=7",
             "pytest-cov",
             "setuptools",
             "tox>=4",
+            "twine",
             "wheel",
         ]
     },
 )
```

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.2/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.2/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.2/src/tidytcells/_utils/abstract_functions.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.2/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/_utils/gene_standardizers.py` & `tidytcells-1.8.2/src/tidytcells/_utils/gene_standardizers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/aa/_main.py` & `tidytcells-1.8.2/src/tidytcells/aa/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/junction/_main.py` & `tidytcells-1.8.2/src/tidytcells/junction/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/mhc/__init__.py` & `tidytcells-1.8.2/src/tidytcells/mhc/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.2/src/tidytcells/mhc/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.2/src/tidytcells/tcr/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.2/src/tidytcells.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.1
+Version: 1.8.2
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tidytcells
 
 ![Tests](https://github.com/yutanagano/tidytcells/actions/workflows/tests.yaml/badge.svg)
 ![Docs](https://readthedocs.org/projects/tidytcells/badge/?version=latest)
 ![License](https://img.shields.io/badge/license-MIT-blue)
 
-`tidytcells` is a lightweight python package that cleans and standardises T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
-The main purpose of the package is to solve the problem of parsing and collating together non-standardised TCR datasets.
+`tidytcells` is a lightweight python package that cleans and standardizes T cell receptor (TCR) and Major Histocompatibility Complex (MHC) data to be [IMGT](https://www.imgt.org/)-compliant.
+The main purpose of the package is to solve the problem of parsing and collating together non-standardized TCR datasets.
 It is often difficult to compile TCR data from multiple sources because the formats/nomenclature of how each dataset encodes TCR and MHC gene names are slightly different, or even inconsistent within themselves.
-`tidytcells` can ameliorate this issue by auto-correcting and auto-standardising your data!
+`tidytcells` can ameliorate this issue by auto-correcting and auto-standardizing your data!
+Check out the [documentation page](https://tidytcells.readthedocs.io).
 
 ## Installation
 
 ### Via [PyPI](https://pypi.org/project/tidytcells/) (recommended)
 
 `tidytcells` can be installed using `pip`:
```

### Comparing `tidytcells-1.8.1/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.2/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/tests/test_aa.py` & `tidytcells-1.8.2/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/tests/test_junction.py` & `tidytcells-1.8.2/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/tests/test_mhc.py` & `tidytcells-1.8.2/tests/test_mhc.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.1/tests/test_tcr.py` & `tidytcells-1.8.2/tests/test_tcr.py`

 * *Files identical despite different names*

