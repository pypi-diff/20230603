# Comparing `tmp/g_batch_prediction_pipeline-0.2.0.tar.gz` & `tmp/g_batch_prediction_pipeline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g_batch_prediction_pipeline-0.2.0.tar", max compression
+gzip compressed data, was "g_batch_prediction_pipeline-0.3.0.tar", max compression
```

## Comparing `g_batch_prediction_pipeline-0.2.0.tar` & `g_batch_prediction_pipeline-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3320 2023-06-03 02:14:11.109864 g_batch_prediction_pipeline-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:43:13.958330 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/__init__.py
--rw-r--r--   0        0        0     8731 2023-06-02 12:55:06.302539 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/batch.py
--rw-r--r--   0        0        0     1295 2023-06-02 12:55:06.307254 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/data.py
--rw-r--r--   0        0        0     4269 2023-06-02 12:55:06.300195 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/monitoring.py
--rw-r--r--   0        0        0     1400 2023-06-03 02:23:37.595895 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/settings.py
--rw-r--r--   0        0        0     3553 2023-06-02 12:55:06.304705 g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/utils.py
--rw-r--r--   0        0        0      652 2023-06-03 04:27:11.088461 g_batch_prediction_pipeline-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 g_batch_prediction_pipeline-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3320 2023-06-03 10:00:32.496000 g_batch_prediction_pipeline-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:43:13.958330 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/__init__.py
+-rw-r--r--   0        0        0     8731 2023-06-03 10:00:32.496306 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/batch.py
+-rw-r--r--   0        0        0     1295 2023-06-03 10:00:32.496528 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/data.py
+-rw-r--r--   0        0        0     4269 2023-06-03 10:00:32.496688 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/monitoring.py
+-rw-r--r--   0        0        0     1450 2023-06-03 10:00:32.496938 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/settings.py
+-rw-r--r--   0        0        0     3553 2023-06-03 10:00:32.497101 g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/utils.py
+-rw-r--r--   0        0        0      652 2023-06-03 10:22:09.949375 g_batch_prediction_pipeline-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 g_batch_prediction_pipeline-0.3.0/PKG-INFO
```

### Comparing `g_batch_prediction_pipeline-0.2.0/README.md` & `g_batch_prediction_pipeline-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/batch.py` & `g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/batch.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/data.py` & `g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/data.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/monitoring.py` & `g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/monitoring.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/settings.py` & `g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,13 +40,14 @@
     """
 
     return Path(os.getenv("ML_PIPELINE_ROOT_DIR", default_value))
 
 
 # The settings will be loaded and the outputs will be saved relative to the 'ML_PIPELINE_ROOT_DIR' directory.
 # Set environment variables.
-os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
+if os.getenv("ML_PIPELINE_ROOT_DIR") is None:
+    os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
 ML_PIPELINE_ROOT_DIR = get_root_dir()
 OUTPUT_DIR = ML_PIPELINE_ROOT_DIR / "output"
 OUTPUT_DIR.mkdir(parents=True, exist_ok=True)
 
 SETTINGS = load_env_vars(root_dir=ML_PIPELINE_ROOT_DIR)
```

### Comparing `g_batch_prediction_pipeline-0.2.0/batch_prediction_pipeline/utils.py` & `g_batch_prediction_pipeline-0.3.0/batch_prediction_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `g_batch_prediction_pipeline-0.2.0/pyproject.toml` & `g_batch_prediction_pipeline-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "g-batch-prediction-pipeline"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Iusztin Paul <p.e.iusztin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "batch_prediction_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "~3.9"
 category-encoders = "^2.6.0"
 hopsworks = "^3.0.5"
 python-dotenv = "^1.0.0"
 lightgbm = "^3.3.5"
 sktime = "^0.16.1"
 google-cloud-storage = "^2.7.0"
 fire = "^0.5.0"
-g-training-pipeline = "^0.1.0"
+g-training-pipeline = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pylint = "^2.11.1"
 isort = "^5.10.3"
 pytest = "^6.2.5"
```

### Comparing `g_batch_prediction_pipeline-0.2.0/PKG-INFO` & `g_batch_prediction_pipeline-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: g-batch-prediction-pipeline
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Iusztin Paul
 Author-email: p.e.iusztin@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: category-encoders (>=2.6.0,<3.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: g-training-pipeline (>=0.1.0,<0.2.0)
+Requires-Dist: g-training-pipeline (>=0.3.0,<0.4.0)
 Requires-Dist: google-cloud-storage (>=2.7.0,<3.0.0)
 Requires-Dist: hopsworks (>=3.0.5,<4.0.0)
 Requires-Dist: lightgbm (>=3.3.5,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sktime (>=0.16.1,<0.17.0)
 Description-Content-Type: text/markdown
```

