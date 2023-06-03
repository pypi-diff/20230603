# Comparing `tmp/g_training_pipeline-0.2.0.tar.gz` & `tmp/g_training_pipeline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g_training_pipeline-0.2.0.tar", max compression
+gzip compressed data, was "g_training_pipeline-0.3.0.tar", max compression
```

## Comparing `g_training_pipeline-0.2.0.tar` & `g_training_pipeline-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2947 2023-06-03 02:12:16.087795 g_training_pipeline-0.2.0/README.md
--rw-r--r--   0        0        0      640 2023-06-03 04:26:39.117088 g_training_pipeline-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 03:43:13.968582 g_training_pipeline-0.2.0/training_pipeline/__init__.py
--rw-r--r--   0        0        0     2216 2023-06-02 09:20:08.027298 g_training_pipeline-0.2.0/training_pipeline/best_config.py
--rw-r--r--   0        0        0       49 2023-06-02 03:43:13.968701 g_training_pipeline-0.2.0/training_pipeline/configs/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-02 10:03:43.501313 g_training_pipeline-0.2.0/training_pipeline/configs/gridsearch.py
--rw-r--r--   0        0        0     4112 2023-06-02 09:26:07.447802 g_training_pipeline-0.2.0/training_pipeline/data.py
--rw-r--r--   0        0        0     5661 2023-06-02 09:15:04.394231 g_training_pipeline-0.2.0/training_pipeline/hyperparameter_tuning.py
--rw-r--r--   0        0        0     2162 2023-06-02 09:15:04.383507 g_training_pipeline-0.2.0/training_pipeline/models.py
--rw-r--r--   0        0        0     1331 2023-06-03 02:12:44.715738 g_training_pipeline-0.2.0/training_pipeline/settings.py
--rw-r--r--   0        0        0    13173 2023-06-02 10:12:30.941900 g_training_pipeline-0.2.0/training_pipeline/train.py
--rw-r--r--   0        0        0     1268 2023-06-02 03:43:13.969125 g_training_pipeline-0.2.0/training_pipeline/transformers.py
--rw-r--r--   0        0        0      285 2023-06-02 09:35:40.841913 g_training_pipeline-0.2.0/training_pipeline/typings.py
--rw-r--r--   0        0        0     3352 2023-06-02 09:21:55.043274 g_training_pipeline-0.2.0/training_pipeline/utils.py
--rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 g_training_pipeline-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2947 2023-06-03 02:12:16.087795 g_training_pipeline-0.3.0/README.md
+-rw-r--r--   0        0        0      670 2023-06-03 09:45:19.941928 g_training_pipeline-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 03:43:13.968582 g_training_pipeline-0.3.0/training_pipeline/__init__.py
+-rw-r--r--   0        0        0     2216 2023-06-02 09:20:08.027298 g_training_pipeline-0.3.0/training_pipeline/best_config.py
+-rw-r--r--   0        0        0       49 2023-06-02 03:43:13.968701 g_training_pipeline-0.3.0/training_pipeline/configs/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-02 10:03:43.501313 g_training_pipeline-0.3.0/training_pipeline/configs/gridsearch.py
+-rw-r--r--   0        0        0     4112 2023-06-02 09:26:07.447802 g_training_pipeline-0.3.0/training_pipeline/data.py
+-rw-r--r--   0        0        0     5661 2023-06-02 09:15:04.394231 g_training_pipeline-0.3.0/training_pipeline/hyperparameter_tuning.py
+-rw-r--r--   0        0        0     2162 2023-06-02 09:15:04.383507 g_training_pipeline-0.3.0/training_pipeline/models.py
+-rw-r--r--   0        0        0     1548 2023-06-03 09:45:41.871509 g_training_pipeline-0.3.0/training_pipeline/settings.py
+-rw-r--r--   0        0        0    13173 2023-06-02 10:12:30.941900 g_training_pipeline-0.3.0/training_pipeline/train.py
+-rw-r--r--   0        0        0     1268 2023-06-02 03:43:13.969125 g_training_pipeline-0.3.0/training_pipeline/transformers.py
+-rw-r--r--   0        0        0      285 2023-06-02 09:35:40.841913 g_training_pipeline-0.3.0/training_pipeline/typings.py
+-rw-r--r--   0        0        0     3352 2023-06-03 09:28:13.835409 g_training_pipeline-0.3.0/training_pipeline/utils.py
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 g_training_pipeline-0.3.0/PKG-INFO
```

### Comparing `g_training_pipeline-0.2.0/README.md` & `g_training_pipeline-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/best_config.py` & `g_training_pipeline-0.3.0/training_pipeline/best_config.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/configs/gridsearch.py` & `g_training_pipeline-0.3.0/training_pipeline/configs/gridsearch.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/data.py` & `g_training_pipeline-0.3.0/training_pipeline/data.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/hyperparameter_tuning.py` & `g_training_pipeline-0.3.0/training_pipeline/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/models.py` & `g_training_pipeline-0.3.0/training_pipeline/models.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/settings.py` & `g_training_pipeline-0.3.0/training_pipeline/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         Path to the root directory of the project.
     """
 
     return Path(os.getenv("ML_PIPELINE_ROOT_DIR", default_value))
 
 
 # Set environment variables.
-os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
+print(f"os.getenv('ML_PIPELINE_ROOT_DIR'): {os.getenv('ML_PIPELINE_ROOT_DIR')}")
+if os.getenv("ML_PIPELINE_ROOT_DIR") is None:
+    os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
 
 ML_PIPELINE_ROOT_DIR = get_root_dir()
+print(f"ML_PIPELINE_ROOT_DIR: {ML_PIPELINE_ROOT_DIR}")
 OUTPUT_DIR = ML_PIPELINE_ROOT_DIR / "output"
 OUTPUT_DIR.mkdir(parents=True, exist_ok=True)
 
 SETTINGS = load_env_vars(root_dir=ML_PIPELINE_ROOT_DIR)
+print(f"SETTINGS: {SETTINGS}")
```

### Comparing `g_training_pipeline-0.2.0/training_pipeline/train.py` & `g_training_pipeline-0.3.0/training_pipeline/train.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/transformers.py` & `g_training_pipeline-0.3.0/training_pipeline/transformers.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/training_pipeline/utils.py` & `g_training_pipeline-0.3.0/training_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.2.0/PKG-INFO` & `g_training_pipeline-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: g-training-pipeline
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Iusztin Paul
 Author-email: p.e.iusztin@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==3.0.1)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: g-feature-pipeline (>=0.2.0,<0.3.0)
 Requires-Dist: hopsworks (>=3.0.5,<4.0.0)
 Requires-Dist: lightgbm (>=3.3.5,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sktime (>=0.16.1,<0.17.0)
```

