# Comparing `tmp/colossalai-nightly-2023.5.6.tar.gz` & `tmp/colossalai-nightly-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.5.6.tar", last modified: Sat May  6 00:13:49 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.6.3.tar", last modified: Sat Jun  3 00:15:29 2023, max compression
```

## Comparing `colossalai-nightly-2023.5.6.tar` & `colossalai-nightly-2023.6.3.tar`

### file list

```diff
@@ -1,873 +1,901 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.423487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/torch_ddp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.455490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.455490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/lazy_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36381 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.949204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.985204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/lazy_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37387 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.929204 colossalai-nightly-2023.6.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.049204 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.057204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.057204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.069204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/version.txt
```

### Comparing `colossalai-nightly-2023.5.6/LICENSE` & `colossalai-nightly-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/PKG-INFO` & `colossalai-nightly-2023.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.5.6
+Version: 2023.6.3
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -134,20 +134,30 @@
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Colossal-AI in the Real World
         
         ### ColossalChat
         
         <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
            </a>
         </div>
         
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
+        [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
+        [[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
+        [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+        
+        <p id="ColossalChat-Speed" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
+        </p>
+        
+        - Up to 10 times faster for RLHF PPO Stage3 Training
         
         <p id="ColossalChat_scaling" align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
         </p>
         
         - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
         
@@ -359,14 +369,30 @@
         By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
         If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
         
         ```shell
         CUDA_EXT=1 pip install .
         ```
         
+        For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
+        
+        ```bash
+        # clone the repository
+        git clone https://github.com/hpcaitech/ColossalAI.git
+        cd ColossalAI
+        
+        # download the cub library
+        wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
+        unzip 1.8.0.zip
+        cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
+        
+        # install
+        CUDA_EXT=1 pip install .
+        ```
+        
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Use Docker
         
         ### Pull from DockerHub
         
         You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.6 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.3 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -92,23 +92,26 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                       chat/ColossalChat%20YouTube.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
+watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chat/ColossalChat%20Speed.jpg]
+- Up to 10 times faster for RLHF PPO Stage3 Training
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -225,15 +228,22 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
+with CUDA 10.2, you can still build ColossalAI from source. However, you need
+to manually download the cub library and copy it to the corresponding
+directory. ```bash # clone the repository git clone https://github.com/
+hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
+github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
+1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
+CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.6/README.md` & `colossalai-nightly-2023.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,20 +123,30 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Colossal-AI in the Real World
 
 ### ColossalChat
 
 <div align="center">
-   <a href="https://chat.colossalai.org/">
-   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+   <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
+   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
    </a>
 </div>
 
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
+[[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
+[[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
+[[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
+[[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+
+<p id="ColossalChat-Speed" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
+</p>
+
+- Up to 10 times faster for RLHF PPO Stage3 Training
 
 <p id="ColossalChat_scaling" align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
 </p>
 
 - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
 
@@ -348,14 +358,30 @@
 By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
 
 ```shell
 CUDA_EXT=1 pip install .
 ```
 
+For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
+
+```bash
+# clone the repository
+git clone https://github.com/hpcaitech/ColossalAI.git
+cd ColossalAI
+
+# download the cub library
+wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
+unzip 1.8.0.zip
+cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
+
+# install
+CUDA_EXT=1 pip install .
+```
+
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Use Docker
 
 ### Pull from DockerHub
 
 You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -85,23 +85,26 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                       chat/ColossalChat%20YouTube.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
+watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chat/ColossalChat%20Speed.jpg]
+- Up to 10 times faster for RLHF PPO Stage3 Training
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -218,15 +221,22 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
+with CUDA 10.2, you can still build ColossalAI from source. However, you need
+to manually download the cub library and copy it to the corresponding
+directory. ```bash # clone the repository git clone https://github.com/
+hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
+github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
+1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
+CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                     # TODO: is there a way to split by device and dtype without appending in the inner loop?
                     per_device_and_dtype_grads[to_unscale.device][to_unscale.dtype].append(to_unscale)
 
             for device, per_dtype_grads in per_device_and_dtype_grads.items():
                 for grads in per_dtype_grads.values():
                     torch._amp_foreach_non_finite_check_and_unscale_(grads, per_device_found_inf.get(device),
                                                                      per_device_inv_scale.get(device))
-        # For tensor parallel paramters it should be all-reduced over tensor parallel process group
+        # For tensor parallel parameters it should be all-reduced over tensor parallel process group
         if gpc.is_initialized(ParallelMode.MODEL) and gpc.get_world_size(ParallelMode.MODEL) > 1:
             vals = [val for val in per_device_found_inf._per_device_tensors.values()]
             coalesced = _flatten_dense_tensors(vals)
             dist.all_reduce(coalesced, op=dist.ReduceOp.MAX, group=gpc.get_group(ParallelMode.MODEL))
             for buf, synced in zip(vals, _unflatten_dense_tensors(coalesced, vals)):
                 buf.copy_(synced)
         return per_device_found_inf._per_device_tensors
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             for (shape_0, shape_1) in zip(input_tensors[0].shape[:-2], input_tensors[1].shape[:-2]):
                 if shape_0 != shape_1:
                     _is_batch_dims_same = False
                     break
         else:
             _is_batch_dims_same = False
 
-        # retireve dimensions
+        # retrieve dimensions
         input_dim_00 = input_tensors[0].shape[-2]
         input_dim_01 = input_tensors[0].shape[-1]
         input_dim_10 = input_tensors[1].shape[-2]
         input_dim_11 = input_tensors[1].shape[-1]
         output_dim_0 = output_tensors[0].shape[-2]
         output_dim_1 = output_tensors[0].shape[-1]
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 self._set_data_ptr(tensor)
 
         # attach them to graph_info
         graph_info.fwd_in = input_tensors
         graph_info.fwd_tmp = buffer_tensors
         graph_info.fwd_out = output_tensors
 
-        # fetch other memory informations
+        # fetch other memory information
         memory_cost = meta_info.memory_cost
         graph_info.fwd_mem_tmp = memory_cost.fwd.temp
         graph_info.fwd_mem_out = memory_cost.fwd.activation
         graph_info.bwd_mem_tmp = memory_cost.bwd.temp
         graph_info.bwd_mem_out = memory_cost.bwd.activation
 
         # fetch flop information
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                 MetaInfo(comm_spec_apply_node,
                          mod_dir=node.meta['info'].mod_dir,
                          activation_checkpoint=tuple(node.meta['info'].activation_checkpoint))
 
     return gm
 
 
-def _act_annotataion_pass(gm: torch.fx.GraphModule):
+def _act_annotation_pass(gm: torch.fx.GraphModule):
     """
     This pass is used to add the act annotation to the new inserted nodes.
     """
     mod_graph = gm.graph
     nodes = tuple(mod_graph.nodes)
 
     for node in nodes:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                     total_shard_size *= device_mesh_info[shard_dim]
                 size[dim] = dim_size * total_shard_size
         size = torch.Size(size)
 
     return size
 
 
-def solution_annotatation_pass(gm: torch.fx.GraphModule, solution: List[int],
+def solution_annotation_pass(gm: torch.fx.GraphModule, solution: List[int],
                                strategies_constructor: StrategiesConstructor):
     """
     This method is used to stick the solution strategy to the nodes and add the information
     required in runtime into graph as placeholder nodes.
     """
     mod_graph = gm.graph
 
@@ -165,15 +165,15 @@
         return target_dim
 
     def _post_processing(node, size_processing_node):
         '''
         This function is used to process the dependency between the size node and its users after
         inserting the size_process_node.
         '''
-        # store original node and processing node pair in node_pairs dictioanry
+        # store original node and processing node pair in node_pairs dictionary
         # It will be used to replace the original node with processing node in slice object
         node_pairs[node] = size_processing_node
         size_processing_node._meta_data = node._meta_data
 
         if hasattr(node.meta['info'], 'activation_checkpoint'):
             MetaInfo(size_processing_node,
                      mod_dir=node.meta['info'].mod_dir,
@@ -384,15 +384,15 @@
 def module_params_sharding_pass(gm: torch.fx.GraphModule, device_mesh: DeviceMesh, overlap=False):
     """
     Apply the sharding action to the module parameters and buffers following the
     instructions of solver solution.
     """
     mod_graph = gm.graph
     nodes = tuple(mod_graph.nodes)
-    # This stream is created for overlaping the communication and computation.
+    # This stream is created for overlapping the communication and computation.
     reduction_stream = torch.cuda.Stream()
 
     def _add_hook_for_grad_communication(node, param, name=None):
 
         comm_actions = node.best_strategy.communication_actions
 
         def _filter_param_to_hook(node, op_data, comm_action, name):
@@ -492,15 +492,15 @@
 
 
 def runtime_preparation_pass(gm: torch.fx.GraphModule,
                              solution: List[int],
                              device_mesh: DeviceMesh,
                              strategies_constructor: StrategiesConstructor,
                              overlap=False):
-    gm, sharding_spec_convert_dict, origin_node_sharding_spec_dict, comm_actions_dict = solution_annotatation_pass(
+    gm, sharding_spec_convert_dict, origin_node_sharding_spec_dict, comm_actions_dict = solution_annotation_pass(
         gm, solution, strategies_constructor)
     gm = size_value_converting_pass(gm, device_mesh)
     gm = node_args_converting_pass(gm, device_mesh)
     # TODO: the pass below should be uncommented after the implementation of implicit_comm_action_apply_pass completed.
     # gm = implicit_comm_action_apply(gm)
     gm = module_params_sharding_pass(gm, device_mesh, overlap=overlap)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy) -> Union[ShardingStrategy, List[ShardingStrategy]]:
         """
         Convert the sharding spec from the logical shape to the physical shape.
         """
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensinal and the partition dim is only 2D,
+        # as input can be multi-dimensional and the partition dim is only 2D,
         # we need to map the partition at logical dim 0 to one of the first few dimensions of the input and output
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_embedding(strategy=strategy,
                                                                                        input_name=str(
                                                                                            self.node.args[0]),
                                                                                        output_name=str(self.node))
         return strategies
 
@@ -217,14 +217,14 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy):
         """
         Convert the sharding spec from the logical shape to the physical shape.
         """
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensinal and the partition dim is only 2D,
+        # as input can be multi-dimensional and the partition dim is only 2D,
         # we need to map the partition at logical dim 0 to one of the first few dimensions of the input and output
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_embedding(strategy=strategy,
                                                                                        input_name=str(
                                                                                            self.node.args[0]),
                                                                                        output_name=str(self.node))
         return strategies
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 __all__ = ['LinearModuleHandler', 'LinearFunctionHandler']
 
 
 def _update_sharding_spec_for_transposed_weight_for_linear(strategy: ShardingStrategy,
                                                            weight_name: str) -> ShardingStrategy:
     """
     This function is a helper function used by both module node handler and function node handler. This function will
-    convert the sharding spec for the transposed weight to the correct partititon spec.
+    convert the sharding spec for the transposed weight to the correct partition spec.
 
     Args:
         strategy (ShardingStrategy): the strategy generated by the strategy generator.
         weight_name (str): the name of the OperationData object for the weight.
     """
     # switch the dimensions of the transposed weight
     sharding_spec = strategy.get_sharding_spec_by_name(weight_name)
@@ -193,15 +193,15 @@
         1. the sharding spec is updated for the transposed weight
         2. the input and output sharding specs are updated to physical shape.
         """
         # switch the dimensions of the transposed weight
         strategy = _update_sharding_spec_for_transposed_weight_for_linear(strategy=strategy, weight_name='weight')
 
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensinal and the partition dim is only 2D,
+        # as input can be multi-dimensional and the partition dim is only 2D,
         # we need to map the partition at dim 0 to one of the first few dimensions of the input
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_linear(strategy=strategy,
                                                                                     input_name=str(self.node.args[0]),
                                                                                     output_name=str(self.node))
         return strategies
 
 
@@ -263,13 +263,13 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy):
         # switch the dimensions of the transposed weight
         strategy = _update_sharding_spec_for_transposed_weight_for_linear(strategy=strategy,
                                                                           weight_name=str(self.node.args[1]))
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensinal and the partition dim is only 2D,
+        # as input can be multi-dimensional and the partition dim is only 2D,
         # we need to map the partition at dim 0 to one of the first few dimensions of the input
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_linear(strategy=strategy,
                                                                                     input_name=str(self.node.args[0]),
                                                                                     output_name=str(self.node))
         return strategies
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 
 def get_matmul_type(input_dim: int, other_dim: int):
     """
     Determine which type of matmul operation should be executed for the given tensor dimensions.
 
     Args:
-        input_dim (int): the number of dimensions for the input tenosr
-        other_dim (int): the number of dimensions for the other tenosr
+        input_dim (int): the number of dimensions for the input tensor
+        other_dim (int): the number of dimensions for the other tensor
     """
     if input_dim == 1 and other_dim == 1:
         matmul_type = MatMulType.DOT
     elif input_dim in [1, 2] and other_dim == 2:
         matmul_type = MatMulType.MM
     elif input_dim == 2 and other_dim == 1:
         matmul_type = MatMulType.MV
@@ -202,15 +202,15 @@
             for dim_idx, broadcast_type in self.broadcast_dim_info[key].items():
                 if broadcast_type == BroadcastType.MULTIPLE:
                     # if the dim is originally 1 and multiplied during broadcast
                     # we set its sharding to R
                     # e.g. [1, 2, 4] x [4, 4, 8] -> [4, 2, 8]
                     # the dim 0 of [1, 2, 4] is multiplied to 4
                     tensor_shape[dim_idx] = 1
-                elif broadcast_type == BroadcastType.PADDDING:
+                elif broadcast_type == BroadcastType.PADDING:
                     # if the dim is padded
                     # we remove its sharding
                     tensor_shape[dim_idx] = None
 
             tensor_shape_before_broadcast = [dim for dim in tensor_shape if dim is not None]
 
             physical_sharding_spec, removed_dims = recover_sharding_spec_for_broadcast_shape(
@@ -264,21 +264,21 @@
             Map the logical batch dim to the physical batch dim
             """
             op_data = op_data_mapping[key]
             sharding_spec = strategy.get_sharding_spec_by_name(op_data.name)
             dim_partition_dict = sharding_spec.dim_partition_dict
             entire_shape = sharding_spec.entire_shape
 
-            # upddate the dimension index for the matrix dimensions
+            # update the dimension index for the matrix dimensions
             if 2 in dim_partition_dict:
                 dim_partition_dict[len(self.batch_dims_before_view) + 1] = dim_partition_dict.pop(2)
             if 1 in dim_partition_dict:
                 dim_partition_dict[len(self.batch_dims_before_view)] = dim_partition_dict.pop(1)
 
-            # map the logical batch dim to phyiscal batch dim
+            # map the logical batch dim to physical batch dim
             if 0 in dim_partition_dict:
                 batch_dim_shard = dim_partition_dict.pop(0)
                 dim_partition_dict[physical_batch_dim] = batch_dim_shard
 
             # the new shape will be the batch dims + the last 2 matrix dims
             shape_before_view = self.batch_dims_before_view + list(entire_shape[-2:])
             sharding_spec.__init__(sharding_spec.device_mesh, shape_before_view, dim_partition_dict)
@@ -410,15 +410,15 @@
         """
         The operands for the dot operation have the same logical shape as the physical shape
         """
         return None, None, None
 
     def _get_logical_shape_for_mm(self):
         """
-        We need to handle the input tensor for a matrix-matrix multiplcation as the input
+        We need to handle the input tensor for a matrix-matrix multiplication as the input
         tensor can be a 1D or 2D tensor. If it is a 1D tensor, 1 will be prepended to its shape
         (e.g. [4] -> [1, 4]).
         """
         if self.input_meta_data.dim() == 1:
             input_logical_shape = [1] + list(self.input_meta_data.shape)
             input_logical_shape = torch.Size(input_logical_shape)
         else:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             assert hasattr(node, 'strategies_vector'), \
                 f'The predecessor node {node_name} has no strategy vector to compute the resharding cost.'
             prev_strategy_vector = node.strategies_vector
             prev_sharding_specs = [
                 prev_strategy.get_sharding_spec_by_name(node_name) for prev_strategy in prev_strategy_vector
             ]
 
-            # create data structrure to store costs
+            # create data structure to store costs
             if node not in resharding_costs:
                 resharding_costs[node] = []
 
             def _compute_resharding_cost(
                     prev_sharding_spec: Union[ShardingSpec,
                                               List[ShardingSpec]], current_sharding_spec: Union[ShardingSpec,
                                                                                                 List[ShardingSpec]],
@@ -208,15 +208,15 @@
 
         for strategy in remove_strategy_list:
             self.strategies_vector.remove(strategy)
 
         return self.strategies_vector
 
     def post_process(self, strategy: ShardingStrategy) -> Union[ShardingStrategy, List[ShardingStrategy]]:
-        # tranform the strategy generated
+        # transform the strategy generated
         # e.g. to process the sharding strategy for the transposed weights
         return strategy
 
     @abstractmethod
     def get_strategy_generator(self) -> List[StrategyGenerator]:
         """
         Define which generators should be used by this NodeHandler object.
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class BatchNormStrategyGenerator(StrategyGenerator):
     """
     A StrategyGenerator which deals with the sharding strategies of batch normalization.
 
     To keep the math consistency, there are two way to do BatchNorm if the input
     shards on batch dimension:
     1. We gather the input partitions through batch dimension, then do the normal BatchNorm.
-    2. We do the SyncBatchNorm on the each input partition seperately, the SyncBN op will help
+    2. We do the SyncBatchNorm on the each input partition separately, the SyncBN op will help
        us to keep the computing correctness.
     In this generator, both methods will be considered.
     """
 
     def validate(self) -> bool:
         '''
         In sanity check, we need make sure the input data having correct dimension size.
@@ -40,15 +40,15 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into conv op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         '''
         # TODO: a constant coefficient need to be added.
         # 1D: (L) * N * Cin
         # 2D: (H * W) * N  * Cin
         # 3D: (H * W  * D) * N  * Cin
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
@@ -208,15 +208,15 @@
         if self.has_bias:
             dim_partition_dict_mapping["bias"] = {}
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for weight and bias.
-        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=mesh_dim_0,
             comm_type=CommType.IMPLICIT)
 
@@ -246,15 +246,15 @@
         if self.has_bias:
             dim_partition_dict_mapping["bias"] = {}
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for gradients of weight and bias.
-        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=[mesh_dim_0, mesh_dim_1],
             comm_type=CommType.IMPLICIT)
 
@@ -294,15 +294,15 @@
                 0: [mesh_dim_1],
             }
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for gradients of weight and bias.
-        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=[mesh_dim_0],
             comm_type=CommType.IMPLICIT)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def update_memory_cost(self, strategy: ShardingStrategy) -> ShardingStrategy:
         # all input, output and outputs have the same shape
         shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
 
         # compute fwd memory cost in bytes
         # as the elementwise ops are not memory-intensive
-        # we approximate the fwd memroy cost to be the output
+        # we approximate the fwd memory cost to be the output
         # and the backward memory cost to be grad of input and other
         input_bytes = self._compute_size_in_bytes(strategy, 'input')
         other_bytes = self._compute_size_in_bytes(strategy, 'other')
         output_bytes = self._compute_size_in_bytes(strategy, 'output')
         fwd_memory_cost = MemoryCost(activation=output_bytes)
         bwd_memory_cost = MemoryCost(activation=input_bytes + other_bytes)
         total_memory_cost = MemoryCost(activation=input_bytes + other_bytes + output_bytes)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into conv op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         # 1D: (L) * N * Cout * Cin * kernel
         # 2D: (H * W) * N * Cout * Cin * kernel
         # 3D: (H * W  * D) * N * Cout * Cin * kernel
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_other_shape = strategy.sharding_specs[self.op_data['other']].get_sharded_shape_per_device()
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
         if self.has_bias:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     def validate(self) -> bool:
         return super().validate()
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         # TODO: a constant coefficient need to be added.
 
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_weight_shape = strategy.sharding_specs[self.op_data['other']].get_sharded_shape_per_device()
         if self.has_bias:
             # bias add is an element wise operation, so the cost is equal to product of output shape.
             bias_compute_cost = reduce(operator.mul, sharded_weight_shape)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .strategy_generator import StrategyGenerator
 
 
 class NormalPoolStrategyGenerator(StrategyGenerator):
     """
     NormalPoolStrategyGenerator is a generic class to generate strategies for pool operation like MaxPoolxd.
     The reason we call this normal pool is AvgPoolxd and MaxPoolxd are taking the kernel size element from image,
-    and reduce them depening on the operation type.
+    and reduce them depending on the operation type.
     """
 
     def validate(self) -> bool:
         '''
         In sanity check, we need make sure the input data having correct dimension size.
         For Pool1d, the dim of input data should be 3([N, C, L]).
         For Pool2d, the dim of input data should be 4([N, C, H, W]).
@@ -31,17 +31,17 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into Pool op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy) -> TrainCycleItem:
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
         # 1D: (Lout) * N * C * kernel
         # 2D: (H * W) * N * Cout * Cin * kernel
         # 3D: (H * W  * D) * N * Cout * Cin * kernel
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
 
         kernel_size = self.op_data["other"].data
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,23 +221,23 @@
                 'sharding_spec of op_data should be a list of sharding specs if op_data.data is a tuple.'
             total_bytes = 0
             for index, sharding_spec in enumerate(strategy.sharding_specs[op_data]):
                 meta_data = op_data.data[index]
                 if isinstance(meta_data, torch.Tensor):
                     element_bytes = _compute_size_in_bytes_helper(sharding_spec, meta_data)
                 else:
-                    # if meta_data is not a tensor, we count the memroy as 0
+                    # if meta_data is not a tensor, we count the memory as 0
                     element_bytes = 0
                 total_bytes += element_bytes
 
         else:
             if isinstance(op_data.data, torch.Tensor):
                 total_bytes = _compute_size_in_bytes_helper(strategy.sharding_specs[op_data], op_data.data)
             else:
-                # if op_data.data is not a tensor, we count the memroy as 0
+                # if op_data.data is not a tensor, we count the memory as 0
                 total_bytes = 0
 
         return total_bytes
 
     def generate(self) -> List[ShardingStrategy]:
         """
         Generate all possible sharding strategies for this operation.
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class CostGraph:
     '''
     A graph data structure to simplify the edge cost graph. It has two main functions:
     1. To feed the quadratic resharding costs into solver, we need to linearize it. We build edge_cost in
     CostGraph, and it stored every combinations of strategies for a src-dst node pair in an 1D list.
     2. To reduce the searching space, we merge computationally-trivial operators, such as
-    element-wise operators, transpose, and reduction, into their following nodes. The merging infomation will
+    element-wise operators, transpose, and reduction, into their following nodes. The merging information will
     be given by the StrategiesVector depending on the type of target node and following nodes.
 
     Argument:
         leaf_strategies(List[StrategiesVector]): It stores StrategiesVector of every nodes on the graph.
         simplify(bool, optional): The generated cost graph will be simplified if it is true. (default to True)
     '''
 
@@ -86,15 +86,15 @@
 
             setattr(dst_node, 'parents', parent_nodes)
             setattr(dst_node, 'children', children_nodes)
 
             if self.simplify and strategies_vector.check_merge():
                 for followed_node in strategies_vector.predecessor_nodes:
                     # we only merge node pairs which src node has a tensor element inside.
-                    # This is necessay because the node without a tensor element inside will not
+                    # This is necessary because the node without a tensor element inside will not
                     # be assigned any strategy.
                     if _check_tensor_in_node(followed_node._meta_data):
                         self.merge_pair.append((followed_node, dst_node))
 
     def get_edge_cost(self, src_node, dst_node):
         return self.edge_costs[(src_node, dst_node)]
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,35 +79,35 @@
         """
         Return the Graph object associated with this analyser.
         """
         return self._graph
 
     def liveness_analysis(self) -> List[LiveStage]:
         """
-        Analyse the graph to obtain the variable liveness information. This function returns
+        Analyses the graph to obtain the variable liveness information. This function returns
         an ordered dictionary where the key is the compute stage ID and the value is a LivenessStage object.
         """
         compute_nodes = self.graph.nodes
         liveness_list = []
 
         # checked: record all variables created since the first stage
         # all: record the live variables only exist until the current stage.
-        #       this can be different from the `checked list`` as some varialbes may be destroyed prior to this stage.
+        #       this can be different from the `checked list`` as some variables may be destroyed prior to this stage.
         # unique: record the unique live variables only exist until the current stage.
         #       this is different from `all list` as some variables are duplicated.
         checked_variables = LiveVariableVector()
         all_live_variables = LiveVariableVector()
         unique_live_vars = LiveVariableVector()
 
         for idx, node in enumerate(compute_nodes):
             #############################
             # find new living variables #
             #############################
             # detect whether the current op is an in-place op
-            # if it is an in-place op, we would deem it as a duplciate var
+            # if it is an in-place op, we would deem it as a duplicate var
             is_inplace = False
             if node.op == 'call_function':
                 # check if this is an inplace op such as torch.nn.functional.relu(x, inplace=True)
                 if node.kwargs.get('inplace', False):
                     is_inplace = True
             elif node.op == 'call_module':
                 # to check if this is an inplace op such as torch.nn.Relu(inplace=True)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                  verbose=False):
         '''
         Solver class will integrate information provided by the components and use ILP solver to find a possible optimal strategies combination for target computing graph.
         Argument:
             graph: The computing graph to be optimized.
             strategies_constructor: It will provide all the possible strategies for each node in the computing graph.
             cost_graph: A graph data structure to simplify the edge cost graph.
-            graph_analyser: graph_analyser will analyse the graph to obtain the variable liveness information, which will be used to generate memory constraints.
+            graph_analyser: graph_analyser will analyses the graph to obtain the variable liveness information, which will be used to generate memory constraints.
             memory_budget: Memory constraint for the solution.
             solution_numbers: If solution_numbers is larger than one, solver will us a serious of solutions based on different memory budget.
             memory_increasing_coefficient: If solution_numbers is larger than one, we will use this coefficient to generate new memory budget.
         '''
         self.graph = graph
         self.strategies_constructor = strategies_constructor
         self.cost_graph = cost_graph
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'BroadcastType', 'is_broadcastable', 'get_broadcast_shape', 'recover_sharding_spec_for_broadcast_shape',
     'comm_actions_for_oprands'
 ]
 
 
 class BroadcastType(Enum):
     EQUAL = auto()
-    PADDDING = auto()
+    PADDING = auto()
     MULTIPLE = auto()
 
 
 def is_broadcastable(shape1: torch.Size, shape2: torch.Size) -> bool:
     """
     Check if two shapes are broadcastable to each other.
     """
@@ -65,26 +65,26 @@
 
     # track the dim and its broadcasting type
     logical_dim_broadcast_info = {}
 
     for i in range(logical_num_dims):
         # get the trailing dim size
         logical_dim_idx = logical_num_dims - i - 1
-        phyiscal_dim_idx = physical_num_dims - i - 1
+        physical_dim_idx = physical_num_dims - i - 1
         logical_dim_size = logical_shape[logical_dim_idx]
 
-        if phyiscal_dim_idx >= 0:
-            physical_dim_size = physical_shape[phyiscal_dim_idx]
+        if physical_dim_idx >= 0:
+            physical_dim_size = physical_shape[physical_dim_idx]
 
             if physical_dim_size == logical_dim_size:
                 logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.EQUAL
             elif physical_dim_size == 1 and physical_dim_size != logical_dim_size:
                 logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.MULTIPLE
         else:
-            logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.PADDDING
+            logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.PADDING
 
     return logical_dim_broadcast_info
 
 
 def recover_sharding_spec_for_broadcast_shape(logical_sharding_spec: ShardingSpec, logical_shape: torch.Size,
                                               physical_shape: torch.Size) -> ShardingSpec:
     """
@@ -113,15 +113,15 @@
     # generate the sharding spec for the physical shape
     physical_dim_partition = {}
     logical_dim_partition = logical_sharding_spec.dim_partition_dict
 
     for shape_dim, mesh_dim in logical_dim_partition.items():
         logical_broadcast_type = logical_dim_broadcast_info[shape_dim]
 
-        if logical_broadcast_type == BroadcastType.PADDDING or logical_broadcast_type == BroadcastType.MULTIPLE:
+        if logical_broadcast_type == BroadcastType.PADDING or logical_broadcast_type == BroadcastType.MULTIPLE:
             removed_dims.extend(mesh_dim)
         else:
             # get the corresponding physical dim
             physical_dim = physical_num_dims - (logical_num_dims - shape_dim)
             physical_dim_partition[physical_dim] = mesh_dim
 
     physical_sharding_spec = ShardingSpec(device_mesh=logical_sharding_spec.device_mesh,
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Args:
         input_ (Union[Node, torch.Tensor]): the input can be a Node object or a PyTorch tensor. If a node is used, it will look for its meta data associated with this node.
         device_mesh (DeviceMesh): a DeviceMesh object which contains the meta information about the cluster.
         dim_partition_dict (Dict[int, List[int]]): a dictionary to specify the sharding specs, the key is the tensor dimension and the value is the mesh dimension for sharding.
     """
 
     if isinstance(input_, Node):
-        assert hasattr(input_, '_meta_data'), f'The given node has no attribte _meta_data'
+        assert hasattr(input_, '_meta_data'), f'The given node has no attribute _meta_data'
         meta_tensor = input_._meta_data
         assert meta_tensor is not None, "The given node's _meta_data attribute is None"
         shape = meta_tensor.shape
     elif isinstance(input_, torch.Tensor):
         shape = input_.shape
     else:
         raise TypeError(
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from typing import Dict, List, Tuple
 
 import torch
 
 
 class PreviousStatus(Enum):
     """
-    This class shows the status of previous comparision.
+    This class shows the status of previous comparison.
     """
     RESET = 0
-    # ORIGIN means the dimension size of original tensor is larger in the previous comparision.
+    # ORIGIN means the dimension size of original tensor is larger in the previous comparison.
     ORIGIN = 1
-    # TGT means the dimension size of target tensor is larger in the previous comparision.
+    # TGT means the dimension size of target tensor is larger in the previous comparison.
     TGT = 2
 
 
 def detect_reshape_mapping(origin_shape: torch.Size, tgt_shape: torch.Size) -> Dict[Tuple[int], Tuple[int]]:
     """
     This method is used to detect the reshape mapping between original tensor and target tensor.
 
@@ -87,15 +87,15 @@
 
             previous_label = PreviousStatus.RESET
 
         elif original_dimension_size > tgt_dimension_size:
             tgt_index += 1
 
             if previous_label == PreviousStatus.TGT:
-                # if the target dimension size is larger in the previous comparision, which means
+                # if the target dimension size is larger in the previous comparison, which means
                 # the origin dimension size has already accumulated larger than target dimension size, so
                 # we need to offload the origin dims and tgt dims into the reshape_mapping_dict.
                 reshape_mapping_dict[tuple(origin_dims)] = tuple(tgt_dims)
                 original_dimension_size = original_dimension_size // tgt_dimension_size
                 origin_dims = [origin_len - origin_index - 1]
                 tgt_dimension_size = tgt_shape[tgt_index]
                 tgt_dims = [tgt_len - tgt_index - 1, tgt_len - tgt_index]
@@ -107,15 +107,15 @@
                 tgt_dims.append(tgt_len - tgt_index - 1)
                 previous_label = PreviousStatus.ORIGIN
 
         else:
             origin_index += 1
 
             if previous_label == PreviousStatus.ORIGIN:
-                # if the origin element is larger in the previous comparision, which means
+                # if the origin element is larger in the previous comparison, which means
                 # the target element has already accumulated larger than origin element, so
                 # we need to offload the origin dims and tgt dims into the reshape_mapping_dict.
                 reshape_mapping_dict[tuple(origin_dims)] = tuple(tgt_dims)
                 tgt_dimension_size = tgt_dimension_size // original_dimension_size
                 tgt_dims = [tgt_len - tgt_index - 1]
                 original_dimension_size = origin_shape[origin_index]
                 origin_dims = [origin_len - origin_index - 1, origin_len - origin_index]
@@ -135,15 +135,15 @@
     """
     This method is used to check whether the reshape operation could implement without converting
     the input to fully replicated status.
 
     Rule:
         For a sharded dimension of input tensor, if it is not the minimum element of the input tuple,
         the function will return false.
-        To illustrate this issue, there are two cases to analyse:
+        To illustrate this issue, there are two cases to analyze:
         1. no sharded dims in the input tuple: we could do the reshape operation safely just as the normal
         operation without distributed tensor.
         2. sharded dims in the input tuple: the sharded dim must be the minimum element, then during shape
         consistency process, torch.cat will be implemented on the sharded dim, and everything after the sharded
         dim get recovered.
 
     Examples:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.6.3/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/booster.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,221 @@
-import warnings
-from contextlib import contextmanager
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Callable, Iterable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
+import warnings
+from packaging import version
+from torch.distributed import ProcessGroup
+
+if version.parse(torch.__version__) >= version.parse('1.12.0'):
+    from torch.distributed.fsdp import FullStateDictConfig
+    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+    from torch.distributed.fsdp import StateDictType
+    from torch.distributed.fsdp.fully_sharded_data_parallel import (
+        BackwardPrefetch,
+        CPUOffload,
+        FullStateDictConfig,
+        MixedPrecision,
+        ShardingStrategy,
+    )
+else:
+    raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
+
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import GeneralCheckpointIO
+from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO, utils
+from colossalai.cluster import DistCoordinator
+from colossalai.interface import ModelWrapper, OptimizerWrapper
+
+from .dp_plugin_base import DPPluginBase
+
+__all__ = ['TorchFSDPPlugin']
+
+
+class TorchFSDPCheckpointIO(GeneralCheckpointIO):
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.coordinator = DistCoordinator()
+
+    def load_unsharded_model(self, model: nn.Module, checkpoint: str, strict: bool):
+        checkpoint = utils.load_state_dict(checkpoint)
+        model.load_state_dict(checkpoint)
+
+    def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: Path):
+        checkpoint = utils.load_state_dict(checkpoint)
+        fsdp_model = optimizer.unwrap_model()
+        sharded_osd = FSDP.scatter_full_optim_state_dict(checkpoint, fsdp_model)
+        optimizer.load_state_dict(sharded_osd)
+
+    def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
+        cfg = FullStateDictConfig(offload_to_cpu=True, rank0_only=True)
+        with FSDP.state_dict_type(model, StateDictType.FULL_STATE_DICT, cfg):
+            full_model_state = model.state_dict()
+        utils.save_state_dict(full_model_state, checkpoint_file_path=checkpoint, use_safetensors=use_safetensors)
+
+    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
+        """
+        Save optimizer to checkpoint but only on master process.
+        """
+        assert isinstance(optimizer, FSDPOptimizerWrapper)
+        fsdp_model = optimizer.unwrap_model()
+        full_optimizer_state = FSDP.full_optim_state_dict(fsdp_model, optim=optimizer, rank0_only=True)
+        utils.save_state_dict(full_optimizer_state, checkpoint_file_path=checkpoint, use_safetensors=False)
 
-from .accelerator import Accelerator
-from .mixed_precision import MixedPrecision, mixed_precision_factory
-from .plugin import Plugin
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
+                           size_per_shard: int, use_safetensors: bool):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
-__all__ = ['Booster']
+    def load_sharded_model(self,
+                           model: nn.Module,
+                           checkpoint_index_file: Path,
+                           strict: bool = False,
+                           use_safetensors: bool = False,
+                           load_sub_module: bool = True):
+        """
+        Load model to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
+    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
+        """
+        Save optimizer to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
 
-class Booster:
+    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str, size_per_shard: int):
+        """
+        Load optimizer to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
+
+    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        if self.coordinator.is_master():
+            super().save_lr_scheduler(lr_scheduler, checkpoint)
+
+
+class TorchFSDPModel(ModelWrapper):
+
+    def __init__(self, module: nn.Module, *args, **kwargs) -> None:
+        super().__init__(module)
+        self.module = FSDP(module, *args, **kwargs)
+
+    def unwrap(self):
+        return self.module
+
+
+class FSDPOptimizerWrapper(OptimizerWrapper):
+
+    def __init__(self, optimizer: Optimizer, model: nn.Module):
+        self.model = model
+        super().__init__(optimizer)
+
+    def unwrap_model(self) -> nn.Module:
+        return self.model
+
+
+class TorchFSDPPlugin(DPPluginBase):
     """
-    Booster is a high-level API for training neural networks. It provides a unified interface for
-    training with different precision, accelerator, and plugin.
+    Plugin for PyTorch FSDP.
 
-    Examples:
-        >>> colossalai.launch(...)
-        >>> plugin = GeminiPlugin(stage=3, ...)
-        >>> booster = Booster(precision='fp16', plugin=plugin)
+    Example:
+        >>> from colossalai.booster import Booster
+        >>> from colossalai.booster.plugin import TorchFSDPPlugin
         >>>
-        >>> model = GPT2()
-        >>> optimizer = Adam(model.parameters())
-        >>> dataloader = Dataloader(Dataset)
-        >>> lr_scheduler = LinearWarmupScheduler()
-        >>> criterion = GPTLMLoss()
-        >>>
-        >>> model, optimizer, lr_scheduler, dataloader = booster.boost(model, optimizer, lr_scheduler, dataloader)
-        >>>
-        >>> for epoch in range(max_epochs):
-        >>>     for input_ids, attention_mask in dataloader:
-        >>>         outputs = model(input_ids, attention_mask)
-        >>>         loss = criterion(outputs.logits, input_ids)
-        >>>         booster.backward(loss, optimizer)
-        >>>         optimizer.step()
-        >>>         lr_scheduler.step()
-        >>>         optimizer.zero_grad()
+        >>> model, train_dataset, optimizer, criterion = ...
+        >>> plugin = TorchFSDPPlugin()
 
+        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
+        >>> booster = Booster(plugin=plugin)
+        >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
-        device (str or torch.device): The device to run the training. Default: 'cuda'.
-        mixed_precision (str or MixedPrecision): The mixed precision to run the training. Default: None.
-                                If the argument is a string, it can be 'fp16', 'fp16_apex', 'bf16', or 'fp8'.
-                                'fp16' would use PyTorch AMP while `fp16_apex` would use Nvidia Apex.
-        plugin (Plugin): The plugin to run the training. Default: None.
+        See https://pytorch.org/docs/stable/fsdp.html for details.
     """
 
-    def __init__(self,
-                 device: str = 'cuda',
-                 mixed_precision: Union[MixedPrecision, str] = None,
-                 plugin: Optional[Plugin] = None) -> None:
-        if plugin is not None:
-            assert isinstance(
-                plugin, Plugin), f'Expected the argument plugin to be an instance of Plugin, but got {type(plugin)}.'
-        self.plugin = plugin
-
-        # set accelerator
-        if self.plugin and self.plugin.control_device():
-            self.accelerator = None
-            warnings.warn('The plugin will control the accelerator, so the device argument will be ignored.')
-        else:
-            self.accelerator = Accelerator(device)
-
-        # set precision
-        if self.plugin and self.plugin.control_precision():
-            warnings.warn('The plugin will control the precision, so the mixed_precision argument will be ignored.')
-            self.mixed_precision = None
-        elif mixed_precision is None:
-            self.mixed_precision = None
-        else:
-            # validate and set precision
-            if isinstance(mixed_precision, str):
-                # the user will take the default arguments for amp training
-                self.mixed_precision = mixed_precision_factory(mixed_precision)
-            elif isinstance(mixed_precision, MixedPrecision):
-                # the user can customize the arguments by passing the precision object
-                self.mixed_precision = mixed_precision
-            else:
-                raise ValueError(
-                    f'Expected the argument mixed_precision to be a string or an instance of Precision, but got {type(mixed_precision)}.'
-                )
-
-        if self.plugin is not None and self.plugin.control_checkpoint_io():
-            self.checkpoint_io = self.plugin.get_checkpoint_io()
-        else:
-            self.checkpoint_io = GeneralCheckpointIO()
+    if version.parse(torch.__version__) >= version.parse('1.12.0'):
+
+        def __init__(
+            self,
+            process_group: Optional[ProcessGroup] = None,
+            sharding_strategy: Optional[ShardingStrategy] = None,
+            cpu_offload: Optional[CPUOffload] = None,
+            auto_wrap_policy: Optional[Callable] = None,
+            backward_prefetch: Optional[BackwardPrefetch] = None,
+            mixed_precision: Optional[MixedPrecision] = None,
+            ignored_modules: Optional[Iterable[torch.nn.Module]] = None,
+            param_init_fn: Optional[Callable[[nn.Module], None]] = None,
+            sync_module_states: bool = False,
+        ):
+            super().__init__()
+            self.fsdp_kwargs = dict(process_group=process_group,
+                                    sharding_strategy=sharding_strategy,
+                                    cpu_offload=cpu_offload,
+                                    auto_wrap_policy=auto_wrap_policy,
+                                    backward_prefetch=backward_prefetch,
+                                    mixed_precision=mixed_precision,
+                                    ignored_modules=ignored_modules,
+                                    param_init_fn=param_init_fn,
+                                    sync_module_states=sync_module_states)
+    else:
+        raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
+
+    def support_no_sync(self) -> bool:
+        False
+
+    def no_sync(self, model: nn.Module) -> Iterator[None]:
+        raise NotImplementedError("Torch fsdp no_sync func not supported yet.")
+
+    def control_precision(self) -> bool:
+        return True
+
+    def supported_precisions(self) -> List[str]:
+        return ['fp16', 'bf16']
 
-    def boost(
+    def control_device(self) -> bool:
+        return True
+
+    def supported_devices(self) -> List[str]:
+        return ['cuda']
+
+    def configure(
         self,
         model: nn.Module,
         optimizer: Optimizer,
         criterion: Callable = None,
         dataloader: DataLoader = None,
         lr_scheduler: LRScheduler = None,
-    ) -> List[Union[nn.Module, Optimizer, LRScheduler, DataLoader]]:
-        """
-        Boost the model, optimizer, criterion, lr_scheduler, and dataloader.
+    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
 
-        Args:
-            model (nn.Module): The model to be boosted.
-            optimizer (Optimizer): The optimizer to be boosted.
-            criterion (Callable): The criterion to be boosted.
-            dataloader (DataLoader): The dataloader to be boosted.
-            lr_scheduler (LRScheduler): The lr_scheduler to be boosted.
-        """
-        # TODO(FrankLeeeee): consider multi-model and multi-optimizer case
-        # TODO(FrankLeeeee): consider multi-dataloader case
-        # transform model for mixed precision
-        if self.plugin:
-            model, optimizer, criterion, dataloader, lr_scheduler = self.plugin.configure(
-                model, optimizer, criterion, dataloader, lr_scheduler)
-
-        if self.plugin and not self.plugin.control_device():
-            # transform model for accelerator
-            model = self.accelerator.configure(model)
-
-        if self.mixed_precision and (self.plugin is None or self.plugin and not self.plugin.control_precision()):
-            # transform model for mixed precision
-            # when mixed_precision is specified and the plugin is not given or does not control the precision
-            model, optimizer, criterion = self.mixed_precision.configure(model, optimizer, criterion)
-
-        return model, optimizer, criterion, dataloader, lr_scheduler
-
-    def backward(self, loss: torch.Tensor, optimizer: Optimizer) -> None:
-        # TODO: implement this method with plugin
-        optimizer.backward(loss)
-
-    def execute_pipeline(self,
-                         data_iter: Iterator,
-                         model: nn.Module,
-                         criterion: Callable[[torch.Tensor], torch.Tensor],
-                         optimizer: Optimizer,
-                         return_loss: bool = True,
-                         return_outputs: bool = False) -> Tuple[Optional[torch.Tensor], ...]:
-        # TODO: implement this method
-        # run pipeline forward backward pass
-        # return loss or outputs if needed
-        pass
-
-    def no_sync(self, model: nn.Module) -> contextmanager:
-        assert self.plugin is not None, f'no_sync is only enabled when a plugin is provided and the plugin supports no_sync.'
-        assert self.plugin.support_no_sync, f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
-        return self.plugin.no_sync(model)
-
-    def load_model(self, model: nn.Module, checkpoint: str, strict: bool = True):
-        self.checkpoint_io.load_model(model, checkpoint, strict)
-
-    def save_model(self,
-                   model: nn.Module,
-                   checkpoint: str,
-                   prefix: str = None,
-                   shard: bool = False,
-                   size_per_shard: int = 1024):
-        self.checkpoint_io.save_model(model, checkpoint, prefix, shard, size_per_shard)
+        # wrap the model with PyTorch FSDP
+        fsdp_model = TorchFSDPModel(model, device_id=torch.cuda.current_device(), **self.fsdp_kwargs)
 
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        self.checkpoint_io.load_optimizer(optimizer, checkpoint)
+        if len(optimizer.param_groups) > 1:
+            warnings.warn(
+                'TorchFSDPPlugin does not support optimizer that use multi param groups. The results may not be as expected if used.'
+            )
+        optimizer.__init__(fsdp_model.parameters(), **optimizer.defaults)
 
-    def save_optimizer(self, optimizer: Optimizer, checkpoint: str, shard: bool = False, size_per_shard: int = 1024):
-        self.checkpoint_io.save_optimizer(optimizer, checkpoint, shard, size_per_shard)
+        if not isinstance(optimizer, FSDPOptimizerWrapper):
+            optimizer = FSDPOptimizerWrapper(optimizer, fsdp_model)
 
-    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
-        self.checkpoint_io.save_lr_scheduler(lr_scheduler, checkpoint)
+        return fsdp_model, optimizer, criterion, dataloader, lr_scheduler
+
+    def control_checkpoint_io(self) -> bool:
+        return True
 
-    def load_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
-        self.checkpoint_io.load_lr_scheduler(lr_scheduler, checkpoint)
+    def get_checkpoint_io(self) -> CheckpointIO:
+        return TorchFSDPCheckpointIO()
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .bf16 import BF16MixedPrecision
 from .fp8 import FP8MixedPrecision
 from .fp16_apex import FP16ApexMixedPrecision
+from .fp16_naive import FP16NaiveMixedPrecision
 from .fp16_torch import FP16TorchMixedPrecision
 from .mixed_precision_base import MixedPrecision
 
 __all__ = [
     'MixedPrecision', 'mixed_precision_factory', 'FP16_Apex_MixedPrecision', 'FP16_Torch_MixedPrecision',
-    'FP32_MixedPrecision', 'BF16_MixedPrecision', 'FP8_MixedPrecision'
+    'FP32_MixedPrecision', 'BF16_MixedPrecision', 'FP8_MixedPrecision', 'FP16NaiveMixedPrecision'
 ]
 
 _mixed_precision_mapping = {
     'fp16': FP16TorchMixedPrecision,
     'fp16_apex': FP16ApexMixedPrecision,
+    'fp16_naive': FP16NaiveMixedPrecision,
     'bf16': BF16MixedPrecision,
     'fp8': FP8MixedPrecision
 }
 
 
 def mixed_precision_factory(mixed_precision_type: str) -> MixedPrecision:
     """
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,27 @@
     def __init__(self) -> None:
         super().__init__()
         assert dist.is_initialized(
         ), 'torch.distributed is not initialized, please use colossalai.launch to create the distributed environment'
         self.rank = dist.get_rank()
         self.world_size = dist.get_world_size()
 
-    def prepare_train_dataloader(self,
-                                 dataset,
-                                 batch_size,
-                                 shuffle=False,
-                                 seed=1024,
-                                 drop_last=False,
-                                 pin_memory=False,
-                                 num_workers=0,
-                                 **kwargs):
+    def prepare_dataloader(self,
+                           dataset,
+                           batch_size,
+                           shuffle=False,
+                           seed=1024,
+                           drop_last=False,
+                           pin_memory=False,
+                           num_workers=0,
+                           **kwargs):
         r"""
         Prepare a dataloader for distributed training. The dataloader will be wrapped by
         `torch.utils.data.DataLoader` and `torch.utils.data.DistributedSampler`.
 
-        Note:
-            1. Evaluation datasets should not be passed to this function.
 
         Args:
             dataset (`torch.utils.data.Dataset`): The dataset to be loaded.
             shuffle (bool, optional): Whether to shuffle the dataset. Defaults to False.
             seed (int, optional): Random worker seed for sampling, defaults to 1024.
             add_sampler: Whether to add ``DistributedDataParallelSampler`` to the dataset. Defaults to True.
             drop_last (bool, optional): Set to True to drop the last incomplete batch, if the dataset size
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import warnings
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
@@ -48,16 +48,24 @@
             save_state_dict(state_dict, checkpoint, use_safetensors)
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
         # TODO(ver217): optimizer state dict is sharded
+        warnings.warn('GeminiPlugin does not support save full optimizer checkpoint now. Save it on every process.')
+        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
         super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
 
+    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
+        warnings.warn(
+            'GeminiPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
+        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
+        super().load_optimizer(optimizer, checkpoint)
+
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """
         Save model to checkpoint but only on master process.
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
@@ -152,30 +160,30 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import GeminiPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = GeminiPlugin()
 
-        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         device (torch.device): device to place the model.
         placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
         pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
         force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
         strict_ddp_mode (bool, optional): use strict ddp mode (only use dp without other parallelism). Defaults to False.
         search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
         hidden_dim (int, optional): the hidden dimension of DNN.
             Users can provide this argument to speed up searching.
             If users do not know this argument before training, it is ok. We will use a default value 1024.
         min_chunk_size_mb (float, optional): the minimum chunk size in MegaByte.
-            If the aggregate size of parameters is still samller than the minimum chunk size,
+            If the aggregate size of parameters is still smaller than the minimum chunk size,
             all parameters will be compacted into one small chunk.
         memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
             This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
             Defaults to 0.0.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
@@ -282,7 +290,10 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return GeminiCheckpointIO()
+
+    def no_sync(self, model: nn.Module) -> Iterator[None]:
+        raise NotImplementedError
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import warnings
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import CheckpointIO
+from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.utils import get_current_device
 from colossalai.zero import zero_model_wrapper, zero_optim_wrapper
 
 from .dp_plugin_base import DPPluginBase
 from .torch_ddp_plugin import TorchDDPCheckpointIO
 
@@ -28,16 +28,25 @@
 
 class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
-        # TODO(ver217): optimizer state dict is sharded
-        super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
+        # TODO(ver217): optimizer state dict is sharded, and cannot get full state dict now
+        warnings.warn(
+            'LowLevelZeroPlugin does not support save full optimizer checkpoint now. Save it on every process.')
+        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
+        GeneralCheckpointIO.save_unsharded_optimizer(self, optimizer, checkpoint, gather_dtensor)
+
+    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
+        warnings.warn(
+            'LowLevelZeroPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
+        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
+        super().load_optimizer(optimizer, checkpoint)
 
 
 class LowLevelZeroModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
         super().__init__(module)
         self.convert_inputs = (precision == 'fp16')
@@ -91,15 +100,15 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import LowLevelZeroPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = LowLevelZeroPlugin()
 
-        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         strage (int, optional): ZeRO stage. Defaults to 1.
         precision (str, optional): precision. Support 'fp16' and 'fp32'. Defaults to 'fp16'.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
@@ -193,7 +202,10 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return LowLevelZeroCheckpointIO()
+
+    def no_sync(self, model: nn.Module) -> Iterator[None]:
+        raise NotImplementedError
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/plugin_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
-from typing import Callable, List, Tuple, Union
+from typing import Callable, Iterator, List, Tuple, Union
 
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
-from torch.utils.data import DataLoader
+from torch.utils.data import DataLoader, Dataset
 
 from colossalai.checkpoint_io import CheckpointIO
 from colossalai.interface import OptimizerWrapper
 
 __all__ = ['Plugin']
 
 
@@ -55,7 +55,29 @@
 
     @abstractmethod
     def get_checkpoint_io(self) -> CheckpointIO:
         """
         Get checkpoint io object for this plugin, only invoked when control_checkpoint_io is True.
         """
         pass
+
+    @abstractmethod
+    def no_sync(self, model: nn.Module) -> Iterator[None]:
+        """
+        Context manager to disable gradient synchronization.
+        """
+        pass
+
+    @abstractmethod
+    def prepare_dataloader(self,
+                           dataset: Dataset,
+                           batch_size: int,
+                           shuffle: bool = False,
+                           seed: int = 1024,
+                           drop_last: bool = False,
+                           pin_memory: bool = False,
+                           num_workers: int = 0,
+                           **kwargs):
+        """Prepare a dataloader for distributed training. The dataloader will be wrapped by
+        `torch.utils.data.DataLoader`
+        """
+        pass
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, List, Tuple, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch.nn as nn
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
@@ -46,14 +46,24 @@
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """
         Save model to checkpoint but only on master process.
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
+    def save_sharded_model(self,
+                           model: nn.Module,
+                           checkpoint_path: str,
+                           gather_dtensor: bool = False,
+                           variant: Optional[str] = None,
+                           max_shard_size: int = 1024,
+                           use_safetensors: bool = False):
+        if self.coordinator.is_master():
+            super().save_sharded_model(model, checkpoint_path, gather_dtensor, variant, max_shard_size, use_safetensors)
+
 
 class TorchDDPModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, *args, **kwargs) -> None:
         super().__init__(module)
         self.module = DDP(module, *args, **kwargs)
 
@@ -68,15 +78,15 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import TorchDDPPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = TorchDDPPlugin()
 
-        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         broadcast_buffers (bool, optional): Whether to broadcast buffers in the beginning of training. Defaults to True.
         bucket_cap_mb (int, optional): The bucket size in MB. Defaults to 25.
         find_unused_parameters (bool, optional): Whether to find unused parameters. Defaults to False.
@@ -138,7 +148,11 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return TorchDDPCheckpointIO()
+
+    def no_sync(self, model: nn.Module) -> Iterator[None]:
+        assert isinstance(model, TorchDDPModel), 'Model is not boosted by TorchDDPPlugin.'
+        return model.module.no_sync()
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/builder/builder.py` & `colossalai-nightly-2023.6.3/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Union
-from typing import Optional
+from typing import Optional, Union
 
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
 from colossalai.interface import ModelWrapper
@@ -80,17 +79,16 @@
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
         """
         # since we only support loaded sharded and unsharded weight format
         # containing no distributed tensors, dtensor -> full tensor conversion
         # should be done offline via our CLI
         # the existence of index file means it is a sharded checkpoint
-        ckpt_path = Path(checkpoint)
         index_file_exists, index_file_path = has_index_file(checkpoint)
-        
+
         # return the origin model instead of the unwrapped model
         origin_model = model
 
         if isinstance(model, ModelWrapper):
             model = model.unwrap()
 
         if index_file_exists:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from pathlib import Path
+import gc
+import logging
+import os
 from functools import reduce
+from pathlib import Path
+from typing import Iterator, Optional, OrderedDict, Tuple
 
 import torch.nn as nn
 from torch.optim import Optimizer
-import logging
-import os
-import gc
-from typing import Optional, Iterator, OrderedDict, Tuple
 
 from .checkpoint_io_base import CheckpointIO
 from .index_file import CheckpointIndexFile
 from .utils import (
-    has_index_file, 
-    load_state_dict, 
-    save_state_dict, 
+    get_base_filenames,
+    get_shard_filename,
+    has_index_file,
     is_safetensors_available,
-    shard_checkpoint,
     load_shard_state_dict,
+    load_state_dict,
     load_state_dict_into_model,
-    get_shard_filename,
-    get_base_filenames
-    )
+    save_state_dict,
+    shard_checkpoint,
+)
 
 __all__ = ['GeneralCheckpointIO']
 
 
 class GeneralCheckpointIO(CheckpointIO):
     """
     Checkpoint IO
     """
+
     def load_unsharded_model(self, model: nn.Module, checkpoint: str, strict: bool):
         checkpoint = load_state_dict(checkpoint)
         model.load_state_dict(checkpoint, strict=strict)
 
     def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
         state_dict = model.state_dict()
 
@@ -65,79 +66,81 @@
         optimizer: Optimizer,
         checkpoint: Path,
         gather_dtensor: bool,
     ):
         # TODO(FrankLeeeee): handle distributed tensors
         save_state_dict(optimizer.state_dict(), checkpoint, use_safetensors=False)
 
-
-    def save_sharded_model(self, model: nn.Module, checkpoint_path: str, gather_dtensor:bool = False, 
-                           variant: Optional[str] = None, max_shard_size: int = 1024, use_safetensors: bool = False):
-        """ 
+    def save_sharded_model(self,
+                           model: nn.Module,
+                           checkpoint_path: str,
+                           gather_dtensor: bool = False,
+                           variant: Optional[str] = None,
+                           max_shard_size: int = 1024,
+                           use_safetensors: bool = False):
+        """
         implement this method as it can be supported by Huggingface model,
         save shard model, save model to multiple files
         """
         if os.path.isfile(checkpoint_path):
             logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
             return
-        
+
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
-        
+
         # shard checkpoint
         state_dict = model.state_dict()
         state_dict_shard = shard_checkpoint(state_dict, max_shard_size=max_shard_size)
 
         weights_name, save_index_file = get_base_filenames(variant, use_safetensors)
         total_size = 0
         index_file = CheckpointIndexFile(checkpoint_path)
         for idx, shard_pair in enumerate(state_dict_shard):
             shard = shard_pair[0]
             shard_file = get_shard_filename(weights_name, idx)
             total_size = total_size + shard_pair[1]
             for key in shard.keys():
                 index_file.append_weight_map(key, shard_file)
-            
+
             checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors)
-        
+
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
-        logging.info(
-            f"The model is going to be split to checkpoint shards. "
-            f"You can find where each parameters has been saved in the "
-            f"index located at {save_index_file}."
-        )
-
-
-    def load_sharded_model(self, model: nn.Module, checkpoint_index_file: Path, strict: bool = False, 
-                           use_safetensors: bool = False, load_sub_module: bool = True):
+        logging.info(f"The model is going to be split to checkpoint shards. "
+                     f"You can find where each parameters has been saved in the "
+                     f"index located at {save_index_file}.")
+
+    def load_sharded_model(self,
+                           model: nn.Module,
+                           checkpoint_index_file: Path,
+                           strict: bool = False,
+                           use_safetensors: bool = False,
+                           load_sub_module: bool = True):
         """
         load shard model, load model from multiple files
         """
         use_safetensors = False
         if "safetensors" in checkpoint_index_file.name:
             use_safetensors = True
 
         if use_safetensors and not is_safetensors_available():
             raise ImportError("`safe_serialization` requires the `safetensors` library: `pip install safetensors`.")
-        
+
         # read checkpoint index file
         ckpt_index_file = CheckpointIndexFile.from_file(checkpoint_index_file)
         checkpoint_files, _ = ckpt_index_file.get_checkpoint_fileanames()
         missing_keys = []
 
         for shard_file in checkpoint_files:
             state_dict = load_shard_state_dict(Path(shard_file), use_safetensors)
             load_state_dict_into_model(model, state_dict, missing_keys, strict, load_sub_module)
             del state_dict
             gc.collect()
 
         if strict:
             remain_keys = reduce(lambda a, b: a & b, map(set, missing_keys))
             if len(remain_keys) > 0:
-                error_msgs = 'Missing key(s) in state_dict: {}. '.format(
-                            ', '.join('"{}"'.format(k) for k in missing_keys))
+                error_msgs = 'Missing key(s) in state_dict: {}. '.format(', '.join(
+                    '"{}"'.format(k) for k in missing_keys))
                 raise RuntimeError('Error(s) in loading state_dict for {}:\n\t{}'.format(
-                                self.__class__.__name__, "\n\t".join(error_msgs)))
-
-
-
+                    self.__class__.__name__, "\n\t".join(error_msgs)))
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/index_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,14 @@
         """
         Get all the weight keys.
         """
         return list(self.weight_map.keys())
     
     def write_index_file(self, save_index_file):
         """
-        Wriete index file.
+        Write index file.
         """
         save_index_file = os.path.join(self.root_path, save_index_file)
         index = {"metadata": self.metadata, "weight_map": self.weight_map}
         with open(save_index_file, "w", encoding="utf-8") as f:
             content = json.dumps(index, indent=2, sort_keys=True) + "\n"
             f.write(content)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # coding=utf-8
+import re
 from pathlib import Path
+from typing import Iterator, List, Mapping, Optional, OrderedDict, Tuple
+
 import torch
 import torch.nn as nn
-from typing import List, Mapping, OrderedDict, Optional, Tuple, Iterator
+
 from colossalai.tensor.d_tensor.d_tensor import DTensor
-import re
 
 SAFE_WEIGHTS_NAME = "model.safetensors"
 WEIGHTS_NAME = "pytorch_model.bin"
 SAFE_WEIGHTS_INDEX_NAME = "model.safetensors.index.json"
 WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
 
 # ======================================
 # General helper functions
 # ======================================
 
+
 def calculate_tensor_size(tensor: torch.Tensor) -> float:
     """
     Calculate the size of a parameter in MB. Used to compute whether a group of params exceed the shard size.
     If so, a new shard should be created.
 
     Args:
-        tenosr (torch.Tensor): the tensor to calculate size for.
+        tensor (torch.Tensor): the tensor to calculate size for.
 
     Returns:
         float: size of the tensor in MB.
     """
     return tensor.numel() * tensor.element_size() / 1024 / 1024
 
+
 def is_safetensors_available() -> bool:
     """
     Check whether safetensors is available.
 
     Returns:
         bool: whether safetensors is available.
     """
@@ -74,15 +78,14 @@
         return False
 
 
 # ======================================
 # Helper functions for saving shard file
 # ======================================
 def shard_checkpoint(state_dict: torch.Tensor, max_shard_size: int = 1024) -> Iterator[Tuple[OrderedDict, int]]:
- 
     """
     Splits a model state dictionary in sub-checkpoints so that the final size of each sub-checkpoint does not exceed a
     given size.
     """
     current_block = {}
     current_block_size = 0
 
@@ -96,43 +99,47 @@
             if current_block_size + weight_size > max_shard_size:
                 ret_block = current_block
                 ret_block_size = current_block_size
                 current_block = {}
                 current_block_size = 0
             current_block[key] = weight
             current_block_size += weight_size
-            
+
         if ret_block != None:
             yield ret_block, ret_block_size
 
     yield current_block, current_block_size
 
 
-def load_shard_state_dict(checkpoint_file: Path, use_safetensors: bool =False):
+def load_shard_state_dict(checkpoint_file: Path, use_safetensors: bool = False):
     """
     load shard state dict into model
     """
     if use_safetensors and not checkpoint_file.suffix == ".safetensors":
         raise Exception("load the model using `safetensors`, but no file endwith .safetensors")
     if use_safetensors:
-        from safetensors.torch import safe_open
         from safetensors.torch import load_file as safe_load_file
+        from safetensors.torch import safe_open
         with safe_open(checkpoint_file, framework="pt") as f:
             metadata = f.metadata()
         if metadata["format"] != "pt":
             raise NotImplementedError(
-                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet."
-            )
+                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet.")
         return safe_load_file(checkpoint_file)
     else:
         return torch.load(checkpoint_file)
-    
-def load_state_dict_into_model(model: nn.Module, state_dict: torch.Tensor, missing_keys: List, strict: bool = False, load_sub_module: bool = True):
+
+
+def load_state_dict_into_model(model: nn.Module,
+                               state_dict: torch.Tensor,
+                               missing_keys: List,
+                               strict: bool = False,
+                               load_sub_module: bool = True):
     r"""Copies parameters and buffers from :attr:`state_dict` into
-    this module and its descendants. 
+    this module and its descendants.
 
     Args:
         state_dict (dict): a dict containing parameters and
             persistent buffers.
     """
     if not isinstance(state_dict, Mapping):
         raise TypeError("Expected state_dict to be dict-like, got {}.".format(type(state_dict)))
@@ -162,19 +169,20 @@
     load(model, state_dict, "", load_sub_module)
     del load
 
     missing_keys = missing_keys.append(sub_missing_keys)
 
     if strict:
         if len(unexpected_keys) > 0:
-            error_msgs = 'Unexpected key(s) in state_dict: {}. '.format(
-                        ', '.join('"{}"'.format(k) for k in unexpected_keys))
+            error_msgs = 'Unexpected key(s) in state_dict: {}. '.format(', '.join(
+                '"{}"'.format(k) for k in unexpected_keys))
             raise RuntimeError('Error(s) in loading state_dict for {}:\n\t{}'.format(
-                               model.__class__.__name__, "\n\t".join(error_msgs)))
-        
+                model.__class__.__name__, "\n\t".join(error_msgs)))
+
+
 # ======================================
 # Helper functions for saving state dict
 # ======================================
 
 
 def save_state_dict(state_dict: dict, checkpoint_file_path: str, use_safetensors: bool) -> None:
     """
@@ -346,14 +354,16 @@
                 index_files
             ) == 1, f'Expected to find one .index.json file in {checkpoint_path}, but found {len(index_files)}'
 
         if len(index_files) == 1:
             return True, index_files[0]
         else:
             return False, None
+    else:
+        raise RuntimeError(f'Invalid checkpoint path {checkpoint_path}. Expected a file or a directory.')
 
 
 def load_state_dict(checkpoint_file_path: Path):
     """
     Load state dict from checkpoint.
 
     Args:
@@ -376,38 +386,38 @@
             for k in f.keys():
                 state_dict[k] = f.get_tensor(k)
         return state_dict
 
     else:
         # load with torch
         return torch.load(checkpoint_file_path)
-    
 
 
 def add_variant(weights_name: str, variant: Optional[str] = None) -> str:
     if variant is not None and len(variant) > 0:
         splits = weights_name.split(".")
         splits = splits[:-1] + [variant] + splits[-1:]
         weights_name = ".".join(splits)
 
     return weights_name
 
 
-def get_base_filenames(variant: str=None, use_safetensors: bool=False):
-        """
-        generate base weight filenames
-        """
-        weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
-        weights_name = add_variant(weights_name, variant)
+def get_base_filenames(variant: str = None, use_safetensors: bool = False):
+    """
+    generate base weight filenames
+    """
+    weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
+    weights_name = add_variant(weights_name, variant)
+
+    save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
+    save_index_file = add_variant(save_index_file, variant)
 
-        save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
-        save_index_file = add_variant(save_index_file, variant)
+    return weights_name, save_index_file
 
-        return weights_name, save_index_file
 
 def get_shard_filename(weights_name: str, idx: int):
     """
     get shard file name
     """
     shard_file = weights_name.replace(".bin", f"-{idx+1:05d}.bin")
     shard_file = shard_file.replace(".safetensors", f"-{idx + 1:05d}.safetensors")
-    return shard_file
+    return shard_file
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.6.3/colossalai/cli/check/check_installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ```
 
     Returns: A table of installation information.
     """
     found_aot_cuda_ext = _check_aot_built_cuda_extension_installed()
     cuda_version = _check_cuda_version()
     torch_version, torch_cuda_version = _check_torch_version()
-    colossalai_verison, prebuilt_torch_version_required, prebuilt_cuda_version_required = _parse_colossalai_version()
+    colossalai_version, prebuilt_torch_version_required, prebuilt_cuda_version_required = _parse_colossalai_version()
 
     # if cuda_version is None, that means either
     # CUDA_HOME is not found, thus cannot compare the version compatibility
     if not cuda_version:
         sys_torch_cuda_compatibility = None
     else:
         sys_torch_cuda_compatibility = _is_compatible([cuda_version, torch_cuda_version])
@@ -53,15 +53,15 @@
     if prebuilt_torch_version_required is None:
         torch_compatibility = None
     else:
         torch_compatibility = _is_compatible([torch_version, prebuilt_torch_version_required])
 
     click.echo(f'#### Installation Report ####')
     click.echo(f'\n------------ Environment ------------')
-    click.echo(f"Colossal-AI version: {to_click_output(colossalai_verison)}")
+    click.echo(f"Colossal-AI version: {to_click_output(colossalai_version)}")
     click.echo(f"PyTorch version: {to_click_output(torch_version)}")
     click.echo(f"System CUDA version: {to_click_output(cuda_version)}")
     click.echo(f"CUDA version required by PyTorch: {to_click_output(torch_cuda_version)}")
     click.echo("")
     click.echo(f"Note:")
     click.echo(f"1. The table above checks the versions of the libraries/tools in the current environment")
     click.echo(f"2. If the System CUDA version is N/A, you can set the CUDA_HOME environment variable to locate it")
@@ -133,23 +133,23 @@
         torch_version_for_aot_build: PyTorch version used for AOT compilation of CUDA kernels.
         cuda_version_for_aot_build: CUDA version used for AOT compilation of CUDA kernels.
     """
     # colossalai version can be in two formats
     # 1. X.X.X+torchX.XXcuXX.X (when colossalai is installed with CUDA extensions)
     # 2. X.X.X (when colossalai is not installed with CUDA extensions)
     # where X represents an integer.
-    colossalai_verison = colossalai.__version__.split('+')[0]
+    colossalai_version = colossalai.__version__.split('+')[0]
 
     try:
         torch_version_for_aot_build = colossalai.__version__.split('torch')[1].split('cu')[0]
         cuda_version_for_aot_build = colossalai.__version__.split('cu')[1]
     except:
         torch_version_for_aot_build = None
         cuda_version_for_aot_build = None
-    return colossalai_verison, torch_version_for_aot_build, cuda_version_for_aot_build
+    return colossalai_version, torch_version_for_aot_build, cuda_version_for_aot_build
 
 
 def _check_aot_built_cuda_extension_installed():
     """
     According to `op_builder/README.md`, the CUDA extension can be built with either
     AOT (ahead-of-time) or JIT (just-in-time) compilation.
     AOT compilation will build CUDA extensions to `colossalai._C` during installation.
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
               help="Specify computing devices to use during execution. String format is <host1>,<host2>,"
               " only effective when used with --hostfile.")
 @click.option(
     "--exclude",
     type=str,
     default=None,
     help=
-    "Specify computing devices to NOT use during execution. Mutually exclusive with --include. Formatting is the same as --includ,"
+    "Specify computing devices to NOT use during execution. Mutually exclusive with --include. Formatting is the same as --include,"
     " only effective when used with --hostfile.")
 @click.option("--num_nodes",
               type=int,
               default=-1,
               help="Total number of worker nodes to use, only effective when used with --hostfile.")
 @click.option("--nproc_per_node", type=int, default=None, help="Number of GPUs to use on each node.")
 @click.option("--master_port",
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/hostinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """
 
         if port is None:
             port = 22    # no port specified, lets just use the ssh port
 
         # socket.getfqdn("127.0.0.1") does not return localhost
         # on some users' machines
-        # thus, we directly return True if hostname is locahost, 127.0.0.1 or 0.0.0.0
+        # thus, we directly return True if hostname is localhost, 127.0.0.1 or 0.0.0.0
         if hostname in ("localhost", "127.0.0.1", "0.0.0.0"):
             return True
 
         hostname = socket.getfqdn(hostname)
         localhost = socket.gethostname()
         localaddrs = socket.getaddrinfo(localhost, port)
         targetaddrs = socket.getaddrinfo(hostname, port)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/multinode_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,14 @@
             conn.send('exit')
 
     def recv_from_all(self) -> dict:
         """
         Receive messages from all hosts
 
         Returns:
-            msg_from_node (dict): a dictionry which contains messages from each node
+            msg_from_node (dict): a dictionary which contains messages from each node
         """
 
         msg_from_node = dict()
         for hostname, conn in self.master_recv_conns.items():
             msg_from_node[hostname] = conn.recv()
         return msg_from_node
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
     # stop all nodes
     runner.stop_all()
 
     # receive the stop status
     msg_from_node = runner.recv_from_all()
 
-    # printe node status
+    # print node status
     click.echo("\n====== Stopping All Nodes =====")
     for hostname, msg in msg_from_node.items():
         click.echo(f"{hostname}: {msg}")
 
     # give the process an exit code
     # so that it behaves like a normal process
     if has_error:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/dist_coordinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             >>>
             >>> @dist_coordinator.on_master_only()
             >>> def print_on_master(msg):
             >>>     print(msg)
         """
         is_master = self.is_master(process_group)
 
-        # define an inner functiuon
+        # define an inner function
         def decorator(func):
 
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 if is_master:
                     return func(*args, **kwargs)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/collective.py` & `colossalai-nightly-2023.6.3/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/p2p.py` & `colossalai-nightly-2023.6.3/colossalai/communication/p2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     """Copy the gradient tensor from the next stage in pipeline as the input gradient of this stage.
 
     Args:
         output_grad_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
         next_rank (int, optional): The rank of the source of the tensor.
 
     Returns:
-        Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]: The input gradient tensor or gradident tensor list.
+        Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]: The input gradient tensor or gradient tensor list.
     """
     if gpc.is_pipeline_last_stage():
         output_tensor_grad = None
     else:
         _, output_tensor_grad = _communicate(recv_next=True,
                                              recv_next_shape=output_grad_shape,
                                              next_rank=next_rank,
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.6.3/colossalai/communication/p2p_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 _pg_manager = {}
 _unpickler = pickle.Unpickler
 
 
 def init_process_group():
-    """intialise process group by dist.new_group in the adjacent stages
+    """initialise process group by dist.new_group in the adjacent stages
 
     Args:
         None
 
     Returns:
         None
     """
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/ring.py` & `colossalai-nightly-2023.6.3/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/communication/utils.py` & `colossalai-nightly-2023.6.3/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/constants.py` & `colossalai-nightly-2023.6.3/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/config.py` & `colossalai-nightly-2023.6.3/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/moe_context.py` & `colossalai-nightly-2023.6.3/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.6.3/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.6.3/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Returns:
             List[Tuple (local_rank, group_world_size, process_group, ranks_in_group, mode)]:
                 A Sequence parallelism's information in list of tuples.
         """
 
         parallel_setting = []
 
-        local_rank, group_world_size, process_group, cpu_grop, ranks_in_group, mode = \
+        local_rank, group_world_size, process_group, cpu_group, ranks_in_group, mode = \
             self._sequence_initializer.init_dist_group()
         # change mode to sequence
         mode = ParallelMode.SEQUENCE
 
-        parallel_setting.append((local_rank, group_world_size, process_group, cpu_grop, ranks_in_group, mode))
+        parallel_setting.append((local_rank, group_world_size, process_group, cpu_group, ranks_in_group, mode))
         parallel_setting.append(self._sequence_dp_initializer.init_dist_group())
         return parallel_setting
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.6.3/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.6.3/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.6.3/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/device/alpha_beta_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             else:
                 beta = 1 / bandwidth
 
             broadcast_list = [alpha, beta]
             dist.broadcast_object_list(broadcast_list, src=process_group[0])
             alpha_beta_dict[process_group] = tuple(broadcast_list)
 
-        # add symmetry pair to the apha_beta_dict
+        # add symmetry pair to the alpha_beta_dict
         symmetry_ab_dict = {}
         for process_group, alpha_beta_pair in alpha_beta_dict.items():
             symmetry_process_group = (process_group[1], process_group[0])
             symmetry_ab_dict[symmetry_process_group] = alpha_beta_pair
 
         alpha_beta_dict.update(symmetry_ab_dict)
 
@@ -377,12 +377,12 @@
             broadcast_object = [latency, bandwidth]
             dist.broadcast_object_list(broadcast_object, src=pg[0])
             return broadcast_object
 
         first_latency, first_bandwidth = _extract_alpha_beta(first_axis, first_axis_process_group)
         second_latency, second_bandwidth = _extract_alpha_beta(second_axis, second_axis_process_group)
         mesh_alpha = [first_latency, second_latency]
-        # The beta values have been enlarged by 1e10 times temporarilly because the computation cost
+        # The beta values have been enlarged by 1e10 times temporarily because the computation cost
         # is still estimated in the unit of TFLOPs instead of time. We will remove this factor in future.
         mesh_beta = [1e10 / first_bandwidth, 1e10 / second_bandwidth]
 
         return mesh_alpha, mesh_beta
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.6.3/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.6.3/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,17 @@
             return [val[offset:offset + self.microbatch_size] for val in data]
         elif isinstance(data, dict):
             return {k: v[offset:offset + self.microbatch_size] for k, v in data.items()}
         else:
             raise TypeError(f"Expected data to be of type torch.Tensor, list, tuple, or dict, but got {type(data)}")
 
     def load_micro_batch(self):
-        mciro_batch_data = self._get_data_slice(self.batch_data, self.microbatch_offset)
+        micro_batch_data = self._get_data_slice(self.batch_data, self.microbatch_offset)
         self.microbatch_offset += self.microbatch_size
-        return self._move_to_device(mciro_batch_data)
+        return self._move_to_device(micro_batch_data)
 
     def pre_processing(self, engine):
         from colossalai.zero.legacy import ShardedModelV2
 
         # TODO: remove this after testing new zero with pipeline parallelism
         model = engine.model
         if isinstance(model, NaiveAMPModel):
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             Tuple[:class:`torch.Tensor`]: A tuple of (output, label, loss), loss and label could be None.
         """
 
         assert forward_only or return_loss, \
             'The argument \'return_loss\' has to be True when \'forward_only\' is False, but got False.'
         self.load_batch(data_iter)
 
-        # num_warmup_microbatches is the step when not all the processers are working
+        # num_warmup_microbatches is the step when not all the processes are working
         num_warmup_microbatches = \
             (gpc.get_world_size(ParallelMode.PIPELINE)
              - gpc.get_local_rank(ParallelMode.PIPELINE) - 1)
         num_warmup_microbatches = min(num_warmup_microbatches, self.num_microbatches)
         num_microbatches_remaining = self.num_microbatches - num_warmup_microbatches
 
         # Input, output tensors only need to be saved when doing backward passes
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.6.3/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
         inputs, outputs = _find_input_and_output_nodes(offload_node_list)
         offload_inputs.append(inputs)
         offload_outputs.append(outputs)
 
     # append code text to body
     for idx, node in enumerate(node_list):
         # if this is the first node of the ckpt region
-        # append the ckpt function defition
+        # append the ckpt function definition
         if idx in start_idx:
             label = start_idx.index(idx)
             ckpt_fn_def = _gen_ckpt_fn_def(label, input_vars[label])
             ckpt_func.append(f'{ckpt_fn_def}\n')
             within_ckpt_region = True
 
         if idx in offload_starts:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 split_node = mod_graph.create_node('call_function', pipe_split)
     gm.recompile()
     return gm
 
 
 def avgnode_split_pass(gm: torch.fx.GraphModule, pp_size: int):
     """
-    In avgnode_split_pass, simpliy split graph by node number.
+    In avgnode_split_pass, simply split graph by node number.
     """
     mod_graph = gm.graph
     avg_num_node = len(mod_graph.nodes) // pp_size
     accumulate_num_node = 0
     for node in mod_graph.nodes:
         if pp_size <= 1:
             break
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/meta_info_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     shape: torch.Size
     dtype: torch.dtype
     requires_grad: bool
     stride: Tuple[int]
     numel: int
     is_tensor: bool
     # TODO: we can add a list of sharding spec here, and record the sharding
-    # behaviour by appending sharding spec into list.
+    # behavior by appending sharding spec into list.
 
 
 def _extract_tensor_metadata(result: torch.Tensor) -> TensorMetadata:
     """
     Extract a TensorMetadata NamedTuple describing `result`.
     """
     shape = result.shape
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             if use_partition_name is not None:
                 use_partition = partitions[use_partition_name]
                 use_partition.inputs.setdefault(def_node.name)
                 if def_partition_name is not None:
                     use_partition.partitions_dependent_on.setdefault(def_partition_name)
 
     node_process_list = list(m.graph.nodes)
-    # split nodes into parititons
+    # split nodes into partitions
     while node_process_list:
         node = node_process_list.pop(0)
         orig_nodes[node.name] = node
 
         if node.op in ["placeholder"]:
             continue
         if node.op == 'output':
@@ -273,15 +273,15 @@
         for dependent in partitions[root_partition].partition_dependents:
             partitions[dependent].partitions_dependent_on.pop(root_partition)
             if not partitions[dependent].partitions_dependent_on:
                 root_partitions.append(dependent)
     if len(sorted_partitions) != len(partitions):
         raise RuntimeError("cycle exists between partitions!")
 
-    # add placeholders to parititons
+    # add placeholders to partitions
     for partition_name in sorted_partitions:
         partition = partitions[partition_name]
         for input in partition.inputs:
             placeholder = partition.graph.placeholder(input)
             placeholder.meta = orig_nodes[input].meta.copy()
             partition.environment[orig_nodes[input]] = placeholder
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/split_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         self.targets: Dict[str, Any] = {}
 
     def __repr__(self) -> str:
         return f"name: {self.name},\n" \
             f" nodes: {self.node_names},\n" \
             f" inputs: {self.inputs},\n" \
             f" outputs: {self.outputs},\n" \
-            f" partitions depenent on: {self.partitions_dependent_on},\n" \
-            f" parition dependents: {self.partition_dependents}"
+            f" partitions dependent on: {self.partitions_dependent_on},\n" \
+            f" partition dependents: {self.partition_dependents}"
 
 
 # Creates subgraphs out of main graph
 @compatibility(is_backward_compatible=True)
 def split_module(
     m: GraphModule,
     root_m: torch.nn.Module,
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/proxy.py` & `colossalai-nightly-2023.6.3/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     @abstractmethod
     def extract_kwargs_from_mod(self):
         """
         This method is used to extract the kwargs for non-bias computation.
 
         For example:
             The kwargs for conv2d module is {} because the attributes like 'padding' or 'groups' are
-            considered during module initilizing. However, we need to consider those attributes as kwargs
+            considered during module initializing. However, we need to consider those attributes as kwargs
             in F.conv2d.
         """
         pass
 
     def create_non_bias_func_proxy(self, input_proxy=None):
         """
         This method is used to create the non_bias_func proxy, the node created by this proxy will
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/experimental.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         if enabled:
             orig_ckpt_func = torch.utils.checkpoint.CheckpointFunction
 
             class PatchedCheckpointFunction(torch.autograd.Function):
 
                 @staticmethod
                 def forward(ctx, run_function, preserve_rng_state, *args):
-                    # signal that the current tracing occurs within activaton checkpoint part
+                    # signal that the current tracing occurs within activation checkpoint part
                     self.inside_torch_checkpoint_func = True
                     out = run_function(*args)
                     self.inside_torch_checkpoint_func = False
                     self.act_ckpt_region_count += 1
                     return out
 
                 @staticmethod
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if self.tracer_type == TracerType.DEFAULT:
             # since meta_args is not given
             # we just fall back to the original torch.fx.Tracer
             proxy = super().create_proxy(kind, target, args, kwargs, name, type_expr, proxy_factory_fn)
             return proxy
 
         # if graph is traced for auto parallelism module, some extra node will be added during
-        # graph construction to deal with the compatability between bias addition and all reduce.
+        # graph construction to deal with the compatibility between bias addition and all reduce.
 
         # if no extra manipulation is applied, we just pass the origin arguments to create_proxy function
         # to create node on computation graph
         origin_arguments = (kind, target, args, kwargs, name, type_expr, proxy_factory_fn)
         # dispatch the arguments generator depending on the kind and target in origin arguments.
         args_metas, _ = extract_meta(*args, **kwargs)
         handle = None
@@ -204,15 +204,15 @@
         if tracer_type == TracerType.DEFAULT:
             self.proxy_cls = Proxy
             self.tracer_type = TracerType.DEFAULT
         elif tracer_type == TracerType.META:
             self.proxy_cls = ColoProxy
             self.tracer_type = TracerType.META
         else:
-            raise ValueError(f"Unrecognised tracer type {tracer_type}")
+            raise ValueError(f"Unrecognized tracer type {tracer_type}")
 
     def _meta_data_computing(self, kind, target, args, kwargs):
 
         if kind == "placeholder" and target in self.meta_args and self.meta_args[target].is_meta:
             meta_out = self.meta_args[target]
             return meta_out
 
@@ -441,15 +441,15 @@
         if enabled:
             orig_ckpt_func = torch.utils.checkpoint.CheckpointFunction
 
             class PatchedCheckpointFunction(torch.autograd.Function):
 
                 @staticmethod
                 def forward(ctx, run_function, preserve_rng_state, *args):
-                    # signal that the current tracing occurs within activaton checkpoint part
+                    # signal that the current tracing occurs within activation checkpoint part
                     self.inside_torch_checkpoint_func = True
                     out = run_function(*args)
                     self.inside_torch_checkpoint_func = False
                     self.act_ckpt_region_count += 1
                     return out
 
                 @staticmethod
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/global_variables.py` & `colossalai-nightly-2023.6.3/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/initialize.py` & `colossalai-nightly-2023.6.3/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/interface/model.py` & `colossalai-nightly-2023.6.3/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     if batch_size > 1:
                         query = rearrange(query, "b s ... -> c (b s) ...", c=1)
                         key, value = self.unpad(torch.stack([query, key, value], dim=2), kv_indices).unbind(dim=2)
                 attn_bias = BlockDiagonalMask.from_seqlens(q_seqlen, kv_seqlen)
             elif attn_mask_type == AttnMaskType.causal:    # gpt style
                 attn_bias = LowerTriangularMask()
 
-            if bias is not None:    # alibi / relative position emebedding
+            if bias is not None:    # alibi / relative position embedding
                 assert allow_alibi, "flash attention with bias is not supported in this system."
                 assert attn_mask_type == AttnMaskType.causal, \
                     "attention with bias is only supported for causal attention so far."
                 attn_bias = attn_bias.add_bias(bias)
 
             out = memory_efficient_attention(query, key, value, attn_bias=attn_bias, p=self.dropout, scale=self.scale)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     max_batch_tokens: int    # max batch token numbers
     max_seq_len: int    # max sequence length
     hidden_size: int    # size of transformer hidden layers
     nhead: int    # number of heads in attention
     attn_prob_dropout_ratio: float    # attention score dropout ratio
     hidden_dropout_ratio: float    # dropout ration before residual
     norm_first: bool    # norm_first
-    fp16: bool    # fp16 presion
+    fp16: bool    # fp16 precision
 
 
 class MultiHeadAttention1DFunc(Function):
 
     @staticmethod
     def forward(ctx, input, input_mask, in_proj_weight, in_proj_bias, out_proj_weight, out_proj_bias, norm_weight,
                 norm_bias, config):
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 def warmup_jit_fusion(batch_size: int,
                       hidden_size: int,
                       seq_length: int = 512,
                       vocab_size: int = 32768,
                       dtype: torch.dtype = torch.float32):
-    """ Compilie JIT functions before the main training steps """
+    """ Compile JIT functions before the main training steps """
 
     embed = Embedding(vocab_size, hidden_size).to(get_current_device())
     linear_1 = Linear(hidden_size, hidden_size * 4, skip_bias_add=True).to(get_current_device())
     linear_2 = Linear(hidden_size * 4, hidden_size, skip_bias_add=True).to(get_current_device())
 
     x = torch.randint(vocab_size, (batch_size, seq_length), dtype=torch.long, device=get_current_device())
     x = embed(x)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     import torch
 
     try:
         torch_cuda_major = torch.version.cuda.split(".")[0]
         torch_cuda_minor = torch.version.cuda.split(".")[1]
     except:
         raise ValueError(
-            "[extension] Cannot retrive the CUDA version in the PyTorch binary given by torch.version.cuda")
+            "[extension] Cannot retrieve the CUDA version in the PyTorch binary given by torch.version.cuda")
     return torch_cuda_major, torch_cuda_minor
 
 
 def get_cuda_bare_metal_version(cuda_dir) -> List[int]:
     """
     Get the System CUDA version from nvcc.
 
@@ -106,15 +106,15 @@
     Returns:
         A tuple of integers in the form of (major, minor, patch).
     """
     import torch
     torch_version = torch.__version__.split('+')[0]
     TORCH_MAJOR = int(torch_version.split('.')[0])
     TORCH_MINOR = int(torch_version.split('.')[1])
-    TORCH_PATCH = int(torch_version.split('.')[2])
+    TORCH_PATCH = int(torch_version.split('.')[2], 16)
     return TORCH_MAJOR, TORCH_MINOR, TORCH_PATCH
 
 
 def check_pytorch_version(min_major_version, min_minor_version) -> bool:
     """
     Compare the current PyTorch version with the minium required version.
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/logging/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/logging/logger.py` & `colossalai-nightly-2023.6.3/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/init.py` & `colossalai-nightly-2023.6.3/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/cpu_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class CPUAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of paramters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `CPUAdam` requires CUDA extensions which can be built during installation or runtime.
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class HybridAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of paramters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
-    `HybriadAdam` requires CUDA extensions which can be built during installation or runtime.
+    `HybridAdam` requires CUDA extensions which can be built during installation or runtime.
 
     This version of Hybrid Adam is an hybrid of CPUAdam and FusedAdam.
 
     * For parameters updating on CPU, it uses CPUAdam.
     * For parameters updating on GPU, it uses FusedAdam.
-    * Hybird precision calculation of fp16 and fp32 is supported, eg fp32 parameters and fp16 gradients.
+    * Hybrid precision calculation of fp16 and fp32 is supported, eg fp32 parameters and fp16 gradients.
 
     :class:`colossalai.nn.optimizer.HybridAdam` may be used as a drop-in replacement for ``torch.optim.AdamW``,
     or ``torch.optim.Adam`` with ``adamw_mode=False``
 
     Adam was been proposed in `Adam: A Method for Stochastic Optimization`_.
 
     Arguments:
@@ -127,15 +127,15 @@
                                           state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
 
                 elif target_device.type == 'cuda':
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
-                    # record the state by gruop and update at once
+                    # record the state by group and update at once
                     g_l.append(p.grad.data)
                     p_l.append(p.data)
                     m_l.append(state['exp_avg'])
                     v_l.append(state['exp_avg_sq'])
 
                 else:
                     raise RuntimeError
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 def _wait_for_data(t, stream: Optional[torch.cuda.streams.Stream]) -> None:
     if stream is None:
         return
     torch.cuda.current_stream().wait_stream(stream)
     # As mentioned in https://pytorch.org/docs/stable/generated/torch.Tensor.record_stream.html,
-    # PyTorch uses the "caching allocator" for memroy allocation for tensors. When a tensor is
-    # freed, its memory is likely to be reused by newly constructed tenosrs.  By default,
+    # PyTorch uses the "caching allocator" for memory allocation for tensors. When a tensor is
+    # freed, its memory is likely to be reused by newly constructed tensors.  By default,
     # this allocator traces whether a tensor is still in use by only the CUDA stream where it
     # was created.   When a tensor is used by additional CUDA streams, we need to call record_stream
     # to tell the allocator about all these streams.  Otherwise, the allocator might free the
     # underlying memory of the tensor once it is no longer used by the creator stream.  This is
     # a notable programming trick when we write programs using multi CUDA streams.
     cur_stream = torch.cuda.current_stream()
     assert isinstance(t, torch.Tensor)
@@ -290,15 +290,15 @@
             )
             print(f'cuda_to_cpu_elapse {elapsed} sec')
         if self._cpu_to_cuda_numel > 0 and "5_evict_in" in self._elapsed_dict:
             elapsed = self._elapsed_dict["5_evict_in"]
             print(
                 f"CPU->CUDA BWD {self._cpu_to_cuda_numel * self.elem_size_in_byte / 1e6 / elapsed} MB/s {self._cpu_to_cuda_numel / 1e6} M elem"
             )
-            print(f'cpu_to_cuda_elpase {elapsed} sec')
+            print(f'cpu_to_cuda_elapse {elapsed} sec')
 
         for k, v in self._elapsed_dict.items():
             print(f'{k}: {v}')
 
         print(f'cache miss ratio {self._cache_miss / self._total_cache}')
 
     @torch.no_grad()
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/registry/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/registry/registry.py` & `colossalai-nightly-2023.6.3/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/d_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/d_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/dist_spec_mgr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from contextlib import contextmanager
 
 import torch
 import torch.distributed as dist
 # from colossalai.nn.layer.utils import divide
 from numpy import prod
-from packaging import version
 
-from colossalai.logging import get_dist_logger
-from colossalai.tensor.distspec import _DistSpec
+from colossalai.tensor.distspec import DistPlacementPattern, _DistSpec
 from colossalai.tensor.process_group import ProcessGroup
 
 
 # TODO(jiaruifang) circle import, move the divide to colossalai.commons.
 # colossalai.tensor shall not import any submodule from colossal.nn
 def divide(numerator, denominator):
     """Only allow exact division.
@@ -167,19 +165,29 @@
         return DistSpecManager._shard_as(tensor, old_dist_spec, dist_spec, pg)
 
     @staticmethod
     def handle_trans_spec(tensor: torch.Tensor, old_dist_spec: _DistSpec, dist_spec: _DistSpec,
                           pg: ProcessGroup) -> torch.Tensor:
         assert isinstance(old_dist_spec, _DistSpec), f"{type(old_dist_spec)} should be _DistSpec"
         assert isinstance(dist_spec, _DistSpec), f"{type(dist_spec)} should be _DistSpec"
-        forward_trans_handle = getattr(DistSpecManager, f'_{old_dist_spec.placement.value}2{dist_spec.placement.value}')
+
+        trans_func_key = (old_dist_spec.placement, dist_spec.placement)
+        trans_funcs = {
+            (DistPlacementPattern.REPLICATE, DistPlacementPattern.REPLICATE): DistSpecManager._r2r,
+            (DistPlacementPattern.REPLICATE, DistPlacementPattern.SHARD): DistSpecManager._r2s,
+            (DistPlacementPattern.SHARD, DistPlacementPattern.REPLICATE): DistSpecManager._s2r,
+            (DistPlacementPattern.SHARD, DistPlacementPattern.SHARD): DistSpecManager._s2s
+        }
+
+        forward_trans_handle = trans_funcs[trans_func_key]
         if not DistSpecManager._use_autograd_function:
             return forward_trans_handle(tensor, old_dist_spec, dist_spec, pg)
-        backward_trans_handle = getattr(DistSpecManager,
-                                        f'_{dist_spec.placement.value}2{old_dist_spec.placement.value}')
+
+        backward_trans_handle = trans_funcs[(dist_spec.placement, old_dist_spec.placement)]
+
         return TransformDistSpec.apply(tensor, old_dist_spec, dist_spec, pg, forward_trans_handle,
                                        backward_trans_handle)
 
     @staticmethod
     @contextmanager
     def no_grad():
         try:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/tensor/utils.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/testing/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/testing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-from .comparison import assert_close, assert_close_loose, assert_equal, assert_equal_in_group, assert_not_equal
+from .comparison import (
+    assert_close,
+    assert_close_loose,
+    assert_equal,
+    assert_equal_in_group,
+    assert_not_equal,
+    check_state_dict_equal,
+)
 from .pytest_wrapper import run_on_environment_flag
 from .utils import (
     clear_cache_before_run,
     free_port,
     parameterize,
     rerun_if_address_is_in_use,
     rerun_on_exception,
     skip_if_not_enough_gpus,
     spawn,
 )
 
 __all__ = [
     'assert_equal', 'assert_not_equal', 'assert_close', 'assert_close_loose', 'assert_equal_in_group', 'parameterize',
     'rerun_on_exception', 'rerun_if_address_is_in_use', 'skip_if_not_enough_gpus', 'free_port', 'spawn',
-    'clear_cache_before_run', 'run_on_environment_flag'
+    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal'
 ]
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/testing/pytest_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
         # this will skip your test
         pytest test_for_something.py
 
     """
     assert isinstance(name, str)
     flag = os.environ.get(name.upper(), '0')
 
-    reason = f'Environment varialbe {name} is {flag}'
+    reason = f'Environment variable {name} is {flag}'
     if flag == '1':
         return pytest.mark.skipif(False, reason=reason)
     else:
         return pytest.mark.skipif(True, reason=reason)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/testing/random.py` & `colossalai-nightly-2023.6.3/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/testing/utils.py` & `colossalai-nightly-2023.6.3/colossalai/testing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,18 +163,18 @@
         @rerun_if_address_is_in_use()
         def test_something():
             ...
 
     """
     # check version
     torch_version = version.parse(torch.__version__)
-    assert torch_version.major == 1
+    assert torch_version.major >= 1
 
     # only torch >= 1.8 has ProcessRaisedException
-    if torch_version.minor >= 8:
+    if torch_version >= version.parse("1.8.0"):
         exception = torch.multiprocessing.ProcessRaisedException
     else:
         exception = Exception
 
     func_wrapper = rerun_on_exception(exception_type=exception, pattern=".*Address already in use.*")
     return func_wrapper
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/common.py` & `colossalai-nightly-2023.6.3/colossalai/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
     else:
         enable_cuda_kernels = params[0].grad.device.type == 'cuda'
     # Norm parameters.
     max_norm = float(max_norm)
     norm_type = float(norm_type)
 
     # Parameters can be on CPU or CUDA
-    # If parameters are on CPU, disable CUDA kernerls
+    # If parameters are on CPU, disable CUDA kernels
 
     # Calculate norm.
     if norm_type == inf:
         total_norm = max(p.grad.data.abs().max() for p in params)
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         # Take max across all model-parallel GPUs.
         if gpc.is_initialized(ParallelMode.MODEL) and gpc.get_world_size(ParallelMode.MODEL) > 1:
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/cuda.py` & `colossalai-nightly-2023.6.3/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/memory.py` & `colossalai-nightly-2023.6.3/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/model/experimental.py` & `colossalai-nightly-2023.6.3/colossalai/utils/model/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/model/lazy_init_context.py` & `colossalai-nightly-2023.6.3/colossalai/utils/model/lazy_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/moe.py` & `colossalai-nightly-2023.6.3/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         memory_size = tensor.element_size() * tensor.storage().size()
         if (tensor.is_leaf or tensor.retains_grad) and tensor.grad is not None:
             grad_memory_size = tensor.grad.element_size() * tensor.grad.storage().size()
             memory_size += grad_memory_size
         return self.mem_format(memory_size)
 
     def mem_format(self, real_memory_size):
-        # format the tensor memory into a reasonal magnitude
+        # format the tensor memory into a reasonable magnitude
         if real_memory_size >= 2**30:
             return str(real_memory_size / (2**30)) + ' GB'
         if real_memory_size >= 2**20:
             return str(real_memory_size / (2**20)) + ' MB'
         if real_memory_size >= 2**10:
             return str(real_memory_size / (2**10)) + ' KB'
         return str(real_memory_size) + ' B'
@@ -67,28 +67,28 @@
     def collect_tensors_state(self):
         for obj in gc.get_objects():
             if torch.is_tensor(obj):
                 # skip cpu tensor when include_cpu is false and the tensor we have collected before
                 if (not self.include_cpu) and obj.device == torch.device('cpu'):
                     continue
                 self.detected.append(id(obj))
-                # skip paramters we had added in __init__ when module is an instance of nn.Module for the first epoch
+                # skip parameters we had added in __init__ when module is an instance of nn.Module for the first epoch
                 if id(obj) not in self.tensor_info:
 
                     name = type(obj).__name__
                     # after backward, we want to update the records, to show you the change
                     if isinstance(self.module, nn.Module) and name == 'Parameter':
                         if obj.grad is not None:
                             # with grad attached
                             for par_name, param in self.module.named_parameters():
                                 if param.requires_grad and param.grad.equal(obj.grad):
                                     name = par_name + ' (with grad)'
                         else:
                             # with no grad attached
-                            # there will be no new paramters created during running
+                            # there will be no new parameters created during running
                             # so it must be in saved_tensor_info
                             continue
                     # we can also marked common tensors as tensor(with grad)
                     if name == 'Tensor' and (obj.is_leaf or obj.retains_grad):
                         if obj.grad is not None:
                             name = name + ' (with grad)'
                     # in fact, common tensor have no grad
@@ -151,15 +151,15 @@
 
         self.info += LINE
         self.info += f"Detect Location: {locate_msg}\n"
         for device in self.devices:
             if device == torch.device('cpu'):
                 continue
             gpu_mem_alloc = self.mem_format(torch.cuda.memory_allocated(device))
-            self.info += f"Totle GPU Memery Allocated on {device} is {gpu_mem_alloc}\n"
+            self.info += f"Total GPU Memory Allocated on {device} is {gpu_mem_alloc}\n"
         self.info += LINE
         self.info += '\n\n'
         if self.show_info:
             print(self.info)
         if self.log is not None:
             with open(self.log + '.log', 'a') as f:
                 f.write(self.info)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/utils/timer.py` & `colossalai-nightly-2023.6.3/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,51 +98,51 @@
             self.__close_one_chunk(self.chunk_groups[group_name][-1])
 
     def access_chunk(self, chunk: Chunk) -> None:
         """Make the chunk can be used for calculation.
         """
         if chunk in self.accessed_chunks:
             return
-        self.__sub_memroy_usage(chunk.memory_usage)
+        self.__sub_memory_usage(chunk.memory_usage)
         if chunk.device_type == 'cpu':
             chunk.shard_move(get_current_device())
         self.__add_accessed_chunk(chunk)
         self.__add_memory_usage(chunk.memory_usage)
 
     def release_chunk(self, chunk: Chunk) -> None:
         """Scatter the chunk in CUDA.
         """
         if chunk not in self.accessed_chunks:
             return
         if chunk.can_release:
-            self.__sub_memroy_usage(chunk.memory_usage)
+            self.__sub_memory_usage(chunk.memory_usage)
             self.__sub_accessed_chunk(chunk)
             self.__add_memory_usage(chunk.memory_usage)
 
     def move_chunk(self, chunk: Chunk, device: torch.device, force_copy: bool = False) -> None:
         """Move the shard of the chunk to the target device.
         """
         if not chunk.can_move or chunk.device_type == device.type:
             return
-        self.__sub_memroy_usage(chunk.memory_usage)
+        self.__sub_memory_usage(chunk.memory_usage)
         chunk.shard_move(device, force_copy)
         self.__add_memory_usage(chunk.memory_usage)
 
     def trans_tensor_state(self, tensor: torch.Tensor, state: TensorState) -> None:
         """Transit tensor state according to pre-defined state machine.
         """
         chunk = self.tensor_chunk_map[tensor]
         chunk.tensor_trans_state(tensor, state)
 
     def reduce_chunk(self, chunk: Chunk) -> bool:
         """Reduce or all reduce the chunk.
         """
         if not chunk.can_reduce:
             return False
-        self.__sub_memroy_usage(chunk.memory_usage)
+        self.__sub_memory_usage(chunk.memory_usage)
         chunk.reduce()
         self.__sub_accessed_chunk(chunk)
         self.__add_memory_usage(chunk.memory_usage)
         return True
 
     def fake_release_chunk(self, chunk: Chunk) -> None:
         """Release gathered chunk in a fake mode.
@@ -224,19 +224,19 @@
         """Register a chunk group.
         """
         if group_name not in self.chunk_groups:
             self.chunk_groups[group_name] = deque()
         return self.chunk_groups[group_name]
 
     def __close_one_chunk(self, chunk: Chunk):
-        self.__sub_memroy_usage(chunk.memory_usage)
+        self.__sub_memory_usage(chunk.memory_usage)
         chunk.close_chunk()
         self.__add_memory_usage(chunk.memory_usage)
 
-    def __sub_memroy_usage(self, usage: Dict[str, int]):
+    def __sub_memory_usage(self, usage: Dict[str, int]):
         for k, v in usage.items():
             self.total_mem[k] -= v
 
     def __add_memory_usage(self, usage: Dict[str, int]):
         for k, v in usage.items():
             self.total_mem[k] += v
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 def classify_params_by_dp_degree(param_order: OrderedParamGenerator,
                                  strict_ddp_flag: bool = False) -> Dict[int, List[ColoParameter]]:
     """classify_params_by_dp_degree
 
     Classify the parameters by their dp degree
 
     Args:
-        param_order (OrderedParamGenerator): the order of param be visied
+        param_order (OrderedParamGenerator): the order of param be vised
         strict_ddp_flag (bool, optional): whether to enable the strict ddp mode. Defaults to False.
 
     Returns:
         Dict[int, List[ColoParameter]]: a dict contains the classification results.
         The keys are dp_degrees and the values are parameters.
     """
     params_dict: Dict[int, List[ColoParameter]] = dict()
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def increase_preop_step(self, param_list: List[torch.nn.Parameter]):
         """
         the time step is increased. param list is used between current and the next
         time step.
 
         Args:
-            param_list (List[torch.nn.Parameter]): a list of torch paramters.
+            param_list (List[torch.nn.Parameter]): a list of torch parameters.
         """
         for p in param_list:
             if p not in self._param_step_dict:
                 self._param_step_dict[p] = [self._preop_step]
             else:
                 self._param_step_dict[p].append(self._preop_step)
             self._param_runtime_order.append(p)
```

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/low_level_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.5.6
+Version: 2023.6.3
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -134,20 +134,30 @@
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Colossal-AI in the Real World
         
         ### ColossalChat
         
         <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
            </a>
         </div>
         
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
+        [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
+        [[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
+        [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+        
+        <p id="ColossalChat-Speed" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
+        </p>
+        
+        - Up to 10 times faster for RLHF PPO Stage3 Training
         
         <p id="ColossalChat_scaling" align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
         </p>
         
         - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
         
@@ -359,14 +369,30 @@
         By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
         If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
         
         ```shell
         CUDA_EXT=1 pip install .
         ```
         
+        For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
+        
+        ```bash
+        # clone the repository
+        git clone https://github.com/hpcaitech/ColossalAI.git
+        cd ColossalAI
+        
+        # download the cub library
+        wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
+        unzip 1.8.0.zip
+        cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
+        
+        # install
+        CUDA_EXT=1 pip install .
+        ```
+        
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Use Docker
         
         ### Pull from DockerHub
         
         You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.6 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.3 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -92,23 +92,26 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                       chat/ColossalChat%20YouTube.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
+watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chat/ColossalChat%20Speed.jpg]
+- Up to 10 times faster for RLHF PPO Stage3 Training
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -225,15 +228,22 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
+with CUDA 10.2, you can still build ColossalAI from source. However, you need
+to manually download the cub library and copy it to the corresponding
+directory. ```bash # clone the repository git clone https://github.com/
+hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
+github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
+1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
+CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,35 @@
 version.txt
 colossalai/__init__.py
 colossalai/constants.py
 colossalai/core.py
 colossalai/global_variables.py
 colossalai/initialize.py
 colossalai/_C/__init__.py
+colossalai/_analyzer/__init__.py
+colossalai/_analyzer/envs.py
+colossalai/_analyzer/_subclasses/__init__.py
+colossalai/_analyzer/_subclasses/_meta_registration.py
+colossalai/_analyzer/_subclasses/_monkey_patch.py
+colossalai/_analyzer/_subclasses/flop_tensor.py
+colossalai/_analyzer/_subclasses/meta_tensor.py
+colossalai/_analyzer/fx/__init__.py
+colossalai/_analyzer/fx/codegen.py
+colossalai/_analyzer/fx/graph_module.py
+colossalai/_analyzer/fx/node_util.py
+colossalai/_analyzer/fx/symbolic_profile.py
+colossalai/_analyzer/fx/passes/__init__.py
+colossalai/_analyzer/fx/passes/graph_profile.py
+colossalai/_analyzer/fx/passes/shape_prop.py
+colossalai/_analyzer/fx/tracer/__init__.py
+colossalai/_analyzer/fx/tracer/bias_addition.py
+colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+colossalai/_analyzer/fx/tracer/proxy.py
+colossalai/_analyzer/fx/tracer/symbolic_trace.py
+colossalai/_analyzer/fx/tracer/tracer.py
 colossalai/amp/__init__.py
 colossalai/amp/amp_type.py
 colossalai/amp/apex_amp/__init__.py
 colossalai/amp/apex_amp/apex_amp.py
 colossalai/amp/naive_amp/__init__.py
 colossalai/amp/naive_amp/_fp16_optimizer.py
 colossalai/amp/naive_amp/_utils.py
@@ -127,23 +148,25 @@
 colossalai/auto_parallel/tensor_shard/utils/sharding.py
 colossalai/booster/__init__.py
 colossalai/booster/accelerator.py
 colossalai/booster/booster.py
 colossalai/booster/mixed_precision/__init__.py
 colossalai/booster/mixed_precision/bf16.py
 colossalai/booster/mixed_precision/fp16_apex.py
+colossalai/booster/mixed_precision/fp16_naive.py
 colossalai/booster/mixed_precision/fp16_torch.py
 colossalai/booster/mixed_precision/fp8.py
 colossalai/booster/mixed_precision/mixed_precision_base.py
 colossalai/booster/plugin/__init__.py
 colossalai/booster/plugin/dp_plugin_base.py
 colossalai/booster/plugin/gemini_plugin.py
 colossalai/booster/plugin/low_level_zero_plugin.py
 colossalai/booster/plugin/plugin_base.py
 colossalai/booster/plugin/torch_ddp_plugin.py
+colossalai/booster/plugin/torch_fsdp_plugin.py
 colossalai/builder/__init__.py
 colossalai/builder/builder.py
 colossalai/checkpoint_io/__init__.py
 colossalai/checkpoint_io/checkpoint_io_base.py
 colossalai/checkpoint_io/general_checkpoint_io.py
 colossalai/checkpoint_io/index_file.py
 colossalai/checkpoint_io/utils.py
```

### Comparing `colossalai-nightly-2023.5.6/op_builder/__init__.py` & `colossalai-nightly-2023.6.3/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/builder.py` & `colossalai-nightly-2023.6.3/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/cpu_adam.py` & `colossalai-nightly-2023.6.3/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/fused_optim.py` & `colossalai-nightly-2023.6.3/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/layernorm.py` & `colossalai-nightly-2023.6.3/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/moe.py` & `colossalai-nightly-2023.6.3/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.6.3/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.6.3/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.6.3/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/op_builder/utils.py` & `colossalai-nightly-2023.6.3/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     import torch
 
     try:
         torch_cuda_major = torch.version.cuda.split(".")[0]
         torch_cuda_minor = torch.version.cuda.split(".")[1]
     except:
         raise ValueError(
-            "[extension] Cannot retrive the CUDA version in the PyTorch binary given by torch.version.cuda")
+            "[extension] Cannot retrieve the CUDA version in the PyTorch binary given by torch.version.cuda")
     return torch_cuda_major, torch_cuda_minor
 
 
 def get_cuda_bare_metal_version(cuda_dir) -> List[int]:
     """
     Get the System CUDA version from nvcc.
 
@@ -106,15 +106,15 @@
     Returns:
         A tuple of integers in the form of (major, minor, patch).
     """
     import torch
     torch_version = torch.__version__.split('+')[0]
     TORCH_MAJOR = int(torch_version.split('.')[0])
     TORCH_MINOR = int(torch_version.split('.')[1])
-    TORCH_PATCH = int(torch_version.split('.')[2])
+    TORCH_PATCH = int(torch_version.split('.')[2], 16)
     return TORCH_MAJOR, TORCH_MINOR, TORCH_PATCH
 
 
 def check_pytorch_version(min_major_version, min_minor_version) -> bool:
     """
     Compare the current PyTorch version with the minium required version.
```

### Comparing `colossalai-nightly-2023.5.6/setup.py` & `colossalai-nightly-2023.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/albert.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/albert.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,37 +23,37 @@
                               num_attention_heads=num_head,
                               max_position_embeddings=sequence_length,
                               num_hidden_layers=num_layer,
                               hidden_dropout_prob=0.,
                               attention_probs_dropout_prob=0.)
         print('building AlbertForSequenceClassification model')
 
-        # adapting huggingface BertForSequenceClassification for single unitest calling interface
-        class ModelAaptor(AlbertForSequenceClassification):
+        # adapting huggingface BertForSequenceClassification for single unittest calling interface
+        class ModelAdaptor(AlbertForSequenceClassification):
 
             def forward(self, input_ids, labels):
                 """
                 inputs: data, label
                 outputs: loss
                 """
                 return super().forward(input_ids=input_ids, labels=labels)[0]
 
-        model = ModelAaptor(config)
+        model = ModelAdaptor(config)
         # if checkpoint and version.parse(transformers.__version__) >= version.parse("4.11.0"):
         #     model.gradient_checkpointing_enable()
 
         return model
 
-    is_distrbuted = torch.distributed.is_initialized()
+    is_distributed = torch.distributed.is_initialized()
     trainloader = get_bert_data_loader(n_class=vocab_size,
                                        batch_size=2,
                                        total_samples=10000,
                                        sequence_length=sequence_length,
-                                       is_distrbuted=is_distrbuted)
+                                       is_distributed=is_distributed)
     testloader = get_bert_data_loader(n_class=vocab_size,
                                       batch_size=2,
                                       total_samples=10000,
                                       sequence_length=sequence_length,
-                                      is_distrbuted=is_distrbuted)
+                                      is_distributed=is_distributed)
 
     criterion = None
     return bert_model_builder, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/beit.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/beit.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
                               device=get_current_device())
         return data, label
 
 
 @non_distributed_component_funcs.register(name='beit')
 def get_training_components():
 
-    def model_buider(checkpoint=False):
+    def model_builder(checkpoint=False):
         model = Beit(img_size=DummyDataLoader.img_size,
                      num_classes=DummyDataLoader.num_class,
                      embed_dim=32,
                      depth=2,
                      num_heads=4)
         return model
 
     trainloader = DummyDataLoader()
     testloader = DummyDataLoader()
 
     criterion = torch.nn.CrossEntropyLoss()
-    return model_buider, trainloader, testloader, torch.optim.Adam, criterion
+    return model_builder, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/bert.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 def get_bert_data_loader(
         n_class,
         batch_size,
         total_samples,
         sequence_length,
         device=torch.device('cpu:0'),
-        is_distrbuted=False,
+        is_distributed=False,
 ):
     train_data = torch.randint(
         low=0,
         high=n_class,
         size=(total_samples, sequence_length),
         device=device,
         dtype=torch.long,
     )
     train_label = torch.randint(low=0, high=2, size=(total_samples,), device=device, dtype=torch.long)
     train_dataset = torch.utils.data.TensorDataset(train_data, train_label)
-    if is_distrbuted:
+    if is_distributed:
         sampler = torch.utils.data.distributed.DistributedSampler(train_dataset)
     else:
         sampler = SequentialSampler(train_dataset)
     train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size, sampler=sampler)
     return train_loader
 
 
@@ -48,37 +48,37 @@
                             num_attention_heads=num_head,
                             max_position_embeddings=sequence_length,
                             num_hidden_layers=num_layer,
                             hidden_dropout_prob=0.,
                             attention_probs_dropout_prob=0.)
         print('building BertForSequenceClassification model')
 
-        # adapting huggingface BertForSequenceClassification for single unitest calling interface
-        class ModelAaptor(BertForSequenceClassification):
+        # adapting huggingface BertForSequenceClassification for single unittest calling interface
+        class ModelAdaptor(BertForSequenceClassification):
 
             def forward(self, input_ids, labels):
                 """
                 inputs: data, label
                 outputs: loss
                 """
                 return super().forward(input_ids=input_ids, labels=labels)[0]
 
-        model = ModelAaptor(config)
+        model = ModelAdaptor(config)
         if checkpoint and version.parse(transformers.__version__) >= version.parse("4.11.0"):
             model.gradient_checkpointing_enable()
 
         return model
 
-    is_distrbuted = torch.distributed.is_initialized()
+    is_distributed = torch.distributed.is_initialized()
     trainloader = get_bert_data_loader(n_class=vocab_size,
                                        batch_size=2,
                                        total_samples=10000,
                                        sequence_length=sequence_length,
-                                       is_distrbuted=is_distrbuted)
+                                       is_distributed=is_distributed)
     testloader = get_bert_data_loader(n_class=vocab_size,
                                       batch_size=2,
                                       total_samples=10000,
                                       sequence_length=sequence_length,
-                                      is_distrbuted=is_distrbuted)
+                                      is_distributed=is_distributed)
 
     criterion = None
     return bert_model_builder, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/registry.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
     def __init__(self):
         self._registry = dict()
 
     def register(self, name):
         assert name not in self._registry
 
-        def _regsiter(callable_):
+        def _register(callable_):
             self._registry[name] = callable_
 
-        return _regsiter
+        return _register
 
     def get_callable(self, name: str):
         return self._registry[name]
 
     def __iter__(self):
         self._idx = 0
         self._len = len(self._registry)
@@ -30,10 +30,10 @@
             self._idx += 1
             return callable_
         else:
             raise StopIteration
 
 
 non_distributed_component_funcs = Registry()
-model_paralle_component_funcs = Registry()
+model_parallel_component_funcs = Registry()
 
-__all__ = ['non_distributed_component_funcs', 'model_paralle_component_funcs']
+__all__ = ['non_distributed_component_funcs', 'model_parallel_component_funcs']
```

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }),
     (torch.where, (torch.rand(2, 3, 224, 224) > 0.5, torch.rand(2, 3, 224, 224, requires_grad=True),
                    torch.rand(2, 3, 224, 224, requires_grad=True)), {}),
 ]
 
 
 @pytest.mark.skipif(version.parse(torch.__version__) < version.parse('1.12.0'), reason='torch version < 12')
-@clear_cache_before_run()
-@parameterize('func, args, kwargs', odd_cases)
+@pytest.mark.parametrize('func, args, kwargs', odd_cases)
 def test_flop_count_function(func, args, kwargs):
     rs_fwd, rs_bwd = flop_count(func, *args, **kwargs, verbose=True)
     assert rs_fwd > 0, f'fwd flop count of {func.__name__} is {rs_fwd}'
     assert rs_bwd > 0, f'bwd flop count of {func.__name__} is {rs_bwd}'
 
 
 if __name__ == '__main__':
```

### Comparing `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

