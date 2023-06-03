# Comparing `tmp/torchtnt-nightly-2023.6.1.tar.gz` & `tmp/torchtnt-nightly-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchtnt-nightly-2023.6.1.tar", last modified: Thu Jun  1 11:23:50 2023, max compression
+gzip compressed data, was "dist/torchtnt-nightly-2023.6.2.tar", last modified: Fri Jun  2 11:23:08 2023, max compression
```

## Comparing `torchtnt-nightly-2023.6.1.tar` & `torchtnt-nightly-2023.6.2.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-02 11:21:40.000000 torchtnt-nightly-2023.6.2/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:23:08.000000 torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.6.1/LICENSE` & `torchtnt-nightly-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/PKG-INFO` & `torchtnt-nightly-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.1 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.2 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.6.1/README.md` & `torchtnt-nightly-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/setup.py` & `torchtnt-nightly-2023.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/auto_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,19 +211,20 @@
         detect_anomaly: whether to enable anomaly detection for the autograd engine https://pytorch.org/docs/stable/autograd.html#anomaly-detection
         clip_grad_norm: max norm of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_norm_.html
         clip_grad_value: max value of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_value_.html
         swa_params: params for stochastic weight averaging https://pytorch.org/docs/stable/optim.html#stochastic-weight-averaging
         torchdynamo_params: params for TorchDynamo https://pytorch.org/docs/stable/dynamo/index.html
         training: if True, the optimizer and optionally LR scheduler will be created after the class is initialized.
 
-            Note:
-                Stochastic Weight Averaging is currently not supported with the FSDP strategy.
+    Note:
+        Stochastic Weight Averaging is currently not supported with the FSDP strategy.
+
+    Note:
+        TorchDynamo support is only available in PyTorch 2.0 or higher.
 
-            Note:
-                TorchDynamo support is only available in PyTorch 2.0 or higher.
     """
 
     def __init__(
         self,
         *,
         module: torch.nn.Module,
         device: Optional[torch.device] = None,
```

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/state.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/train.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.6.2/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,29 @@
     get_global_rank,
     get_process_group_backend_from_device,
     get_world_size,
     PGWrapper,
     sync_bool,
 )
 from .early_stop_checker import EarlyStopChecker
-from .env import init_from_env
+from .env import init_from_env, seed
 from .fsspec import get_filesystem
 from .lr_scheduler import TLRScheduler
 from .memory import get_tensor_size_bytes_map, measure_rss_deltas, RSSProfiler
 from .misc import days_to_secs, transfer_batch_norm_stats, transfer_weights
 from .oom import is_out_of_cpu_memory, is_out_of_cuda_memory, is_out_of_memory_error
 from .progress import Progress
 from .rank_zero_log import (
     rank_zero_critical,
     rank_zero_debug,
     rank_zero_error,
     rank_zero_info,
     rank_zero_print,
     rank_zero_warn,
 )
-from .seed import seed
 from .timer import FullSyncPeriodicTimer, get_timer_summary, Timer
 from .version import (
     get_python_version,
     get_torch_version,
     is_torch_version_ge_1_13_1,
     is_torch_version_geq_1_10,
     is_torch_version_geq_1_11,
@@ -68,14 +67,15 @@
     "get_global_rank",
     "get_process_group_backend_from_device",
     "get_world_size",
     "PGWrapper",
     "sync_bool",
     "EarlyStopChecker",
     "init_from_env",
+    "seed",
     "get_filesystem",
     "get_tensor_size_bytes_map",
     "measure_rss_deltas",
     "RSSProfiler",
     "days_to_secs",
     "is_out_of_cpu_memory",
     "is_out_of_cuda_memory",
@@ -83,15 +83,14 @@
     "Progress",
     "rank_zero_critical",
     "rank_zero_debug",
     "rank_zero_error",
     "rank_zero_info",
     "rank_zero_print",
     "rank_zero_warn",
-    "seed",
     "FullSyncPeriodicTimer",
     "get_timer_summary",
     "transfer_batch_norm_stats",
     "transfer_weights",
     "Timer",
     "TLRScheduler",
     "get_python_version",
```

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/device.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,25 @@
     """
     Simple logger for TensorBoard.
 
     On construction, the logger creates a new events file that logs
     will be written to.  If the environment variable `RANK` is defined,
     logger will only log if RANK = 0.
 
-    NOTE: If using the logger with distributed training:
-    - This logger can call collective operations
-    - Logs will be written on rank 0 only
-    - Logger must be constructed synchronously *after* initializing distributed process group.
+    Note:
+        If using this logger with distributed training:
+
+        - This logger can call collective operations
+        - Logs will be written on rank 0 only
+        - Logger must be constructed synchronously *after* initializing the distributed process group.
 
     Args:
         path (str): path to write logs to
-        *args, **kwargs: Extra arguments to pass to SummaryWriter
+        *args: Extra positional arguments to pass to SummaryWriter
+        **kwargs: Extra keyword arguments to pass to SummaryWriter
 
     Examples::
 
         from torchtnt.utils.loggers import TensorBoardLogger
         logger = TensorBoardLogger()
         logger.log("accuracy", 23.56, 10)
         logger.close()
```

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt/utils/version.py` & `torchtnt-nightly-2023.6.2/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.1 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.2 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.6.2/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
 torchtnt/utils/memory.py
 torchtnt/utils/misc.py
 torchtnt/utils/oom.py
 torchtnt/utils/progress.py
 torchtnt/utils/rank_zero_log.py
-torchtnt/utils/seed.py
 torchtnt/utils/test_utils.py
 torchtnt/utils/timer.py
 torchtnt/utils/version.py
 torchtnt/utils/data/__init__.py
 torchtnt/utils/data/data_prefetcher.py
 torchtnt/utils/data/iterators.py
 torchtnt/utils/data/multi_dataloader.py
```

