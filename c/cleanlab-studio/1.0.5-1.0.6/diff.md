# Comparing `tmp/cleanlab-studio-1.0.5.tar.gz` & `tmp/cleanlab-studio-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.5.tar", last modified: Fri May 12 20:04:29 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.6.tar", last modified: Sat Jun  3 04:37:22 2023, max compression
```

## Comparing `cleanlab-studio-1.0.5.tar` & `cleanlab-studio-1.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.271629 cleanlab-studio-1.0.6/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.275629 cleanlab-studio-1.0.6/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.275629 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.5/LICENSE` & `cleanlab-studio-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/PKG-INFO` & `cleanlab-studio-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.5
+Version: 1.0.6
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.0.5/README.md` & `cleanlab-studio-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.6/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.6/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,19 @@
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     status: JSONDict = res.json()
     return status
 
 
+def delete_project(api_key: str, project_id: str) -> None:
+    res = requests.delete(project_base_url + f"/{project_id}", headers=_construct_headers(api_key))
+    handle_api_error(res)
+
+
 def poll_progress(
     progress_id: str, request_function: Callable[[str], JSONDict], description: str
 ) -> JSONDict:
     with tqdm(total=1, desc=description, bar_format="{desc}: {percentage:3.0f}%|{bar}|") as pbar:
         res = request_function(progress_id)
         while res["status"] != "complete":
             if res["status"] == "error":
```

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.6/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/studio/clean.py` & `cleanlab-studio-1.0.6/cleanlab_studio/studio/clean.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.6/cleanlab_studio/studio/studio.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,19 +109,28 @@
             cleanset_id, project_id, label_column, include_action=True
         )
         if pyspark_exists and isinstance(dataset, pyspark.sql.DataFrame):
             from pyspark.sql.functions import udf
 
             spark = dataset.sparkSession
             cl_cols_df = spark.createDataFrame(cl_cols)
-            # XXX this does not handle excluded columns correctly, because the API
-            # returns all rows regardless and doesn't let us distinguish between
-            # excluded and non-excluded rows
+            corrected_ds = dataset.alias("corrected_ds")
+            if id_col not in corrected_ds.columns:
+                from pyspark.sql.functions import (
+                    row_number,
+                    monotonically_increasing_id,
+                )
+                from pyspark.sql.window import Window
+
+                corrected_ds = corrected_ds.withColumn(
+                    id_col,
+                    row_number().over(Window.orderBy(monotonically_increasing_id())) - 1,
+                )
             both = cl_cols_df.select([id_col, "action", "cleanlab_clean_label"]).join(
-                dataset.select([id_col, label_column]),
+                corrected_ds.select([id_col, label_column]),
                 on=id_col,
                 how="left",
             )
             final = both.withColumn(
                 "__cleanlab_final_label",
                 # XXX hacky, relies on no labels being "None" (the string)
                 # instead, use original JSON, which uses null values where it's not specified
@@ -129,33 +138,40 @@
                     both[label_column],
                     "cleanlab_clean_label",
                 ),
             )
             new_labels = final.select(
                 [id_col, "action", "__cleanlab_final_label"]
             ).withColumnRenamed("__cleanlab_final_label", label_column)
-            corrected_df = (
-                dataset.drop(label_column)
+            return (
+                corrected_ds.drop(label_column)
                 .join(new_labels, on=id_col, how="right")
                 .where(new_labels["action"] != "exclude")
                 .drop("action")
             )
-            return corrected_df
-
         elif isinstance(dataset, pd.DataFrame):
-            joined_ds = dataset.join(cl_cols.set_index(id_col), on=id_col)
+            joined_ds: pd.DataFrame
+            if id_col in dataset.columns:
+                joined_ds = dataset.join(cl_cols.set_index(id_col), on=id_col)
+            else:
+                joined_ds = dataset.join(cl_cols.set_index(id_col).sort_values(by=id_col))
             joined_ds["__cleanlab_final_label"] = joined_ds["cleanlab_clean_label"].where(
                 joined_ds["cleanlab_clean_label"] != "None", dataset[label_column]
             )
 
             corrected_ds = dataset.copy()
             corrected_ds[label_column] = joined_ds["__cleanlab_final_label"]
             corrected_ds = corrected_ds[joined_ds["action"] != "exclude"]
             return corrected_ds
 
+        else:
+            raise ValueError(
+                f"Provided unsupported dataset of type: {type(dataset)}. We currently support applying corrections to pandas or pyspark dataframes"
+            )
+
     def create_project(
         self,
         dataset_id: str,
         project_name: str,
         modality: Literal["text", "tabular", "image"],
         *,
         task_type: Literal["multi-class", "multi-label"] = "multi-class",
@@ -229,7 +245,12 @@
         :return: True if cleanset is ready, False otherwise
         """
         return clean.poll_cleanset_status(self._api_key, cleanset_id, timeout)
 
     def get_latest_cleanset_id(self, project_id: str) -> str:
         """Gets latest cleanset ID for a project"""
         return api.get_latest_cleanset_id(self._api_key, project_id)
+
+    def delete_project(self, project_id: str) -> None:
+        """Deletes project with given ID"""
+        api.delete_project(self._api_key, project_id)
+        print(f"Successfully deleted project: {project_id}")
```

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.6/cleanlab_studio/studio/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 ) -> str:
     upload_id = upload_dataset_file(api_key, dataset_source)
     schema = get_proposed_schema(api_key, upload_id)
 
     if (schema is None or schema.get("immutable", False)) and (
         schema_overrides is not None or modality is not None or id_column is not None
     ):
-        print(
-            "Warning: schema_overrides, modality, and id_column parameters will be ignored for simple zip uploads"
+        raise ValueError(
+            "Schema_overrides, modality, and id_column parameters cannot be provided for simple zip uploads"
         )
 
     if schema is not None and not schema.get("immutable", False):
         schema["metadata"]["name"] = dataset_source.dataset_name
         if schema_overrides is not None:
             for field in schema_overrides:
                 schema["fields"][field] = schema_overrides[field]
```

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.6/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.5
+Version: 1.0.6
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.0.5/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.6/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/setup.py` & `cleanlab-studio-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/tests/bench.py` & `cleanlab-studio-1.0.6/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.6/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.6/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.6/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.5/tests/datasets/utils.py` & `cleanlab-studio-1.0.6/tests/datasets/utils.py`

 * *Files identical despite different names*

