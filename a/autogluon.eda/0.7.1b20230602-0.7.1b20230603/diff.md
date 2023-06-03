# Comparing `tmp/autogluon.eda-0.7.1b20230602.tar.gz` & `tmp/autogluon.eda-0.7.1b20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.eda-0.7.1b20230602.tar", last modified: Fri Jun  2 09:04:18 2023, max compression
+gzip compressed data, was "autogluon.eda-0.7.1b20230603.tar", last modified: Sat Jun  3 09:04:12 2023, max compression
```

## Comparing `autogluon.eda-0.7.1b20230602.tar` & `autogluon.eda-0.7.1b20230603.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.710040 autogluon.eda-0.7.1b20230602/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-02 09:04:18.710040 autogluon.eda-0.7.1b20230602/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-02 09:04:18.710040 autogluon.eda-0.7.1b20230602/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon/eda/auto/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/auto/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.710040 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-02 09:03:27.000000 autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/shift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:18.706040 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:18.000000 autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-03 09:04:12.989571 autogluon.eda-0.7.1b20230603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.981570 autogluon.eda-0.7.1b20230603/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.981570 autogluon.eda-0.7.1b20230603/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/src/autogluon/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/src/autogluon/eda/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/auto/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.985571 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-03 09:03:22.000000 autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/shift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:04:12.981570 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:04:12.000000 autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/zip-safe
```

### Comparing `autogluon.eda-0.7.1b20230602/PKG-INFO` & `autogluon.eda-0.7.1b20230603/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.eda-0.7.1b20230602/setup.cfg` & `autogluon.eda-0.7.1b20230603/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/setup.py` & `autogluon.eda-0.7.1b20230603/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/__init__.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/anomaly.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/anomaly.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/base.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/dataset.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/explain.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/interaction.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/missing.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/model.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/shift.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/analysis/transform.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/auto/simple.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/auto/simple.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/state.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/state.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/common.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/common.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/utils/defaults.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/__init__.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/anomaly.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/anomaly.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/base.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/dataset.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/explain.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/interaction.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/jupyter.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/jupyter.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/layouts.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/layouts.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/missing.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/model.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon/eda/visualization/shift.py` & `autogluon.eda-0.7.1b20230603/src/autogluon/eda/visualization/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/PKG-INFO` & `autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.eda-0.7.1b20230602/src/autogluon.eda.egg-info/SOURCES.txt` & `autogluon.eda-0.7.1b20230603/src/autogluon.eda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

