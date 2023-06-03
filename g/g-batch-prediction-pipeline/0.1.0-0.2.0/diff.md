# Comparing `tmp/g_batch_prediction_pipeline-0.1.0.tar.gz` & `tmp/g_batch_prediction_pipeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g_batch_prediction_pipeline-0.1.0.tar", max compression
+gzip compressed data, was "g_batch_prediction_pipeline-0.2.0.tar", max compression
```

## Comparing `g_batch_prediction_pipeline-0.1.0.tar` & `g_batch_prediction_pipeline-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3320 2023-06-03 02:14:11.109864 g_batch_prediction_pipeline-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:43:13.958330 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/__init__.py
--rw-r--r--   0        0        0     8731 2023-06-02 12:55:06.302539 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/batch.py
--rw-r--r--   0        0        0     1295 2023-06-02 12:55:06.307254 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/data.py
--rw-r--r--   0        0        0     4269 2023-06-02 12:55:06.300195 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/monitoring.py
--rw-r--r--   0        0        0     1400 2023-06-03 02:23:37.595895 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/settings.py
--rw-r--r--   0        0        0     3553 2023-06-02 12:55:06.304705 g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/utils.py
--rw-r--r--   0        0        0      652 2023-06-02 12:36:37.753691 g_batch_prediction_pipeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 g_batch_prediction_pipeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3320 2023-06-03 02:14:11.109864 g_batch_prediction_pipeline-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:43:13.958330 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/__init__.py
+-rw-r--r--   0        0        0     8731 2023-06-02 12:55:06.302539 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/batch.py
+-rw-r--r--   0        0        0     1295 2023-06-02 12:55:06.307254 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/data.py
+-rw-r--r--   0        0        0     4269 2023-06-02 12:55:06.300195 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/monitoring.py
+-rw-r--r--   0        0        0     1400 2023-06-03 02:23:37.595895 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/settings.py
+-rw-r--r--   0        0        0     3553 2023-06-02 12:55:06.304705 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/utils.py
+-rw-r--r--   0        0        0      652 2023-06-03 04:27:11.088461 g_batch_prediction_pipeline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 g_batch_prediction_pipeline-0.2.0/PKG-INFO
```

### Comparing `g_batch_prediction_pipeline-0.1.0/README.md` & `g_batch_prediction_pipeline-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/batch.py` & `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/batch.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/data.py` & `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/data.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/monitoring.py` & `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/monitoring.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/settings.py` & `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/settings.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/batch_prediction_pipeline/utils.py` & `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.1.0/pyproject.toml` & `g_batch_prediction_pipeline-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "g-batch-prediction-pipeline"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Iusztin Paul <p.e.iusztin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "batch_prediction_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `g_batch_prediction_pipeline-0.1.0/PKG-INFO` & `g_batch_prediction_pipeline-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g-batch-prediction-pipeline
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Iusztin Paul
 Author-email: p.e.iusztin@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: category-encoders (>=2.6.0,<3.0.0)
```

