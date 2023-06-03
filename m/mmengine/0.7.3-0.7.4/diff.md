# Comparing `tmp/mmengine-0.7.3.tar.gz` & `tmp/mmengine-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.7.3.tar", last modified: Fri Apr 28 07:14:41 2023, max compression
+gzip compressed data, was "dist/mmengine-0.7.4.tar", last modified: Sat Jun  3 15:55:57 2023, max compression
```

## Comparing `mmengine-0.7.3.tar` & `mmengine-0.7.4.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 07:13:18.000000 mmengine-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-28 07:14:41.000000 mmengine-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-04-28 07:13:18.000000 mmengine-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27397 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    63458 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    25968 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30321 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24176 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   100487 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30072 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 07:14:41.000000 mmengine-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-28 07:13:18.000000 mmengine-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-03 15:54:29.000000 mmengine-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-06-03 15:55:57.000000 mmengine-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-03 15:54:29.000000 mmengine-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29215 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63464 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25968 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100622 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36462 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-03 15:55:57.000000 mmengine-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-03 15:54:29.000000 mmengine-0.7.4/setup.py
```

### Comparing `mmengine-0.7.3/PKG-INFO` & `mmengine-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.7.3
+Version: 0.7.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -84,22 +84,22 @@
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
         ## What's New
         
-        v0.7.3 was released on 2023-04-28.
+        v0.7.4 was released on 2023-06-03.
         
         ### Highlights
         
-        - Support using MLflow to record experiment data
-        - Support registering callable objects to the registry
+        - Support using [`ClearML`](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) to record experiment data
+        - Add [`Sophia`](https://mmengine.readthedocs.io/en/latest/common_usage/better_optimizers.html#sophia) optimizers
         
-        Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v074-06032023) for more details.
         
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
```

### Comparing `mmengine-0.7.3/README.md` & `mmengine-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,22 @@
 
    - Defines the training process just like playing with Legos.
    - Provides rich components and strategies.
    - Complete controls on the training process with different levels of APIs.
 
 ## What's New
 
-v0.7.3 was released on 2023-04-28.
+v0.7.4 was released on 2023-06-03.
 
 ### Highlights
 
-- Support using MLflow to record experiment data
-- Support registering callable objects to the registry
+- Support using [`ClearML`](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) to record experiment data
+- Add [`Sophia`](https://mmengine.readthedocs.io/en/latest/common_usage/better_optimizers.html#sophia) optimizers
 
-Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
+Read [Changelog](./docs/en/notes/changelog.md#v074-06032023) for more details.
 
 ## Installation
 
 Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
 
 Install MMEngine
```

### Comparing `mmengine-0.7.3/mmengine/analysis/complexity_analysis.py` & `mmengine-0.7.4/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/analysis/jit_analysis.py` & `mmengine-0.7.4/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/analysis/jit_handles.py` & `mmengine-0.7.4/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/analysis/print_helper.py` & `mmengine-0.7.4/mmengine/analysis/print_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,22 +721,23 @@
     """
     if input_shape is None and inputs is None:
         raise ValueError('One of "input_shape" and "inputs" should be set.')
     elif input_shape is not None and inputs is not None:
         raise ValueError('"input_shape" and "inputs" cannot be both set.')
 
     if inputs is None:
+        device = next(model.parameters()).device
         if is_tuple_of(input_shape, int):  # tuple of int, construct one tensor
-            inputs = (torch.randn(1, *input_shape), )
+            inputs = (torch.randn(1, *input_shape).to(device), )
         elif is_tuple_of(input_shape, tuple) and all([
                 is_tuple_of(one_input_shape, int)
                 for one_input_shape in input_shape  # type: ignore
         ]):  # tuple of tuple of int, construct multiple tensors
             inputs = tuple([
-                torch.randn(1, *one_input_shape)
+                torch.randn(1, *one_input_shape).to(device)
                 for one_input_shape in input_shape  # type: ignore
             ])
         else:
             raise ValueError(
                 '"input_shape" should be either a `tuple of int` (to construct'
                 'one input tensor) or a `tuple of tuple of int` (to construct'
                 'multiple input tensors).')
```

### Comparing `mmengine-0.7.3/mmengine/config/config.py` & `mmengine-0.7.4/mmengine/config/config.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/config/utils.py` & `mmengine-0.7.4/mmengine/config/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dataset/__init__.py` & `mmengine-0.7.4/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dataset/base_dataset.py` & `mmengine-0.7.4/mmengine/dataset/base_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import functools
 import gc
 import logging
-import os.path as osp
 import pickle
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from torch.utils.data import Dataset
 
-from mmengine.fileio import list_from_file, load
+from mmengine.fileio import join_path, list_from_file, load
 from mmengine.logging import print_log
 from mmengine.registry import TRANSFORMS
 from mmengine.utils import is_abs
 
 
 class Compose:
     """Compose multiple transforms sequentially.
@@ -151,25 +150,24 @@
                   }
                 ]
               },
             ]
         }
 
     Args:
-        ann_file (str): Annotation file path. Defaults to ''.
+        ann_file (str, optional): Annotation file path. Defaults to ''.
         metainfo (dict, optional): Meta information for dataset, such as class
             information. Defaults to None.
-        data_root (str): The root directory for ``data_prefix`` and
+        data_root (str, optional): The root directory for ``data_prefix`` and
             ``ann_file``. Defaults to ''.
         data_prefix (dict): Prefix for training data. Defaults to
             dict(img_path='').
         filter_cfg (dict, optional): Config for filter data. Defaults to None.
         indices (int or Sequence[int], optional): Support using first few
             data in annotation file to facilitate training/testing on a smaller
-            dataset. Defaults to None which means using all ``data_infos``.
         serialize_data (bool, optional): Whether to hold memory using
             serialized objects, when enabled, data loader workers can use
             shared RAM from master process instead of making a copy. Defaults
             to True.
         pipeline (list, optional): Processing pipeline. Defaults to [].
         test_mode (bool, optional): ``test_mode=True`` means in test phase.
             Defaults to False.
@@ -210,40 +208,37 @@
         {'task_name': custom_task_name, dataset_type: custom_type}
     """
 
     METAINFO: dict = dict()
     _fully_initialized: bool = False
 
     def __init__(self,
-                 ann_file: str = '',
+                 ann_file: Optional[str] = '',
                  metainfo: Optional[dict] = None,
-                 data_root: str = '',
+                 data_root: Optional[str] = '',
                  data_prefix: dict = dict(img_path=''),
                  filter_cfg: Optional[dict] = None,
                  indices: Optional[Union[int, Sequence[int]]] = None,
                  serialize_data: bool = True,
                  pipeline: List[Union[dict, Callable]] = [],
                  test_mode: bool = False,
                  lazy_init: bool = False,
                  max_refetch: int = 1000):
-
+        self.ann_file = ann_file
+        self._metainfo = self._load_metainfo(copy.deepcopy(metainfo))
         self.data_root = data_root
         self.data_prefix = copy.copy(data_prefix)
-        self.ann_file = ann_file
         self.filter_cfg = copy.deepcopy(filter_cfg)
         self._indices = indices
         self.serialize_data = serialize_data
         self.test_mode = test_mode
         self.max_refetch = max_refetch
         self.data_list: List[dict] = []
         self.data_bytes: np.ndarray
 
-        # Set meta information.
-        self._metainfo = self._load_metainfo(copy.deepcopy(metainfo))
-
         # Join paths.
         self._join_prefix()
 
         # Build pipeline.
         self.pipeline = Compose(pipeline)
         # Full initialize the dataset.
         if not lazy_init:
@@ -335,16 +330,16 @@
         Returns:
             list or list[dict]: Parsed annotation.
         """
         for prefix_key, prefix in self.data_prefix.items():
             assert prefix_key in raw_data_info, (
                 f'raw_data_info: {raw_data_info} dose not contain prefix key'
                 f'{prefix_key}, please check your data_prefix.')
-            raw_data_info[prefix_key] = osp.join(prefix,
-                                                 raw_data_info[prefix_key])
+            raw_data_info[prefix_key] = join_path(prefix,
+                                                  raw_data_info[prefix_key])
         return raw_data_info
 
     def filter_data(self) -> List[dict]:
         """Filter annotations according to filter_cfg. Defaults return all
         ``data_list``.
 
         If some ``data_list`` could be filtered according to specific logic,
@@ -535,28 +530,26 @@
             >>> self.data_prefix
             dict(img='/d/e')
             >>> self.ann_file
             'a/b/c/f'
         """
         # Automatically join annotation file path with `self.root` if
         # `self.ann_file` is not an absolute path.
-        if not is_abs(self.ann_file) and self.ann_file:
-            self.ann_file = osp.join(self.data_root, self.ann_file)
+        if self.ann_file and not is_abs(self.ann_file) and self.data_root:
+            self.ann_file = join_path(self.data_root, self.ann_file)
         # Automatically join data directory with `self.root` if path value in
         # `self.data_prefix` is not an absolute path.
         for data_key, prefix in self.data_prefix.items():
-            if isinstance(prefix, str):
-                if not is_abs(prefix):
-                    self.data_prefix[data_key] = osp.join(
-                        self.data_root, prefix)
-                else:
-                    self.data_prefix[data_key] = prefix
-            else:
+            if not isinstance(prefix, str):
                 raise TypeError('prefix should be a string, but got '
                                 f'{type(prefix)}')
+            if not is_abs(prefix) and self.data_root:
+                self.data_prefix[data_key] = join_path(self.data_root, prefix)
+            else:
+                self.data_prefix[data_key] = prefix
 
     @force_full_init
     def get_subset_(self, indices: Union[Sequence[int], int]) -> None:
         """The in-place version of ``get_subset`` to convert dataset to a
         subset of original dataset.
 
         This method will convert the original dataset to a subset of dataset.
```

### Comparing `mmengine-0.7.3/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.7.4/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dataset/sampler.py` & `mmengine-0.7.4/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dataset/utils.py` & `mmengine-0.7.4/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/device/utils.py` & `mmengine-0.7.4/mmengine/device/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 import os
 from typing import Optional
 
 import torch
 
 try:
     import torch_npu  # noqa: F401
+    import torch_npu.npu.utils as npu_utils
 
     # Enable operator support for dynamic shape and
     # binary operator support on the NPU.
     npu_jit_compile = bool(os.getenv('NPUJITCompile', False))
     torch.npu.set_compile_mode(jit_compile=npu_jit_compile)
     IS_NPU_AVAILABLE = hasattr(torch, 'npu') and torch.npu.is_available()
 except Exception:
     IS_NPU_AVAILABLE = False
 
+try:
+    import torch_dipu  # noqa: F401
+    IS_DIPU_AVAILABLE = True
+except Exception:
+    IS_DIPU_AVAILABLE = False
+
 
 def get_max_cuda_memory(device: Optional[torch.device] = None) -> int:
     """Returns the maximum GPU memory occupied by tensors in megabytes (MB) for
     a given device. By default, this returns the peak allocated memory since
     the beginning of this program.
 
     Args:
@@ -58,23 +65,36 @@
     """Return True if mps devices exist.
 
     It's specialized for mac m1 chips and require torch version 1.12 or higher.
     """
     return hasattr(torch.backends, 'mps') and torch.backends.mps.is_available()
 
 
+def is_dipu_available() -> bool:
+    return IS_DIPU_AVAILABLE
+
+
+def is_npu_support_full_precision() -> bool:
+    """Returns True if npu devices support full precision training."""
+    version_of_support_full_precision = 220
+    return IS_NPU_AVAILABLE and npu_utils.get_soc_version(
+    ) >= version_of_support_full_precision
+
+
 DEVICE = 'cpu'
 if is_npu_available():
     DEVICE = 'npu'
 elif is_cuda_available():
     DEVICE = 'cuda'
 elif is_mlu_available():
     DEVICE = 'mlu'
 elif is_mps_available():
     DEVICE = 'mps'
+elif is_dipu_available():
+    DEVICE = 'dipu'
 
 
 def get_device() -> str:
     """Returns the currently existing device type.
 
     Returns:
         str: cuda | npu | mlu | mps | cpu.
```

### Comparing `mmengine-0.7.3/mmengine/dist/__init__.py` & `mmengine-0.7.4/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dist/dist.py` & `mmengine-0.7.4/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/dist/utils.py` & `mmengine-0.7.4/mmengine/dist/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/evaluator/evaluator.py` & `mmengine-0.7.4/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/evaluator/metric.py` & `mmengine-0.7.4/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/evaluator/utils.py` & `mmengine-0.7.4/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/__init__.py` & `mmengine-0.7.4/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/__init__.py` & `mmengine-0.7.4/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/base.py` & `mmengine-0.7.4/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/http_backend.py` & `mmengine-0.7.4/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.7.4/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/local_backend.py` & `mmengine-0.7.4/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.7.4/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.7.4/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.7.4/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/file_client.py` & `mmengine-0.7.4/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/handlers/base.py` & `mmengine-0.7.4/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.7.4/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.7.4/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.7.4/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.7.4/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/io.py` & `mmengine-0.7.4/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/fileio/parse.py` & `mmengine-0.7.4/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/__init__.py` & `mmengine-0.7.4/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.7.4/mmengine/hooks/checkpoint_hook.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import hashlib
 import logging
 import os.path as osp
 import pickle
+from collections import deque
 from math import inf
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Sequence, Union
 
 from mmengine.dist import is_main_process, master_only
 from mmengine.fileio import FileClient, get_file_backend
 from mmengine.logging import print_log
@@ -81,15 +82,15 @@
             name. If specified, must contain one and only one "{}", which will
             be replaced with ``epoch + 1`` if ``by_epoch=True`` else
             ``iteration + 1``.
             Defaults to None, which means "epoch_{}.pth" or "iter_{}.pth"
             accordingly.
         backend_args (dict, optional): Arguments to instantiate the
             prefix of uri corresponding backend. Defaults to None.
-            New in v0.2.0.
+            `New in version 0.2.0.`
         published_keys (str, List[str], optional): If ``save_last`` is ``True``
             or ``save_best`` is not ``None``, it will automatically
             publish model with keys in the list after training.
             Defaults to None.
             `New in version 0.7.1.`
     Examples:
         >>> # Save best based on single metric
@@ -238,14 +239,16 @@
         if isinstance(published_keys, str):
             published_keys = [published_keys]
         elif isinstance(published_keys, (list, tuple)):
             assert len(published_keys) == len(set(published_keys)), (
                 'Find duplicate elements in "published_keys".')
         self.published_keys = published_keys
 
+        self.last_ckpt = None
+
     def before_train(self, runner) -> None:
         """Finish all operations, related to checkpoint.
 
         This function will get the appropriate file client, and the directory
         to save these checkpoints of the model.
 
         Args:
@@ -290,14 +293,33 @@
                     if best_ckpt_name not in runner.message_hub.runtime_info:
                         self.best_ckpt_path_dict[key_indicator] = None
                     else:
                         self.best_ckpt_path_dict[
                             key_indicator] = runner.message_hub.get_info(
                                 best_ckpt_name)
 
+        if self.max_keep_ckpts > 0:
+            keep_ckpt_ids = []
+            if 'keep_ckpt_ids' in runner.message_hub.runtime_info:
+                keep_ckpt_ids = runner.message_hub.get_info('keep_ckpt_ids')
+
+                while len(keep_ckpt_ids) > self.max_keep_ckpts:
+                    step = keep_ckpt_ids.pop(0)
+                    if is_main_process():
+                        path = self.file_backend.join_path(
+                            self.out_dir, self.filename_tmpl.format(step))
+                        if self.file_backend.isfile(path):
+                            self.file_backend.remove(path)
+                        elif self.file_backend.isdir(path):
+                            # checkpoints saved by deepspeed are directories
+                            self.file_backend.rmtree(path)
+
+            self.keep_ckpt_ids: deque = deque(keep_ckpt_ids,
+                                              self.max_keep_ckpts)
+
     def after_train_epoch(self, runner) -> None:
         """Save the checkpoint and synchronize buffers after each epoch.
 
         Args:
             runner (Runner): The runner of the training process.
         """
         if not self.by_epoch:
@@ -333,22 +355,21 @@
 
         Args:
             runner (Runner): The runner of the training process.
         """
         if self.published_keys is None:
             return
 
-        if self.save_last and 'last_ckpt' in runner.message_hub.runtime_info:
-            last_ckpt = runner.message_hub.get_info('last_ckpt')
-            self._publish_model(runner, last_ckpt)
+        if self.save_last and self.last_ckpt is not None:
+            self._publish_model(runner, self.last_ckpt)
 
         if getattr(self, 'best_ckpt_path', None) is not None:
             self._publish_model(runner, str(self.best_ckpt_path))
         if getattr(self, 'best_ckpt_path_dict', None) is not None:
-            for key, best_ckpt in self.best_ckpt_path_dict.items():
+            for best_ckpt in self.best_ckpt_path_dict.values():
                 self._publish_model(runner, best_ckpt)
 
     @master_only
     def _publish_model(self, runner, ckpt_path: str) -> None:
         """Remove unnecessary keys from ckpt_path and save the new checkpoint.
 
         Args:
@@ -375,65 +396,78 @@
         final_path = osp.splitext(ckpt_path)[0] + f'-{sha[:8]}.pth'
         save_checkpoint(checkpoint, final_path)
         print_log(
             f'The checkpoint ({ckpt_path}) is published to '
             f'{final_path}.',
             logger='current')
 
-    def _save_checkpoint(self, runner) -> None:
-        """Save the current checkpoint and delete outdated checkpoint.
-
-        Args:
-            runner (Runner): The runner of the training process.
-        """
-        if self.by_epoch:
-            ckpt_filename = self.filename_tmpl.format(runner.epoch + 1)
-        else:
-            ckpt_filename = self.filename_tmpl.format(runner.iter + 1)
+    def _save_checkpoint_with_step(self, runner, step, meta):
+        # remove other checkpoints before save checkpoint to make the
+        # self.keep_ckpt_ids are saved as expected
+        if self.max_keep_ckpts > 0:
+            # _save_checkpoint and _save_best_checkpoint may call this
+            # _save_checkpoint_with_step in one epoch
+            if len(self.keep_ckpt_ids) > 0 and self.keep_ckpt_ids[-1] == step:
+                pass
+            else:
+                if len(self.keep_ckpt_ids) == self.max_keep_ckpts:
+                    _step = self.keep_ckpt_ids.popleft()
+                    if is_main_process():
+                        ckpt_path = self.file_backend.join_path(
+                            self.out_dir, self.filename_tmpl.format(_step))
+
+                        if self.file_backend.isfile(ckpt_path):
+                            self.file_backend.remove(ckpt_path)
+                        elif self.file_backend.isdir(ckpt_path):
+                            # checkpoints saved by deepspeed are directories
+                            self.file_backend.rmtree(ckpt_path)
+
+                self.keep_ckpt_ids.append(step)
+                runner.message_hub.update_info('keep_ckpt_ids',
+                                               list(self.keep_ckpt_ids))
+
+        ckpt_filename = self.filename_tmpl.format(step)
+        self.last_ckpt = self.file_backend.join_path(self.out_dir,
+                                                     ckpt_filename)
+        runner.message_hub.update_info('last_ckpt', self.last_ckpt)
 
         runner.save_checkpoint(
             self.out_dir,
             ckpt_filename,
             self.file_client_args,
             save_optimizer=self.save_optimizer,
             save_param_scheduler=self.save_param_scheduler,
+            meta=meta,
             by_epoch=self.by_epoch,
             backend_args=self.backend_args,
             **self.args)
 
         # Model parallel-like training should involve pulling sharded states
         # from all ranks, but skip the following procedure.
         if not is_main_process():
             return
 
-        runner.message_hub.update_info(
-            'last_ckpt',
-            self.file_backend.join_path(self.out_dir, ckpt_filename))
-
-        # remove other checkpoints
-        if self.max_keep_ckpts > 0:
-            if self.by_epoch:
-                current_ckpt = runner.epoch + 1
-            else:
-                current_ckpt = runner.iter + 1
-            redundant_ckpts = range(
-                current_ckpt - self.max_keep_ckpts * self.interval, 0,
-                -self.interval)
-            for _step in redundant_ckpts:
-                ckpt_path = self.file_backend.join_path(
-                    self.out_dir, self.filename_tmpl.format(_step))
-                if self.file_backend.isfile(ckpt_path):
-                    self.file_backend.remove(ckpt_path)
-                else:
-                    break
-
         save_file = osp.join(runner.work_dir, 'last_checkpoint')
-        filepath = self.file_backend.join_path(self.out_dir, ckpt_filename)
         with open(save_file, 'w') as f:
-            f.write(filepath)
+            f.write(self.last_ckpt)  # type: ignore
+
+    def _save_checkpoint(self, runner) -> None:
+        """Save the current checkpoint and delete outdated checkpoint.
+
+        Args:
+            runner (Runner): The runner of the training process.
+        """
+        if self.by_epoch:
+            step = runner.epoch + 1
+            meta = dict(epoch=step, iter=runner.iter)
+        else:
+            step = runner.iter + 1
+            meta = dict(epoch=runner.epoch, iter=step)
+
+        self._save_checkpoint_with_step(runner, step, meta=meta)
 
     def _save_best_checkpoint(self, runner, metrics) -> None:
         """Save the current checkpoint and delete outdated checkpoint.
 
         Args:
             runner (Runner): The runner of the training process.
             metrics (dict): Evaluation results of all metrics.
@@ -444,18 +478,21 @@
         if self.by_epoch:
             ckpt_filename = self.filename_tmpl.format(runner.epoch)
             cur_type, cur_time = 'epoch', runner.epoch
         else:
             ckpt_filename = self.filename_tmpl.format(runner.iter)
             cur_type, cur_time = 'iter', runner.iter
 
+        meta = dict(epoch=runner.epoch, iter=runner.iter)
+
         # handle auto in self.key_indicators and self.rules before the loop
         if 'auto' in self.key_indicators:
             self._init_rule(self.rules, [list(metrics.keys())[0]])
 
+        best_ckpt_updated = False
         # save best logic
         # get score from messagehub
         for key_indicator, rule in zip(self.key_indicators, self.rules):
             key_score = metrics[key_indicator]
 
             if len(self.key_indicators) == 1:
                 best_score_key = 'best_score'
@@ -471,21 +508,26 @@
             else:
                 best_score = runner.message_hub.get_info(best_score_key)
 
             if key_score is None or not self.is_better_than[key_indicator](
                     key_score, best_score):
                 continue
 
+            best_ckpt_updated = True
+
             best_score = key_score
             runner.message_hub.update_info(best_score_key, best_score)
 
-            if best_ckpt_path and \
-               self.file_backend.isfile(best_ckpt_path) and \
-               is_main_process():
-                self.file_backend.remove(best_ckpt_path)
+            if best_ckpt_path and is_main_process():
+                if self.file_backend.isfile(best_ckpt_path):
+                    self.file_backend.remove(best_ckpt_path)
+                else:
+                    # checkpoints saved by deepspeed are directories
+                    self.file_backend.rmtree(best_ckpt_path)
+
                 runner.logger.info(
                     f'The previous best checkpoint {best_ckpt_path} '
                     'is removed')
 
             best_ckpt_name = f'best_{key_indicator}_{ckpt_filename}'
             # Replace illegal characters for filename with `_`
             best_ckpt_name = best_ckpt_name.replace('/', '_')
@@ -503,20 +545,29 @@
                     self.best_ckpt_path_dict[key_indicator])
             runner.save_checkpoint(
                 self.out_dir,
                 filename=best_ckpt_name,
                 file_client_args=self.file_client_args,
                 save_optimizer=False,
                 save_param_scheduler=False,
+                meta=meta,
                 by_epoch=False,
                 backend_args=self.backend_args)
             runner.logger.info(
                 f'The best checkpoint with {best_score:0.4f} {key_indicator} '
                 f'at {cur_time} {cur_type} is saved to {best_ckpt_name}.')
 
+        # save checkpoint again to update the best_score and best_ckpt stored
+        # in message_hub because the checkpoint saved in `after_train_epoch`
+        # or `after_train_iter` stage only keep the previous best checkpoint
+        # not the current best checkpoint which causes the current best
+        # checkpoint can not be removed when resuming training.
+        if best_ckpt_updated and self.last_ckpt is not None:
+            self._save_checkpoint_with_step(runner, cur_time, meta)
+
     def _init_rule(self, rules, key_indicators) -> None:
         """Initialize rule, key_indicator, comparison_func, and best score. If
         key_indicator is a list of string and rule is a string, all metric in
         the key_indicator will share the same rule.
 
         Here is the rule to determine which rule is used for key indicator when
         the rule is not specific (note that the key indicator matching is case-
```

### Comparing `mmengine-0.7.3/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.7.4/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/ema_hook.py` & `mmengine-0.7.4/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.7.4/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/hook.py` & `mmengine-0.7.4/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.7.4/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/logger_hook.py` & `mmengine-0.7.4/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.7.4/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.7.4/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/profiler_hook.py` & `mmengine-0.7.4/mmengine/hooks/profiler_hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,38 +44,51 @@
             `torch.profile.schedule <https://pytorch.org/docs/stable/
             profiler.html#torch.profiler.schedule>`_.
             Defaults to None, which means profiling without a schedule
         on_trace_ready (callable, dict, optional): Either a handler or a dict
             of generating handler. Defaults to None, which means profiling
             without an on_trace_ready.The Callable type needs to construct its
             own function that can handle 'torch.autograd.profiler.profile'.
-            Two officially recommended ways are provided, namely terminal
-            display or tensorboard display. The terminal display content can be
-            adjusted through 'EventList.table()'
-            from 'torch.autograd.profiler_util.py'.
-            If using tensorboard, save to '{work_dir}/tf_tracing_logs'
-            by default.
+            Two officially recommended ways are provided:
+
+            - ``schedule=dict(type='log_trace')``: Print the profiling result
+              in the terminal. See more details in the `PyTorch official tutorial`_.
+              The configurable arguments are the same as
+              ``prof.key_averages().table``
+            - ``scheduler=dict(type='tb_trace')``: Profile the performance
+              with tensorboard. See more details in the tutorial
+              `profile with tensorboard`_.
+
         record_shapes (bool): Save information about operator's input shapes.
             Defaults to False.
         profile_memory (bool): Track tensor memory allocation/deallocation.
             Defaults to False.
         with_stack (bool): Record source information (file and line number)
             for the ops. Defaults to False.
         with_flops (bool): Use formula to estimate the FLOPS of specific
             operators (matrix multiplication and 2D convolution).
             Defaults to False.
         json_trace_path (str, optional): Exports the collected trace in Chrome
             JSON format. Chrome use 'chrome://tracing' view json file.
             Defaults to None, which means profiling does not store json files.
 
+    Warnings:
+        The profiler will be closed after ``profile_times`` iterations
+        automatically. Please make sure the configuration of your scheduler
+        will not close the profiler before the iteration reach the value of
+        ``profile_times``
+
     Examples:
         >>> # tensorboard trace
         >>> trace_config = dict(type='tb_trace')
         >>> profiler_hook_cfg = dict(on_trace_ready=trace_config)
-    """
+
+    .. _PyTorch official tutorial: https://pytorch.org/tutorials/recipes/recipes/profiler_recipe.html#using-profiler-to-analyze-execution-time
+    .. _profile with tensorboard: https://pytorch.org/tutorials/intermediate/tensorboard_profiler_tutorial.html#pytorch-profiler-with-tensorboard
+    """  # noqa: E501
     priority = 'VERY_LOW'
 
     def __init__(self,
                  *,
                  by_epoch: bool = True,
                  profile_times: int = 1,
                  activity_with_cpu: bool = True,
@@ -131,16 +144,16 @@
         self.on_trace_ready = on_trace_ready
         self.record_shapes = record_shapes
         self.profile_memory = profile_memory
         self.with_stack = with_stack
         self.with_flops = with_flops
 
         self.json_trace_path = json_trace_path
+        self._closed = False
 
-    @master_only
     def before_run(self, runner):
         """Initialize the profiler.
 
         Through the runner parameter, the validity of the parameter is further
         determined.
         """
         max_times = runner.max_epochs if self.by_epoch else runner.max_iters
@@ -208,31 +221,31 @@
                                  f'"tb_trace", but got {trace_type}')
         else:
             raise ValueError(
                 '``on_trace_ready`` should be a handler, or dict, or None, '
                 f'but got {self.on_trace_ready}')
         return _on_trace_ready
 
-    @master_only
     def after_train_epoch(self, runner):
         """Determine if the content is exported."""
-        if self.by_epoch and runner.epoch == self.profile_times - 1:
+        # `after_train_epoch` will also be called in IterBasedTrainLoop.
+        # Here we check `self._closed` to avoid exiting twice.
+        if not self._closed:
             self._export_chrome_trace(runner)
 
-    @master_only
     def after_train_iter(self, runner, batch_idx, data_batch, outputs):
-        """Update the content according to the schedule, and determine if the
-        content is exported."""
-        if self.schedule is None:
+        """profiler will call `step` method if it is not closed."""
+        if not self._closed:
             self.profiler.step()
-        if not self.by_epoch and runner.iter == self.profile_times - 1:
+        if runner.iter == self.profile_times - 1 and not self.by_epoch:
             self._export_chrome_trace(runner)
 
     def _export_chrome_trace(self, runner):
         """Exporting content."""
+        self._closed = True
         runner.logger.info('profiler may take a few minutes...')
         self.profiler.__exit__(None, None, None)
         if self.json_trace_path is not None:
             self.profiler.export_chrome_trace(self.json_trace_path)
 
 
 @HOOKS.register_module()
```

### Comparing `mmengine-0.7.3/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.7.4/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.7.4/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.7.4/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.7.4/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hub/hub.py` & `mmengine-0.7.4/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hub/mmcls.json` & `mmengine-0.7.4/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hub/openmmlab.json` & `mmengine-0.7.4/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/hub/torchvision_0.12.json` & `mmengine-0.7.4/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/infer/infer.py` & `mmengine-0.7.4/mmengine/infer/infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             Defaults to None.
         weights (str, optional): Path to the checkpoint. If it is not specified
             and model is a model name of metafile, the weights will be loaded
             from metafile. Defaults to None.
         device (str, optional): Device to run inference. If None, the available
             device will be automatically used. Defaults to None.
         scope (str, optional): The scope of the model. Defaults to None.
+        show_progress (bool): Control whether to display the progress bar during
+            the inference process. Defaults to True.
+            `New in version 0.7.4.`
 
     Note:
         Since ``Inferencer`` could be used to infer batch data,
         `collate_fn` should be defined. If `collate_fn` is not defined in config
         file, the `collate_fn` will be `pseudo_collate` by default.
     """  # noqa: E501
 
@@ -135,15 +138,16 @@
     visualize_kwargs: set = set()
     postprocess_kwargs: set = set()
 
     def __init__(self,
                  model: Union[ModelType, str, None] = None,
                  weights: Optional[str] = None,
                  device: Optional[str] = None,
-                 scope: Optional[str] = None) -> None:
+                 scope: Optional[str] = None,
+                 show_progress: bool = True) -> None:
         if scope is None:
             default_scope = DefaultScope.get_current_instance()
             if default_scope is not None:
                 scope = default_scope.scope_name
         self.scope = scope
         # Load config to cfg
         cfg: ConfigType
@@ -174,14 +178,15 @@
             device = get_device()
 
         self.model = self._init_model(cfg, weights, device)  # type: ignore
         self.pipeline = self._init_pipeline(cfg)
         self.collate_fn = self._init_collate(cfg)
         self.visualizer = self._init_visualizer(cfg)
         self.cfg = cfg
+        self.show_progress = show_progress
 
     def __call__(
         self,
         inputs: InputsType,
         return_datasamples: bool = False,
         batch_size: int = 1,
         **kwargs,
@@ -209,15 +214,16 @@
             postprocess_kwargs,
         ) = self._dispatch_kwargs(**kwargs)
 
         ori_inputs = self._inputs_to_list(inputs)
         inputs = self.preprocess(
             ori_inputs, batch_size=batch_size, **preprocess_kwargs)
         preds = []
-        for data in track(inputs, description='Inference'):
+        for data in (track(inputs, description='Inference')
+                     if self.show_progress else inputs):
             preds.extend(self.forward(data, **forward_kwargs))
         visualization = self.visualize(
             ori_inputs, preds,
             **visualize_kwargs)  # type: ignore  # noqa: E501
         results = self.postprocess(preds, visualization, return_datasamples,
                                    **postprocess_kwargs)
         return results
```

### Comparing `mmengine-0.7.3/mmengine/logging/history_buffer.py` & `mmengine-0.7.4/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/logging/logger.py` & `mmengine-0.7.4/mmengine/logging/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -372,15 +372,20 @@
             return local_rank
         cuda_visible_devices = os.getenv('CUDA_VISIBLE_DEVICES', None)
         if cuda_visible_devices is None:
             num_device = torch.cuda.device_count()
             cuda_visible_devices = list(range(num_device))
         else:
             cuda_visible_devices = cuda_visible_devices.split(',')
-        return int(cuda_visible_devices[local_rank])
+        try:
+            return int(cuda_visible_devices[local_rank])
+        except ValueError:
+            # handle case for Multi-Instance GPUs
+            # see #1148 for details
+            return cuda_visible_devices[local_rank]
 
 
 def _get_host_info() -> str:
     """Get hostname and username.
 
     Return empty string if exception raised, e.g. ``getpass.getuser()`` will
     lead to error in docker container
```

### Comparing `mmengine-0.7.3/mmengine/logging/message_hub.py` & `mmengine-0.7.4/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/__init__.py` & `mmengine-0.7.4/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/averaged_model.py` & `mmengine-0.7.4/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/base_model/base_model.py` & `mmengine-0.7.4/mmengine/model/base_model/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
         Accepts ``batch_inputs`` and ``data_sample`` processed by
         :attr:`data_preprocessor`, and returns results according to mode
         arguments.
 
         During non-distributed training, validation, and testing process,
         ``forward`` will be called by ``BaseModel.train_step``,
-        ``BaseModel.val_step`` and ``BaseModel.val_step`` directly.
+        ``BaseModel.val_step`` and ``BaseModel.test_step`` directly.
 
         During distributed data parallel training process,
         ``MMSeparateDistributedDataParallel.train_step`` will first call
         ``DistributedDataParallel.forward`` to enable automatic
         gradient synchronization, and then call ``forward`` to get training
         loss.
```

### Comparing `mmengine-0.7.3/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.7.4/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/base_module.py` & `mmengine-0.7.4/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/test_time_aug.py` & `mmengine-0.7.4/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/utils.py` & `mmengine-0.7.4/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/weight_init.py` & `mmengine-0.7.4/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/wrappers/__init__.py` & `mmengine-0.7.4/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/wrappers/distributed.py` & `mmengine-0.7.4/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.7.4/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.7.4/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/model/wrappers/utils.py` & `mmengine-0.7.4/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/__init__.py` & `mmengine-0.7.4/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/__init__.py` & `mmengine-0.7.4/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.7.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.7.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/builder.py` & `mmengine-0.7.4/mmengine/optim/optimizer/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 from typing import List, Union
 
 import torch
 import torch.nn as nn
 
 from mmengine.config import Config, ConfigDict
-from mmengine.device import is_npu_available
+from mmengine.device import is_npu_available, is_npu_support_full_precision
 from mmengine.registry import OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS
 from .optimizer_wrapper import OptimWrapper
 
 
 def register_torch_optimizers() -> List[str]:
     """Register optimizers in ``torch.optim`` to the ``OPTIMIZERS`` registry.
 
@@ -101,14 +101,38 @@
         optimizers.append('Lion')
     return optimizers
 
 
 LION_OPTIMIZERS = register_lion_optimizers()
 
 
+def register_sophia_optimizers() -> List[str]:
+    """Register Sophia optimizer to the ``OPTIMIZERS`` registry.
+
+    Returns:
+        List[str]: A list of registered optimizers' name.
+    """
+    optimizers = []
+    try:
+        import Sophia
+    except ImportError:
+        pass
+    else:
+        for module_name in dir(Sophia):
+            _optim = getattr(Sophia, module_name)
+            if inspect.isclass(_optim) and issubclass(_optim,
+                                                      torch.optim.Optimizer):
+                OPTIMIZERS.register_module(module=_optim)
+                optimizers.append(module_name)
+    return optimizers
+
+
+SOPHIA_OPTIMIZERS = register_sophia_optimizers()
+
+
 def build_optim_wrapper(model: nn.Module,
                         cfg: Union[dict, Config, ConfigDict]) -> OptimWrapper:
     """Build function of OptimWrapper.
 
     If ``constructor`` is set in the ``cfg``, this method will build an
     optimizer wrapper constructor, and use optimizer wrapper constructor to
     build the optimizer wrapper. If ``constructor`` is not set, the
@@ -124,17 +148,17 @@
     """
     optim_wrapper_cfg = copy.deepcopy(cfg)
     constructor_type = optim_wrapper_cfg.pop('constructor',
                                              'DefaultOptimWrapperConstructor')
     paramwise_cfg = optim_wrapper_cfg.pop('paramwise_cfg', None)
 
     # Since the current generation of NPU(Ascend 910) only supports
-    # mixed precision training, here we turn on mixed precision by default
-    # on the NPU to make the training normal
-    if is_npu_available():
+    # mixed precision training, here we turn on mixed precision
+    # to make the training normal
+    if is_npu_available() and not is_npu_support_full_precision():
         optim_wrapper_cfg['type'] = 'AmpOptimWrapper'
 
     optim_wrapper_constructor = OPTIM_WRAPPER_CONSTRUCTORS.build(
         dict(
             type=constructor_type,
             optim_wrapper_cfg=optim_wrapper_cfg,
             paramwise_cfg=paramwise_cfg))
```

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.7.4/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.7.4/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/scheduler/__init__.py` & `mmengine-0.7.4/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.7.4/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.7.4/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.7.4/mmengine/optim/scheduler/param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,27 +181,27 @@
         """Adjusts the parameter value of each parameter group based on the
         specified schedule."""
         # Raise a warning if old pattern is detected
         # https://github.com/pytorch/pytorch/issues/20124
         if self._global_step == 0:
             if not hasattr(self.optimizer.step, '_with_counter'):
                 warnings.warn(
-                    'Seems like `optimizer.step()` has been overridden after'
-                    'parameter value scheduler initialization. Please, make'
-                    'sure to call `optimizer.step()` before'
-                    '`scheduler.step()`. See more details at'
+                    'Seems like `optimizer.step()` has been overridden after '
+                    'parameter value scheduler initialization. Please, make '
+                    'sure to call `optimizer.step()` before '
+                    '`scheduler.step()`. See more details at '
                     'https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate',  # noqa: E501
                     UserWarning)
 
             # Just check if there were two first scheduler.step() calls
             # before optimizer.step()
             elif self.optimizer._global_step < 0:
                 warnings.warn(
-                    'Detected call of `scheduler.step()` before'
-                    '`optimizer.step()`. In PyTorch 1.1.0 and later, you'
+                    'Detected call of `scheduler.step()` before '
+                    '`optimizer.step()`. In PyTorch 1.1.0 and later, you '
                     'should call them in the opposite order: '
                     '`optimizer.step()` before `scheduler.step()`. '
                     'Failure to do this will result in PyTorch skipping '
                     'the first value of the parameter value schedule. '
                     'See more details at https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate',  # noqa: E501
                     UserWarning)
         self._global_step += 1
```

### Comparing `mmengine-0.7.3/mmengine/registry/__init__.py` & `mmengine-0.7.4/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/registry/build_functions.py` & `mmengine-0.7.4/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/registry/default_scope.py` & `mmengine-0.7.4/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/registry/registry.py` & `mmengine-0.7.4/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/registry/root.py` & `mmengine-0.7.4/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/registry/utils.py` & `mmengine-0.7.4/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/__init__.py` & `mmengine-0.7.4/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/amp.py` & `mmengine-0.7.4/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/base_loop.py` & `mmengine-0.7.4/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/checkpoint.py` & `mmengine-0.7.4/mmengine/runner/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,18 +648,19 @@
 
     Args:
         state_dict (OrderedDict): Model weights on GPU.
 
     Returns:
         OrderedDict: Model weights on GPU.
     """
+    # stash metadata to put in state_dict later
+    metadata = getattr(state_dict, '_metadata', OrderedDict())
     state_dict = apply_to(state_dict, lambda x: hasattr(x, 'cpu'),
                           lambda x: x.cpu())
-    # Keep metadata in state_dict
-    state_dict._metadata = getattr(state_dict, '_metadata', OrderedDict())
+    state_dict._metadata = metadata
     return state_dict
 
 
 @deprecated_function(
     since='0.3.0',
     removed_in='0.5.0',
     instructions='`_save_to_state_dict` will be deprecated in the future, '
```

### Comparing `mmengine-0.7.3/mmengine/runner/log_processor.py` & `mmengine-0.7.4/mmengine/runner/log_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,19 @@
                 log_str = (f'Iter({mode}) '
                            f'[{cur_iter_str}/{runner.max_iters}]  ')
             else:
                 dataloader_len = self._get_dataloader_size(runner, mode)
                 cur_iter_str = str(batch_idx + 1).rjust(
                     len(str(dataloader_len)))
                 log_str = (f'Iter({mode}) [{cur_iter_str}/{dataloader_len}]  ')
+        # Add global iter.
+        if isinstance(runner._train_loop, dict) or runner._train_loop is None:
+            tag['iter'] = 0
+        else:
+            tag['iter'] = runner.iter + 1
         # Concatenate lr, momentum string with log header.
         log_str += f'{lr_str}  '
         # If IterTimerHook used in runner, eta, time, and data_time should be
         # recorded.
         if (all(item in log_tag for item in ['time', 'data_time'])
                 and 'eta' in runner.message_hub.runtime_info):
             eta = runner.message_hub.get_info('eta')
```

### Comparing `mmengine-0.7.3/mmengine/runner/loops.py` & `mmengine-0.7.4/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/priority.py` & `mmengine-0.7.4/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/runner/runner.py` & `mmengine-0.7.4/mmengine/runner/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2086,15 +2086,15 @@
     def save_checkpoint(
         self,
         out_dir: str,
         filename: str,
         file_client_args: Optional[dict] = None,
         save_optimizer: bool = True,
         save_param_scheduler: bool = True,
-        meta: dict = None,
+        meta: Optional[dict] = None,
         by_epoch: bool = True,
         backend_args: Optional[dict] = None,
     ):
         """Save checkpoints.
 
         ``CheckpointHook`` invokes this method to save checkpoints
         periodically.
@@ -2108,16 +2108,16 @@
                 Please use `backend_args` instead.
             save_optimizer (bool): Whether to save the optimizer to
                 the checkpoint. Defaults to True.
             save_param_scheduler (bool): Whether to save the param_scheduler
                 to the checkpoint. Defaults to True.
             meta (dict, optional): The meta information to be saved in the
                 checkpoint. Defaults to None.
-            by_epoch (bool): Whether the scheduled momentum is updated by
-                epochs. Defaults to True.
+            by_epoch (bool): Decide the number of epoch or iteration saved in
+                checkpoint. Defaults to True.
             backend_args (dict, optional): Arguments to instantiate the
                 prefix of uri corresponding backend. Defaults to None.
                 New in v0.2.0.
         """
         if meta is None:
             meta = {}
         elif not isinstance(meta, dict):
@@ -2125,17 +2125,19 @@
                 f'meta should be a dict or None, but got {type(meta)}')
 
         if by_epoch:
             # self.epoch increments 1 after
             # `self.call_hook('after_train_epoch)` but `save_checkpoint` is
             # called by `after_train_epoch`` method of `CheckpointHook` so
             # `epoch` should be `self.epoch + 1`
-            meta.update(epoch=self.epoch + 1, iter=self.iter)
+            meta.setdefault('epoch', self.epoch + 1)
+            meta.setdefault('iter', self.iter)
         else:
-            meta.update(epoch=self.epoch, iter=self.iter + 1)
+            meta.setdefault('epoch', self.epoch)
+            meta.setdefault('iter', self.iter + 1)
 
         if file_client_args is not None:
             warnings.warn(
                 '"file_client_args" will be deprecated in future. '
                 'Please use "backend_args" instead', DeprecationWarning)
             if backend_args is not None:
                 raise ValueError(
@@ -2302,14 +2304,15 @@
             env_cfg (dict): The environment config of the runner.
         """
         # Collect and log environment information.
         env = collect_env()
         runtime_env = OrderedDict()
         runtime_env.update(env_cfg)
         runtime_env.update(self._randomness_cfg)
+        runtime_env['seed'] = self._seed
         runtime_env['Distributed launcher'] = self._launcher
         runtime_env['Distributed training'] = self._distributed
         runtime_env['GPU number'] = self._world_size
 
         env_info = '\n    ' + '\n    '.join(f'{k}: {v}'
                                             for k, v in env.items())
         runtime_env_info = '\n    ' + '\n    '.join(
```

### Comparing `mmengine-0.7.3/mmengine/runner/utils.py` & `mmengine-0.7.4/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/structures/base_data_element.py` & `mmengine-0.7.4/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/structures/instance_data.py` & `mmengine-0.7.4/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/structures/label_data.py` & `mmengine-0.7.4/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/structures/pixel_data.py` & `mmengine-0.7.4/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/testing/__init__.py` & `mmengine-0.7.4/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/testing/_internal/distributed.py` & `mmengine-0.7.4/mmengine/testing/_internal/distributed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 # Copyright (c) https://github.com/pytorch/pytorch
 # Modified from https://github.com/pytorch/pytorch/blob/master/torch/testing/_internal/common_distributed.py  # noqa: E501
-
 import faulthandler
 import logging
 import multiprocessing
 import sys
 import tempfile
 import threading
 import time
@@ -63,14 +62,17 @@
     # but we still want to ensure we didn't run into any other errors.
     TEST_ERROR_EXIT_CODE = 10
 
     # do not early terminate for distributed tests.
     def _should_stop_test_suite(self) -> bool:
         return False
 
+    def prepare_subprocess(self):
+        pass
+
     @property
     def world_size(self) -> int:
         return 2
 
     @property
     def timeout(self) -> int:
         return 1000
@@ -165,15 +167,18 @@
             if signal_pipe in ready_pipes:
                 return
 
     @classmethod
     def _run(cls, rank: int, test_name: str, file_name: str,
              parent_pipe) -> None:
         self = cls(test_name)
-
+        try:
+            self.prepare_subprocess()
+        except Exception:
+            raise sys.exit(MultiProcessTestCase.TEST_ERROR_EXIT_CODE)
         self.rank = rank
         self.file_name = file_name
         self.run_test(test_name, parent_pipe)
 
     def run_test(self, test_name: str, parent_pipe) -> None:
         # Start event listener thread.
         signal_recv_pipe, signal_send_pipe = torch.multiprocessing.Pipe(
@@ -323,33 +328,30 @@
             for i, process in errored_processes:
                 # Get error from pipe.
                 error_message = self.pid_to_pipe[process.pid].recv()
                 error += (
                     'Process {} exited with error code {} and exception:\n{}\n'
                     .format(i, MultiProcessTestCase.TEST_ERROR_EXIT_CODE,
                             error_message))
-
             raise RuntimeError(error)
         # If no process exited uncleanly, we check for timeouts, and then
         # ensure each process exited cleanly.
         for i, p in enumerate(self.processes):
             if p.exitcode is None:
                 raise RuntimeError(
                     f'Process {i} terminated or timed out after '
                     '{elapsed_time} seconds')
-            self.assertEqual(
-                p.exitcode,
-                first_process.exitcode,
-                msg=f'Expect process {i} exit code to match Process 0 exit '
-                'code of {first_process.exitcode}, but got {p.exitcode}')
+
         for skip in TEST_SKIPS.values():
             if first_process.exitcode == skip.exit_code:
                 raise unittest.SkipTest(skip.message)
-        self.assertEqual(
-            first_process.exitcode,
-            0,
-            msg=f'Expected zero exit code but got {first_process.exitcode} '
-            f'for pid: {first_process.pid}')
+
+        # Skip the unittest since the raised error maybe not caused by
+        # the tested function. For example, in CI environment, the tested
+        # method could be terminated by system signal for the limited
+        # resources.
+        self.skipTest(f'Skip test {self._testMethodName} due to '
+                      'the program abort')
 
     @property
     def is_master(self) -> bool:
         return self.rank == 0
```

### Comparing `mmengine-0.7.3/mmengine/testing/compare.py` & `mmengine-0.7.4/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/testing/runner_test_case.py` & `mmengine-0.7.4/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/__init__.py` & `mmengine-0.7.4/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/hub.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/misc.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/trace.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.7.4/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/manager.py` & `mmengine-0.7.4/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/misc.py` & `mmengine-0.7.4/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/package_utils.py` & `mmengine-0.7.4/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/path.py` & `mmengine-0.7.4/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/progressbar.py` & `mmengine-0.7.4/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/timer.py` & `mmengine-0.7.4/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/utils/version_utils.py` & `mmengine-0.7.4/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/version.py` & `mmengine-0.7.4/mmengine/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.7.3/mmengine/visualization/utils.py` & `mmengine-0.7.4/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine/visualization/vis_backend.py` & `mmengine-0.7.4/mmengine/visualization/vis_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import functools
 import logging
 import os
 import os.path as osp
 import warnings
 from abc import ABCMeta, abstractmethod
 from collections.abc import MutableMapping
-from typing import Any, Callable, Optional, Sequence, Union
+from typing import Any, Callable, List, Optional, Sequence, Union
 
 import cv2
 import numpy as np
 import torch
 
 from mmengine.config import Config
 from mmengine.fileio import dump
@@ -343,41 +343,47 @@
     Args:
         save_dir (str, optional): The root directory to save the files
             produced by the visualizer.
         init_kwargs (dict, optional): wandb initialization
             input parameters.
             See `wandb.init <https://docs.wandb.ai/ref/python/init>`_ for
             details. Defaults to None.
-        define_metric_cfg (dict, optional):
-            A dict of metrics and summary for wandb.define_metric.
+        define_metric_cfg (dict or list[dict], optional):
+            When a dict is set, it is a dict of metrics and summary for
+            ``wandb.define_metric``.
             The key is metric and the value is summary.
-            When ``define_metric_cfg={'coco/bbox_mAP': 'max'}``,
-            The maximum value of ``coco/bbox_mAP`` is logged on wandb UI.
+            When a list is set, each dict should be a valid argument of
+            the ``define_metric``.
+            For example, ``define_metric_cfg={'coco/bbox_mAP': 'max'}``,
+            means the maximum value of ``coco/bbox_mAP`` is logged on wandb UI.
+            When ``define_metric_cfg=[dict(name='loss',
+            step_metric='epoch')]``,
+            the "loss" will be plotted against the epoch.
             See `wandb define_metric <https://docs.wandb.ai/ref/python/
             run#define_metric>`_ for details.
-            Default: None
-        commit: (bool, optional) Save the metrics dict to the wandb server
+            Defaults to None.
+        commit (bool, optional) Save the metrics dict to the wandb server
             and increment the step.  If false `wandb.log` just updates the
             current metrics dict with the row argument and metrics won't be
             saved until `wandb.log` is called with `commit=True`.
             Defaults to True.
-        log_code_name: (str, optional) The name of code artifact.
+        log_code_name (str, optional) The name of code artifact.
             By default, the artifact will be named
             source-$PROJECT_ID-$ENTRYPOINT_RELPATH. See
             `wandb log_code <https://docs.wandb.ai/ref/python/run#log_code>`_
             for details. Defaults to None.
-            New in version 0.3.0.
+            `New in version 0.3.0.`
         watch_kwargs (optional, dict): Agurments for ``wandb.watch``.
-            New in version 0.4.0.
+            `New in version 0.4.0.`
     """
 
     def __init__(self,
                  save_dir: str,
                  init_kwargs: Optional[dict] = None,
-                 define_metric_cfg: Optional[dict] = None,
+                 define_metric_cfg: Union[dict, list, None] = None,
                  commit: Optional[bool] = True,
                  log_code_name: Optional[str] = None,
                  watch_kwargs: Optional[dict] = None):
         super().__init__(save_dir)
         self._init_kwargs = init_kwargs
         self._define_metric_cfg = define_metric_cfg
         self._commit = commit
@@ -396,16 +402,22 @@
             import wandb
         except ImportError:
             raise ImportError(
                 'Please run "pip install wandb" to install wandb')
 
         wandb.init(**self._init_kwargs)
         if self._define_metric_cfg is not None:
-            for metric, summary in self._define_metric_cfg.items():
-                wandb.define_metric(metric, summary=summary)
+            if isinstance(self._define_metric_cfg, dict):
+                for metric, summary in self._define_metric_cfg.items():
+                    wandb.define_metric(metric, summary=summary)
+            elif isinstance(self._define_metric_cfg, list):
+                for metric_cfg in self._define_metric_cfg:
+                    wandb.define_metric(**metric_cfg)
+            else:
+                raise ValueError('define_metric_cfg should be dict or list')
         self._wandb = wandb
 
     @property  # type: ignore
     @force_init_env
     def experiment(self):
         """Return wandb object.
 
@@ -636,41 +648,47 @@
         >>> vis_backend.add_scalars({'loss': 0.1,'acc':0.8})
         >>> cfg = Config(dict(a=1, b=dict(b1=[0, 1])))
         >>> vis_backend.add_config(cfg)
 
     Args:
         save_dir (str): The root directory to save the files
             produced by the backend.
-        exp_name (str, optional): The experiment name. Default to None.
-        run_name (str, optional): The run name. Default to None.
+        exp_name (str, optional): The experiment name. Defaults to None.
+        run_name (str, optional): The run name. Defaults to None.
         tags (dict, optional): The tags to be added to the experiment.
-            Default to None.
+            Defaults to None.
         params (dict, optional): The params to be added to the experiment.
-            Default to None.
-        tracking_uri (str, optional): The tracking uri. Default to None.
+            Defaults to None.
+        tracking_uri (str, optional): The tracking uri. Defaults to None.
         artifact_suffix (Tuple[str] or str, optional): The artifact suffix.
-            Default to ('.json', '.log', '.py', 'yaml').
+            Defaults to ('.json', '.log', '.py', 'yaml').
+        tracked_config_keys (dict, optional): The top level keys of config that
+            will be added to the experiment. If it is None, which means all
+            the config will be added. Defaults to None.
+            `New in version 0.7.4.`
     """
 
     def __init__(self,
                  save_dir: str,
                  exp_name: Optional[str] = None,
                  run_name: Optional[str] = None,
                  tags: Optional[dict] = None,
                  params: Optional[dict] = None,
                  tracking_uri: Optional[str] = None,
                  artifact_suffix: SUFFIX_TYPE = ('.json', '.log', '.py',
-                                                 'yaml')):
+                                                 'yaml'),
+                 tracked_config_keys: Optional[dict] = None):
         super().__init__(save_dir)
         self._exp_name = exp_name
         self._run_name = run_name
         self._tags = tags
         self._params = params
         self._tracking_uri = tracking_uri
         self._artifact_suffix = artifact_suffix
+        self._tracked_config_keys = tracked_config_keys
 
     def _init_env(self):
         """Setup env for MLflow."""
         if not os.path.exists(self._save_dir):
             os.makedirs(self._save_dir, exist_ok=True)  # type: ignore
 
         try:
@@ -725,15 +743,21 @@
     def add_config(self, config: Config, **kwargs) -> None:
         """Record the config to mlflow.
 
         Args:
             config (Config): The Config object
         """
         self.cfg = config
-        self._mlflow.log_params(self._flatten(self.cfg))
+        if self._tracked_config_keys is None:
+            self._mlflow.log_params(self._flatten(self.cfg))
+        else:
+            tracked_cfg = dict()
+            for k in self._tracked_config_keys:
+                tracked_cfg[k] = self.cfg[k]
+            self._mlflow.log_params(self._flatten(tracked_cfg))
         self._mlflow.log_text(self.cfg.pretty_text, 'config.py')
 
     @force_init_env
     def add_image(self,
                   name: str,
                   image: np.ndarray,
                   step: int = 0,
@@ -772,36 +796,38 @@
         """Record the scalar's data to mlflow.
 
         Args:
             scalar_dict (dict): Key-value pair storing the tag and
                 corresponding values.
             step (int): Global step value to record. Default to 0.
             file_path (str, optional): Useless parameter. Just for
-                interface unification. Default to None.
+                interface unification. Defaults to None.
         """
         assert isinstance(scalar_dict, dict)
         assert 'step' not in scalar_dict, 'Please set it directly ' \
                                           'through the step parameter'
         self._mlflow.log_metrics(scalar_dict, step)
 
     def close(self) -> None:
         """Close the mlflow."""
+        if not hasattr(self, '_mlflow'):
+            return
+
         file_paths = dict()
         for filename in scandir(self.cfg.work_dir, self._artifact_suffix,
                                 True):
             file_path = osp.join(self.cfg.work_dir, filename)
             relative_path = os.path.relpath(file_path, self.cfg.work_dir)
             dir_path = os.path.dirname(relative_path)
             file_paths[file_path] = dir_path
 
         for file_path, dir_path in file_paths.items():
             self._mlflow.log_artifact(file_path, dir_path)
 
-        if hasattr(self, '_mlflow'):
-            self._mlflow.end_run()
+        self._mlflow.end_run()
 
     def _flatten(self, d, parent_key='', sep='.') -> dict:
         """Flatten the dict."""
         items = dict()
         for k, v in d.items():
             new_key = parent_key + sep + k if parent_key else k
             if isinstance(v, MutableMapping):
@@ -812,7 +838,148 @@
                         items.update(
                             self._flatten(x, new_key + sep + str(i), sep=sep))
                 else:
                     items[new_key] = v
             else:
                 items[new_key] = v
         return items
+
+
+@VISBACKENDS.register_module()
+class ClearMLVisBackend(BaseVisBackend):
+    """Clearml visualization backend class. It requires `clearml`_ to be
+    installed.
+
+    Examples:
+        >>> from mmengine.visualization import ClearMLVisBackend
+        >>> from mmengine import Config
+        >>> import numpy as np
+        >>> vis_backend = ClearMLVisBackend(save_dir='temp_dir')
+        >>> img = np.random.randint(0, 256, size=(10, 10, 3))
+        >>> vis_backend.add_image('img.png', img)
+        >>> vis_backend.add_scalar('mAP', 0.6)
+        >>> vis_backend.add_scalars({'loss': 0.1,'acc':0.8})
+        >>> cfg = Config(dict(a=1, b=dict(b1=[0, 1])))
+        >>> vis_backend.add_config(cfg)
+
+    Args:
+        save_dir (str, optional): Useless parameter. Just for
+            interface unification. Defaults to None.
+        init_kwargs (dict, optional): A dict contains the arguments of
+            ``clearml.Task.init`` . See `taskinit`_  for more details.
+            Defaults to None
+        artifact_suffix (Tuple[str] or str): The artifact suffix.
+            Defaults to ('.py', 'pth').
+
+    .. _clearml:
+        https://clear.ml/docs/latest/docs/
+
+    .. _taskinit:
+        https://clear.ml/docs/latest/docs/references/sdk/task/#taskinit
+    """
+
+    def __init__(self,
+                 save_dir: Optional[str] = None,
+                 init_kwargs: Optional[dict] = None,
+                 artifact_suffix: SUFFIX_TYPE = ('.py', '.pth')):
+        super().__init__(save_dir)  # type: ignore
+        self._init_kwargs = init_kwargs
+        self._artifact_suffix = artifact_suffix
+
+    def _init_env(self) -> None:
+        try:
+            import clearml
+        except ImportError:
+            raise ImportError(
+                'Please run "pip install clearml" to install clearml')
+
+        task_kwargs = self._init_kwargs or {}
+        self._clearml = clearml
+        self._task = self._clearml.Task.init(**task_kwargs)
+        self._logger = self._task.get_logger()
+
+    @property  # type: ignore
+    @force_init_env
+    def experiment(self):
+        """Return clearml object."""
+        return self._clearml
+
+    @force_init_env
+    def add_config(self, config: Config, **kwargs) -> None:
+        """Record the config to clearml.
+
+        Args:
+            config (Config): The Config object
+        """
+        self.cfg = config
+        self._task.connect_configuration(vars(config))
+
+    @force_init_env
+    def add_image(self,
+                  name: str,
+                  image: np.ndarray,
+                  step: int = 0,
+                  **kwargs) -> None:
+        """Record the image to clearml.
+
+        Args:
+            name (str): The image identifier.
+            image (np.ndarray): The image to be saved. The format
+                should be RGB.
+            step (int): Global step value to record. Defaults to 0.
+        """
+        self._logger.report_image(
+            title=name, series=name, iteration=step, image=image)
+
+    @force_init_env
+    def add_scalar(self,
+                   name: str,
+                   value: Union[int, float, torch.Tensor, np.ndarray],
+                   step: int = 0,
+                   **kwargs) -> None:
+        """Record the scalar data to clearml.
+
+        Args:
+            name (str): The scalar identifier.
+            value (int, float, torch.Tensor, np.ndarray): Value to save.
+            step (int): Global step value to record. Defaults to 0.
+        """
+        self._logger.report_scalar(
+            title=name, series=name, value=value, iteration=step)
+
+    @force_init_env
+    def add_scalars(self,
+                    scalar_dict: dict,
+                    step: int = 0,
+                    file_path: Optional[str] = None,
+                    **kwargs) -> None:
+        """Record the scalar's data to clearml.
+
+        Args:
+            scalar_dict (dict): Key-value pair storing the tag and
+                corresponding values.
+            step (int): Global step value to record. Defaults to 0.
+            file_path (str, optional): Useless parameter. Just for
+                interface unification. Defaults to None.
+        """
+        assert 'step' not in scalar_dict, 'Please set it directly ' \
+                                          'through the step parameter'
+        for key, value in scalar_dict.items():
+            self._logger.report_scalar(
+                title=key, series=key, value=value, iteration=step)
+
+    def close(self) -> None:
+        """Close the clearml."""
+        if not hasattr(self, '_clearml'):
+            return
+
+        file_paths: List[str] = list()
+        if (hasattr(self, 'cfg')
+                and osp.isdir(getattr(self.cfg, 'work_dir', ''))):
+            for filename in scandir(self.cfg.work_dir, self._artifact_suffix,
+                                    False):
+                file_path = osp.join(self.cfg.work_dir, filename)
+                file_paths.append(file_path)
+
+        for file_path in file_paths:
+            self._task.upload_artifact(os.path.basename(file_path), file_path)
+        self._task.close()
```

### Comparing `mmengine-0.7.3/mmengine/visualization/visualizer.py` & `mmengine-0.7.4/mmengine/visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/mmengine.egg-info/PKG-INFO` & `mmengine-0.7.4/mmengine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.7.3
+Version: 0.7.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -84,22 +84,22 @@
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
         ## What's New
         
-        v0.7.3 was released on 2023-04-28.
+        v0.7.4 was released on 2023-06-03.
         
         ### Highlights
         
-        - Support using MLflow to record experiment data
-        - Support registering callable objects to the registry
+        - Support using [`ClearML`](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) to record experiment data
+        - Add [`Sophia`](https://mmengine.readthedocs.io/en/latest/common_usage/better_optimizers.html#sophia) optimizers
         
-        Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v074-06032023) for more details.
         
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
```

### Comparing `mmengine-0.7.3/mmengine.egg-info/SOURCES.txt` & `mmengine-0.7.4/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.3/setup.py` & `mmengine-0.7.4/setup.py`

 * *Files identical despite different names*

