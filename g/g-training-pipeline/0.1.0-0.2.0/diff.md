# Comparing `tmp/g_training_pipeline-0.1.0.tar.gz` & `tmp/g_training_pipeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g_training_pipeline-0.1.0.tar", max compression
+gzip compressed data, was "g_training_pipeline-0.2.0.tar", max compression
```

## Comparing `g_training_pipeline-0.1.0.tar` & `g_training_pipeline-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2983 2023-06-02 09:30:16.441912 g_training_pipeline-0.1.0/README.md
--rw-r--r--   0        0        0      640 2023-06-02 12:32:18.408018 g_training_pipeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 03:43:13.968582 g_training_pipeline-0.1.0/training_pipeline/__init__.py
--rw-r--r--   0        0        0     2216 2023-06-02 09:20:08.027298 g_training_pipeline-0.1.0/training_pipeline/best_config.py
--rw-r--r--   0        0        0       49 2023-06-02 03:43:13.968701 g_training_pipeline-0.1.0/training_pipeline/configs/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-02 10:03:43.501313 g_training_pipeline-0.1.0/training_pipeline/configs/gridsearch.py
--rw-r--r--   0        0        0     4112 2023-06-02 09:26:07.447802 g_training_pipeline-0.1.0/training_pipeline/data.py
--rw-r--r--   0        0        0     5661 2023-06-02 09:15:04.394231 g_training_pipeline-0.1.0/training_pipeline/hyperparameter_tuning.py
--rw-r--r--   0        0        0     2162 2023-06-02 09:15:04.383507 g_training_pipeline-0.1.0/training_pipeline/models.py
--rw-r--r--   0        0        0     1324 2023-06-02 10:22:33.016142 g_training_pipeline-0.1.0/training_pipeline/settings.py
--rw-r--r--   0        0        0    13173 2023-06-02 10:12:30.941900 g_training_pipeline-0.1.0/training_pipeline/train.py
--rw-r--r--   0        0        0     1268 2023-06-02 03:43:13.969125 g_training_pipeline-0.1.0/training_pipeline/transformers.py
--rw-r--r--   0        0        0      285 2023-06-02 09:35:40.841913 g_training_pipeline-0.1.0/training_pipeline/typings.py
--rw-r--r--   0        0        0     3352 2023-06-02 09:21:55.043274 g_training_pipeline-0.1.0/training_pipeline/utils.py
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 g_training_pipeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2947 2023-06-03 02:12:16.087795 g_training_pipeline-0.2.0/README.md
+-rw-r--r--   0        0        0      640 2023-06-03 04:26:39.117088 g_training_pipeline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 03:43:13.968582 g_training_pipeline-0.2.0/training_pipeline/__init__.py
+-rw-r--r--   0        0        0     2216 2023-06-02 09:20:08.027298 g_training_pipeline-0.2.0/training_pipeline/best_config.py
+-rw-r--r--   0        0        0       49 2023-06-02 03:43:13.968701 g_training_pipeline-0.2.0/training_pipeline/configs/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-02 10:03:43.501313 g_training_pipeline-0.2.0/training_pipeline/configs/gridsearch.py
+-rw-r--r--   0        0        0     4112 2023-06-02 09:26:07.447802 g_training_pipeline-0.2.0/training_pipeline/data.py
+-rw-r--r--   0        0        0     5661 2023-06-02 09:15:04.394231 g_training_pipeline-0.2.0/training_pipeline/hyperparameter_tuning.py
+-rw-r--r--   0        0        0     2162 2023-06-02 09:15:04.383507 g_training_pipeline-0.2.0/training_pipeline/models.py
+-rw-r--r--   0        0        0     1331 2023-06-03 02:12:44.715738 g_training_pipeline-0.2.0/training_pipeline/settings.py
+-rw-r--r--   0        0        0    13173 2023-06-02 10:12:30.941900 g_training_pipeline-0.2.0/training_pipeline/train.py
+-rw-r--r--   0        0        0     1268 2023-06-02 03:43:13.969125 g_training_pipeline-0.2.0/training_pipeline/transformers.py
+-rw-r--r--   0        0        0      285 2023-06-02 09:35:40.841913 g_training_pipeline-0.2.0/training_pipeline/typings.py
+-rw-r--r--   0        0        0     3352 2023-06-02 09:21:55.043274 g_training_pipeline-0.2.0/training_pipeline/utils.py
+-rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 g_training_pipeline-0.2.0/PKG-INFO
```

### Comparing `g_training_pipeline-0.1.0/README.md` & `g_training_pipeline-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # Training Pipeline
 
 Check out this
 [Medium article](https://medium.com/towards-data-science/a-guide-to-building-effective-training-pipelines-for-maximum-results-6fdaef594cee)
 for more details about this module.
 
-## Install for Development
-
-```shell
-~/energy-forecasting                   $ cd training-pipeline && rm poetry.lock
-~/energy-forecasting/training-pipeline $ bash ../scripts/devops/virtual_environment/poetry_install.sh
-~/energy-forecasting/training-pipeline $ source .venv/bin/activate
-```
-
-Check the
-[Set Up Additional Tools](https://github.com/iusztinpaul/energy-forecasting#-set-up-additional-tools-)
-and [Usage](https://github.com/iusztinpaul/energy-forecasting#usage) sections to
-see **how to set up** the **additional tools** and **credentials** you need to
-run this project.
-
 ## Create Environment File
 
 ```shell
-~/energy-forecasting/training-pipeline $ cp .env.default .env
+~/energy-forecasting $ cp .env.default .env
 ```
 
 The command `cp .env.default .env` is used to create a copy of the
 `.env.default` file and name it `.env`. In many projects, the `.env` file is
 used to store environment variables that the application needs to run. The
 `.env.default` file is usually a template that includes all the environment
 variables that the application expects, but with default values. By copying it
 to `.env`, you can customize these values for your own environment.
 
 ## Set Up the ML_PIPELINE_ROOT_DIR Variable
 
 ```shell
-~/energy-forecasting/training-pipeline $ export ML_PIPELINE_ROOT_DIR=$(pwd)
+~/energy-forecasting $ export ML_PIPELINE_ROOT_DIR=$(pwd)
 ```
 
 The command `export ML_PIPELINE_ROOT_DIR=$(pwd)` is setting the value of the
 `ML_PIPELINE_ROOT_DIR` environment variable to the current directory. In this
 context, `$(pwd)` is a command substitution that gets replaced with the output
 of the `pwd` command, which prints the path of the current directory. The
 `export` command then makes this variable available to child processes of the
 current shell.
 
 In essence, `ML_PIPELINE_ROOT_DIR` is an environment variable that is set to the
 path of the current directory. This can be useful for scripts or programs that
 need to reference the root directory of the ML pipeline, as they can simply
 refer to `ML_PIPELINE_ROOT_DIR` instead of needing to know the exact path.
 
+## Install for Development
+
+```shell
+~/energy-forecasting                   $ cd training-pipeline && rm poetry.lock
+~/energy-forecasting/training-pipeline $ bash ../scripts/devops/virtual_environment/poetry_install.sh
+~/energy-forecasting/training-pipeline $ source .venv/bin/activate
+```
+
+Check the
+[Set Up Additional Tools](https://github.com/iusztinpaul/energy-forecasting#-set-up-additional-tools-)
+and [Usage](https://github.com/iusztinpaul/energy-forecasting#usage) sections to
+see **how to set up** the **additional tools** and **credentials** you need to
+run this project.
+
 ## Usage for Development
 
 **Run the scripts in the following order:**
 
 1. Start the hyperparameter tuning script:
 
     ```shell
```

### Comparing `g_training_pipeline-0.1.0/pyproject.toml` & `g_training_pipeline-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "g-training-pipeline"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Iusztin Paul <p.e.iusztin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "training_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `g_training_pipeline-0.1.0/training_pipeline/best_config.py` & `g_training_pipeline-0.2.0/training_pipeline/best_config.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/configs/gridsearch.py` & `g_training_pipeline-0.2.0/training_pipeline/configs/gridsearch.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/data.py` & `g_training_pipeline-0.2.0/training_pipeline/data.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/hyperparameter_tuning.py` & `g_training_pipeline-0.2.0/training_pipeline/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/models.py` & `g_training_pipeline-0.2.0/training_pipeline/models.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/settings.py` & `g_training_pipeline-0.2.0/training_pipeline/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
         Path to the root directory of the project.
     """
 
     return Path(os.getenv("ML_PIPELINE_ROOT_DIR", default_value))
 
 
 # Set environment variables.
-os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd())
+os.environ["ML_PIPELINE_ROOT_DIR"] = str(Path.cwd().parent)
 
 ML_PIPELINE_ROOT_DIR = get_root_dir()
 OUTPUT_DIR = ML_PIPELINE_ROOT_DIR / "output"
 OUTPUT_DIR.mkdir(parents=True, exist_ok=True)
 
 SETTINGS = load_env_vars(root_dir=ML_PIPELINE_ROOT_DIR)
```

### Comparing `g_training_pipeline-0.1.0/training_pipeline/train.py` & `g_training_pipeline-0.2.0/training_pipeline/train.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/transformers.py` & `g_training_pipeline-0.2.0/training_pipeline/transformers.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/training_pipeline/utils.py` & `g_training_pipeline-0.2.0/training_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `g_training_pipeline-0.1.0/PKG-INFO` & `g_training_pipeline-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g-training-pipeline
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Iusztin Paul
 Author-email: p.e.iusztin@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==3.0.1)
@@ -21,59 +21,59 @@
 
 # Training Pipeline
 
 Check out this
 [Medium article](https://medium.com/towards-data-science/a-guide-to-building-effective-training-pipelines-for-maximum-results-6fdaef594cee)
 for more details about this module.
 
-## Install for Development
-
-```shell
-~/energy-forecasting                   $ cd training-pipeline && rm poetry.lock
-~/energy-forecasting/training-pipeline $ bash ../scripts/devops/virtual_environment/poetry_install.sh
-~/energy-forecasting/training-pipeline $ source .venv/bin/activate
-```
-
-Check the
-[Set Up Additional Tools](https://github.com/iusztinpaul/energy-forecasting#-set-up-additional-tools-)
-and [Usage](https://github.com/iusztinpaul/energy-forecasting#usage) sections to
-see **how to set up** the **additional tools** and **credentials** you need to
-run this project.
-
 ## Create Environment File
 
 ```shell
-~/energy-forecasting/training-pipeline $ cp .env.default .env
+~/energy-forecasting $ cp .env.default .env
 ```
 
 The command `cp .env.default .env` is used to create a copy of the
 `.env.default` file and name it `.env`. In many projects, the `.env` file is
 used to store environment variables that the application needs to run. The
 `.env.default` file is usually a template that includes all the environment
 variables that the application expects, but with default values. By copying it
 to `.env`, you can customize these values for your own environment.
 
 ## Set Up the ML_PIPELINE_ROOT_DIR Variable
 
 ```shell
-~/energy-forecasting/training-pipeline $ export ML_PIPELINE_ROOT_DIR=$(pwd)
+~/energy-forecasting $ export ML_PIPELINE_ROOT_DIR=$(pwd)
 ```
 
 The command `export ML_PIPELINE_ROOT_DIR=$(pwd)` is setting the value of the
 `ML_PIPELINE_ROOT_DIR` environment variable to the current directory. In this
 context, `$(pwd)` is a command substitution that gets replaced with the output
 of the `pwd` command, which prints the path of the current directory. The
 `export` command then makes this variable available to child processes of the
 current shell.
 
 In essence, `ML_PIPELINE_ROOT_DIR` is an environment variable that is set to the
 path of the current directory. This can be useful for scripts or programs that
 need to reference the root directory of the ML pipeline, as they can simply
 refer to `ML_PIPELINE_ROOT_DIR` instead of needing to know the exact path.
 
+## Install for Development
+
+```shell
+~/energy-forecasting                   $ cd training-pipeline && rm poetry.lock
+~/energy-forecasting/training-pipeline $ bash ../scripts/devops/virtual_environment/poetry_install.sh
+~/energy-forecasting/training-pipeline $ source .venv/bin/activate
+```
+
+Check the
+[Set Up Additional Tools](https://github.com/iusztinpaul/energy-forecasting#-set-up-additional-tools-)
+and [Usage](https://github.com/iusztinpaul/energy-forecasting#usage) sections to
+see **how to set up** the **additional tools** and **credentials** you need to
+run this project.
+
 ## Usage for Development
 
 **Run the scripts in the following order:**
 
 1. Start the hyperparameter tuning script:
 
     ```shell
```

