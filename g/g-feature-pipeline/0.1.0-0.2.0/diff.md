# Comparing `tmp/g_feature_pipeline-0.1.0.tar.gz` & `tmp/g_feature_pipeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g_feature_pipeline-0.1.0.tar", max compression
+gzip compressed data, was "g_feature_pipeline-0.2.0.tar", max compression
```

## Comparing `g_feature_pipeline-0.1.0.tar` & `g_feature_pipeline-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3438 2023-06-03 02:10:46.283764 g_feature_pipeline-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:43:13.960266 g_feature_pipeline-0.1.0/feature_pipeline/__init__.py
--rw-r--r--   0        0        0     1119 2023-06-02 07:04:53.636510 g_feature_pipeline-0.1.0/feature_pipeline/clean_feature_store.py
--rw-r--r--   0        0        0      173 2023-06-02 03:43:13.960397 g_feature_pipeline-0.1.0/feature_pipeline/etl/__init__.py
--rw-r--r--   0        0        0     1267 2023-06-02 03:43:13.960452 g_feature_pipeline-0.1.0/feature_pipeline/etl/cleaning.py
--rw-r--r--   0        0        0     3045 2023-06-02 07:28:46.969348 g_feature_pipeline-0.1.0/feature_pipeline/etl/extract.py
--rw-r--r--   0        0        0     3106 2023-06-02 07:27:14.975975 g_feature_pipeline-0.1.0/feature_pipeline/etl/load.py
--rw-r--r--   0        0        0     4109 2023-06-02 07:28:46.971633 g_feature_pipeline-0.1.0/feature_pipeline/etl/validation.py
--rw-r--r--   0        0        0     4311 2023-06-02 07:28:46.961982 g_feature_pipeline-0.1.0/feature_pipeline/feature_view.py
--rw-r--r--   0        0        0     2691 2023-06-02 09:12:34.100668 g_feature_pipeline-0.1.0/feature_pipeline/pipeline.py
--rw-r--r--   0        0        0     1190 2023-06-03 02:06:24.990518 g_feature_pipeline-0.1.0/feature_pipeline/settings.py
--rw-r--r--   0        0        0     1227 2023-06-02 03:43:13.960883 g_feature_pipeline-0.1.0/feature_pipeline/utils.py
--rw-r--r--   0        0        0      600 2023-06-02 12:47:56.462334 g_feature_pipeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 g_feature_pipeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3438 2023-06-03 02:10:46.283764 g_feature_pipeline-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:43:13.960266 g_feature_pipeline-0.2.0/feature_pipeline/__init__.py
+-rw-r--r--   0        0        0     1119 2023-06-02 07:04:53.636510 g_feature_pipeline-0.2.0/feature_pipeline/clean_feature_store.py
+-rw-r--r--   0        0        0      173 2023-06-02 03:43:13.960397 g_feature_pipeline-0.2.0/feature_pipeline/etl/__init__.py
+-rw-r--r--   0        0        0     1267 2023-06-02 03:43:13.960452 g_feature_pipeline-0.2.0/feature_pipeline/etl/cleaning.py
+-rw-r--r--   0        0        0     3045 2023-06-02 07:28:46.969348 g_feature_pipeline-0.2.0/feature_pipeline/etl/extract.py
+-rw-r--r--   0        0        0     3106 2023-06-02 07:27:14.975975 g_feature_pipeline-0.2.0/feature_pipeline/etl/load.py
+-rw-r--r--   0        0        0     4109 2023-06-02 07:28:46.971633 g_feature_pipeline-0.2.0/feature_pipeline/etl/validation.py
+-rw-r--r--   0        0        0     4311 2023-06-02 07:28:46.961982 g_feature_pipeline-0.2.0/feature_pipeline/feature_view.py
+-rw-r--r--   0        0        0     2691 2023-06-02 09:12:34.100668 g_feature_pipeline-0.2.0/feature_pipeline/pipeline.py
+-rw-r--r--   0        0        0     1240 2023-06-03 08:22:37.811179 g_feature_pipeline-0.2.0/feature_pipeline/settings.py
+-rw-r--r--   0        0        0     1227 2023-06-02 03:43:13.960883 g_feature_pipeline-0.2.0/feature_pipeline/utils.py
+-rw-r--r--   0        0        0      600 2023-06-03 08:23:02.882633 g_feature_pipeline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 g_feature_pipeline-0.2.0/PKG-INFO
```

### Comparing `g_feature_pipeline-0.1.0/README.md` & `g_feature_pipeline-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/clean_feature_store.py` & `g_feature_pipeline-0.2.0/feature_pipeline/clean_feature_store.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/etl/cleaning.py` & `g_feature_pipeline-0.2.0/feature_pipeline/etl/cleaning.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/etl/extract.py` & `g_feature_pipeline-0.2.0/feature_pipeline/etl/extract.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/etl/load.py` & `g_feature_pipeline-0.2.0/feature_pipeline/etl/load.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/etl/validation.py` & `g_feature_pipeline-0.2.0/feature_pipeline/etl/validation.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/feature_view.py` & `g_feature_pipeline-0.2.0/feature_pipeline/feature_view.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/pipeline.py` & `g_feature_pipeline-0.2.0/feature_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/settings.py` & `g_feature_pipeline-0.2.0/feature_pipeline/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,13 +35,14 @@
     Returns:
         Path to the root directory of the project.
     """
     return Path(os.getenv("ML_PIPELINE_ROOT_DIR", default_value))
 
 
 # Set environment variables.
-os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
+if os.getenv("ML_PIPELINE_ROOT_DIR") is None:
+    os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
 ML_PIPELINE_ROOT_DIR = get_root_dir()
 OUTPUT_DIR = ML_PIPELINE_ROOT_DIR / "output"
 OUTPUT_DIR.mkdir(parents=True, exist_ok=True)
 
 SETTINGS = load_env_vars(root_dir=ML_PIPELINE_ROOT_DIR)
```

### Comparing `g_feature_pipeline-0.1.0/feature_pipeline/utils.py` & `g_feature_pipeline-0.2.0/feature_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `g_feature_pipeline-0.1.0/pyproject.toml` & `g_feature_pipeline-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "G-feature-pipeline"
-version = "0.1.0"
+name = "g-feature-pipeline"
+version = "0.2.0"
 description = ""
 authors = ["Iusztin Paul <p.e.iusztin@gmail.com>", "Kurtis Pykes <kurtispykes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "feature_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `g_feature_pipeline-0.1.0/PKG-INFO` & `g_feature_pipeline-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g-feature-pipeline
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Iusztin Paul
 Author-email: p.e.iusztin@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: fire (>=0.5.0,<0.6.0)
```

