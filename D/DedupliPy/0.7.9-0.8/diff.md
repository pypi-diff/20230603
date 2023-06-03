# Comparing `tmp/DedupliPy-0.7.9.tar.gz` & `tmp/DedupliPy-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/fritshermans/Documents/deduplipy/dist/tmpnymixy8k/DedupliPy-0.7.9.tar", last modified: Sun Apr  3 16:03:36 2022, max compression
+gzip compressed data, was "DedupliPy-0.8.tar", last modified: Sat Jun  3 06:55:23 2023, max compression
```

## Comparing `DedupliPy-0.7.9.tar` & `DedupliPy-0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/
--rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 16:03:35.000000 DedupliPy-0.7.9/DedupliPy.egg-info/PKG-INFO
--rw-r--r--   0 fritshermans   (501) staff       (20)     1212 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/SOURCES.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)        1 2022-04-03 16:03:35.000000 DedupliPy-0.7.9/DedupliPy.egg-info/dependency_links.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)      461 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/requires.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)       10 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/top_level.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)     1070 2021-05-04 14:47:45.000000 DedupliPy-0.7.9/LICENSE
--rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/PKG-INFO
--rw-r--r--   0 fritshermans   (501) staff       (20)     2988 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/README.md
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/
--rw-r--r--   0 fritshermans   (501) staff       (20)       22 2022-04-03 16:02:24.000000 DedupliPy-0.7.9/deduplipy/__init__.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/active_learning/
--rw-r--r--   0 fritshermans   (501) staff       (20)       94 2021-04-20 16:52:14.000000 DedupliPy-0.7.9/deduplipy/active_learning/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     9429 2022-04-03 15:56:00.000000 DedupliPy-0.7.9/deduplipy/active_learning/active_learning.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      596 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/active_learning/utils_active_learning.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/blocking/
--rw-r--r--   0 fritshermans   (501) staff       (20)      196 2021-06-18 15:04:38.000000 DedupliPy-0.7.9/deduplipy/blocking/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     5257 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/blocking/blocking.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     4000 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/blocking/blocking_rules.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2523 2021-05-06 17:56:34.000000 DedupliPy-0.7.9/deduplipy/blocking/set_cover.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/
--rw-r--r--   0 fritshermans   (501) staff       (20)       86 2021-04-29 14:44:28.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2342 2022-04-03 14:21:19.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/classifier_pipeline.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/clustering/
--rw-r--r--   0 fritshermans   (501) staff       (20)      160 2022-04-03 14:20:03.000000 DedupliPy-0.7.9/deduplipy/clustering/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2538 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/clustering/clustering.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     1216 2022-04-02 17:14:16.000000 DedupliPy-0.7.9/deduplipy/clustering/fill_missing_edges.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      228 2022-04-03 14:20:03.000000 DedupliPy-0.7.9/deduplipy/config.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/data/
--rw-r--r--   0 fritshermans   (501) staff       (20)    13367 2021-04-10 13:53:23.000000 DedupliPy-0.7.9/deduplipy/data/stoxx50_extended_with_id.xlsx
--rw-r--r--   0 fritshermans   (501) staff       (20)    52700 2021-05-04 08:25:31.000000 DedupliPy-0.7.9/deduplipy/data/voter_names.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)   535135 2021-11-02 18:44:54.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_17k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)  1048954 2021-11-02 18:39:56.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_35k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)  2488637 2021-11-02 17:44:06.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_80k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)     1204 2022-04-03 07:39:34.000000 DedupliPy-0.7.9/deduplipy/datasets.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/deduplicator/
--rw-r--r--   0 fritshermans   (501) staff       (20)       67 2021-04-20 16:52:58.000000 DedupliPy-0.7.9/deduplipy/deduplicator/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)    10030 2022-04-03 14:21:19.000000 DedupliPy-0.7.9/deduplipy/deduplicator/deduplicator.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/sampling/
--rw-r--r--   0 fritshermans   (501) staff       (20)      132 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/sampling/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     5922 2022-04-03 15:17:25.000000 DedupliPy-0.7.9/deduplipy/sampling/minhash_sampling.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2485 2022-04-03 15:28:39.000000 DedupliPy-0.7.9/deduplipy/sampling/naive_sampling.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     1051 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/sampling/sampler.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/string_metrics/
--rw-r--r--   0 fritshermans   (501) staff       (20)      233 2021-05-10 18:42:39.000000 DedupliPy-0.7.9/deduplipy/string_metrics/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2060 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/string_metrics/string_metrics.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      103 2021-05-04 13:45:36.000000 DedupliPy-0.7.9/pyproject.toml
--rw-r--r--   0 fritshermans   (501) staff       (20)       38 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/setup.cfg
--rw-r--r--   0 fritshermans   (501) staff       (20)     1333 2022-04-03 16:02:24.000000 DedupliPy-0.7.9/setup.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.339322 DedupliPy-0.8/
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.325176 DedupliPy-0.8/DedupliPy.egg-info/
+-rw-r--r--   0 fritshermans   (501) staff       (20)     3453 2023-06-03 06:55:23.000000 DedupliPy-0.8/DedupliPy.egg-info/PKG-INFO
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1212 2023-06-03 06:55:23.000000 DedupliPy-0.8/DedupliPy.egg-info/SOURCES.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)        1 2023-06-03 06:55:23.000000 DedupliPy-0.8/DedupliPy.egg-info/dependency_links.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)      482 2023-06-03 06:55:23.000000 DedupliPy-0.8/DedupliPy.egg-info/requires.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)       10 2023-06-03 06:55:23.000000 DedupliPy-0.8/DedupliPy.egg-info/top_level.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1070 2021-05-04 14:47:45.000000 DedupliPy-0.8/LICENSE
+-rw-r--r--   0 fritshermans   (501) staff       (20)     3453 2023-06-03 06:55:23.339147 DedupliPy-0.8/PKG-INFO
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2988 2022-04-03 14:20:08.000000 DedupliPy-0.8/README.md
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.325703 DedupliPy-0.8/deduplipy/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       20 2023-06-03 06:53:44.000000 DedupliPy-0.8/deduplipy/__init__.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.326507 DedupliPy-0.8/deduplipy/active_learning/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       94 2021-04-20 16:52:14.000000 DedupliPy-0.8/deduplipy/active_learning/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     9441 2023-04-16 10:14:14.000000 DedupliPy-0.8/deduplipy/active_learning/active_learning.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      596 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/active_learning/utils_active_learning.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.327489 DedupliPy-0.8/deduplipy/blocking/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      196 2021-06-18 15:04:38.000000 DedupliPy-0.8/deduplipy/blocking/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     5257 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/blocking/blocking.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     4000 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/blocking/blocking_rules.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2523 2021-05-06 17:56:34.000000 DedupliPy-0.8/deduplipy/blocking/set_cover.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.327942 DedupliPy-0.8/deduplipy/classifier_pipeline/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       86 2021-04-29 14:44:28.000000 DedupliPy-0.8/deduplipy/classifier_pipeline/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2342 2022-04-03 14:21:19.000000 DedupliPy-0.8/deduplipy/classifier_pipeline/classifier_pipeline.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.328575 DedupliPy-0.8/deduplipy/clustering/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      160 2022-04-03 14:20:03.000000 DedupliPy-0.8/deduplipy/clustering/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2538 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/clustering/clustering.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1216 2022-04-02 17:14:16.000000 DedupliPy-0.8/deduplipy/clustering/fill_missing_edges.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      228 2022-04-03 14:20:03.000000 DedupliPy-0.8/deduplipy/config.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.332161 DedupliPy-0.8/deduplipy/data/
+-rw-r--r--   0 fritshermans   (501) staff       (20)    13367 2021-04-10 13:53:23.000000 DedupliPy-0.8/deduplipy/data/stoxx50_extended_with_id.xlsx
+-rw-r--r--   0 fritshermans   (501) staff       (20)    52700 2021-05-04 08:25:31.000000 DedupliPy-0.8/deduplipy/data/voter_names.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)   535135 2021-11-02 18:44:54.000000 DedupliPy-0.8/deduplipy/data/voter_names_17k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)  1048954 2021-11-02 18:39:56.000000 DedupliPy-0.8/deduplipy/data/voter_names_35k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)  2488637 2021-11-02 17:44:06.000000 DedupliPy-0.8/deduplipy/data/voter_names_80k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1204 2022-04-03 07:39:34.000000 DedupliPy-0.8/deduplipy/datasets.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.335902 DedupliPy-0.8/deduplipy/deduplicator/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       67 2021-04-20 16:52:58.000000 DedupliPy-0.8/deduplipy/deduplicator/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)    10059 2023-04-16 10:14:14.000000 DedupliPy-0.8/deduplipy/deduplicator/deduplicator.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.338346 DedupliPy-0.8/deduplipy/sampling/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      132 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/sampling/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     5961 2023-04-16 10:14:14.000000 DedupliPy-0.8/deduplipy/sampling/minhash_sampling.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2495 2023-04-16 10:14:14.000000 DedupliPy-0.8/deduplipy/sampling/naive_sampling.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1051 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/sampling/sampler.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2023-06-03 06:55:23.338877 DedupliPy-0.8/deduplipy/string_metrics/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      233 2021-05-10 18:42:39.000000 DedupliPy-0.8/deduplipy/string_metrics/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2060 2022-04-03 14:20:08.000000 DedupliPy-0.8/deduplipy/string_metrics/string_metrics.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      103 2021-05-04 13:45:36.000000 DedupliPy-0.8/pyproject.toml
+-rw-r--r--   0 fritshermans   (501) staff       (20)       38 2023-06-03 06:55:23.339375 DedupliPy-0.8/setup.cfg
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1338 2023-06-03 06:53:44.000000 DedupliPy-0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DedupliPy-0.7.9/DedupliPy.egg-info/PKG-INFO` & `DedupliPy-0.8/DedupliPy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: DedupliPy
-Version: 0.7.9
+Version: 0.8
 Summary: End-to-end deduplication solution
 Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: dev
@@ -94,9 +92,7 @@
 This will start the interactive learning session in which you provide input on whether a pair is a match (y) or not (n).
 During active learning you will get the message that training may be finished once algorithm training has converged.
 Predictions on (new) data are obtained as follows:
 
 ```python
 result = myDedupliPy.predict(df)
 ```
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.9 Summary: End-to-end
+Metadata-Version: 2.1 Name: DedupliPy Version: 0.8 Summary: End-to-end
 deduplication solution Home-page: https://github.com/fritshermans/deduplipy
-Author: Frits Hermans License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown Provides-Extra: base Provides-Extra:
-dev Provides-Extra: docs License-File: LICENSE  [![Version](https://
-img.shields.io/pypi/v/deduplipy)](https://pypi.org/project/deduplipy/) ![]
-(https://img.shields.io/github/license/fritshermans/deduplipy) [![Downloads]
-(https://pepy.tech/badge/deduplipy)](https://pepy.tech/project/deduplipy) [!
-[Conda - Platform](https://img.shields.io/conda/pn/conda-forge/
-deduplipy?logo=anaconda&style=flat)][#conda-forge-package] [![Conda (channel
-only)](https://img.shields.io/conda/vn/conda-forge/
-deduplipy?logo=anaconda&style=flat&color=orange)][#conda-forge-package] [!
-[Conda Recipe](https://img.shields.io/static/v1?logo=conda-
+Author: Frits Hermans Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6.9 Description-Content-Type: text/
+markdown Provides-Extra: base Provides-Extra: dev Provides-Extra: docs License-
+File: LICENSE  [![Version](https://img.shields.io/pypi/v/deduplipy)](https://
+pypi.org/project/deduplipy/) ![](https://img.shields.io/github/license/
+fritshermans/deduplipy) [![Downloads](https://pepy.tech/badge/deduplipy)]
+(https://pepy.tech/project/deduplipy) [![Conda - Platform](https://
+img.shields.io/conda/pn/conda-forge/deduplipy?logo=anaconda&style=flat)]
+[#conda-forge-package] [![Conda (channel only)](https://img.shields.io/conda/
+vn/conda-forge/deduplipy?logo=anaconda&style=flat&color=orange)][#conda-forge-
+package] [![Conda Recipe](https://img.shields.io/static/v1?logo=conda-
 forge&style=flat&color=green&label=recipe&message=deduplipy)][#conda-forge-
 feedstock] [![Docs - GitHub.io](https://img.shields.io/static/
 v1?logo=readthdocs&style=flat&color=pink&label=docs&message=deduplipy)][#docs-
 package] [#pypi-package]: https://pypi.org/project/deduplipy/ [#conda-forge-
 package]: https://anaconda.org/conda-forge/deduplipy [#conda-forge-feedstock]:
 https://github.com/conda-forge/deduplipy-feedstock [#docs-package]: https://
 deduplipy.readthedocs.io/en/latest/  # DedupliPy [https://
```

### Comparing `DedupliPy-0.7.9/DedupliPy.egg-info/SOURCES.txt` & `DedupliPy-0.8/DedupliPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/LICENSE` & `DedupliPy-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/PKG-INFO` & `DedupliPy-0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: DedupliPy
-Version: 0.7.9
+Version: 0.8
 Summary: End-to-end deduplication solution
 Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: dev
@@ -94,9 +92,7 @@
 This will start the interactive learning session in which you provide input on whether a pair is a match (y) or not (n).
 During active learning you will get the message that training may be finished once algorithm training has converged.
 Predictions on (new) data are obtained as follows:
 
 ```python
 result = myDedupliPy.predict(df)
 ```
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.9 Summary: End-to-end
+Metadata-Version: 2.1 Name: DedupliPy Version: 0.8 Summary: End-to-end
 deduplication solution Home-page: https://github.com/fritshermans/deduplipy
-Author: Frits Hermans License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown Provides-Extra: base Provides-Extra:
-dev Provides-Extra: docs License-File: LICENSE  [![Version](https://
-img.shields.io/pypi/v/deduplipy)](https://pypi.org/project/deduplipy/) ![]
-(https://img.shields.io/github/license/fritshermans/deduplipy) [![Downloads]
-(https://pepy.tech/badge/deduplipy)](https://pepy.tech/project/deduplipy) [!
-[Conda - Platform](https://img.shields.io/conda/pn/conda-forge/
-deduplipy?logo=anaconda&style=flat)][#conda-forge-package] [![Conda (channel
-only)](https://img.shields.io/conda/vn/conda-forge/
-deduplipy?logo=anaconda&style=flat&color=orange)][#conda-forge-package] [!
-[Conda Recipe](https://img.shields.io/static/v1?logo=conda-
+Author: Frits Hermans Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6.9 Description-Content-Type: text/
+markdown Provides-Extra: base Provides-Extra: dev Provides-Extra: docs License-
+File: LICENSE  [![Version](https://img.shields.io/pypi/v/deduplipy)](https://
+pypi.org/project/deduplipy/) ![](https://img.shields.io/github/license/
+fritshermans/deduplipy) [![Downloads](https://pepy.tech/badge/deduplipy)]
+(https://pepy.tech/project/deduplipy) [![Conda - Platform](https://
+img.shields.io/conda/pn/conda-forge/deduplipy?logo=anaconda&style=flat)]
+[#conda-forge-package] [![Conda (channel only)](https://img.shields.io/conda/
+vn/conda-forge/deduplipy?logo=anaconda&style=flat&color=orange)][#conda-forge-
+package] [![Conda Recipe](https://img.shields.io/static/v1?logo=conda-
 forge&style=flat&color=green&label=recipe&message=deduplipy)][#conda-forge-
 feedstock] [![Docs - GitHub.io](https://img.shields.io/static/
 v1?logo=readthdocs&style=flat&color=pink&label=docs&message=deduplipy)][#docs-
 package] [#pypi-package]: https://pypi.org/project/deduplipy/ [#conda-forge-
 package]: https://anaconda.org/conda-forge/deduplipy [#conda-forge-feedstock]:
 https://github.com/conda-forge/deduplipy-feedstock [#docs-package]: https://
 deduplipy.readthedocs.io/en/latest/  # DedupliPy [https://
```

### Comparing `DedupliPy-0.7.9/README.md` & `DedupliPy-0.8/README.md`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/active_learning/active_learning.py` & `DedupliPy-0.8/deduplipy/active_learning/active_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         """
         if self.verbose:
             print(f'\nNr. {self.counter_total + 1} ({self.counter_positive}+/{self.counter_negative}-)')
         else:
             print(f'\nNr. {self.counter_total + 1} ({self.counter_positive}+/{self.counter_negative}-)')
         print("Is this a match? (y)es, (n)o, (p)revious, (s)kip, (f)inish")
-        with pd.option_context('display.max_colwidth', -1):
+        with pd.option_context('display.max_colwidth', None):
             print('->', query_inst[[f'{col_name}_1' for col_name in self.col_names]].iloc[0].to_string())
             print('->', query_inst[[f'{col_name}_2' for col_name in self.col_names]].iloc[0].to_string())
         user_input = input_assert("", ['y', 'n', 'p', 'f', 's'])
         # replace 'y' and 'n' with '1' and '0' to make them valid y labels
         user_input = user_input.replace('y', '1').replace('n', '0')
         # replace 'p' (previous) by '-1', 'f' (finished) by '9', and 's' (skip) by '8'
         user_input = user_input.replace('p', '-1').replace('f', '9').replace('s', '8')
@@ -165,15 +165,15 @@
             elif y_new == 9:  # finish labelling (input is 'f')
                 break
             query_inst_prev = X.iloc[query_idx]
             if y_new != 8:  # skip case (input is 's')
                 self.learner.teach([X.iloc[query_idx]['similarities'].iloc[0]], y_new)
                 train_sample_to_add = X.iloc[query_idx].copy()
                 train_sample_to_add['y'] = y_new
-                self.train_samples = self.train_samples.append(train_sample_to_add, ignore_index=True)
+                self.train_samples = pd.concat([self.train_samples, train_sample_to_add]).reset_index(drop=True)
             X = X.drop(query_idx).reset_index(drop=True)
             last_uncertainty_improvement = self._get_last_uncertainty_improvement()
             if (self.counter_total >= self.min_nr_entries) and last_uncertainty_improvement:
                 if self.verbose:
                     print(f"Last uncertainty improvement: {last_uncertainty_improvement:.3f}")
                     print(f'Uncertainty: {uncertainty:.3f}')
                 if (uncertainty < self.uncertainty_threshold) | (
```

### Comparing `DedupliPy-0.7.9/deduplipy/active_learning/utils_active_learning.py` & `DedupliPy-0.8/deduplipy/active_learning/utils_active_learning.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/blocking/blocking.py` & `DedupliPy-0.8/deduplipy/blocking/blocking.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/blocking/blocking_rules.py` & `DedupliPy-0.8/deduplipy/blocking/blocking_rules.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/blocking/set_cover.py` & `DedupliPy-0.8/deduplipy/blocking/set_cover.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/classifier_pipeline/classifier_pipeline.py` & `DedupliPy-0.8/deduplipy/classifier_pipeline/classifier_pipeline.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/clustering/clustering.py` & `DedupliPy-0.8/deduplipy/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/clustering/fill_missing_edges.py` & `DedupliPy-0.8/deduplipy/clustering/fill_missing_edges.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/data/stoxx50_extended_with_id.xlsx` & `DedupliPy-0.8/deduplipy/data/stoxx50_extended_with_id.xlsx`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/data/voter_names.csv` & `DedupliPy-0.8/deduplipy/data/voter_names.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/data/voter_names_17k.csv` & `DedupliPy-0.8/deduplipy/data/voter_names_17k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/data/voter_names_35k.csv` & `DedupliPy-0.8/deduplipy/data/voter_names_35k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/data/voter_names_80k.csv` & `DedupliPy-0.8/deduplipy/data/voter_names_80k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/datasets.py` & `DedupliPy-0.8/deduplipy/datasets.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/deduplicator/deduplicator.py` & `DedupliPy-0.8/deduplipy/deduplicator/deduplicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
         """
         n_samples_minhash = n_samples // 2
         minhash_pairs = MinHashSampler(self.col_names).sample(X, n_samples_minhash)
         # the number of minhash samples can be (much) smaller than n_samples//2, in such case take more random pairs:
         n_samples_naive = n_samples - len(minhash_pairs)
         naive_pairs = NaiveSampler(self.col_names).sample(X, n_samples_naive)
-        pairs = naive_pairs.append(minhash_pairs)
+        pairs = pd.concat([naive_pairs, minhash_pairs]).reset_index(drop=True)
         return pairs.drop_duplicates()
 
     def _calculate_string_similarities(self, X: pd.DataFrame) -> pd.DataFrame:
         X.reset_index(drop=True, inplace=True)  # need to reset the index because of the list comprehension below
         metrics_col_names = []
         for field in self.field_info.keys():
             for metric in self.field_info[field]:
```

### Comparing `DedupliPy-0.7.9/deduplipy/sampling/minhash_sampling.py` & `DedupliPy-0.8/deduplipy/sampling/minhash_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             minhash_result = (minhash_result
                               .merge(df.drop(columns=[col]), left_on='row_number_1', right_on='row_number')
                               .drop(columns=['row_number']))
             minhash_result = (minhash_result
                               .merge(df.drop(columns=[col]), left_on='row_number_2', right_on='row_number',
                                      suffixes=("_1", "_2"))
                               .drop(columns=['row_number']))
-            minhash_pairs = minhash_pairs.append(minhash_result, ignore_index=True)
+            minhash_pairs = pd.concat([minhash_pairs, minhash_result]).reset_index(drop=True)
 
         # mean of Jaccard similarities over all columns is used for thresholding
         minhash_pairs = (minhash_pairs
                          .groupby(['row_number_1', 'row_number_2'] + self.pairs_col_names, as_index=False)
                          ['jaccard_sim'].mean()
                          .drop(columns=['row_number_1', 'row_number_2']))
 
@@ -127,11 +127,11 @@
         """
         minhash_pairs = self._create_minhash_pairs(X, threshold)
 
         stratified_sample = self._get_stratified_sample(minhash_pairs, n_samples)
 
         non_stratified_sample = self._get_non_stratified_sample(minhash_pairs, stratified_sample, n_samples)
 
-        sample = stratified_sample.append(non_stratified_sample)[self.pairs_col_names]
+        sample = pd.concat([stratified_sample, non_stratified_sample]).reset_index(drop=True)[self.pairs_col_names]
         sample['synthetic_perfect_match'] = False
 
         return sample
```

### Comparing `DedupliPy-0.7.9/deduplipy/sampling/naive_sampling.py` & `DedupliPy-0.8/deduplipy/sampling/naive_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 
         perfect_matches = pairs_table[pairs_table[f'{ROW_ID}_1'] == pairs_table[f'{ROW_ID}_2']].iloc[
                           :self.n_perfect_matches]
         perfect_matches['synthetic_perfect_match'] = True
 
         pairs_table = pairs_table[
             pairs_table[f'{ROW_ID}_1'] < pairs_table[f'{ROW_ID}_2']]
-        pairs_table = perfect_matches.append(pairs_table, ignore_index=True)
+        pairs_table = pd.concat([perfect_matches, pairs_table]).reset_index(drop=True)
         pairs_table = pairs_table[self.pairs_col_names+['synthetic_perfect_match']].reset_index(drop=True)
         return pairs_table.head(n_samples)
```

### Comparing `DedupliPy-0.7.9/deduplipy/sampling/sampler.py` & `DedupliPy-0.8/deduplipy/sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/deduplipy/string_metrics/string_metrics.py` & `DedupliPy-0.8/deduplipy/string_metrics/string_metrics.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.9/setup.py` & `DedupliPy-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'pandas',
     'numpy',
     'scipy',
     'scikit-learn',
     'networkx',
     'python-Levenshtein',
     'thefuzz',
-    'modAL',
+    'modAL-python',
     'openpyxl',
     'pytest',
     'fancyimpute',
     'pyminhash'
 ]
 
 util_packages = [
@@ -28,15 +28,15 @@
 
 dev_packages = base_packages + util_packages + docs_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='DedupliPy',
-      version='0.7.9',
+      version='0.8',
       author="Frits Hermans",
       description="End-to-end deduplication solution",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/fritshermans/deduplipy",
       classifiers=[
           "Programming Language :: Python :: 3",
```

