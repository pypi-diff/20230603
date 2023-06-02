# Comparing `tmp/deepspeed-0.9.2.tar.gz` & `tmp/deepspeed-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepspeed-0.9.2.tar", last modified: Wed May  3 17:31:51 2023, max compression
+gzip compressed data, was "deepspeed-0.9.3.tar", last modified: Fri Jun  2 22:12:58 2023, max compression
```

## Comparing `deepspeed-0.9.2.tar` & `deepspeed-0.9.3.tar`

### file list

```diff
@@ -1,604 +1,638 @@
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.312835 deepspeed-0.9.2/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.2/LICENSE
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.2/MANIFEST.in
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27421 2023-05-03 17:31:51.312835 deepspeed-0.9.2/PKG-INFO
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26538 2023-05-03 17:31:31.000000 deepspeed-0.9.2/README.md
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.822835 deepspeed-0.9.2/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.2/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/bin/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/deepspeed
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/deepspeed.pt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.2/bin/ds_bench
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.2/bin/ds_elastic
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds_report
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds_ssh
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/dsr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:49.000000 deepspeed-0.9.2/build.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.772835 deepspeed-0.9.2/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.842835 deepspeed-0.9.2/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.862835 deepspeed-0.9.2/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.862835 deepspeed-0.9.2/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.892835 deepspeed-0.9.2/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.2/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.892835 deepspeed-0.9.2/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.912835 deepspeed-0.9.2/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.912835 deepspeed-0.9.2/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.922835 deepspeed-0.9.2/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.922835 deepspeed-0.9.2/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18600 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8918 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35842 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    24466 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    78079 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2517 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28591 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    34052 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18300 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8317 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.942835 deepspeed-0.9.2/deepspeed/autotuning/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54204 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/autotuning/autotuner.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.952835 deepspeed-0.9.2/deepspeed/autotuning/config_templates/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero0.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero1.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero2.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero3.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5945 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.952835 deepspeed-0.9.2/deepspeed/autotuning/tuner/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/base_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/cost_model.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/index_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/model_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15054 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.962835 deepspeed-0.9.2/deepspeed/checkpoint/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/checkpoint/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12009 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/deepspeed_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_3d_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_meg_2d.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/universal_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      936 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/zero_checkpoint.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.972835 deepspeed-0.9.2/deepspeed/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/backend.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27476 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/comm/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1256 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13128 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/comm/torch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/comm/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.982835 deepspeed-0.9.2/deepspeed/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36034 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10519 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/compress.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4959 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12303 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8039 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7814 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.992835 deepspeed-0.9.2/deepspeed/elasticity/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2452 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/elastic_agent.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/elasticity.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4793 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/env_report.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/git_version_info.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-05-03 17:31:49.000000 deepspeed-0.9.2/deepspeed/git_version_info_installed.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9506 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/inference/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    28924 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/inference/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/launcher/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/launcher/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      352 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/launcher/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    19078 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/launcher/launch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12206 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/launcher/multinode_runner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23389 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/launcher/runner.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/model_implementations/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/vae.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.012835 deepspeed-0.9.2/deepspeed/model_implementations/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/features/cuda_graph.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.022835 deepspeed-0.9.2/deepspeed/model_implementations/transformers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/clip_encoder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7828 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.032835 deepspeed-0.9.2/deepspeed/module_inject/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4815 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/auto_tp.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.042835 deepspeed-0.9.2/deepspeed/module_inject/containers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      838 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23997 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/base_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3718 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5150 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2807 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/clip.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/distil_bert.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.052835 deepspeed-0.9.2/deepspeed/module_inject/containers/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      181 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3791 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2486 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/meta_tensor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2249 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gpt2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4476 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptj.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4819 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptneo.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5495 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptneox.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5045 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3913 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6280 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/vae.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/inject.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3825 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/layers.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14122 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/load_checkpoint.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/module_quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7723 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35871 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/replace_module.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      930 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/replace_policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1653 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.052835 deepspeed-0.9.2/deepspeed/moe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/experts.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/mappings.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/sharded_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/monitor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2529 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/csv_monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/tensorboard.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/wandb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/nebula/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/ops/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/ops/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adagrad/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adagrad/cpu_adagrad.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/adam/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8546 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6878 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/multi_tensor_apply.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/aio/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/aio/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.792835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_test/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_test/single_process_config.json
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.092835 deepspeed-0.9.2/deepspeed/ops/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18600 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8918 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35842 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    24466 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    78079 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2517 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28591 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    34052 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18300 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8317 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/lamb/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/lamb/fused_lamb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.132835 deepspeed-0.9.2/deepspeed/ops/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.142835 deepspeed-0.9.2/deepspeed/ops/quantizer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/quantizer/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/quantizer/quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.142835 deepspeed-0.9.2/deepspeed/ops/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/random_ltd/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4901 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/random_ltd/dropping_utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/matmul.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_attention_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_self_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42462 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparsity_config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/matmul.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/transformer/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.172835 deepspeed-0.9.2/deepspeed/ops/transformer/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/bias_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5612 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9986 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4763 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13927 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4585 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18473 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/moe_inference.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      551 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1227 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1007 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1273 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1424 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1215 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/residual_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1059 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1513 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      875 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/triton_ops.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/pipe/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/profiling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1708 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1098 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.192835 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47039 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/profiler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.212835 deepspeed-0.9.2/deepspeed/runtime/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/checkpointing.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/runtime/bf16_optimizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      654 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4982 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/coalesced_collectives.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/mpi.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/nccl.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/compression/cupy.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39541 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/config_utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12806 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.242835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25015 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/dataloader.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/eigenvalue.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   154538 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.252835 deepspeed-0.9.2/deepspeed/runtime/fp16/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/fused_optimizer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11093 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/loss_scaler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.252835 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/zoadam.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/unfused_optimizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20256 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/hybrid_engine.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/lr_schedules.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.262835 deepspeed-0.9.2/deepspeed/runtime/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56847 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/module.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/p2p.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/schedule.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/topology.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/progressive_layer_drop.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/sparse_tensor.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/state_dict_factory.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.272835 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/aio_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/async_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/optimizer_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35806 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/weight_quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.282835 deepspeed-0.9.2/deepspeed/runtime/zero/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/contiguous_memory_allocator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/linear.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21571 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/mics.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/mics_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/offload_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21889 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/zero/parameter_offload.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    72389 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/partition_parameters.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22345 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/zero/partitioned_param_coordinator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   113908 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/stage3.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110844 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/stage_1_and_2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/test.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/tiling.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.302835 deepspeed-0.9.2/deepspeed/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      717 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/comms_logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/debug.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/exceptions.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/groups.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/init_on_device.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/mixed_precision_linkage.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/nvtx.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/tensor_fragment.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8765 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/timer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      200 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/types.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/utils/zero_to_fp32.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed.egg-info/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27421 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20147 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/entry_points.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1086 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/requires.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.302835 deepspeed-0.9.2/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.2/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.2/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.312835 deepspeed-0.9.2/requirements/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-1bit-mpi.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-autotuning-ml.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-autotuning.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.2/requirements/requirements-dev.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.2/requirements/requirements-inf.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.2/requirements/requirements-readthedocs.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.2/requirements/requirements-sd.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-sparse_attn.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.2/requirements/requirements.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-05-03 17:31:51.312835 deepspeed-0.9.2/setup.cfg
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11318 2023-04-21 00:47:36.000000 deepspeed-0.9.2/setup.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-04-21 00:48:17.000000 deepspeed-0.9.2/version.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.3/LICENSE
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.3/MANIFEST.in
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27468 2023-06-02 22:12:58.850620 deepspeed-0.9.3/PKG-INFO
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26538 2023-05-03 17:31:31.000000 deepspeed-0.9.3/README.md
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6385 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/bin/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/deepspeed
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/deepspeed.pt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.3/bin/ds_bench
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.3/bin/ds_elastic
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds_report
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds_ssh
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/dsr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:57.000000 deepspeed-0.9.3/build.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.500620 deepspeed-0.9.3/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.500620 deepspeed-0.9.3/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.510620 deepspeed-0.9.3/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.520620 deepspeed-0.9.3/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.520620 deepspeed-0.9.3/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.550620 deepspeed-0.9.3/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.3/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.550620 deepspeed-0.9.3/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.580620 deepspeed-0.9.3/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.580620 deepspeed-0.9.3/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/deepspeed/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.600620 deepspeed-0.9.3/deepspeed/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6385 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54184 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/autotuner.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/config_templates/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero0.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero1.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero2.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero3.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5943 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/tuner/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2754 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/base_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/cost_model.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/index_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/model_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15053 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.620620 deepspeed-0.9.3/deepspeed/checkpoint/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/checkpoint/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12012 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/checkpoint/deepspeed_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_3d_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_meg_2d.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/universal_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2534 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/checkpoint/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/zero_checkpoint.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.630620 deepspeed-0.9.3/deepspeed/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/comm/backend.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2248 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/ccl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27788 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/comm/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1276 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      259 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/reduce_op.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13128 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/comm/torch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/comm/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.630620 deepspeed-0.9.3/deepspeed/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36033 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11886 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/compress.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25067 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5569 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14637 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8161 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7818 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/elasticity/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4703 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/elasticity/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2454 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/elasticity/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/elastic_agent.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/elasticity.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/env_report.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/git_version_info.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed/git_version_info_installed.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9501 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/inference/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    31552 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/inference/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/launcher/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/launcher/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      375 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14601 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/launch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16568 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/multinode_runner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24125 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/runner.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/vae.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/features/cuda_graph.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.650620 deepspeed-0.9.3/deepspeed/model_implementations/transformers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/clip_encoder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8247 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.660620 deepspeed-0.9.3/deepspeed/module_inject/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4998 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/auto_tp.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/module_inject/containers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12798 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/base_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3690 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5289 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2822 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/clip.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3109 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/distil_bert.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/module_inject/containers/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      275 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4788 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/gated_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7273 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4129 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1200 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2930 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/meta_tensor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7120 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/split_qkv.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2221 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gpt2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4768 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptj.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5002 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptneo.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5571 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptneox.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5797 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/llama.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5017 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3936 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6599 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/vae.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/inject.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4592 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/layers.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14597 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/load_checkpoint.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/module_quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8259 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    44312 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/replace_module.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      989 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/replace_policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1762 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/moe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/experts.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/mappings.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/sharded_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/monitor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2485 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/monitor/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/csv_monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/tensorboard.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/wandb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/nebula/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/nebula/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/nebula/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/nebula/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/ops/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/ops/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adagrad/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adagrad/cpu_adagrad.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/adam/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adam/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8544 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/adam/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8767 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/adam/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adam/multi_tensor_apply.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/aio/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/aio/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_test/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_test/single_process_config.json
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/lamb/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/lamb/fused_lamb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.730620 deepspeed-0.9.3/deepspeed/ops/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29590 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1238 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/quantizer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/quantizer/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/quantizer/quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/random_ltd/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4902 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/random_ltd/dropping_utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/matmul.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_attention_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_self_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42463 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparsity_config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/matmul.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/transformer/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/transformer/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/bias_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5725 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9830 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4853 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13853 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6212 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18454 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/moe_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      536 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1496 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1404 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4472 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3129 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2660 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/residual_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2460 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2131 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1447 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/triton_ops.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/pipe/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/profiling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/profiling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1959 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1243 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47248 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/profiler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/checkpointing.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/runtime/bf16_optimizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      653 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4981 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/coalesced_collectives.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/mpi.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/nccl.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/compression/cupy.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39863 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/config_utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12971 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25023 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/dataloader.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/eigenvalue.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   155145 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/fp16/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/fused_optimizer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11492 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/loss_scaler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/zoadam.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/unfused_optimizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21045 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/hybrid_engine.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/lr_schedules.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.810620 deepspeed-0.9.3/deepspeed/runtime/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56845 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/module.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/p2p.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/schedule.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/topology.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/progressive_layer_drop.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/sparse_tensor.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/state_dict_factory.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.820620 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/aio_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/async_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/optimizer_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35805 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/weight_quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.830620 deepspeed-0.9.3/deepspeed/runtime/zero/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/contiguous_memory_allocator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/linear.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21571 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/mics.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/mics_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/offload_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22194 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/parameter_offload.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    72665 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/partition_parameters.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22356 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/partitioned_param_coordinator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   114250 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/stage3.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110843 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/stage_1_and_2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/test.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/tiling.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.840620 deepspeed-0.9.3/deepspeed/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      751 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/comms_logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/debug.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/exceptions.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/groups.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/init_on_device.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/mixed_precision_linkage.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5158 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/numa.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/nvtx.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/tensor_fragment.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     9477 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/timer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      434 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/types.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/utils/zero_to_fp32.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/deepspeed.egg-info/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27468 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21258 2023-06-02 22:12:58.000000 deepspeed-0.9.3/deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/entry_points.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1146 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/requires.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29590 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1238 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.3/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/requirements/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-1bit-mpi.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-autotuning-ml.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-autotuning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       28 2023-06-02 22:08:07.000000 deepspeed-0.9.3/requirements/requirements-cpu.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.3/requirements/requirements-dev.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.3/requirements/requirements-inf.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.3/requirements/requirements-readthedocs.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.3/requirements/requirements-sd.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-sparse_attn.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       25 2023-06-02 22:08:07.000000 deepspeed-0.9.3/requirements/requirements-sparse_pruning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.3/requirements/requirements.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-06-02 22:12:58.850620 deepspeed-0.9.3/setup.cfg
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11424 2023-06-02 22:08:07.000000 deepspeed-0.9.3/setup.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-05-03 17:31:59.000000 deepspeed-0.9.3/version.txt
```

### Comparing `deepspeed-0.9.2/LICENSE` & `deepspeed-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/PKG-INFO` & `deepspeed-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.2
+Version: 0.9.3
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
-License: MIT
+License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,15 @@
 Provides-Extra: 1bit
 Provides-Extra: 1bit_mpi
 Provides-Extra: readthedocs
 Provides-Extra: dev
 Provides-Extra: autotuning
 Provides-Extra: autotuning_ml
 Provides-Extra: sparse_attn
+Provides-Extra: sparse
 Provides-Extra: inf
 Provides-Extra: sd
 Provides-Extra: all
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
```

### Comparing `deepspeed-0.9.2/README.md` & `deepspeed-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/accelerator/abstract_accelerator.py` & `deepspeed-0.9.3/accelerator/abstract_accelerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class DeepSpeedAccelerator(ABC):
 
     def __init__(self):
         self._name = None
         self._communication_backend_name = None
 
+    @abc.abstractmethod
+    def is_synchronized_device(self):
+        ...
+
     # Device APIs
     @abc.abstractmethod
     def device_name(self, device_index):
         ...
 
     @abc.abstractmethod
     def device(self, device_index):
```

### Comparing `deepspeed-0.9.2/accelerator/cuda_accelerator.py` & `deepspeed-0.9.3/accelerator/cuda_accelerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,16 @@
 
 class CUDA_Accelerator(DeepSpeedAccelerator):
 
     def __init__(self):
         self._name = 'cuda'
         self._communication_backend_name = 'nccl'
 
-        # begin initialize for create_op_builder()
-        # put all valid class name <--> class type mapping into class_dict
-        op_builder_dir = self.op_builder_dir()
-        op_builder_module = importlib.import_module(op_builder_dir)
-        for _, module_name, _ in pkgutil.iter_modules([os.path.dirname(op_builder_module.__file__)]):
-            # avoid self references
-            if module_name != 'all_ops' and module_name != 'builder':
-                module = importlib.import_module("{}.{}".format(op_builder_dir, module_name))
-                for member_name in module.__dir__():
-                    if member_name.endswith(
-                            'Builder'
-                    ) and member_name != "OpBuilder" and member_name != "CUDAOpBuilder" and member_name != "TorchCPUOpBuilder":  # avoid abstract classes
-                        if not member_name in self.class_dict:
-                            self.class_dict[member_name] = getattr(module, member_name)
-        # end initialize for create_op_builder()
+    def is_synchronized_device(self):
+        return False
 
     # Device APIs
     def device_name(self, device_index=None):
         if device_index == None:
             return 'cuda'
         return 'cuda:{}'.format(device_index)
 
@@ -231,25 +218,48 @@
             return "op_builder"
         except ImportError:
             return "deepspeed.ops.op_builder"
 
     # dict that holds class name <--> class type mapping i.e.
     # 'AsyncIOBuilder': <class 'op_builder.async_io.AsyncIOBuilder'>
     # this dict will be filled at init stage
-    class_dict = {}
+    class_dict = None
+
+    def _lazy_init_class_dict(self):
+        if self.class_dict != None:
+            return
+        else:
+            self.class_dict = {}
+            # begin initialize for create_op_builder()
+            # put all valid class name <--> class type mapping into class_dict
+            op_builder_dir = self.op_builder_dir()
+            op_builder_module = importlib.import_module(op_builder_dir)
+            for _, module_name, _ in pkgutil.iter_modules([os.path.dirname(op_builder_module.__file__)]):
+                # avoid self references
+                if module_name != 'all_ops' and module_name != 'builder' and module_name != 'cpu':
+                    module = importlib.import_module("{}.{}".format(op_builder_dir, module_name))
+                    for member_name in module.__dir__():
+                        if member_name.endswith(
+                                'Builder'
+                        ) and member_name != "OpBuilder" and member_name != "CUDAOpBuilder" and member_name != "TorchCPUOpBuilder":  # avoid abstract classes
+                            if not member_name in self.class_dict:
+                                self.class_dict[member_name] = getattr(module, member_name)
+            # end initialize for create_op_builder()
 
     # create an instance of op builder and return, name specified by class_name
     def create_op_builder(self, class_name):
+        self._lazy_init_class_dict()
         if class_name in self.class_dict:
             return self.class_dict[class_name]()
         else:
             return None
 
     # return an op builder class, name specified by class_name
     def get_op_builder(self, class_name):
+        self._lazy_init_class_dict()
         if class_name in self.class_dict:
             return self.class_dict[class_name]
         else:
             return None
 
     def build_extension(self):
         from torch.utils.cpp_extension import BuildExtension
```

### Comparing `deepspeed-0.9.2/bin/ds_bench` & `deepspeed-0.9.3/bin/ds_bench`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/bin/ds_elastic` & `deepspeed-0.9.3/bin/ds_elastic`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/bin/ds_ssh` & `deepspeed-0.9.3/bin/ds_ssh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.3/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.3/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.3/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.3/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.3/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.3/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.3/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/StopWatch.h` & `deepspeed-0.9.3/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/Timer.h` & `deepspeed-0.9.3/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/context.h` & `deepspeed-0.9.3/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/conversion_utils.h` & `deepspeed-0.9.3/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.3/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/cpu_adam.h` & `deepspeed-0.9.3/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.3/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.3/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.3/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/dropout.h` & `deepspeed-0.9.3/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.3/csrc/includes/ds_kernel_utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 #if __CUDA_ARCH__ >= 530
 #define HALF_PRECISION_AVAILABLE = 1
 #define PTX_AVAILABLE
 #endif  // __CUDA_ARCH__ >= 530
 
 #if __CUDA_ARCH__ >= 800
 #define ASYNC_COPY_AVAILABLE
-#define BF16_AVAILABLE
 #endif  // __CUDA_ARCH__ >= 800
 
 #include <cooperative_groups.h>
 
 #endif  //__HIP_PLATFORM_HCC__
 
 inline int next_pow2(const int val)
```

### Comparing `deepspeed-0.9.2/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.3/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/feed_forward.h` & `deepspeed-0.9.3/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/gelu.h` & `deepspeed-0.9.3/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/gemm_test.h` & `deepspeed-0.9.3/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/general_kernels.h` & `deepspeed-0.9.3/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.3/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/normalize_layer.h` & `deepspeed-0.9.3/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/quantization.h` & `deepspeed-0.9.3/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/quantization_utils.h` & `deepspeed-0.9.3/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/reduction_utils.h` & `deepspeed-0.9.3/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/simd.h` & `deepspeed-0.9.3/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/softmax.h` & `deepspeed-0.9.3/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.3/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/includes/type_shim.h` & `deepspeed-0.9.3/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/quantization/dequantize.cu` & `deepspeed-0.9.3/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.3/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.3/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/quantization/quantize.cu` & `deepspeed-0.9.3/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.3/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.3/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.3/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.3/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.3/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.3/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.3/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.3/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.3/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.3/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/gelu.cu`

 * *Files 15% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(gelu(data_f + bias_f));
         }
@@ -66,23 +67,22 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_gelu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_gelu<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_GELU(T) \
+    template void launch_bias_gelu<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_GELU(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_gelu<__nv_bfloat16>(__nv_bfloat16*,
-                                              const __nv_bfloat16*,
-                                              int,
-                                              int,
-                                              cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_GELU(__nv_bfloat16)
 #endif
-template void launch_bias_gelu<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_GELU(__half)
 
 /*
 In-place channels-last bias add
 */
 template <typename T>
 __global__ void fused_bias_add(T* input, const T* bias, int total_count, int intermediate_size)
 {
@@ -91,15 +91,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(data_f + bias_f);
         }
@@ -123,23 +124,22 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_add<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_add<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_ADD(T) \
+    template void launch_bias_add<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_ADD(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_add<__nv_bfloat16>(__nv_bfloat16*,
-                                             const __nv_bfloat16*,
-                                             int,
-                                             int,
-                                             cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_ADD(__nv_bfloat16)
 #endif
-template void launch_bias_add<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_ADD(__half)
 
 __global__ void fused_bias_residual(float* residual,
                                     const float* hidden_state,
                                     const float* attn,
                                     const float* bias,
                                     const float* attn_bias,
                                     const int total_count,
@@ -278,52 +278,22 @@
                                                               attn_bias,
                                                               total_count,
                                                               hidden_dim / 4,
                                                               1.0 / mp_size,
                                                               preln);
 }
 
-template void launch_bias_residual<
-    float>(float*, float*, float*, float*, float*, int, int, int, bool, cudaStream_t);
-#ifdef BF16_AVAILABLE
-template void launch_bias_residual<__nv_bfloat16>(__nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  int,
-                                                  int,
-                                                  int,
-                                                  bool,
-                                                  cudaStream_t);
-#endif
-template void launch_bias_residual<
-    __half>(__half*, __half*, __half*, __half*, __half*, int, int, int, bool, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_RESIDUAL(T) \
+    template void launch_bias_residual<T>(T*, T*, T*, T*, T*, int, int, int, bool, cudaStream_t);
 
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(float);
 #ifdef BF16_AVAILABLE
-template __global__ void fused_bias_residual(__nv_bfloat16* residual,
-                                             const __nv_bfloat16* hidden_state,
-                                             const __nv_bfloat16* attn,
-                                             const __nv_bfloat16* bias,
-                                             const __nv_bfloat16* attn_bias,
-                                             const int total_count,
-                                             const int intermediate_size,
-                                             const float mp_scale,
-                                             const bool preln);
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(__nv_bfloat16);
 #endif
-
-template __global__ void fused_bias_residual(__half* residual,
-                                             const __half* hidden_state,
-                                             const __half* attn,
-                                             const __half* bias,
-                                             const __half* attn_bias,
-                                             const int total_count,
-                                             const int intermediate_size,
-                                             const float mp_scale,
-                                             const bool preln);
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(__half);
 
 __global__ void gptj_residual_add(float* residual,
                                   const float* hidden_state,
                                   const float* attn,
                                   const float* bias,
                                   const float* attn_bias,
                                   const int total_count,
@@ -442,66 +412,23 @@
     dim3 block_dims(1024);
     dim3 grid_dims((total_count - 1) / 1024 + 1);  // (batch_size);
 
     gptj_residual_add<<<grid_dims, block_dims, 0, stream>>>(
         residual, hidden_state, attn, bias, attn_bias, total_count, hidden_dim / 4, 1.0 / mp_size);
 }
 
-template void launch_gptj_residual_add<float>(float*,
-                                              float*,
-                                              float*,
-                                              float*,
-                                              float*,
-                                              int,
-                                              int,
-                                              int,
-                                              cudaStream_t);
-
-#ifdef BF16_AVAILABLE
-template void launch_gptj_residual_add<__nv_bfloat16>(__nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      int,
-                                                      int,
-                                                      int,
-                                                      cudaStream_t);
-#endif
-
-template void launch_gptj_residual_add<__half>(__half*,
-                                               __half*,
-                                               __half*,
-                                               __half*,
-                                               __half*,
-                                               int,
-                                               int,
-                                               int,
-                                               cudaStream_t);
+#define INSTANTIATE_GPT_RES_ADD(T) \
+    template void launch_gptj_residual_add<T>(T*, T*, T*, T*, T*, int, int, int, cudaStream_t);
 
+INSTANTIATE_GPT_RES_ADD(float);
+INSTANTIATE_GPT_RES_ADD(__half);
 #ifdef BF16_AVAILABLE
-template __global__ void gptj_residual_add(__nv_bfloat16* residual,
-                                           const __nv_bfloat16* hidden_state,
-                                           const __nv_bfloat16* attn,
-                                           const __nv_bfloat16* bias,
-                                           const __nv_bfloat16* attn_bias,
-                                           const int total_count,
-                                           const int intermediate_size,
-                                           const float mp_scale);
+INSTANTIATE_GPT_RES_ADD(__nv_bfloat16);
 #endif
 
-template __global__ void gptj_residual_add(__half* residual,
-                                           const __half* hidden_state,
-                                           const __half* attn,
-                                           const __half* bias,
-                                           const __half* attn_bias,
-                                           const int total_count,
-                                           const int intermediate_size,
-                                           const float mp_scale);
-
 template <typename T>
 __global__ void moe_res_matmul(T* residual, T* coef, T* mlp_out, int seq_len, int hidden_dim)
 {
     constexpr int granularity = 16;
     constexpr int vals_per_access = granularity / sizeof(T);
 
     T* residual_seq = residual + blockIdx.x * hidden_dim;
@@ -538,36 +465,22 @@
 {
     dim3 grid_dim(seq_len);
     dim3 block_dim(1024);
     moe_res_matmul<<<grid_dim, block_dim, 0, stream>>>(
         residual, coef, mlp_out, seq_len, hidden_dim);
 }
 
-template void launch_moe_res_matmul(float* residual,
-                                    float* coef,
-                                    float* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+#define INSTANTIATE_LAUNCH_MOE_RES_MATMUL(T) \
+    template void launch_moe_res_matmul<T>(T*, T*, T*, int, int, cudaStream_t);
 
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(float);
 #ifdef BF16_AVAILABLE
-template void launch_moe_res_matmul(__nv_bfloat16* residual,
-                                    __nv_bfloat16* coef,
-                                    __nv_bfloat16* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(__nv_bfloat16);
 #endif
-
-template void launch_moe_res_matmul(__half* residual,
-                                    __half* coef,
-                                    __half* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(__half);
 
 template <typename T>
 __global__ void pad_data_kernel(T* padded_output, T* output, int head_size, int padded_head_size)
 {
     using T2 =
         typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
@@ -603,49 +516,23 @@
               cudaStream_t stream)
 {
     dim3 grid_dim((bsz - 1) / 16 + 1);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_data_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, head_size / 8, padded_head_size / 8);
 }
-template void pad_data(__half* padded_output,
-                       __half* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
 
-#ifdef BF16_AVAILABLE
-template void pad_data(__nv_bfloat16* padded_output,
-                       __nv_bfloat16* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
-#endif
-
-template void pad_data(float* padded_output,
-                       float* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
+#define INSTANTIATE_PAD_DATA(T) template void pad_data(T*, T*, int, int, int, cudaStream_t stream);
 
+INSTANTIATE_PAD_DATA(float);
+INSTANTIATE_PAD_DATA(__half);
 #ifdef BF16_AVAILABLE
-template __global__ void pad_data_kernel(__nv_bfloat16* padded_output,
-                                         __nv_bfloat16* output,
-                                         int head_size,
-                                         int padded_head_size);
+INSTANTIATE_PAD_DATA(__nv_bfloat16);
 #endif
 
-template __global__ void pad_data_kernel(__half* padded_output,
-                                         __half* output,
-                                         int head_size,
-                                         int padded_head_size);
-
 template <typename T>
 __global__ void pad_head_seq_kernel(T* padded_output,
                                     T* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
@@ -692,42 +579,22 @@
 {
     dim3 grid_dim(bsz, padded_seq_len / 16);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_head_seq_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, seq_len, padded_seq_len, head_size / 8, padded_head_size / 8);
 }
 
-template void pad_head_seq(__half* padded_output,
-                           __half* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+#define INSTANTIATE_PAD_HEAD_SEQ(T) \
+    template void pad_head_seq<T>(T*, T*, int, int, int, int, int, cudaStream_t);
 
+INSTANTIATE_PAD_HEAD_SEQ(__half);
 #ifdef BF16_AVAILABLE
-template void pad_head_seq(__nv_bfloat16* padded_output,
-                           __nv_bfloat16* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+INSTANTIATE_PAD_HEAD_SEQ(__nv_bfloat16);
 #endif
-
-template void pad_head_seq(float* padded_output,
-                           float* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+INSTANTIATE_PAD_HEAD_SEQ(float);
 
 // TODO(cmikeh2): evaluate different GeLU performance
 __device__ __forceinline__ float old_gelu(float val)
 {
     // 1 / sqrt(2)
     constexpr float rsqrt_2 = 0.707106769084930419922;
     return val * 0.5f * (1.0f + erff(val * rsqrt_2));
@@ -735,20 +602,23 @@
 
 namespace fused_geglu {
 constexpr int threads = 256;
 constexpr int steps = 2;
 constexpr int granularity = 16;
 }  // namespace fused_geglu
 
-template <typename T>
-__global__ void fused_bias_geglu(T* output,
-                                 const T* activation,
-                                 const T* bias,
-                                 int base_channels,
-                                 int total_elems)
+__device__ __forceinline__ float silu(float val) { return val / (1.0f + expf(-val)); }
+
+template <typename T, bool useGelu>
+__global__ void fused_gate_activation(T* output,
+                                      const T* activation,
+                                      const T* bias,
+                                      int base_channels,
+                                      int output_stride,
+                                      int total_elems)
 {
     constexpr int T_per_access = fused_geglu::granularity / sizeof(T);
     constexpr int T_per_step = T_per_access * fused_geglu::threads;
     constexpr int T_per_block = T_per_step * fused_geglu::steps;
 
     const int id = blockIdx.x * T_per_block + threadIdx.x * T_per_access;
 
@@ -765,41 +635,45 @@
             const int seq_id = iter_id / base_channels;
             const int seq_offset = seq_id * base_channels * 2;
 
             mem_access::load_global<fused_geglu::granularity>(activation_buffer_1,
                                                               activation + seq_offset + channel_id);
             mem_access::load_global<fused_geglu::granularity>(
                 activation_buffer_2, activation + seq_offset + channel_id + base_channels);
-            mem_access::load_global<fused_geglu::granularity>(bias_buffer_1, bias + channel_id);
-            mem_access::load_global<fused_geglu::granularity>(bias_buffer_2,
-                                                              bias + channel_id + base_channels);
+            mem_access::load_global<fused_geglu::granularity>(
+                bias_buffer_1, bias + channel_id, bias != nullptr);
+            mem_access::load_global<fused_geglu::granularity>(
+                bias_buffer_2, bias + channel_id + base_channels, bias != nullptr);
 
             // Since the GeLU is going to happen at float, might as well
             // convert
 #pragma unroll
             for (int v = 0; v < T_per_access; v++) {
                 T hidden_state = activation_buffer_1[v] + bias_buffer_1[v];
                 T pre_gate = activation_buffer_2[v] + bias_buffer_2[v];
-                float gate_f = old_gelu(conversion::to<float>(pre_gate));
+                float pre_gate_f = conversion::to<float>(pre_gate);
+                float gate_f = (useGelu) ? old_gelu(pre_gate_f) : silu(pre_gate_f);
                 T gate = conversion::to<T>(gate_f);
                 activation_buffer_1[v] = hidden_state * gate;
             }
 
-            mem_access::store_global<fused_geglu::granularity>(output + iter_id,
-                                                               activation_buffer_1);
+            mem_access::store_global<fused_geglu::granularity>(
+                output + seq_id * output_stride + channel_id, activation_buffer_1);
         }
     }
 }
 
 template <typename T>
-void launch_fused_bias_geglu(T* output,
+void launch_gated_activation(T* output,
                              const T* activation,
                              const T* bias,
                              int rows,
+                             int output_stride,
                              int elems_per_row,
+                             bool use_gelu,
                              cudaStream_t stream)
 {
     /*
     Fused bias GEGLU is a variant of the gated activation functions.
     The input here is a matrix of [batch, seq_len, 2 * intermediate_dim]
     where the second half of the channels act as GeLU gates for the first
     half.
@@ -812,26 +686,25 @@
 
     const int base_channels = elems_per_row / 2;
     const int total_elems = base_channels * rows;
 
     dim3 block(fused_geglu::threads);
     dim3 grid((total_elems + T_per_block - 1) / T_per_block);
 
-    fused_bias_geglu<<<grid, block, 0, stream>>>(
-        output, activation, bias, base_channels, total_elems);
+    if (use_gelu) {
+        fused_gate_activation<T, true><<<grid, block, 0, stream>>>(
+            output, activation, bias, base_channels, output_stride, total_elems);
+    } else {
+        fused_gate_activation<T, false><<<grid, block, 0, stream>>>(
+            output, activation, bias, base_channels, output_stride, total_elems);
+    }
 }
 
-template void launch_fused_bias_geglu(__half*,
-                                      const __half*,
-                                      const __half*,
-                                      int,
-                                      int,
-                                      cudaStream_t);
+#define INSTANTIATE_LAUNCH_GATED_ACTIVATION(T) \
+    template void launch_gated_activation(     \
+        T*, const T*, const T*, int, int, int, bool, cudaStream_t);
+
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(__half);
 #ifdef BF16_AVAILABLE
-template void launch_fused_bias_geglu(__nv_bfloat16*,
-                                      const __nv_bfloat16*,
-                                      const __nv_bfloat16*,
-                                      int,
-                                      int,
-                                      cudaStream_t);
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(__nv_bfloat16);
 #endif
-template void launch_fused_bias_geglu(float*, const float*, const float*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(float);
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files 12% similar despite different names*

```diff
@@ -42,27 +42,25 @@
     cg::thread_block_tile<hw_warp_size> warp = cg::tiled_partition<hw_warp_size>(tb);
 
     // X-dimension of the block
     const int block_offset = (tb.group_index().x * (maxThreads / threadsPerGroup) * elems_per_row) +
                              (tb.thread_index().y * elems_per_row);
     const int thread_offset = tb.thread_index().x * T_per_load;
     const int base_offset = block_offset + thread_offset;
-    const int stride = tb.size() * T_per_load;
+    const int stride = blockDim.x * T_per_load;
 
     float sum = reduce::init<rop::Add, float>();
 
     const T* input_base = vals + base_offset;
 
     T local_buffer[unRoll * T_per_load];
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
-        T residual_buffer[T_per_load];
-        T bias_buffer[T_per_load];
 
         mem_access::load_global<ln::granularity>(
             iteration_buffer, input_base + i * stride, thread_offset + i * stride < elems_per_row);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
             float vals_up_cast = conversion::to<float>(iteration_buffer[j]);
@@ -87,16 +85,16 @@
         }
     }
 
     reduce::partitioned_block<rop::Add, threadsPerGroup>(tb, warp, mean_diff);
     const float variance = mean_diff / elems_per_row;
     const float denom = __frsqrt_rn(variance + epsilon);
 
-    const T mean_compute = conversion::to<T>(mean);
-    const T denom_compute = conversion::to<T>(denom);
+    // const T mean_compute = conversion::to<T>(mean);
+    // const T denom_compute = conversion::to<T>(denom);
 
     T* block_output = output + block_offset;
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
         const int iter_idx = i * stride + thread_offset;
@@ -105,16 +103,19 @@
         T gamma_local[T_per_load], beta_local[T_per_load];
 
         mem_access::load_global<ln::granularity>(gamma_local, gamma + iter_idx, do_loads);
         mem_access::load_global<ln::granularity>(beta_local, beta + iter_idx, do_loads);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
-            iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
-            iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            float val = conversion::to<float>(iteration_buffer[j]);
+            val = (val - mean) * denom;
+            val =
+                val * conversion::to<float>(gamma_local[j]) + conversion::to<float>(beta_local[j]);
+            iteration_buffer[j] = conversion::to<T>(val);
         }
 
         if (do_loads) {
             mem_access::store_global<ln::granularity>(block_output + iter_idx, iteration_buffer);
         }
     }
 }
@@ -185,34 +186,22 @@
         LAUNCH_FUSED_LN(3 * internal_unRoll, maxThreads, maxThreads);
     } else if (external_unRoll == 4) {
         // 12289 - 16384 elems
         LAUNCH_FUSED_LN(4 * internal_unRoll, maxThreads, maxThreads);
     }
 }
 
-template void launch_fused_ln(__half*,
-                              const __half*,
-                              const __half*,
-                              const __half*,
-                              float,
-                              int,
-                              int,
-                              cudaStream_t);
+#define INSTANTIATE_FUSED_LN(T) \
+    template void launch_fused_ln(T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
+
+INSTANTIATE_FUSED_LN(__half);
 #ifdef BF16_AVAILABLE
-template void launch_fused_ln(__nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              float,
-                              int,
-                              int,
-                              cudaStream_t);
+INSTANTIATE_FUSED_LN(__nv_bfloat16);
 #endif
-template void
-launch_fused_ln(float*, const float*, const float*, const float*, float, int, int, cudaStream_t);
+INSTANTIATE_FUSED_LN(float);
 
 /*
 Fused resiual + bias + layer norm implementation. Assumes elems_per_row % 8
 is equal to 0.
 
 TODO(cmikeh2): Goal is to deprecate this implementation. The bias + residual
 need to be fused into compute-bound producer operations.
@@ -280,15 +269,15 @@
             bias_buffer, bias_base + i * stride, thread_offset + i * stride < elems_per_row);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
             float vals_up_cast = conversion::to<float>(iteration_buffer[j]);
             float res_up_cast = conversion::to<float>(residual_buffer[j]);
             float bias_up_cast = conversion::to<float>(bias_buffer[j]);
-            vals_up_cast += res_up_cast + bias_up_cast;
+            vals_up_cast = vals_up_cast + bias_up_cast + res_up_cast;
             sum = reduce::element<rop::Add>(sum, vals_up_cast);
             iteration_buffer[j] = conversion::to<T>(vals_up_cast);
         }
 
         if (preLnResidual && (thread_offset + i * stride < elems_per_row)) {
             mem_access::store_global<ln::granularity>(res_output + base_offset + i * stride,
                                                       iteration_buffer);
@@ -311,17 +300,14 @@
         }
     }
 
     reduce::partitioned_block<rop::Add, threadsPerGroup>(tb, warp, mean_diff);
     const float variance = mean_diff / elems_per_row;
     const float denom = __frsqrt_rn(variance + epsilon);
 
-    const T mean_compute = conversion::to<T>(mean);
-    const T denom_compute = conversion::to<T>(denom);
-
     T* block_output = output + block_offset;
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
         const int iter_idx = i * stride + thread_offset;
         const bool do_loads = iter_idx < elems_per_row;
@@ -329,16 +315,21 @@
         T gamma_local[T_per_load], beta_local[T_per_load];
 
         mem_access::load_global<ln::granularity>(gamma_local, gamma + iter_idx, do_loads);
         mem_access::load_global<ln::granularity>(beta_local, beta + iter_idx, do_loads);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
-            iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
-            iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            // iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
+            // iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            float val = conversion::to<float>(iteration_buffer[j]);
+            val = (val - mean) * denom;
+            val =
+                val * conversion::to<float>(gamma_local[j]) + conversion::to<float>(beta_local[j]);
+            iteration_buffer[j] = conversion::to<T>(val);
         }
 
         if (do_loads) {
             mem_access::store_global<ln::granularity>(block_output + iter_idx, iteration_buffer);
         }
     }
 }
@@ -487,81 +478,26 @@
         LAUNCH_FUSED_RES_LN_STORE_PRE_LN_RES(3 * internal_unRoll, maxThreads, maxThreads);
     } else if (external_unRoll == 4) {
         // 12289 - 16384 elems
         LAUNCH_FUSED_RES_LN_STORE_PRE_LN_RES(4 * internal_unRoll, maxThreads, maxThreads);
     }
 }
 
-// No-store specializations
-template void launch_fused_residual_ln(__half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
+#define INSTANTIATE_RES_LN(T)                  \
+    template void launch_fused_residual_ln<T>( \
+        T*, const T*, const T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
+
+#define INSTANTIATE_PRE_LN_RES(T)                               \
+    template void launch_fused_residual_ln_store_pre_ln_res<T>( \
+        T*, T*, const T*, const T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
 
+INSTANTIATE_RES_LN(__half);
+INSTANTIATE_RES_LN(float);
 #ifdef BF16_AVAILABLE
-template void launch_fused_residual_ln(__nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
+INSTANTIATE_RES_LN(__nv_bfloat16);
 #endif
 
-template void launch_fused_residual_ln(float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
-
-// Store specializations
-template void launch_fused_residual_ln_store_pre_ln_res(__half*,
-                                                        __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
-
+INSTANTIATE_PRE_LN_RES(__half);
+INSTANTIATE_PRE_LN_RES(float);
 #ifdef BF16_AVAILABLE
-template void launch_fused_residual_ln_store_pre_ln_res(__nv_bfloat16*,
-                                                        __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
+INSTANTIATE_PRE_LN_RES(__nv_bfloat16);
 #endif
-
-template void launch_fused_residual_ln_store_pre_ln_res(float*,
-                                                        float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 #include "inference_cuda_layers.h"
 
 std::array<int, 3> gemm_algos = std::array<int, 3>({99, 99, 99});
 
 // NOTE: This activation function type enum should be always in sync
 // with the python counterpart, otherwise the casting from python binding
 // will be incorrect.
-enum class ActivationFuncType { UNKNOWN = 0, GELU = 1, ReLU = 2 };
+enum class ActivationFuncType { UNKNOWN = 0, GELU = 1, ReLU = 2, GATED_GELU = 3, GATED_SILU = 4 };
+
+enum class NormType { UNKNOWN = 0, LayerNorm = 1, GroupNorm = 2, RMSNorm = 3 };
 
 enum class TransformerType : uint8_t { UNKNOWN = 0, GPTType = 1, BERTType = 2 };
 
 // NOTE: this is a temporary and dodgy solution to distinguish GPT and BERT style models
 // based on the dimensions of the corresponding attention mask.
 inline auto infer_transformer_type(at::Tensor& attn_mask) -> TransformerType
 {
@@ -137,15 +139,15 @@
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     float alpha = 1;
     float gemm_beta = 0.0;
 
     /*
     // Reallocate memory if we received a new prompt
     if (!workspace || input.size(1) != 1) {
-        allocate_workspace<T>(W.size(1), InferenceContext::Instance().GetMaxTokenLenght(),
+        allocate_workspace<T>(W.size(1), InferenceContext::Instance().GetMaxTokenLength(),
     Q.size(0), 1, head_size); workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     }
     */
 
     auto O = at::from_blob(workspace, {Q.size(1), Q.size(2), W.size(1)}, options);
     unsigned m = W.size(1);
     unsigned n = Q.size(1) * Q.size(2);
@@ -378,15 +380,15 @@
                                 &alpha,
                                 &gemm_beta,
                                 (T*)prev_key_cont,
                                 (T*)query_cont,
                                 workspace,
                                 CUBLAS_OP_T,
                                 CUBLAS_OP_N,
-                                InferenceContext::Instance().GetMaxTokenLenght() * k,
+                                InferenceContext::Instance().GetMaxTokenLength() * k,
                                 seq_len * k,
                                 seq_len * soft_len,
                                 bsz * heads,
 #ifdef __HIP_PLATFORM_HCC__
                                 rocblas_gemm_algo_standard);
 #else
                                 CUBLAS_GEMM_DEFAULT_TENSOR_OP);
@@ -411,15 +413,15 @@
                                 &alpha,
                                 &gemm_beta,
                                 (T*)prev_value_cont,
                                 workspace,
                                 (T*)output,
                                 CUBLAS_OP_N,
                                 CUBLAS_OP_N,
-                                InferenceContext::Instance().GetMaxTokenLenght() * k,
+                                InferenceContext::Instance().GetMaxTokenLength() * k,
                                 seq_len * soft_len,
                                 seq_len * k,
                                 bsz * heads,
 #ifdef __HIP_PLATFORM_HCC__
                                 rocblas_gemm_algo_standard);
 #else
                                 CUBLAS_GEMM_DEFAULT_TENSOR_OP);
@@ -462,19 +464,19 @@
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     size_t buf_size = bsz * seq_len * hidden_dim;
     auto output = torch::from_blob(workspace + 4 * buf_size, {bsz, seq_len, hidden_dim}, options);
 
     auto query_cont = workspace + 5 * buf_size;
     size_t offset =
-        10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLenght()) +
-        layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
+        10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLength()) +
+        layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLength() * hidden_dim;
     unsigned all_tokens = soft_len;
     auto kv_cache = workspace + offset + (hidden_dim / heads) * (is_prompt ? 0 : soft_len - 1);
-    size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
+    size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLength() * hidden_dim;
 
     T* temp_buf = (T*)output.data_ptr() + at::numel(output);
     launch_bias_add_transform_0213<T>((T*)query_cont,
                                       kv_cache,
                                       kv_cache + value_offset,
                                       (T*)query_key_value.data_ptr(),
                                       nullptr,
@@ -485,28 +487,26 @@
                                       hidden_dim,
                                       heads,
                                       rotary_dim,
                                       rotate_half,
                                       rotate_every_two,
                                       InferenceContext::Instance().GetCurrentStream(),
                                       3,
-                                      InferenceContext::Instance().GetMaxTokenLenght());
+                                      InferenceContext::Instance().GetMaxTokenLength());
     if (rotary_dim > 0 && rotate_half)
         launch_apply_rotary_pos_emb(query_cont,
                                     kv_cache,
                                     k,
                                     seq_len,
                                     rotary_dim,
                                     (is_prompt ? 0 : soft_len - 1),
                                     heads,
                                     bsz,
-                                    rotate_half,
-                                    rotate_every_two,
                                     InferenceContext::Instance().GetCurrentStream(),
-                                    InferenceContext::Instance().GetMaxTokenLenght());
+                                    InferenceContext::Instance().GetMaxTokenLength());
 
     attention_unfused<T>(workspace + offset,
                          (T*)query_cont,
                          attn_mask,
                          workspace + offset + value_offset,
                          temp_buf,
                          bsz,
@@ -529,25 +529,25 @@
                                output.size(2),
                                InferenceContext::Instance().GetCurrentStream(false),
                                1);
 
     if (layer_id == num_layers - 1) InferenceContext::Instance().advance_tokens();
     auto prev_key = torch::from_blob(workspace + offset,
                                      {bsz, heads, all_tokens, k},
-                                     {hidden_dim * InferenceContext::Instance().GetMaxTokenLenght(),
-                                      k * InferenceContext::Instance().GetMaxTokenLenght(),
+                                     {hidden_dim * InferenceContext::Instance().GetMaxTokenLength(),
+                                      k * InferenceContext::Instance().GetMaxTokenLength(),
                                       k,
                                       1},
                                      options);
 
     auto prev_value =
         torch::from_blob(workspace + offset + value_offset,
                          {bsz, heads, all_tokens, k},
-                         {hidden_dim * InferenceContext::Instance().GetMaxTokenLenght(),
-                          k * InferenceContext::Instance().GetMaxTokenLenght(),
+                         {hidden_dim * InferenceContext::Instance().GetMaxTokenLength(),
+                          k * InferenceContext::Instance().GetMaxTokenLength(),
                           k,
                           1},
                          options);
 
     return {output, prev_key, prev_value};
 }
 
@@ -563,45 +563,52 @@
                      (T*)bias.data_ptr(),
                      intermediate_size,
                      bsz,
                      InferenceContext::Instance().GetCurrentStream());
     return input_cont;
 }
 
-at::Tensor ds_bias_geglu(at::Tensor& activation, at::Tensor& bias)
+#define DISPATCH_GATED_ACT(T_TYPE, C_TYPE)                                         \
+    if (activation.options().dtype() == torch::T_TYPE) {                           \
+        launch_gated_activation((C_TYPE*)output.data_ptr(),                        \
+                                (const C_TYPE*)activation.data_ptr(),              \
+                                (const C_TYPE*)bias.data_ptr(),                    \
+                                rows,                                              \
+                                out_channels,                                      \
+                                channels,                                          \
+                                activation_type == ActivationFuncType::GATED_GELU, \
+                                InferenceContext::Instance().GetCurrentStream());  \
+    }
+
+at::Tensor ds_gated_activation(at::Tensor& activation, at::Tensor& bias, int actFun)
 {
     /*
     Used in FF of Stable diffusion
     */
 
+    const ActivationFuncType activation_type = static_cast<ActivationFuncType>(actFun);
+
+    assert(activation_type == ActivationFuncType::GATED_GELU ||
+           activation_type == ActivationFuncType::GATED_SILU);
+
     const int batch_size = activation.size(0);
     const int seq_len = activation.size(1);
     const int channels = activation.size(2);
 
     const int rows = batch_size * seq_len;
     // Dimensionality is cut in half
     const int out_channels = channels / 2;
 
     auto output = at::empty({batch_size, seq_len, out_channels}, activation.options());
 
-    if (activation.options().dtype() == torch::kFloat32) {
-        launch_fused_bias_geglu((float*)output.data_ptr(),
-                                (const float*)activation.data_ptr(),
-                                (const float*)bias.data_ptr(),
-                                rows,
-                                channels,
-                                InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_bias_geglu((__half*)output.data_ptr(),
-                                (const __half*)activation.data_ptr(),
-                                (const __half*)bias.data_ptr(),
-                                rows,
-                                channels,
-                                InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_GATED_ACT(kFloat, float);
+    DISPATCH_GATED_ACT(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_GATED_ACT(kBFloat16, __nv_bfloat16);
+#endif
 
     return output;
 }
 
 template <typename T>
 at::Tensor ds_bias_relu(at::Tensor& input, at::Tensor& bias)
 {
@@ -647,43 +654,107 @@
     //                      bsz,
     //                      input_cont.size(2),
     //                      (bias.size(0) > 1),
     //                      InferenceContext::Instance().GetCurrentStream());
     return input_cont;
 }
 
+#define DISPATCH_LAYER_NORM(T_TYPE, C_TYPE)                               \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_fused_ln((C_TYPE*)output.data_ptr(),                       \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        (const C_TYPE*)beta.data_ptr(),                   \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 at::Tensor ds_layer_norm(at::Tensor& input, at::Tensor& gamma, at::Tensor& beta, float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_ln((__half*)output.data_ptr(),
-                        (const __half*)input.data_ptr(),
-                        (const __half*)gamma.data_ptr(),
-                        (const __half*)beta.data_ptr(),
-                        epsilon,
-                        rows,
-                        elems_per_row,
-                        InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_ln((float*)output.data_ptr(),
-                        (const float*)input.data_ptr(),
-                        (const float*)gamma.data_ptr(),
-                        (const float*)beta.data_ptr(),
-                        epsilon,
-                        rows,
-                        elems_per_row,
-                        InferenceContext::Instance().GetCurrentStream());
+    DISPATCH_LAYER_NORM(kFloat, float);
+    DISPATCH_LAYER_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_LAYER_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
+    return output;
+}
+
+#define DISPATCH_RMS_NORM(T_TYPE, C_TYPE)                                 \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_rms_norm((C_TYPE*)output.data_ptr(),                       \
+                        (C_TYPE*)nullptr,                                 \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)nullptr,                           \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
     }
 
+at::Tensor ds_rms_norm(at::Tensor& input, at::Tensor& gamma, float epsilon)
+{
+    // Get number of dims of tensor
+    int num_dims = input.dim();
+    const int rows = (num_dims == 2) ? input.size(0) : input.size(0) * input.size(1);
+    const int elems_per_row = (num_dims == 2) ? input.size(1) : input.size(2);
+
+    auto output = at::empty_like(input);
+
+    DISPATCH_RMS_NORM(kFloat, float);
+    DISPATCH_RMS_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_RMS_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
     return output;
 }
 
+#define DISPATCH_PRE_RMS_NORM(T_TYPE, C_TYPE)                             \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_rms_norm((C_TYPE*)output.data_ptr(),                       \
+                        (C_TYPE*)res_out.data_ptr(),                      \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)residual.data_ptr(),               \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
+    }
+
+std::vector<at::Tensor> ds_pre_rms_norm(at::Tensor& input,
+                                        at::Tensor& residual,
+                                        at::Tensor& gamma,
+                                        float epsilon)
+{
+    // Get number of dims of tensor
+    int num_dims = input.dim();
+    const int rows = (num_dims == 2) ? input.size(0) : input.size(0) * input.size(1);
+    const int elems_per_row = (num_dims == 2) ? input.size(1) : input.size(2);
+
+    auto output = at::empty_like(input);
+    auto res_out = at::empty_like(residual);
+
+    DISPATCH_PRE_RMS_NORM(kFloat, float);
+    DISPATCH_PRE_RMS_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_PRE_RMS_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
+    return {output, res_out};
+}
+
 template <typename T>
 void ds_layer_norm_internal(T* workspace,
                             at::Tensor& input,
                             at::Tensor& gamma,
                             at::Tensor& beta,
                             float epsilon)
 {
@@ -694,91 +765,83 @@
                     (const T*)beta.data_ptr(),
                     epsilon,
                     bsz,
                     input.size(2),
                     InferenceContext::Instance().GetCurrentStream());
 }
 
+#define DISPATCH_LAYER_NORM_RESIDUAL(T_TYPE, C_TYPE)                               \
+    if (input.options().dtype() == torch::T_TYPE) {                                \
+        launch_fused_residual_ln((C_TYPE*)output.data_ptr(),                       \
+                                 (const C_TYPE*)input.data_ptr(),                  \
+                                 (const C_TYPE*)residual.data_ptr(),               \
+                                 (const C_TYPE*)bias.data_ptr(),                   \
+                                 (const C_TYPE*)gamma.data_ptr(),                  \
+                                 (const C_TYPE*)beta.data_ptr(),                   \
+                                 epsilon,                                          \
+                                 rows,                                             \
+                                 elems_per_row,                                    \
+                                 InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 /* Currently only used in unit testing */
 at::Tensor ds_layer_norm_residual(at::Tensor& input,
                                   at::Tensor& bias,
                                   at::Tensor& residual,
                                   at::Tensor& gamma,
                                   at::Tensor& beta,
                                   float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_residual_ln((__half*)output.data_ptr(),
-                                 (const __half*)input.data_ptr(),
-                                 (const __half*)residual.data_ptr(),
-                                 (const __half*)bias.data_ptr(),
-                                 (const __half*)gamma.data_ptr(),
-                                 (const __half*)beta.data_ptr(),
-                                 epsilon,
-                                 rows,
-                                 elems_per_row,
-                                 InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_residual_ln((float*)output.data_ptr(),
-                                 (const float*)input.data_ptr(),
-                                 (const float*)residual.data_ptr(),
-                                 (const float*)bias.data_ptr(),
-                                 (const float*)gamma.data_ptr(),
-                                 (const float*)beta.data_ptr(),
-                                 epsilon,
-                                 rows,
-                                 elems_per_row,
-                                 InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_LAYER_NORM_RESIDUAL(kFloat, float);
+    DISPATCH_LAYER_NORM_RESIDUAL(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_LAYER_NORM_RESIDUAL(kBFloat16, __nv_bfloat16);
+#endif
 
     return output;
 }
 
+#define DISPATCH_PRE_LAYER_NORM_RESIDUAL(T_TYPE, C_TYPE)      \
+    if (input.options().dtype() == torch::T_TYPE) {           \
+        launch_fused_residual_ln_store_pre_ln_res(            \
+            (C_TYPE*)norm_output.data_ptr(),                  \
+            (C_TYPE*)res_output.data_ptr(),                   \
+            (const C_TYPE*)input.data_ptr(),                  \
+            (const C_TYPE*)residual.data_ptr(),               \
+            (const C_TYPE*)bias.data_ptr(),                   \
+            (const C_TYPE*)gamma.data_ptr(),                  \
+            (const C_TYPE*)beta.data_ptr(),                   \
+            epsilon,                                          \
+            rows,                                             \
+            elems_per_row,                                    \
+            InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 /* Currently only used in unit testing */
 std::vector<at::Tensor> ds_layer_norm_residual_store_pre_ln_res(at::Tensor& input,
                                                                 at::Tensor& bias,
                                                                 at::Tensor& residual,
                                                                 at::Tensor& gamma,
                                                                 at::Tensor& beta,
                                                                 float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto norm_output = at::empty_like(input);
     auto res_output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_residual_ln_store_pre_ln_res((__half*)norm_output.data_ptr(),
-                                                  (__half*)res_output.data_ptr(),
-                                                  (const __half*)input.data_ptr(),
-                                                  (const __half*)residual.data_ptr(),
-                                                  (const __half*)bias.data_ptr(),
-                                                  (const __half*)gamma.data_ptr(),
-                                                  (const __half*)beta.data_ptr(),
-                                                  epsilon,
-                                                  rows,
-                                                  elems_per_row,
-                                                  InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_residual_ln_store_pre_ln_res((float*)norm_output.data_ptr(),
-                                                  (float*)res_output.data_ptr(),
-                                                  (const float*)input.data_ptr(),
-                                                  (const float*)residual.data_ptr(),
-                                                  (const float*)bias.data_ptr(),
-                                                  (const float*)gamma.data_ptr(),
-                                                  (const float*)beta.data_ptr(),
-                                                  epsilon,
-                                                  rows,
-                                                  elems_per_row,
-                                                  InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kFloat, float);
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kBFloat16, __nv_bfloat16);
+#endif
 
     return {norm_output, res_output};
 }
 
 template <typename T>
 void quantized_gemm(void* output,
                     T* input,
@@ -875,26 +938,89 @@
                         (transposed_mode || q_int8) ? weight.size(0) : weight.size(1),
                         bsz,
                         InferenceContext::Instance().GetCurrentStream());
     return torch::from_blob(workspace, input.sizes(), input.options());
 }
 
 template <typename T>
+std::vector<at::Tensor> ds_rms_qkv(at::Tensor& input,
+                                   at::Tensor& weight,
+                                   at::Tensor& q_scale,
+                                   at::Tensor& gamma,
+                                   const float epsilon,
+                                   bool q_int8,
+                                   bool transposed_mode)
+{
+    const int bsz = input.size(0) * input.size(1);
+    T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
+    T* rms_norm_ptr = workspace + (3 * bsz * input.size(2));
+    int out_size = (transposed_mode || q_int8) ? weight.size(0) : weight.size(1);
+
+    auto options = at::TensorOptions()
+                       .dtype(input.options().dtype())
+                       .layout(at::kStrided)
+                       .device(at::kCUDA)
+                       .requires_grad(false);
+    auto rms_norm = at::from_blob(rms_norm_ptr, input.sizes(), options);
+    auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
+
+    launch_rms_norm((T*)rms_norm.data_ptr(),
+                    (T*)nullptr,
+                    (const T*)input.data_ptr(),
+                    (const T*)nullptr,
+                    (const T*)gamma.data_ptr(),
+                    epsilon,
+                    bsz,
+                    input.size(2),
+                    InferenceContext::Instance().GetCurrentStream());
+
+    if (q_int8) {
+        quantized_gemm<T>((T*)output.data_ptr(),
+                          (T*)rms_norm.data_ptr(),
+                          weight,
+                          q_scale,
+                          q_scale.size(0),
+                          bsz,
+                          input.size(2));
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       weight.size(transposed_mode ? 0 : 1),
+                       bsz,
+                       input.size(2),
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight.data_ptr(),
+                       (T*)rms_norm.data_ptr(),
+                       (T*)output.data_ptr(),
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard);
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP);
+#endif
+    }
+
+    return {output, rms_norm};
+}
+
+template <typename T>
 std::vector<at::Tensor> ds_qkv_gemm(at::Tensor& input,
                                     at::Tensor& weight,
                                     at::Tensor& q_scale,
                                     at::Tensor& bias,
                                     at::Tensor& gamma,
                                     at::Tensor& beta,
                                     const float epsilon,
                                     bool add_bias,
-                                    unsigned num_layers,
-                                    bool external_cache,
-                                    unsigned mp_size,
-                                    unsigned rank,
                                     bool q_int8,
                                     bool transposed_mode)
 {
     int bsz = input.size(0) * input.size(1);
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     int out_size = (transposed_mode || q_int8) ? weight.size(0) : weight.size(1);
 
@@ -962,48 +1088,14 @@
                    rocblas_gemm_algo_standard);
 #else
                    CUBLAS_GEMM_DEFAULT_TENSOR_OP);
 #endif
 }
 
 template <typename T>
-at::Tensor ds_qkv_gemm_int8(at::Tensor& input,
-                            at::Tensor& weight,
-                            at::Tensor& bias,
-                            at::Tensor& gamma,
-                            at::Tensor& beta,
-                            const float epsilon,
-                            at::Tensor& q_scale,
-                            int groups,
-                            bool add_bias)
-{
-    int bsz = input.size(0) * input.size(1);
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    auto inp_norm = ds_layer_norm(input_cont, gamma, beta, epsilon);
-
-    quantized_gemm<T>(output, inp_norm, weight, q_scale, groups, 0);
-    if (add_bias)
-        launch_bias_add((T*)output.data_ptr(),
-                        (T*)bias.data_ptr(),
-                        weight.size(1),
-                        bsz,
-                        InferenceContext::Instance().GetCurrentStream());
-
-    return output;
-}
-
-template <typename T>
 at::Tensor ds_linear_layer(at::Tensor& input,
                            at::Tensor& weight,
                            at::Tensor& bias,
                            bool add_bias,
                            bool do_flash_attn,
                            int num_heads,
                            bool transposed_mode)
@@ -1203,39 +1295,14 @@
         at::from_blob(key_pad_ptr,
                       {query.size(0), heads, key_value_length, padded_head_size},
                       query.options()),
         at::from_blob(value_pad_ptr,
                       {query.size(0), heads, key_value_length, padded_head_size},
                       query.options())};
 }
-template <typename T>
-at::Tensor ds_linear_layer_int8(at::Tensor& input,
-                                at::Tensor& weight,
-                                at::Tensor& bias,
-                                at::Tensor& q_scale,
-                                int groups)
-{
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-    int bsz = input_cont.size(0) * input_cont.size(1);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    quantized_gemm<T>(output, input_cont, weight, q_scale, groups, 0);
-    launch_bias_add((T*)output.data_ptr(),
-                    (T*)bias.data_ptr(),
-                    weight.size(1),
-                    bsz,
-                    InferenceContext::Instance().GetCurrentStream());
-    return output;
-}
 
 template <typename T>
 at::Tensor ds_vector_matmul(at::Tensor& input,
                             at::Tensor& weight,
                             bool async_op,
                             at::Tensor& q_scale,
                             bool q_int8,
@@ -1465,60 +1532,166 @@
                                          act_func_type,
                                          transposed_mode);
 
     return {output, res_add};
 }
 
 template <typename T>
-std::vector<at::Tensor> ds_mlp_gemm_int8(at::Tensor& input,
-                                         at::Tensor& residual,
-                                         at::Tensor& input_bias,
-                                         at::Tensor& weight,
-                                         at::Tensor& bias,
-                                         at::Tensor& gamma,
-                                         at::Tensor& beta,
-                                         const float epsilon,
-                                         at::Tensor& q_scale,
-                                         int groups,
-                                         bool preLayerNorm)
-{
-    auto input_cont = input.contiguous();
+std::vector<at::Tensor> ds_rms_mlp_gemm(at::Tensor& input,
+                                        at::Tensor& residual,
+                                        at::Tensor& weight_interm,
+                                        at::Tensor& weight_out,
+                                        at::Tensor& gamma,
+                                        const float epsilon,
+                                        at::Tensor& q_scale,
+                                        at::Tensor& q_scale1,
+                                        bool q_int8,
+                                        int activation_type,
+                                        bool transposed_mode)
+{
+    const int bsz = input.size(0) * input.size(1);
+    const size_t input_neurons = input.size(2);
+    const size_t mlp_1_out_neurons = transposed_mode ? weight_interm.size(0)
+                                                     : weight_interm.size(1);
+    const size_t mlp_2_in_neurons = transposed_mode ? weight_out.size(1) : weight_out.size(0);
+
     auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
+                       .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
+    T* output_ptr = (T*)InferenceContext::Instance().GetWorkSpace() + torch::numel(input);
+    T* inp_norm_ptr = output_ptr + torch::numel(input);
+    T* intermediate_ptr = inp_norm_ptr + torch::numel(input);
+
+    auto output = at::from_blob(output_ptr, input.sizes(), options);
+    auto inp_norm = at::from_blob(inp_norm_ptr, input.sizes(), options);
+    auto intermediate_gemm =
+        at::from_blob(intermediate_ptr, {input.size(0), input.size(1), mlp_1_out_neurons}, options);
 
-    int bsz = input_cont.size(0) * input_cont.size(1);
-    auto inp_norm = at::empty_like(input_cont);
+    auto act_func_type = static_cast<ActivationFuncType>(activation_type);
 
-    auto residual_add = (preLayerNorm ? at::empty_like(input_cont) : inp_norm);
-    quantized_gemm<T>(output, inp_norm, weight, q_scale, groups, 0);
-    launch_bias_gelu((T*)output.data_ptr(),
-                     (T*)bias.data_ptr(),
-                     weight.size(1),
-                     bsz,
-                     InferenceContext::Instance().GetCurrentStream());
+    // RMS Norm, we'll update the residual in-place
+    launch_rms_norm((T*)inp_norm.data_ptr(),
+                    (T*)residual.data_ptr(),
+                    (const T*)input.data_ptr(),
+                    (const T*)residual.data_ptr(),
+                    (const T*)gamma.data_ptr(),
+                    epsilon,
+                    bsz,
+                    input_neurons,
+                    InferenceContext::Instance().GetCurrentStream());
+
+    if (q_int8) {
+        quantized_gemm<T>(intermediate_ptr,
+                          (T*)inp_norm.data_ptr(),
+                          weight_interm,
+                          q_scale,
+                          q_scale.size(0),
+                          bsz,
+                          input_neurons);
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       mlp_1_out_neurons,
+                       bsz,
+                       input_neurons,
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight_interm.data_ptr(),
+                       (T*)inp_norm.data_ptr(),
+                       intermediate_ptr,
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard);
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP);
+#endif
+    }
+
+    if (act_func_type == ActivationFuncType::GELU) {
+        launch_bias_gelu(intermediate_ptr,
+                         (T*)nullptr,
+                         mlp_1_out_neurons,
+                         bsz,
+                         InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::ReLU) {
+        launch_bias_relu(intermediate_ptr,
+                         (T*)nullptr,
+                         mlp_1_out_neurons,
+                         bsz,
+                         InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::GATED_GELU) {
+        launch_gated_activation(intermediate_ptr,
+                                (const T*)intermediate_ptr,
+                                (const T*)nullptr,
+                                bsz,
+                                mlp_1_out_neurons,
+                                mlp_1_out_neurons,
+                                true,
+                                InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::GATED_SILU) {
+        launch_gated_activation(intermediate_ptr,
+                                (const T*)intermediate_ptr,
+                                (const T*)nullptr,
+                                bsz,
+                                mlp_1_out_neurons,
+                                mlp_1_out_neurons,
+                                false,
+                                InferenceContext::Instance().GetCurrentStream());
+    }
 
-    return {output, residual_add};
+    if (q_int8) {
+        quantized_gemm<T>(output.data_ptr(),
+                          intermediate_ptr,
+                          weight_out,
+                          q_scale1,
+                          q_scale1.size(0),
+                          bsz,
+                          input.size(2));
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       input_neurons,
+                       bsz,
+                       mlp_2_in_neurons,
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight_out.data_ptr(),
+                       intermediate_ptr,
+                       (T*)output.data_ptr(),
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard,
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP,
+#endif
+                       mlp_1_out_neurons);
+    }
+
+    return {output, residual};
 }
 
 template <typename T>
 at::Tensor fused_gemm_gelu(at::Tensor& input,
                            at::Tensor& weight,
                            at::Tensor& weight_scale,
                            at::Tensor& bias,
                            at::Tensor& weight_out,
                            at::Tensor& weight_out_scale,
-                           const float epsilon,
-                           bool preLayerNorm,
                            bool q_int8,
-                           bool async_op,
                            bool transposed_mode)
 {
     auto options = at::TensorOptions()
                        .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
@@ -1637,21 +1810,43 @@
             hidden_size,
             bsz,
             mp_size,
             InferenceContext::Instance().GetCurrentStream());
     return residual;
 }
 
+#define DISPATCH_VECTOR_ADD(T_TYPE, C_TYPE)                                         \
+    if (a.scalar_type() == at::k##T_TYPE) {                                         \
+        launch_vector_add<C_TYPE>((C_TYPE*)(a.data_ptr()),                          \
+                                  (const C_TYPE*)(a.data_ptr()),                    \
+                                  (const C_TYPE*)(b.data_ptr()),                    \
+                                  gamma,                                            \
+                                  total_elems,                                      \
+                                  InferenceContext::Instance().GetCurrentStream()); \
+    }
+
+at::Tensor& _vector_add(at::Tensor& a, at::Tensor& b, float gamma)
+{
+    const int total_elems = a.numel();
+
+    DISPATCH_VECTOR_ADD(Float, float)
+    DISPATCH_VECTOR_ADD(Half, __half)
+#ifdef BF16_AVAILABLE
+    DISPATCH_VECTOR_ADD(BFloat16, __nv_bfloat16)
+#endif
+
+    return a;
+}
+
 std::vector<at::Tensor> apply_rotary_pos_emb(at::Tensor& mixed_query,
                                              at::Tensor& key_layer,
                                              unsigned rotary_dim,
                                              unsigned offset,
                                              unsigned num_heads,
-                                             bool rotate_half,
-                                             bool rotate_every_two)
+                                             bool rotate_half)
 {
     auto query_cont = mixed_query.contiguous();
     auto key_cont = key_layer.contiguous();
 
     unsigned bsz = mixed_query.size(0);
     unsigned head_size = mixed_query.size(2) / num_heads;
     unsigned seq_len = mixed_query.size(1);
@@ -1661,130 +1856,103 @@
                                            (float*)key_cont.data_ptr(),
                                            head_size,
                                            seq_len,
                                            rotary_dim,
                                            offset,
                                            num_heads,
                                            bsz,
-                                           rotate_half,
-                                           rotate_every_two,
                                            InferenceContext::Instance().GetCurrentStream(),
-                                           InferenceContext::Instance().GetMaxTokenLenght());
+                                           InferenceContext::Instance().GetMaxTokenLength());
     else
         launch_apply_rotary_pos_emb<__half>((__half*)query_cont.data_ptr(),
                                             (__half*)key_cont.data_ptr(),
                                             head_size,
                                             seq_len,
                                             rotary_dim,
                                             offset,
                                             num_heads,
                                             bsz,
-                                            rotate_half,
-                                            rotate_every_two,
                                             InferenceContext::Instance().GetCurrentStream(),
-                                            InferenceContext::Instance().GetMaxTokenLenght());
+                                            InferenceContext::Instance().GetMaxTokenLength());
     return {query_cont, key_cont};
 }
 
-template <typename T>
-at::Tensor fused_gemm_gelu_int8(at::Tensor& input,
-                                at::Tensor& weight,
-                                at::Tensor& bias,
-                                const float epsilon,
-                                at::Tensor& q_scale,
-                                int groups,
-                                bool preLayerNorm)
-{
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    int bsz = input_cont.size(0) * input_cont.size(1);
-
-    quantized_gemm<T>(output, input_cont, weight, q_scale, groups, 0);
-    launch_bias_gelu((T*)output.data_ptr(),
-                     (T*)bias.data_ptr(),
-                     weight.size(1),
-                     bsz,
-                     InferenceContext::Instance().GetCurrentStream());
-
-    return output;
-}
+#define DISPATCH_MOE_RESIDUAL(T_TYPE, C_TYPE)                                           \
+    if (moe_res.scalar_type() == torch::T_TYPE) {                                       \
+        launch_moe_res_matmul<C_TYPE>((C_TYPE*)moe_res.data_ptr(),                      \
+                                      (C_TYPE*)coef.data_ptr(),                         \
+                                      (C_TYPE*)output.data_ptr(),                       \
+                                      M,                                                \
+                                      N,                                                \
+                                      InferenceContext::Instance().GetCurrentStream()); \
+    }
 
 at::Tensor moe_res_matmul(at::Tensor& moe_res, at::Tensor& coef, at::Tensor& output)
 {
     int M = moe_res.size(0) * moe_res.size(1);
     int N = moe_res.size(2);
     InferenceContext::Instance().SynchComm();
-    if (moe_res.scalar_type() == at::kFloat) {
-        launch_moe_res_matmul<float>((float*)moe_res.data_ptr(),
-                                     (float*)coef.data_ptr(),
-                                     (float*)output.data_ptr(),
-                                     M,
-                                     N,
-                                     at::cuda::getCurrentCUDAStream());
-    } else {
-        launch_moe_res_matmul<__half>((__half*)moe_res.data_ptr(),
-                                      (__half*)coef.data_ptr(),
-                                      (__half*)output.data_ptr(),
-                                      M,
-                                      N,
-                                      at::cuda::getCurrentCUDAStream());
-    }
+
+    DISPATCH_MOE_RESIDUAL(kFloat, float)
+    DISPATCH_MOE_RESIDUAL(kHalf, __half)
+#ifdef BF16_AVAILABLE
+    DISPATCH_MOE_RESIDUAL(kBFloat16, __nv_bfloat16)
+#endif
+
     return output;
 }
 
 void ds_release_workspace() { InferenceContext::Instance().release_workspace(); }
 
 bool ds_retake_workspace() { return InferenceContext::Instance().retake_workspace(); }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
     m.def("softmax_context_int8",
           &ds_softmax_context1<__half>,
           "DeepSpeed attention with int8 (CUDA)");
-    m.def("bias_geglu", &ds_bias_geglu, "DeepSpeed Bias GEGLU (CUDA)");
+
+    // The following functions handle type dispatching internally
+    m.def("gated_activation", &ds_gated_activation, "DeepSpeed Bias GEGLU (CUDA)");
     m.def("layer_norm", &ds_layer_norm, "DeepSpeed layer norm (CUDA)");
     m.def(
         "_layer_norm_residual", &ds_layer_norm_residual, "DeepSpeed layer norm + residual (CUDA)");
     m.def("layer_norm_residual_store_pre_ln_res",
           &ds_layer_norm_residual_store_pre_ln_res,
           "DeepSpeed layer norm + store pre Layernorm residual (CUDA)");
-    m.def("qkv_gemm_int8", &ds_qkv_gemm_int8<__half>, "DeepSpeed qkv gemm with int8 (CUDA)");
-    m.def("mlp_gemm_int8", &ds_mlp_gemm_int8<__half>, "DeepSpeed mlp with int8 (CUDA)");
-    m.def("vector_matmul_int8",
-          &ds_vector_matmul_int8<__half>,
-          "DeepSpeed vector-MM with int8 (CUDA)");
-    m.def("linear_layer_int8",
-          &ds_linear_layer_int8<__half>,
-          "DeepSpeed linear_layer with int8 (CUDA)");
+    m.def("rms_norm", &ds_rms_norm, "DeepSpeed rms norm (CUDA)");
+    m.def("pre_rms_norm", &ds_pre_rms_norm, "DeepSpeed pre rms norm (CUDA)");
+    m.def("_vector_add", &_vector_add, "DeepSpeed vector add (CUDA)");
     m.def("apply_rotary_pos_emb", &apply_rotary_pos_emb, "DeepSpeed mlp with fp16 (CUDA)");
     m.def("moe_res_matmul", &moe_res_matmul, "DeepSpeed moe residual matmul (CUDA)");
     m.def("reset_cache", &reset_cache, "Reset Cache for generation tasks");
     m.def("release_workspace", &ds_release_workspace, "DeepSpeed Release Workspace");
     m.def("retake_workspace", &ds_retake_workspace, "DeepSpeed Retake Workspace");
 
+    // The following functions are templated and need to be explicitly instantiated and bound
+    // to different python methods
 #define DEF_OPS(_name, _dtype)                                                                    \
     m.def("softmax_" #_name, &ds_softmax<_dtype>, "DeepSpeed SoftMax with " #_name " (CUDA)");    \
     m.def("softmax_context_" #_name,                                                              \
           &ds_softmax_context<_dtype>,                                                            \
-          "DeepSpeed attention with _name (CUDA)");                                               \
+          "DeepSpeed attention with " #_name " (CUDA)");                                          \
     m.def("bias_gelu_" #_name, &ds_bias_gelu<_dtype>, "DeepSpeed Gelu with " #_name " (CUDA)");   \
     m.def("bias_add_" #_name, &ds_bias_add<_dtype>, "DeepSpeed Bias Add with " #_name " (CUDA)"); \
     m.def("bias_relu_" #_name, &ds_bias_relu<_dtype>, "DeepSpeed ReLU with " #_name " (CUDA)");   \
     m.def("bias_residual_" #_name,                                                                \
           &ds_bias_residual<_dtype>,                                                              \
           "DeepSpeed residual-bias add with " #_name " (CUDA)");                                  \
     m.def("qkv_gemm_" #_name, &ds_qkv_gemm<_dtype>, "DeepSpeed qkv gemm with " #_name " (CUDA)"); \
+    m.def("rms_qkv_gemm_" #_name,                                                                 \
+          &ds_rms_qkv<_dtype>,                                                                    \
+          "DeepSpeed rms qkv gemm with " #_name " (CUDA)");                                       \
     m.def("mlp_gemm_" #_name, &ds_mlp_gemm<_dtype>, "DeepSpeed mlp with " #_name " (CUDA)");      \
+    m.def("rms_mlp_gemm_" #_name,                                                                 \
+          &ds_rms_mlp_gemm<_dtype>,                                                               \
+          "DeepSpeed rms mlp gemm with " #_name " (CUDA)");                                       \
     m.def("vector_matmul_" #_name,                                                                \
           &ds_vector_matmul<_dtype>,                                                              \
           "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
     m.def("linear_layer_" #_name,                                                                 \
           &ds_linear_layer<_dtype>,                                                               \
           "DeepSpeed linear_layer with " #_name " (CUDA)");                                       \
     m.def("fused_gemm_gelu_" #_name,                                                              \
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/relu.cu`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(relu(data_f + bias_f));
         }
@@ -56,16 +57,15 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_relu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_relu<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_RELU(T) \
+    template void launch_bias_relu<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_RELU(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_relu<__nv_bfloat16>(__nv_bfloat16*,
-                                              const __nv_bfloat16*,
-                                              int,
-                                              int,
-                                              cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_RELU(__nv_bfloat16)
 #endif
-template void launch_bias_relu<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_RELU(__half)
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/softmax.cu`

 * *Files 5% similar despite different names*

```diff
@@ -483,66 +483,37 @@
         } else if (iterations == 64) {
             LAUNCH_ATTN_SOFTMAX_V2(64);
         }
     } else
         throw std::runtime_error("Unsupport Seq_Length!");
 }
 
-template void launch_attn_softmax_v2(float* vals,
-                                     float* mask,
-                                     float* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+#define INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(T)                  \
+    template void launch_attn_softmax_v2(T* vals,              \
+                                         T* mask,              \
+                                         T* alibi,             \
+                                         float layer_scale,    \
+                                         bool triangular,      \
+                                         bool recompute,       \
+                                         bool local_attention, \
+                                         int window_size,      \
+                                         int batch_size,       \
+                                         int heads,            \
+                                         int num_seq,          \
+                                         int sequence_length,  \
+                                         int head_offset,      \
+                                         int mask_stride,      \
+                                         int mp_size,          \
+                                         cudaStream_t stream);
 
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(float);
 #ifdef BF16_AVAILABLE
-template void launch_attn_softmax_v2(__nv_bfloat16* vals,
-                                     __nv_bfloat16* mask,
-                                     __nv_bfloat16* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(__nv_bfloat16);
 #endif
-
-template void launch_attn_softmax_v2(__half* vals,
-                                     __half* mask,
-                                     __half* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(__half);
 
 #define DEF_ATTN_SOFTMAX_V2_HALF(_iter)                                           \
     template __global__ void attn_softmax_v2<__half, _iter>(__half * vals,        \
                                                             __half * mask,        \
                                                             __half * alibi,       \
                                                             float layer_scale,    \
                                                             bool triangular,      \
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.3/csrc/transformer/inference/csrc/transform.cu`

 * *Files 4% similar despite different names*

```diff
@@ -236,51 +236,37 @@
                                                                 rotary_dim >> 3,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
 
+#define INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(T)             \
+    template void launch_bias_add_transform_0213<T>(T*,           \
+                                                    T*,           \
+                                                    T*,           \
+                                                    const T*,     \
+                                                    const T*,     \
+                                                    int,          \
+                                                    int,          \
+                                                    unsigned,     \
+                                                    int,          \
+                                                    int,          \
+                                                    int,          \
+                                                    int,          \
+                                                    bool,         \
+                                                    bool,         \
+                                                    cudaStream_t, \
+                                                    int,          \
+                                                    int)
+
 #ifdef BF16_AVAILABLE
-template void launch_bias_add_transform_0213(__nv_bfloat16* output,
-                                             __nv_bfloat16* k_cache,
-                                             __nv_bfloat16* v_cache,
-                                             const __nv_bfloat16* vals,
-                                             const __nv_bfloat16* bias,
-                                             int batch_size,
-                                             int seq_length,
-                                             unsigned seq_offset,
-                                             int all_tokens,
-                                             int hidden_dim,
-                                             int heads,
-                                             int rotary_dim,
-                                             bool rotate_half,
-                                             bool rotate_every_two,
-                                             cudaStream_t stream,
-                                             int trans_count,
-                                             int max_out_tokens);
+INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(__nv_bfloat16);
 #endif
-
-template void launch_bias_add_transform_0213(__half* output,
-                                             __half* k_cache,
-                                             __half* v_cache,
-                                             const __half* vals,
-                                             const __half* bias,
-                                             int batch_size,
-                                             int seq_length,
-                                             unsigned seq_offset,
-                                             int all_tokens,
-                                             int hidden_dim,
-                                             int heads,
-                                             int rotary_dim,
-                                             bool rotate_half,
-                                             bool rotate_every_two,
-                                             cudaStream_t stream,
-                                             int trans_count,
-                                             int max_out_tokens);
+INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(__half);
 
 // Bias add
 
 __global__ void pad_add_transform_0213(float* output,
                                        const float* vals,
                                        int hidden_dim,
                                        int seq_length,
@@ -364,36 +350,23 @@
     hidden_dim >>= 3;
     dim3 block_dim((padded_head_size >> 3), heads, 2);
     dim3 grid_dim(batch_size, padded_seq_len / 2);
     pad_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(
         output, vals, hidden_dim, seq_length, padded_seq_len, heads, padded_head_size >> 3);
 }
 
+#define INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(T) \
+    template void launch_pad_add_transform_0213<T>(         \
+        T*, const T*, int, int, int, int, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(__half);
 #ifdef BF16_AVAILABLE
-template void launch_pad_add_transform_0213(__nv_bfloat16* output,
-                                            const __nv_bfloat16* vals,
-                                            int batch_size,
-                                            int hidden_dim,
-                                            int seq_length,
-                                            int padded_seq_len,
-                                            int heads,
-                                            int padded_head_size,
-                                            cudaStream_t stream);
+INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(__nv_bfloat16);
 #endif
 
-template void launch_pad_add_transform_0213(__half* output,
-                                            const __half* vals,
-                                            int batch_size,
-                                            int hidden_dim,
-                                            int seq_length,
-                                            int padded_seq_len,
-                                            int heads,
-                                            int padded_head_size,
-                                            cudaStream_t stream);
-
 // Bias add
 template <typename T>
 __global__ void bias_add_transform_0213(T* output,
                                         const T* vals,
                                         const T* bias,
                                         int hidden_dim,
                                         int seq_length,
@@ -567,30 +540,14 @@
         int iter_offset =
             (iter_row % blockDim.y) * d2_out_stride + (iter_row / blockDim.y) * matrix_stride;
         output_vec[out_index + iter_offset] =
             in_data[iter_row * d2_stride + d3 + (d2 % 2) * (d1_stride * blockDim.z)];
     }
 }
 
-template __global__ void bias_add_transform_0213_v2(__half* output,
-                                                    const __half* vals,
-                                                    const __half* bias,
-                                                    int hidden_dim,
-                                                    int seq_length,
-                                                    int heads);
-
-#ifdef BF16_AVAILABLE
-template __global__ void bias_add_transform_0213_v2(__nv_bfloat16* output,
-                                                    const __nv_bfloat16* vals,
-                                                    const __nv_bfloat16* bias,
-                                                    int hidden_dim,
-                                                    int seq_length,
-                                                    int heads);
-#endif
-
 template <typename T>
 __global__ void transform4d_0213(T* out,
                                  const T* in,
                                  int heads,
                                  int seq_length,
                                  int hidden_dim,
                                  int head_ext);
@@ -703,28 +660,14 @@
 #pragma unroll
     for (int iter = 0; iter < 2; iter++) {
         int iter_id = iter * iteration_stride + iter_index;
         out_vec[output_offset + iter_id] = in_data[iter_id];
     }
 }
 
-#ifdef BF16_AVAILABLE
-template __global__ void transform4d_0213_v2(__nv_bfloat16* out,
-                                             const __nv_bfloat16* in,
-                                             int heads,
-                                             int seq_length,
-                                             int hidden_dim);
-#endif
-
-template __global__ void transform4d_0213_v2(__half* out,
-                                             const __half* in,
-                                             int heads,
-                                             int seq_length,
-                                             int hidden_dim);
-
 // 3 * [B A S N] - > [B S C*H]
 template <>
 void launch_transform4d_0213<float>(float* out,
                                     const float* in,
                                     int batch_size,
                                     int heads,
                                     int seq_length,
@@ -753,26 +696,14 @@
     int head_ext = (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 grid_dims(batch_size, trans_count, (seq_length * head_ext));
     dim3 block_dims(hidden_dim / heads, (heads / head_ext));
     transform4d_0213<<<grid_dims, block_dims, 0, stream>>>(
         out, in, heads, seq_length, hidden_dim, head_ext);
 }
 
+#define INSTANTIATE_2B_LAUNCH_TRANSFORM4D(T) \
+    template void launch_transform4d_0213<T>(T*, const T*, int, int, int, int, cudaStream_t, int);
+
+INSTANTIATE_2B_LAUNCH_TRANSFORM4D(__half)
 #ifdef BF16_AVAILABLE
-template void launch_transform4d_0213(__nv_bfloat16* out,
-                                      const __nv_bfloat16* in,
-                                      int batch_size,
-                                      int heads,
-                                      int seq_length,
-                                      int hidden_dim,
-                                      cudaStream_t stream,
-                                      int trans_count);
+INSTANTIATE_2B_LAUNCH_TRANSFORM4D(__nv_bfloat16)
 #endif
-
-template void launch_transform4d_0213(__half* out,
-                                      const __half* in,
-                                      int batch_size,
-                                      int heads,
-                                      int seq_length,
-                                      int hidden_dim,
-                                      cudaStream_t stream,
-                                      int trans_count);
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         size_t workSpaceSize = ((external_cache ? (activation_size + temp_size)
                                                 : (activation_size + temp_size + cache_size))) *
                                _max_seq_len * elem_size;
         temp_size *= _max_seq_len * elem_size;
 
         if (_max_seq_len < min_out_tokens) {
             printf(
-                "Allocatable workspace available (%d tokens) is less than minimum requested "
+                "Allocatable workspace available (%ld tokens) is less than minimum requested "
                 "workspace (%d tokens)\n",
                 _max_seq_len,
                 min_out_tokens);
             throw std::runtime_error("Workspace can't be allocated, not enough memory");
         }
 
         if (!_workspace) {
@@ -171,15 +171,15 @@
                    _free_memory_size,
                    total_size);
             throw std::runtime_error("Workspace is null.");
         }
         _workSpaceSize = workSpaceSize;
         _attention_unfused_workspace_offset = workSpaceSize - temp_size;
     }
-    inline size_t GetMaxTokenLenght() const { return _max_seq_len; }
+    inline size_t GetMaxTokenLength() const { return _max_seq_len; }
 
     cudaEvent_t GetCompEvent(int id) { return id == 1 ? _comp1_event : _comp2_event; }
 
     size_t get_workspace_size() const { return _workSpaceSize; }
     void* GetWorkSpace() { return _workspace; }
     void* GetAttentionUnfusedWorkspace()
     {
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 // DeepSpeed Team
 
 #pragma once
 
 #include <assert.h>
 #include <cublas_v2.h>
 #include <cuda.h>
+#ifdef BF16_AVAILABLE
 #include <cuda_bf16.h>
+#endif
 #include <cuda_fp16.h>
 #include <cuda_runtime.h>
 #ifndef __HIP_PLATFORM_HCC__
 #include <mma.h>
 #endif
 #include <stdio.h>
 
@@ -24,44 +26,47 @@
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const float* A,
                    const float* B,
                    float* C,
-                   rocblas_gemm_algo algo)
+                   rocblas_gemm_algo algo,
+                   int b_stride = -1)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const float* A,
                    const float* B,
                    float* C,
-                   cublasGemmAlgo_t algo)
+                   cublasGemmAlgo_t algo,
+                   int b_stride = -1)
 #endif
 {
+    const int ldb = (b_stride == -1) ? ((transb == CUBLAS_OP_N) ? k : n) : b_stride;
 #ifdef __HIP_PLATFORM_HCC__
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
                                             n,
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
                                             rocblas_datatype_f32_r,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
                                             rocblas_datatype_f32_r,
-                                            (transb == rocblas_operation_none) ? k : n,
+                                            ldb,
                                             (const void*)beta,
                                             C,
                                             rocblas_datatype_f32_r,
                                             m,
                                             C,
                                             rocblas_datatype_f32_r,
                                             m,
@@ -78,15 +83,15 @@
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
                                          CUDA_R_32F,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
                                          CUDA_R_32F,
-                                         (transb == CUBLAS_OP_N) ? k : n,
+                                         ldb,
                                          (const void*)beta,
                                          C,
                                          CUDA_R_32F,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
@@ -116,30 +121,33 @@
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const T* A,
                    const T* B,
                    T* C,
-                   rocblas_gemm_algo algo)
+                   rocblas_gemm_algo algo,
+                   int b_stride = -1)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const T* A,
                    const T* B,
                    T* C,
-                   cublasGemmAlgo_t algo)
+                   cublasGemmAlgo_t algo,
+                   int b_stride = -1)
 #endif
 {
+    const int ldb = (b_stride == -1) ? ((transb == CUBLAS_OP_N) ? k : n) : b_stride;
 #ifdef __HIP_PLATFORM_HCC__
     constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
                                                                      : rocblas_datatype_bf16_r;
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
@@ -147,15 +155,15 @@
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
                                             rocblas_dtype_16,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
                                             rocblas_dtype_16,
-                                            (transb == rocblas_operation_none) ? k : n,
+                                            ldb,
                                             (const void*)beta,
                                             (void*)C,
                                             rocblas_dtype_16,
                                             m,
                                             (void*)C,
                                             rocblas_dtype_16,
                                             m,
@@ -173,15 +181,15 @@
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
                                          cublas_dtype_16,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
                                          cublas_dtype_16,
-                                         (transb == CUBLAS_OP_N) ? k : n,
+                                         ldb,
                                          (const void*)beta,
                                          (void*)C,
                                          cublas_dtype_16,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
```

### Comparing `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,21 @@
 void launch_bias_gelu(T* input,
                       const T* bias,
                       int intermediate_size,
                       int batch_size,
                       cudaStream_t stream);
 
 template <typename T>
-void launch_fused_bias_geglu(T* output,
+void launch_gated_activation(T* output,
                              const T* activation,
                              const T* bias,
                              int rows,
+                             int output_stride,
                              int elems_per_row,
+                             bool use_gelu,
                              cudaStream_t stream);
 
 // Fused bias add with relu activation
 template <typename T>
 void launch_bias_relu(T* input,
                       const T* bias,
                       int intermediate_size,
@@ -114,14 +116,25 @@
                                                const T* beta,
                                                float epsilon,
                                                int rows,
                                                int elems_per_row,
                                                cudaStream_t stream);
 
 template <typename T>
+void launch_rms_norm(T* norm_output,
+                     T* res_output,
+                     const T* vals,
+                     const T* residual,
+                     const T* gamma,
+                     float epsilon,
+                     int rows,
+                     int elems_per_row,
+                     cudaStream_t stream);
+
+template <typename T>
 void launch_dequantize(T* output,
                        const int8_t* input,
                        const float* qscale,
                        unsigned output_size,
                        unsigned hidden_dim,
                        unsigned groups,
                        unsigned merge_count,
@@ -151,16 +164,14 @@
                                  T* key_layer,
                                  unsigned head_size,
                                  unsigned seq_len,
                                  unsigned rotary_dim,
                                  unsigned offset,
                                  unsigned num_heads,
                                  unsigned batch,
-                                 bool rotate_half,
-                                 bool rotate_every_two,
                                  cudaStream_t stream,
                                  int max_out_tokens);
 
 template <typename T>
 void launch_moe_res_matmul(T* residual,
                            T* coef,
                            T* mlp_out,
@@ -220,7 +231,15 @@
                                    int batch_size,
                                    int hidden_dim,
                                    int seq_length,
                                    int padded_seq_len,
                                    int heads,
                                    int padded_head_size,
                                    cudaStream_t stream);
+
+template <typename T>
+void launch_vector_add(T* out,
+                       const T* a,
+                       const T* b,
+                       float gamma,
+                       int num_elems,
+                       cudaStream_t stream);
```

### Comparing `deepspeed-0.9.2/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.3/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.3/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/__init__.py` & `deepspeed-0.9.3/deepspeed/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/accelerator/abstract_accelerator.py` & `deepspeed-0.9.3/deepspeed/accelerator/abstract_accelerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class DeepSpeedAccelerator(ABC):
 
     def __init__(self):
         self._name = None
         self._communication_backend_name = None
 
+    @abc.abstractmethod
+    def is_synchronized_device(self):
+        ...
+
     # Device APIs
     @abc.abstractmethod
     def device_name(self, device_index):
         ...
 
     @abc.abstractmethod
     def device(self, device_index):
```

### Comparing `deepspeed-0.9.2/deepspeed/accelerator/cuda_accelerator.py` & `deepspeed-0.9.3/deepspeed/accelerator/cuda_accelerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,16 @@
 
 class CUDA_Accelerator(DeepSpeedAccelerator):
 
     def __init__(self):
         self._name = 'cuda'
         self._communication_backend_name = 'nccl'
 
-        # begin initialize for create_op_builder()
-        # put all valid class name <--> class type mapping into class_dict
-        op_builder_dir = self.op_builder_dir()
-        op_builder_module = importlib.import_module(op_builder_dir)
-        for _, module_name, _ in pkgutil.iter_modules([os.path.dirname(op_builder_module.__file__)]):
-            # avoid self references
-            if module_name != 'all_ops' and module_name != 'builder':
-                module = importlib.import_module("{}.{}".format(op_builder_dir, module_name))
-                for member_name in module.__dir__():
-                    if member_name.endswith(
-                            'Builder'
-                    ) and member_name != "OpBuilder" and member_name != "CUDAOpBuilder" and member_name != "TorchCPUOpBuilder":  # avoid abstract classes
-                        if not member_name in self.class_dict:
-                            self.class_dict[member_name] = getattr(module, member_name)
-        # end initialize for create_op_builder()
+    def is_synchronized_device(self):
+        return False
 
     # Device APIs
     def device_name(self, device_index=None):
         if device_index == None:
             return 'cuda'
         return 'cuda:{}'.format(device_index)
 
@@ -231,25 +218,48 @@
             return "op_builder"
         except ImportError:
             return "deepspeed.ops.op_builder"
 
     # dict that holds class name <--> class type mapping i.e.
     # 'AsyncIOBuilder': <class 'op_builder.async_io.AsyncIOBuilder'>
     # this dict will be filled at init stage
-    class_dict = {}
+    class_dict = None
+
+    def _lazy_init_class_dict(self):
+        if self.class_dict != None:
+            return
+        else:
+            self.class_dict = {}
+            # begin initialize for create_op_builder()
+            # put all valid class name <--> class type mapping into class_dict
+            op_builder_dir = self.op_builder_dir()
+            op_builder_module = importlib.import_module(op_builder_dir)
+            for _, module_name, _ in pkgutil.iter_modules([os.path.dirname(op_builder_module.__file__)]):
+                # avoid self references
+                if module_name != 'all_ops' and module_name != 'builder' and module_name != 'cpu':
+                    module = importlib.import_module("{}.{}".format(op_builder_dir, module_name))
+                    for member_name in module.__dir__():
+                        if member_name.endswith(
+                                'Builder'
+                        ) and member_name != "OpBuilder" and member_name != "CUDAOpBuilder" and member_name != "TorchCPUOpBuilder":  # avoid abstract classes
+                            if not member_name in self.class_dict:
+                                self.class_dict[member_name] = getattr(module, member_name)
+            # end initialize for create_op_builder()
 
     # create an instance of op builder and return, name specified by class_name
     def create_op_builder(self, class_name):
+        self._lazy_init_class_dict()
         if class_name in self.class_dict:
             return self.class_dict[class_name]()
         else:
             return None
 
     # return an op builder class, name specified by class_name
     def get_op_builder(self, class_name):
+        self._lazy_init_class_dict()
         if class_name in self.class_dict:
             return self.class_dict[class_name]
         else:
             return None
 
     def build_extension(self):
         from torch.utils.cpp_extension import BuildExtension
```

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/autotuner.py` & `deepspeed-0.9.3/deepspeed/autotuning/autotuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     def __init__(self, args, active_resources):
         self.args = args
         self.selected_exp_dir = None
 
         assert tabulate is not None, "Missing required package `tabulate`, please install with `pip install deepspeed[autotuning]`."
 
-        logger.debug(f"autotunning args={args}")
+        logger.debug(f"autotuning args={args}")
 
         self.user_config = self._get_user_config(args.user_args)
         assert self.user_config is not None, "DeepSpeed configuration is not provided"
 
         self.autotuning_config = DeepSpeedAutotuningConfig(self.user_config)
         if self.user_config[AUTOTUNING]:
             if AUTOTUNING_EXPS_DIR in self.user_config[AUTOTUNING].keys():
@@ -97,15 +97,15 @@
         assert self.exp_num_gpus <= self.rm.num_gpus_per_node, "num_gpus in the autotuning configuration must not be less than the --num_gpus value in the train script if any"
         assert self.exp_num_nodes <= len(
             self.rm.nodes
         ), "num_nodes in the autotuning configuration must not be less than the --num_nodes value in the train script if any"
 
         self.records = {}
         self.optimal_cmd = None
-        self.optmal_ds_config = None
+        self.optimal_ds_config = None
 
         self.mlflow_parent_id = None
 
     def print_tuning_results(self):
         """Print the autotuning results in tabular format.
         """
         best_space_records = self.get_best_space_records()
@@ -427,15 +427,14 @@
         self.activation_mem = self.get_activation_memory_per_gpu()
         logger.info(
             f"The model requires at least {memory_to_string(self.activation_mem, postfix='B')} activation memory for micro batch size 1."
         )
 
         #TODO: FIX THIS
         stage = self.user_config.get(ZERO_OPTIMIZATION, {}).get(ZERO_OPTIMIZATION_STAGE, "all")
-        stage = "all"
         user_zero_stages = [stage] if not isinstance(stage, list) else stage
         logger.info(f"User-defined zero stages are {stage}.")
 
         mbs = 0
         max_mbs = 0
         metric_val = 0
 
@@ -634,15 +633,15 @@
         else:
             best_metric_val = fast_best_metric_val
             best_mbs = fast_best_mbs
 
         logger.info(f"End tuning for space: {tuning_space_name}")
         return max_micro_batch_size, best_mbs, best_metric_val
 
-    def get_plauteu_mbs(self, tuning_space_name):
+    def get_plateau_mbs(self, tuning_space_name):
         if tuning_space_name not in self.records:
             return 0
         space_records = self.records[tuning_space_name]
         sorted_space_records = sorted(space_records, key=lambda x: x[0][DS_CONFIG][TRAIN_MICRO_BATCH_SIZE_PER_GPU])
         prev_metric_val = None
         prev_micro_batch_size = 0
         for (exp, metric_val, _) in sorted_space_records:
@@ -658,15 +657,15 @@
         return plateau_mbs
 
     def get_model_num_params(self):
         if self.model_info and "num_params" in self.model_info:
             return self.model_info["num_params"]
 
     def model_info_profile_run(self):
-        """Does a model information profling experiment that collects the number of model parameters and activation memory.\
+        """Does a model information profiling experiment that collects the number of model parameters and activation memory.\
             The experiment produces a "profile_model_info" folder under self.results_dir.
         Returns:
             [dict]: a model information dictionary, e.g., {"num_params": 335144976, "trainable_num_params": 335144976, "activation_mem_per_gpu": 324358144, "rank": 0}
         """
         logger.info("Starting model info profile run.")
         model_info = self.autotuning_config.model_info
         if model_info and MODEL_INFO_NUM_PARAMS in model_info:
@@ -798,15 +797,15 @@
                 logger.info(f"micro batch size = {mbs} was not run successfully")
 
         self.rm.clear()
 
         if tuning_micro_batch_sizes_overwritten:
             return tuning_micro_batch_sizes
 
-        # in a auto-detected tuning_micro_batch_sizs list, max_micro_batch_size might not be performant as the memory consumption is close to max
+        # in a auto-detected tuning_micro_batch_sizes list, max_micro_batch_size might not be performant as the memory consumption is close to max
         # try smaller values while gas stays the same
         # if finding a more performant mbs value, use it to replace max_micro_batch_size in the list
         min_micro_batch_size_with_same_gas = (tuning_micro_batch_sizes[-2] +
                                               1) if len(tuning_micro_batch_sizes) > 1 else min_micro_batch_size
 
         prev_best_metric_val = max_micro_batch_size_metric_val
         prev_best_mbs = max_micro_batch_size
@@ -1089,22 +1088,22 @@
 
             cmd_path = os.path.join(self.results_dir, "cmd_optimal.txt")
             with open(cmd_path, "w") as fd:
                 fd.write(" ".join(cmd))
                 fd.write("\n")
                 fd.flush()
             self.optimal_cmd = cmd
-            self.optmal_ds_config = ds_config
+            self.optimal_ds_config = ds_config
             logger.info(
                 f"Wrote the optimal DeepSpeed configuration found by autotuning to {ds_config_path}, and the corresponding DeepSpeed command to {cmd_path}"
             )
 
     def run_after_tuning(self):
         """ Launches the training with the optimal DeepSpeed configuration found through the autotuning process.
-            "ds_config_optimal.json" describing the optmimal DeepSpeed configuration as well the command used to launch training "cmd_optimal.txt" are saved to self.results_dir.
+            "ds_config_optimal.json" describing the optimal DeepSpeed configuration as well the command used to launch training "cmd_optimal.txt" are saved to self.results_dir.
         """
         if self.optimal_cmd:
             result = subprocess.Popen(self.optimal_cmd)
             result.wait()
 
             logger.info(f"Done running with the optimal DeepSpeed configuration using {self.optimal_cmd}")
         else:
```

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/config.py` & `deepspeed-0.9.3/deepspeed/autotuning/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/constants.py` & `deepspeed-0.9.3/deepspeed/autotuning/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 #########################################
-# autotunner implementation constants
+# autotuner implementation constants
 #########################################
 
 import os
 
 DEFAULT_TEMPLATE_PATH_ZERO_0 = os.path.join(os.path.dirname(os.path.realpath(__file__)), "config_templates",
                                             "template_zero0.json")
 DEFAULT_TEMPLATE_PATH_ZERO_1 = os.path.join(os.path.dirname(os.path.realpath(__file__)), "config_templates",
@@ -113,28 +113,28 @@
 }
 '''
 MODEL_INFO = "model_info"
 MODEL_INFO_PROFILE = "profile"
 MODEL_INFO_PROFILE_DEFAULT = False
 MODEL_INFO_NUM_PARAMS = "num_params"
 MODEL_INFO_NUM_PARAMS_DEFAULT = None
-MODEL_INFO_HIDDEN_SIZE = "hideen_size"
+MODEL_INFO_HIDDEN_SIZE = "hidden_size"
 MODEL_INFO_HIDDEN_SIZE_DEFAULT = None
 MODEL_INFO_NUM_LAYERS = "num_layers"
 MODEL_INFO_NUM_LAYERS_DEFAULT = None
 
 MODEL_INFO_KEY_DEFAULT_DICT = {
     MODEL_INFO_PROFILE: MODEL_INFO_PROFILE_DEFAULT,
     MODEL_INFO_NUM_PARAMS: MODEL_INFO_NUM_PARAMS_DEFAULT,
     MODEL_INFO_HIDDEN_SIZE: MODEL_INFO_HIDDEN_SIZE_DEFAULT,
     MODEL_INFO_NUM_LAYERS: MODEL_INFO_NUM_LAYERS_DEFAULT
 }
 
 #########################################
-# autotunner search space constants
+# autotuner search space constants
 #########################################
 
 DEFAULT_HF_CONFIG = {
     "train_batch_size": "auto",
     "train_micro_batch_size_per_gpu": "auto",
     "gradient_accumulation_steps": "auto",
 }
```

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/scheduler.py` & `deepspeed-0.9.3/deepspeed/autotuning/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/tuner/base_tuner.py` & `deepspeed-0.9.3/deepspeed/autotuning/tuner/base_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def update(self):
         """"Update the tuner with what configurations have been evaluated and their performance results"""
 
     def tune(self, sample_size=1, n_trials=1000, early_stopping=None):
         i = 0
         try:
             while i < n_trials and self.has_next():
-                # Select the next batch of configuratiosn for evaluation
+                # Select the next batch of configuration for evaluation
                 sampled_exps = self.next_batch(sample_size)
                 # Generate experiments for measurement of performance
                 exp_paths = write_experiments(sampled_exps, self.rm.exps_dir)
                 self.rm.schedule_experiments(exp_paths)
                 self.rm.run()
                 exp, metric_val = self.rm.parse_results(self.metric)
                 if self.best_exp == None or self.best_metric_val == None or (metric_val
@@ -64,9 +64,9 @@
                 if early_stopping and i >= self.best_iter + early_stopping:
                     logger.info(
                         f"Tuner early stopped at iteration {i}. Best iteration is {self.best_iter}. Early stopping threshold is {early_stopping}"
                     )
                     break
             return i
         except:
-            logger.info("Tunner Error:", sys.exc_info()[0])
+            logger.info("Tuner Error:", sys.exc_info()[0])
             return i
```

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/tuner/cost_model.py` & `deepspeed-0.9.3/deepspeed/autotuning/tuner/cost_model.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/tuner/index_based_tuner.py` & `deepspeed-0.9.3/deepspeed/autotuning/tuner/index_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/tuner/model_based_tuner.py` & `deepspeed-0.9.3/deepspeed/autotuning/tuner/model_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/tuner/utils.py` & `deepspeed-0.9.3/deepspeed/autotuning/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/autotuning/utils.py` & `deepspeed-0.9.3/deepspeed/autotuning/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         prune_config(config, ignored_keys)
         pruned_list.append(config)
 
     return remove_dupe_dicts(pruned_list)
 
 
 def get_tuning_keys(tuning_space: dict):
-    """Outputs the list of tunnable parameters in the tuning space dict.
+    """Outputs the list of tunable parameters in the tuning space dict.
 
     Args:
         tuning_space (dict): a configuration dictionary containing tunable parameters as lists of values.
 
     Returns:
         A list of strings
     """
```

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/__init__.py` & `deepspeed-0.9.3/deepspeed/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/constants.py` & `deepspeed-0.9.3/deepspeed/checkpoint/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/deepspeed_checkpoint.py` & `deepspeed-0.9.3/deepspeed/checkpoint/deepspeed_checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,19 +94,19 @@
 
     def show_tp_embedding_map(self):
         self._dump_mapping(self.tp_to_embedding_map, 'tp_to_embedding_layers')
 
     def show_tp_final_norm_map(self):
         self._dump_mapping(self.tp_to_final_norm_map, 'tp_to_final_norm_layers')
 
-    def show_pp_tranformer_map(self):
-        self._dump_mapping(self.pp_to_transformer_map, 'pp_to_tranformer_layers')
+    def show_pp_transformer_map(self):
+        self._dump_mapping(self.pp_to_transformer_map, 'pp_to_transformer_layers')
 
     def show_transformer_file_map(self):
-        self._dump_mapping(self.transformer_file_map, 'rank_to_tranformer_files')
+        self._dump_mapping(self.transformer_file_map, 'rank_to_transformer_files')
 
     def _build_global_state(self):
         sd = torch.load(self.mp_rank_files[0], map_location=torch.device('cpu'))
         self.global_state[ITERATION_KEY] = sd.get(ITERATION_KEY, 0)
         self.global_state[ARGS_KEY] = sd.get(ARGS_KEY, None)
 
     def get_zero_checkpoint_state(self, pp_index, tp_index, dp_index) -> dict:
```

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/reshape_3d_utils.py` & `deepspeed-0.9.3/deepspeed/checkpoint/reshape_3d_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/reshape_meg_2d.py` & `deepspeed-0.9.3/deepspeed/checkpoint/reshape_meg_2d.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/reshape_utils.py` & `deepspeed-0.9.3/deepspeed/checkpoint/reshape_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/universal_checkpoint.py` & `deepspeed-0.9.3/deepspeed/checkpoint/universal_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/checkpoint/zero_checkpoint.py` & `deepspeed-0.9.3/deepspeed/checkpoint/zero_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/comm/backend.py` & `deepspeed-0.9.3/deepspeed/comm/backend.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/comm/comm.py` & `deepspeed-0.9.3/deepspeed/comm/comm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 """
     DeepSpeed Communication Package: deepspeed.comm
     deepspeed.comm
-        -- import and use deepspeeed.ops.comm
+        -- import and use deepspeed.ops.comm
         -- use torch.distributed directly if both this package and torch.distributed use the same NCCL version
         -- use custom collectives
             -- can either use torch.dist or ds.ops.comm?
         Note: the old 1-bit compressed allreduce variants that resided in deepspeed.runtime.comm will be moved here as well.
     deepspeed.comm API
         -- must be kept fully compatible (same signatures) as torch.dist API to ensure backward/cross-framework compatibility.
         -- e.g. if a client code used
@@ -17,60 +17,56 @@
             instead of
             import torch.distributed as dist
             The code should work without breaking any of the public torch.distributed functionality
     Future:
         -- deepspeed groups API should be brought into ds.comm
 """
 
-from enum import Enum
 import torch
 import os
 
 from ..constants import TORCH_DISTRIBUTED_DEFAULT_PORT, default_pg_timeout
 from .constants import *
+from .reduce_op import *
 from deepspeed.accelerator import get_accelerator
-
-
-class ReduceOp(Enum):
-    SUM = 0
-    PRODUCT = 1
-    MIN = 2
-    MAX = 3
-    BAND = 4
-    BOR = 5
-    BXOR = 6
-    AVG = 7
-    UNUSED = 8
-
+from deepspeed.comm.ccl import CCLBackend
 
 from deepspeed.utils.comms_logging import CommsLogger
 from deepspeed.utils import timer, get_caller_func
 from deepspeed.comm.torch import TorchBackend
 
 from deepspeed import utils
 from datetime import timedelta
 
 # Current deepspeed.comm backend (cdb) global object for simple access by client code
-use_ds_backend = False
 cdb = None
 
 # Create global timer for ops
 timers = timer.SynchronizedWallClockTimer()
 timer_summary = {}
 
 comms_logger = CommsLogger()
 
 # Maintain objects of all initialized ds backends and assign them using the API functions in this file
 nccl_backend = None
 mpi_backend = None
+ccl_backend = None
 
 # This should be set here so all rank/size information from the launcher can be propagated
 from deepspeed.comm.utils import *
 
 
+class ProcessGroup():
+
+    def __init__(self, comm_id, ranks=[]):
+        self.ranks = ranks
+        self.comm_id = comm_id
+        self.size = len(ranks)
+
+
 def _configure_using_config_file(config):
     if config.comms_logger_enabled:
         comms_logger.configure(config)
 
 
 def configure(
     deepspeed_config=None,
@@ -139,26 +135,32 @@
 
 # For compatibility with torch distributed's init_process_group, we shall retain the signature from PyTorch code.
 # DeepSpeed NCCL/MPI backend may not need all these params as we will have our own implementation.
 # Please read full torch.distributed API docs from https://pytorch.org/docs/stable/distributed.html
 
 
 # UNUSED: Future helper function to initialize DS backends
-def init_deepspeed_backend(ds_backend):
+def init_deepspeed_backend(ds_backend, timeout, init_method):
     global cdb
     global nccl_backend
     global mpi_backend
-    global use_ds_backend
+    global ccl_backend
+
+    rank = int(os.environ["RANK"])
+    size = int(os.environ["WORLD_SIZE"])
 
     if ds_backend == NCCL_BACKEND:
         utils.logger.warn("NCCL backend in DeepSpeed not yet implemented")
     elif ds_backend == MPI_BACKEND:
         utils.logger.warn("MPI backend in DeepSpeed not yet implemented")
     elif ds_backend == GLOO_BACKEND:
         utils.logger.warn("Gloo backend in DeepSpeed not yet implemented")
+    elif ds_backend == CCL_BACKEND:
+        ccl_backend = CCLBackend(rank=rank, world_size=size, timeout=timeout, init_method=init_method)
+        utils.logger.info(f"Initialize {ds_backend} backend")
     else:
         utils.logger.warn(f"DeepSpeed does not support {ds_backend} backend")
 
 
 def is_initialized():
     #assert cdb is not None, 'DeepSpeed backend not set, please initialize it using init_process_group()'
     if cdb is None:
@@ -185,34 +187,31 @@
 
     # TODO: load other ops. Clients including deepspeed itself should use deepspeed.comm to import
     # any communication related primitives from this package.
     # use hasattr(deepspeed.csrc.ops, "_comm") or something
     return True
 
 
-def set_backend(backend_name):
-    if not use_ds_backend:
-        utils.logger.error(
-            "DeepSpeed communication backend is required. Please use deepspeed.comm.init_distributed(backend, use_deepspeed=True) to use this functionality"
-        )
-        raise RuntimeError('Error: Custom DeepSpeed backend called without initializing DeepSpeed distributed.')
-
+def set_backend():
     global cdb
     global nccl_backend
     global mpi_backend
+    global ccl_backend
+
+    backend_name = get_accelerator().communication_backend_name()
 
-    try:
-        if backend_name == NCCL_BACKEND:
-            if nccl_backend is not None and nccl_backend.is_initialized():
-                cdb = nccl_backend
-        elif backend_name == MPI_BACKEND:
-            if mpi_backend is not None and mpi_backend.is_initialized():
-                cdb = mpi_backend
-    except Exception as inst:
-        print(inst)
+    if backend_name == NCCL_BACKEND:
+        if nccl_backend is not None and nccl_backend.is_initialized():
+            cdb = nccl_backend
+    elif backend_name == MPI_BACKEND:
+        if mpi_backend is not None and mpi_backend.is_initialized():
+            cdb = mpi_backend
+    elif backend_name == CCL_BACKEND:
+        if ccl_backend is not None and ccl_backend.is_initialized():
+            cdb = ccl_backend
 
 
 @timed_op
 def broadcast(tensor, src, group=None, async_op=False, prof=False, log_name='broadcast', debug=get_caller_func()):
     global cdb
     return cdb.broadcast(tensor=tensor, src=src, group=group, async_op=async_op)
 
@@ -253,15 +252,15 @@
                                      group=group,
                                      async_op=async_op,
                                      prof=prof,
                                      debug=debug)
     else:
         if get_rank() == 0:
             utils.logger.warning_once("unable to find torch.distributed.reduce_scatter_tensor. will fall back to "
-                                      "torch.distributed.all_gather which will result in suboptimal performance. "
+                                      "torch.distributed.reduce_scatter which will result in suboptimal performance. "
                                       "please consider upgrading your pytorch installation.")
         input_tensor_lst = list(torch.chunk(tensor, cdb.get_world_size(group)))
         return reduce_scatter(output_tensor,
                               input_tensor_lst,
                               op=op,
                               group=group,
                               async_op=async_op,
@@ -388,15 +387,15 @@
     global cdb
     return cdb.scatter(tensor=tensor, scatter_list=scatter_list, src=src, group=group, async_op=async_op)
 
 
 @timed_op
 def barrier(group=None, async_op=False, device_ids=None, prof=False, log_name='barrier', debug=get_caller_func()):
     global cdb
-    return cdb.barrier(group=group, async_op=async_op, device_ids=device_ids)
+    return cdb.barrier(group=group, async_op=async_op)
 
 
 @timed_op
 def monitored_barrier(group=None,
                       timeout=None,
                       wait_all_ranks=False,
                       prof=False,
@@ -585,14 +584,18 @@
     global cdb
 
     configure(deepspeed_config=config)
 
     if dist_init_required is None:
         dist_init_required = cdb is None or not cdb.is_initialized()
 
+    if cdb is None:
+        init_deepspeed_backend(get_accelerator().communication_backend_name(), timeout, init_method)
+        set_backend()
+        utils.logger.info(f'cdb={cdb}')
     if cdb is None and torch.distributed.is_initialized():
         # The user initialized torch.dist themselves, create cdb and short-circuit
         cdb = TorchBackend(dist_backend, timeout, init_method)
         return
 
     if dist_init_required is False:
         assert (
```

### Comparing `deepspeed-0.9.2/deepspeed/comm/config.py` & `deepspeed-0.9.3/deepspeed/comm/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/comm/constants.py` & `deepspeed-0.9.3/deepspeed/comm/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 NCCL_BACKEND = 'nccl'
+CCL_BACKEND = 'ccl'
 MPI_BACKEND = 'mpi'
 GLOO_BACKEND = 'gloo'
 SCCL_BACKEND = 'sccl'
 
 DEFAULT_AML_MASTER_PORT = "54965"
 DEFAULT_AML_NCCL_SOCKET_IFNAME = "^docker0,lo"
```

### Comparing `deepspeed-0.9.2/deepspeed/comm/torch.py` & `deepspeed-0.9.3/deepspeed/comm/torch.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/comm/utils.py` & `deepspeed-0.9.3/deepspeed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/compression/basic_layer.py` & `deepspeed-0.9.3/deepspeed/compression/basic_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepspeed.utils import logger
 
 g_mpu = None
 
 
 class QuantAct(nn.Module):
     """
-    Class to quantize given activations. Note that when using this function, the input acttivation quantization range will be fixed for all
+    Class to quantize given activations. Note that when using this function, the input activation quantization range will be fixed for all
     tokens/images for inference. This generally will affect some accuracy but achieve better latency performance.
     Parameters:
     ----------
     act_range_momentum : float, default 0.95
         Momentum for updating the activation quantization range.
     quant_mode : str, default 'symmetric'
     """
@@ -669,15 +669,15 @@
     rank = dist.get_rank(group=group)
     output = input_list[rank].contiguous()
 
     return output
 
 
 def _gather(input_):
-    """Gather tensors and concatinate along the last dimension."""
+    """Gather tensors and concatenate along the last dimension."""
     group = g_mpu.get_model_parallel_group()
 
     # Bypass the function if we are using only 1 GPU.
     if dist.get_world_size(group=group) == 1:
         return input_
 
     # Size and dimension.
@@ -704,15 +704,15 @@
 
     @staticmethod
     def backward(ctx, grad_output):
         return _reduce(grad_output)
 
 
 class _ReduceFromModelParallelRegion(torch.autograd.Function):
-    """All-redcue the input from the model parallel region."""
+    """All-reduce the input from the model parallel region."""
 
     @staticmethod
     def forward(ctx, input_):
         return _reduce(input_)
 
     @staticmethod
     def backward(ctx, grad_output):
@@ -728,15 +728,15 @@
 
     @staticmethod
     def backward(ctx, grad_output):
         return _gather(grad_output)
 
 
 class _GatherFromModelParallelRegion(torch.autograd.Function):
-    """Gather the input from model parallel region and concatinate."""
+    """Gather the input from model parallel region and concatenate."""
 
     @staticmethod
     def forward(ctx, input_):
         return _gather(input_)
 
     @staticmethod
     def backward(ctx, grad_output):
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/compress.py` & `deepspeed-0.9.3/deepspeed/compression/compress.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 from .helper import compression_preparation, fix_compression, recursive_getattr, is_module_compressible
 from .config import get_compression_config
 from ..runtime.config_utils import dict_raise_error_on_duplicate_keys
 from .constants import *
 import os
 import json
 
+try:
+    import neural_compressor as nc
+except ImportError as e:
+    nc = None
+
 
 def check_deepspeed_config(config):
     if isinstance(config, dict):
         return config
     elif os.path.exists(config):
         return json.load(open(config, "r"), object_pairs_hook=dict_raise_error_on_duplicate_keys)
     else:
@@ -113,14 +118,34 @@
     if compress_methods[LAYER_REDUCTION][LAYER_REDUCTION_ENABLED]:
         assert teacher_model is not None, "Teacher model is required for layer reduction"
         student_initialization(c_model, teacher_model, deepspeed_config)
 
     layer_added_compress_methods = get_compress_methods(c_model, compress_methods, mpu=mpu)
     compression_preparation(c_model, layer_added_compress_methods, mpu)
 
+    # For sparse pruning snip_momentum method
+    shared_parameters = compress_methods[SPARSE_PRUNING][SHARED_PARAMETERS]
+    if shared_parameters[SPARSE_PRUNING_ENABLED] and \
+        shared_parameters[SPARSE_PRUNING_METHOD] == SPARSE_PRUNING_METHOD_SNIP_MOMENTUM:
+
+        assert nc is not None, "please ensure the neural_compressor python package is installed by pip or conda if user wants to use snip_momentum sparse pruning"
+
+        from .helper import generate_pruners, register_on_step_begin
+        from nc import WeightPruningConfig
+
+        config = WeightPruningConfig(target_sparsity=1 - shared_parameters[SPARSE_PRUNING_DENSE_RATIO],
+                                     pattern=shared_parameters[SPARSE_PRUNING_BLOCK_PATTERN],
+                                     pruning_frequency=shared_parameters[SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE],
+                                     start_step=shared_parameters[SPARSE_PRUNING_SCHEDULE_OFFSET],
+                                     end_step=shared_parameters[SPARSE_PRUNING_SCHEDULE_OFFSET_END],
+                                     excluded_op_names=shared_parameters[SPARSE_PRUNING_EXCLUDED_MODULES])
+        pruners = generate_pruners(config, c_model)
+        c_model.pruners = pruners
+        register_on_step_begin(c_model)
+
     return model
 
 
 def redundancy_clean(model, deepspeed_config, mpu=None):
     """
     Remove the redundancy of a model
     Args:
@@ -183,25 +208,25 @@
     student_layer = [i for i in range(len(teacher_layer))]
     other_module_name = compress_methods[OTHER_MODULE_NAME]
     '''
         name_prefix (`str`)
             The prefix name before the layer #.
             Example 1: bert.encoder.layer, for BERT_base model's prefix name
             Example 2: transformer.h, for GPT-2 hugging face prefix name
-        teacher_layer (`list of intergers`)
-            The layer of teacher will be used for student's reinitializedion
+        teacher_layer (`list of integers`)
+            The layer of teacher will be used for student's reinitialization
             Example 1: [1,3,5,7,9], means we want to matches the 2nd/4th/6th/8th/10th layer of teacher to the first 5 layers of student
         student_layer (`list` or None)
-            The layer of student need to be re-intiialized
+            The layer of student need to be re-initialized
             Example 1: None, means we want to reinitialize all the layers
             Example 1: [0,1,2,3,4], means  we want to reinitialize the first 5 layers
         other_module_name (`list of string`)
-            The modules will be used for student's reinitializedion
+            The modules will be used for student's reinitialization
             Example 1: ['bert.pooler', 'bert.embeddings', 'classifier'], means we want to apply the weight in teacher's embedding/pooler/classier module to the student
-            Example 2: ['transformer.w', 'transformer.ln_f', 'lm_head'], means we want to apply the weight in teacher's embeddingn layers module to the student
+            Example 2: ['transformer.w', 'transformer.ln_f', 'lm_head'], means we want to apply the weight in teacher's embedding layers module to the student
     Note that teacher_layer should matches student layer
     '''
     assert len(student_layer) == len(teacher_layer)
     for s_name, t_name in zip(student_layer, teacher_layer):
         s_module = recursive_getattr(student_model, module_name_prefix + '.' + str(s_name))
         t_module = recursive_getattr(teacher_model, module_name_prefix + '.' + str(t_name))
         for s_param, t_param in zip(s_module.parameters(), t_module.parameters()):
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/config.py` & `deepspeed-0.9.3/deepspeed/compression/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from .constants import *
 import copy
-from ..runtime.config_utils import get_scalar_param
+from ..runtime.config_utils import get_scalar_param, get_list_param
 
 
 def get_compression_config(param_dict):
     #
     output = {}
 
     if COMPRESSION_TRAINING not in param_dict.keys():
@@ -217,34 +217,52 @@
     output = {}
     if SPARSE_PRUNING not in param_dict.keys():
         param_dict[SPARSE_PRUNING] = {SHARED_PARAMETERS: {}, DIFFERENT_GROUPS: {}}
     sub_param_dict = param_dict[SPARSE_PRUNING]
     # shared parameters
     output[SHARED_PARAMETERS] = get_sparse_pruning_shared_parameters(sub_param_dict)
     # each sub-groups
-    if output[SHARED_PARAMETERS][SPARSE_PRUNING_ENABLED]:
+    if output[SHARED_PARAMETERS][SPARSE_PRUNING_ENABLED] and output[SHARED_PARAMETERS][
+            SPARSE_PRUNING_METHOD] != SPARSE_PRUNING_METHOD_SNIP_MOMENTUM:
         assert DIFFERENT_GROUPS in sub_param_dict.keys(
-        ), f"Sparse Pruning is enabled, {DIFFERENT_GROUPS} must be specified"
+        ), f"Sparse Pruning is enabled and not snip_momentum method, {DIFFERENT_GROUPS} must be specified"
     output[DIFFERENT_GROUPS] = get_sparse_pruning_different_groups(sub_param_dict)
     return output
 
 
 def get_sparse_pruning_shared_parameters(param_dict):
     output = {}
+
     if SHARED_PARAMETERS in param_dict.keys():
         sub_param_dict = param_dict[SHARED_PARAMETERS]
         output[SPARSE_PRUNING_ENABLED] = get_scalar_param(sub_param_dict, SPARSE_PRUNING_ENABLED,
                                                           SPARSE_PRUNING_ENABLED_DEFAULT)
         output[SPARSE_PRUNING_METHOD] = get_scalar_param(sub_param_dict, SPARSE_PRUNING_METHOD,
                                                          SPARSE_PRUNING_METHOD_DEFAULT)
         assert output[SPARSE_PRUNING_METHOD] in [
-            SPARSE_PRUNING_METHOD_L1, SPARSE_PRUNING_METHOD_TOPK
-        ], f"Invalid sparse pruning method. Supported types: [{SPARSE_PRUNING_METHOD_L1}, {SPARSE_PRUNING_METHOD_TOPK}]"
+            SPARSE_PRUNING_METHOD_L1, SPARSE_PRUNING_METHOD_TOPK, SPARSE_PRUNING_METHOD_SNIP_MOMENTUM
+        ], f"Invalid sparse pruning method. Supported types: [{SPARSE_PRUNING_METHOD_L1}, {SPARSE_PRUNING_METHOD_TOPK}, {SPARSE_PRUNING_METHOD_SNIP_MOMENTUM}]"
         output[SPARSE_PRUNING_SCHEDULE_OFFSET] = get_scalar_param(sub_param_dict, SPARSE_PRUNING_SCHEDULE_OFFSET,
                                                                   SPARSE_PRUNING_SCHEDULE_OFFSET_DEFAULT)
+        if output[SPARSE_PRUNING_METHOD] == SPARSE_PRUNING_METHOD_SNIP_MOMENTUM:
+            output[SPARSE_PRUNING_BLOCK_PATTERN] = get_scalar_param(sub_param_dict, SPARSE_PRUNING_BLOCK_PATTERN,
+                                                                    SPARSE_PRUNING_BLOCK_PATTERN_DEFAULT)
+            output[SPARSE_PRUNING_DENSE_RATIO] = get_scalar_param(sub_param_dict, SPARSE_PRUNING_DENSE_RATIO,
+                                                                  SPARSE_PRUNING_DENSE_RATIO_DEFAULT)
+            assert output[SPARSE_PRUNING_DENSE_RATIO] > 0 and output[
+                SPARSE_PRUNING_DENSE_RATIO] < 1, f"Invalid dense_ratio value. Must be less than 1"
+            output[SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE] = get_scalar_param(
+                sub_param_dict, SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE, SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE_DEFAULT)
+            output[SPARSE_PRUNING_EXCLUDED_MODULES] = get_list_param(sub_param_dict, SPARSE_PRUNING_EXCLUDED_MODULES,
+                                                                     SPARSE_PRUNING_EXCLUDED_MODULES_DEFAULT)
+            output[SPARSE_PRUNING_SCHEDULE_OFFSET_END] = get_scalar_param(sub_param_dict,
+                                                                          SPARSE_PRUNING_SCHEDULE_OFFSET_END,
+                                                                          output[SPARSE_PRUNING_SCHEDULE_OFFSET])
+            assert output[SPARSE_PRUNING_SCHEDULE_OFFSET] <= output[
+                SPARSE_PRUNING_SCHEDULE_OFFSET_END], f"Invalid schedule_offset and schedule_offset_end values"
     else:
         output[SPARSE_PRUNING_ENABLED] = SPARSE_PRUNING_ENABLED_DEFAULT
         output[SPARSE_PRUNING_METHOD] = SPARSE_PRUNING_METHOD_DEFAULT
         output[SPARSE_PRUNING_SCHEDULE_OFFSET] = SPARSE_PRUNING_SCHEDULE_OFFSET_DEFAULT
     return output
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/constants.py` & `deepspeed-0.9.3/deepspeed/compression/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # It has several sub-components
 # #########################################
 COMPRESSION_TRAINING = "compression_training"
 SHARED_PARAMETERS = "shared_parameters"
 DIFFERENT_GROUPS = "different_groups"
 TECHNIQUE_ENABLED = "enabled"
 TECHNIQUE_SCHEDULE_OFFSET = "schedule_offset"
+TECHNIQUE_SCHEDULE_OFFSET_END = "schedule_offset_end"
 DIFFERENT_GROUPS_PARAMETERS = "params"
 DIFFERENT_GROUPS_MODULE_SCOPE = "modules"
 DIFFERENT_GROUPS_MODULE_SCOPE_DEFAULT = "*"
 DIFFERENT_GROUPS_RELATED_MODULE_SCOPE = "related_modules"
 DIFFERENT_GROUPS_RELATED_MODULE_SCOPE_DEFAULT = None
 # COMPRESSION_TRAINING_ENABLED = "enabled"
 # COMPRESSION_TRAINING_ENABLED_DEFAULT = False
@@ -28,15 +29,15 @@
 LAYER_REDUCTION_ENABLED_DEFAULT = False
 KEEP_NUMBER_LAYER = "keep_number_layer"
 MODULE_NAME_PREFIX = "module_name_prefix"
 TEACHER_LAYER = "teacher_layer"
 OTHER_MODULE_NAME = "other_module_name"
 
 ####
-# Weight Quantzation
+# Weight Quantization
 ####
 WEIGHT_QUANTIZATION = "weight_quantization"
 
 WEIGHT_QUANTIZATION_PERIOD = "quantization_period"
 WEIGHT_QUANTIZATION_PERIOD_DEFAULT = 1
 
 WEIGHT_QUANTIZE_IN_FORWARD_ENABLED = "quantize_weight_in_forward"
@@ -107,19 +108,33 @@
 SPARSE_PRUNING_ENABLED = TECHNIQUE_ENABLED
 SPARSE_PRUNING_ENABLED_DEFAULT = False
 
 SPARSE_PRUNING_METHOD = "method"
 SPARSE_PRUNING_METHOD_DEFAULT = "l1"
 SPARSE_PRUNING_METHOD_L1 = "l1"
 SPARSE_PRUNING_METHOD_TOPK = "topk"
+SPARSE_PRUNING_METHOD_SNIP_MOMENTUM = "snip_momentum"
+
+SPARSE_PRUNING_BLOCK_PATTERN = "block_pattern"
+SPARSE_PRUNING_BLOCK_PATTERN_DEFAULT = "4x1"
+
+SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE = "schedule_offset_stride"
+SPARSE_PRUNING_SCHEDULE_OFFSET_STRIDE_DEFAULT = 1
 
 SPARSE_PRUNING_SCHEDULE_OFFSET = TECHNIQUE_SCHEDULE_OFFSET
 SPARSE_PRUNING_SCHEDULE_OFFSET_DEFAULT = 1000
 
+SPARSE_PRUNING_SCHEDULE_OFFSET_END = TECHNIQUE_SCHEDULE_OFFSET_END
+SPARSE_PRUNING_SCHEDULE_OFFSET_END_DEFAULT = SPARSE_PRUNING_SCHEDULE_OFFSET_DEFAULT
+
 SPARSE_PRUNING_DENSE_RATIO = "dense_ratio"
+SPARSE_PRUNING_DENSE_RATIO_DEFAULT = 0.1
+
+SPARSE_PRUNING_EXCLUDED_MODULES = "excluded_modules"
+SPARSE_PRUNING_EXCLUDED_MODULES_DEFAULT = []
 ###
 # Row Pruning
 ###
 ROW_PRUNING = "row_pruning"
 
 ROW_PRUNING_ENABLED = TECHNIQUE_ENABLED
 ROW_PRUNING_ENABLED_DEFAULT = False
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/helper.py` & `deepspeed-0.9.3/deepspeed/compression/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 import torch
 from .basic_layer import Embedding_Compress, LinearLayer_Compress, Conv2dLayer_Compress, BNLayer_Compress, ColumnParallelLinear_Compress, RowParallelLinear_Compress
 from .constants import *
+from deepspeed.utils import logger
+
+try:
+    from neural_compressor.compression import pruner as nc_pruner
+except ImportError as e:
+    nc_pruner = None
 
 
 def recursive_getattr(model, module_name):
     """
     Recursively get the attribute of a module.
     Args:
         model (`torch.nn.Module`)
@@ -172,29 +178,29 @@
 
     if mpu is not None:
         ret = ret or isinstance(module, mpu.RowParallelLinear) or isinstance(module, mpu.ColumnParallelLinear)
 
     return ret
 
 
-def compression_preparation(model, compression_techinique_list, mpu):
+def compression_preparation(model, compression_technique_list, mpu):
     """
     Prepare the compression techniques of a model.
     Args:
         model (`torch.nn.Module`)
             The model to prepare the compression techniques of.
-        compression_techinique_list (`list`)
+        compression_technique_list (`list`)
             The list of compression techniques to prepare the model to.
             list[]
     """
     # Here we first replace all module with our linear wrapper
     for module_name, module in model.named_modules():
         if is_module_compressible(module, mpu):
             module_replacement(model, module_name, mpu=mpu)
-    for module_name_lists, _, compression_technique in compression_techinique_list:
+    for module_name_lists, _, compression_technique in compression_technique_list:
         for mnl in module_name_lists:
             for module_name in mnl:
                 module_replacement(model, module_name, compression_technique)
 
     return model
 
 
@@ -242,7 +248,75 @@
             new_module.weight.data = old_module.weight.data.t().contiguous()
             if new_module.bias is not None:
                 new_module.bias.data = old_module.bias.data.view(-1)
 
             recursive_setattr(c_model, name, new_module)
 
     return model
+
+
+def generate_pruners(config, model):
+    """Generate pruners.
+    Args:
+        config (`neural_compressor.WeightPruningConfig`)
+            The object to the class WeightPruningConfig.
+        model (`torch.nn.module`)
+            The torch module object to be pruned.
+    """
+    assert nc_pruner is not None, "please ensure the neural_compressor python package is installed by pip or conda if user wants to use snip_momentum sparse pruning"
+    from nc_pruner.utils import process_config, parse_to_prune
+    from nc_pruner.pruners import get_pruner
+    assert isinstance(model, torch.nn.Module)
+    pruners_info = process_config(config)
+    pruners = []
+    for info in pruners_info:
+        modules = parse_to_prune(info, model)
+        if modules == {}:
+            logger.warning("one pruner hooks no layers, please have a check")
+
+        pruners.append(get_pruner(info, modules))
+        info['modules'] = [key for key in modules.keys()]
+        info['len_of_modules'] = len(info['modules'])
+        logger.info(info)
+    return pruners
+
+
+def register_on_step_begin(model):
+    """Mount on_step_begin to the model.
+    Args:
+        model (`torch.nn.module`)
+            The torch module object to be pruned.
+    """
+
+    def hook(module, input):
+        for pruner in module.pruners:
+            pruner.on_step_begin(0)
+
+    hook_handle = model.register_forward_pre_hook(hook)
+    return hook_handle
+
+
+def rewrite_optimizer_step(opt: torch.optim.Optimizer):
+    """Mount on_before/after_optimizer_step to the optimizer.
+    Args:
+        model (`torch.opt.Optimizer`)
+            The torch optimizer object to be hooked.
+    """
+
+    def new_step(self, closure=None):
+        if hasattr(self, "pruners"):
+            for pruner in self.pruners:
+                pruner.on_before_optimizer_step()
+
+        if closure is not None:
+            res = self.orig_step(closure)
+        else:
+            res = self.orig_step()
+        if hasattr(self, "pruners"):
+            for pruner in self.pruners:
+                pruner.on_after_optimizer_step()
+        return res
+
+    opt.orig_step = opt.step
+    import types
+    opt.step = types.MethodType(new_step, opt)
+    return opt
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/scheduler.py` & `deepspeed-0.9.3/deepspeed/compression/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,17 @@
     def check_sparse_pruning(self):
         # check sparse pruning
         sp = self.different_compression_methods[SPARSE_PRUNING]
         if not sp[TECHNIQUE_ENABLED]:
             return
         else:
             shared_parameters = sp[SHARED_PARAMETERS]
-            if self.training_steps >= shared_parameters[TECHNIQUE_SCHEDULE_OFFSET]:
+            if self.training_steps >= shared_parameters[
+                    TECHNIQUE_SCHEDULE_OFFSET] and self.training_steps <= shared_parameters[
+                        TECHNIQUE_SCHEDULE_OFFSET_END]:
                 for group_name, module_name_list, method_parameters in sp[DIFFERENT_GROUPS]:
                     for module_name in module_name_list:
                         module = recursive_getattr(self.model, module_name)
                         module.sparse_pruning_enabled = True
                 if not self.verbose[SPARSE_PRUNING]:
                     logger.info(f'Sparse pruning is enabled at step {self.training_steps}')
                     self.verbose[SPARSE_PRUNING] = True
```

### Comparing `deepspeed-0.9.2/deepspeed/compression/utils.py` & `deepspeed-0.9.3/deepspeed/compression/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     def forward(ctx, input, num_bits, min_value=None, max_value=None, num_groups=1):
         """
         Args:
             inputs (`torch.FloatTensor`)
                 The input which needs to be quantized
             num_bits (int, >=4)
                 Number of bits to use for quantization
-            min_value/max_vlue (torch.FloatTensor)
+            min_value/max_value (torch.FloatTensor)
                 Used for static activation quantization
             num_groups (int)
                 How many groups to partition the quantization into
         Returns:
             quantized_input (`torch.FloatTensor`)
                 Quantized input
         """
@@ -110,15 +110,15 @@
     def forward(ctx, input, num_bits, min_value=None, max_value=None, num_groups=1):
         """
         Args:
             inputs (`torch.FloatTensor`)
                 The input which needs to be quantized
             num_bits (int, >=4)
                 Number of bits to use for quantization
-            min_value/max_vlue (torch.FloatTensor)
+            min_value/max_value (torch.FloatTensor)
                 Used for static activation quantization
             num_groups (int)
                 How many groups to partition the quantization into
         Returns:
             quantized_input (`torch.FloatTensor`)
                 Quantized input
         """
@@ -154,15 +154,15 @@
     def forward(ctx, input, num_bits, min_value=None, max_value=None, num_groups=1):
         """
         Args:
             inputs (`torch.FloatTensor`)
                 The input which needs to be quantized
             num_bits (int)
                 Dummy variable
-            min_value/max_vlue (torch.FloatTensor)
+            min_value/max_value (torch.FloatTensor)
                 Used for static activation quantization; for now they are dummy variable
             num_groups (int)
                 How many groups to partition the quantization into
         Returns:
             quantized_input (`torch.FloatTensor`)
                 Quantized input
         """
@@ -195,15 +195,15 @@
     def forward(ctx, input, num_bits, min_value=None, max_value=None, num_groups=1):
         """
         Args:
             inputs (`torch.FloatTensor`)
                 The input which needs to be quantized
             num_bits (int)
                 Dummy variable
-            min_value/max_vlue (torch.FloatTensor)
+            min_value/max_value (torch.FloatTensor)
                 Used for static activation quantization; for now they are dummy variable
             num_groups (int)
                 How many groups to partition the quantization into
         Returns:
             quantized_input (`torch.FloatTensor`)
                 Quantized input
         """
```

### Comparing `deepspeed-0.9.2/deepspeed/constants.py` & `deepspeed-0.9.3/deepspeed/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/elasticity/config.py` & `deepspeed-0.9.3/deepspeed/elasticity/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         if self.min_gpus < 1 or self.max_gpus < 1:
             raise ElasticityConfigError("Elasticity min/max gpus must be > 0, "
                                         f"given min_gpus: {self.min_gpus}, max_gpus: {self.max_gpus}")
         if self.max_gpus < self.min_gpus:
             raise ElasticityConfigError("Elasticity min_gpus cannot be greater than max_gpus, "
                                         f"given min_gpus: {self.min_gpus}, max_gpus: {self.max_gpus}")
 
-        self.model_parallel_size = param_dict.get(MODEL_PARLLEL_SIZE, MODEL_PARLLEL_SIZE_DEFAULT)
+        self.model_parallel_size = param_dict.get(MODEL_PARALLEL_SIZE, MODEL_PARALLEL_SIZE_DEFAULT)
         if self.model_parallel_size < 1:
             raise ElasticityConfigError("Model-Parallel size cannot be less than 1, "
                                         f"given model-parallel size: {self.model_parallel_size}")
 
         self.num_gpus_per_node = param_dict.get(NUM_GPUS_PER_NODE, NUM_GPUS_PER_NODE_DEFAULT)
         if self.num_gpus_per_node < 1:
             raise ElasticityConfigError("Number of GPUs per node cannot be less than 1, "
```

### Comparing `deepspeed-0.9.2/deepspeed/elasticity/constants.py` & `deepspeed-0.9.3/deepspeed/elasticity/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 MIN_GPUS_DEFAULT = 1
 MAX_GPUS = 'max_gpus'
 MAX_GPUS_DEFAULT = 10000
 
 NUM_GPUS_PER_NODE = 'num_gpus_per_node'
 NUM_GPUS_PER_NODE_DEFAULT = 1
 
-MODEL_PARLLEL_SIZE = "model_parallel_size"
-MODEL_PARLLEL_SIZE_DEFAULT = 1
+MODEL_PARALLEL_SIZE = "model_parallel_size"
+MODEL_PARALLEL_SIZE_DEFAULT = 1
 
 # Minimum running time (minutes) before the scheduler will scale us, 0 implies it's unknown
 MIN_TIME = "min_time"
 MIN_TIME_DEFAULT = 0
 
 # When finding a suitable batch size, attempt to find one that is closest
 # to the max train batch size given.
```

### Comparing `deepspeed-0.9.2/deepspeed/elasticity/elastic_agent.py` & `deepspeed-0.9.3/deepspeed/elasticity/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/elasticity/elasticity.py` & `deepspeed-0.9.3/deepspeed/elasticity/elasticity.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/env_report.py` & `deepspeed-0.9.3/deepspeed/env_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     print(h[0], "." * (max_dots - len(h[0])), h[1], "." * (max_dots2 - len(h[1])), h[2])
     print("-" * (max_dots + max_dots2 + len(h[0]) + len(h[1])))
     installed = f"{GREEN}[YES]{END}"
     no = f"{YELLOW}[NO]{END}"
     for op_name, builder in ALL_OPS.items():
         dots = "." * (max_dots - len(op_name))
         is_compatible = OKAY if builder.is_compatible(verbose) else no
-        is_installed = installed if installed_ops[op_name] else no
+        is_installed = installed if installed_ops.get(op_name, False) else no
         dots2 = '.' * ((len(h[1]) + (max_dots2 - len(h[1]))) - (len(is_installed) - color_len))
         print(op_name, dots, is_installed, dots2, is_compatible)
     print("-" * (max_dots + max_dots2 + len(h[0]) + len(h[1])))
 
 
 def ninja_installed():
     try:
```

### Comparing `deepspeed-0.9.2/deepspeed/git_version_info.py` & `deepspeed-0.9.3/deepspeed/git_version_info.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/git_version_info_installed.py` & `deepspeed-0.9.3/deepspeed/git_version_info_installed.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-version='0.9.2'
+version='0.9.3'
 git_hash='unknown'
 git_branch='unknown'
 installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False, 'utils': False}
 compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True, 'utils': True}
 torch_info={'version': '1.9', 'bf16_support': False, 'cuda_version': '10.2', 'nccl_version': '2.7', 'hip_version': '0.0'}
```

### Comparing `deepspeed-0.9.2/deepspeed/inference/config.py` & `deepspeed-0.9.3/deepspeed/inference/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 from enum import Enum
 
 
 class DtypeEnum(Enum):
     # The torch dtype must always be the first value (so we return torch.dtype)
     fp16 = torch.float16, "torch.float16", "fp16", "float16", "half"
     fp32 = torch.float32, "torch.float32", "fp32", "float32", "float"
+    bf16 = torch.bfloat16, "torch.bfloat16", "bf16", "bfloat16", "bfloat"
     int8 = torch.int8, "torch.int8", "int8"
 
-    # bf16 not supported
-    # bf16 = torch.bfloat16, "torch.bfloat16", "bf16", "bfloat16"
-
     # Copied from https://stackoverflow.com/a/43210118
     # Allows us to use multiple values for each Enum index and returns first
     # listed value when Enum is called
     def __new__(cls, *values):
         obj = object.__new__(cls)
         # first value is canonical value
         obj._value_ = values[0]
@@ -182,15 +180,15 @@
     Transformer layer (e.g. (True, 8) shows we quantize the model using 8
     groups for all the network except the MLP part that we use 8 extra
     grouping). Expects a dictionary containing values for
     :any:`QuantizationConfig`.
     """
 
     #todo: refactor the following 3 into the new checkpoint_config
-    checkpoint: str = None
+    checkpoint: Union[str, Dict] = None
     """
     Path to deepspeed compatible checkpoint or path to JSON with load policy.
     """
 
     base_dir: str = None
     """
     This shows the root directory under which all the checkpoint files exists.
```

### Comparing `deepspeed-0.9.2/deepspeed/inference/engine.py` & `deepspeed-0.9.3/deepspeed/inference/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,16 +147,18 @@
             if config.tensor_parallel.tp_size > 1:
                 self.build_alibi_tensor()
 
         if get_accelerator().device_name() == 'cuda' and config.enable_cuda_graph:
             assert pkg_version.parse(torch.__version__) >= pkg_version.parse("1.10"), \
                 "If you want to use cuda graph, please upgrade torch to at least v1.10"
 
-        if config.checkpoint and not config.replace_with_kernel_inject:
-            self._load_checkpoint(config.checkpoint)
+        # Check if model passed to engine is loaded w/ meta tensors, in which case
+        # kernel injection must be enabled.
+        # NOTE: This check assumes a Hugging Face hierarchy for the device type i.e. module.device.type
+        self.model_meta_device = self.module.device.type == 'meta' if hasattr(self.module, "device") else False
 
         # convert model to intended dtype
         if config.dtype:
             self._convert_to_dtype(config)
 
         if self.mpu:
             config.tensor_parallel.tp_size = dist.get_world_size(group=self.mpu.get_model_parallel_group())
@@ -169,34 +171,30 @@
             moe, _ = has_moe_layers(self.module)
         else:
             moe = False
 
         if moe and dist.get_world_size() > 1:
             self._create_ep_parallel_group(config.moe.moe_experts)
 
-        # retain this from the old conditional argument being passed to apply_injection_policy()
-        if not config.replace_with_kernel_inject:
-            config.checkpoint = None
-
-        # We only support three modes: 1) user specified policy for tensor-parallelism, 2) kernel injection (replace_with_kernel_inject), and 3) automatic tensor parallelism.
+        # We only support three modes: 1) user specified policy for tensor-parallelism, 2) kernel injection (replace_with_kernel_inject), and 3) automatic tensor parallelism if tp_size > 1.
         if self.injection_dict:
             # 1. User specified Tensor Parallelism
             assert not config.replace_with_kernel_inject, "Cannot use both user specified injection policy and kernel injection"
             for client_module, injection_policy in self.injection_dict.items():
                 # construct the tuple and pass that instead of a string or dict.
                 if isinstance(injection_policy, str):
                     config.injection_policy_tuple = (injection_policy, )
                 else:
                     config.injection_policy_tuple = injection_policy
                 self._apply_injection_policy(config, client_module)
         else:
             if config.replace_with_kernel_inject:
                 # 2. DeepSpeed Kernel Injection
                 self._apply_injection_policy(config)
-            else:
+            elif config.tensor_parallel.tp_size > 1:
                 # 3. Automatic Tensor Parallelism
                 parser_dict = AutoTP.tp_parser(model)
                 print("AutoTP: ", parser_dict)
                 for client_module, injection_policy in parser_dict:
                     if isinstance(injection_policy, str):
                         config.injection_policy_tuple = (injection_policy, )
                     else:
@@ -251,15 +249,15 @@
     def _post_forward_hook(self, module, input, output):
         if self.use_cuda_events:
             self.timers(INFERENCE_MODEL_TIMER).stop()
             elapsed_time = self.timers(INFERENCE_MODEL_TIMER).elapsed(reset=True)
         else:
             get_accelerator().synchronize()
             self._end = time.time()
-            elapsed_time = self._end - self._start
+            elapsed_time = (self._end - self._start) * 1e3  # convert seconds to ms
         self._model_times.append(elapsed_time)
 
     def _create_model_parallel_group(self, config):
         # Call the init process
         if InferenceEngine.inference_mp_group is None:
             init_distributed()
             local_rank = int(os.getenv('LOCAL_RANK', '0'))
@@ -339,24 +337,46 @@
         self.mp_replace = ReplaceWithTensorSlicing(
             mp_group=self.mp_group, mp_size=self._config.tensor_parallel.tp_size)  #, out_dim=0, in_dim=1)
         error_msgs = []
 
         def load(module, state_dict, prefix):
             args = (state_dict, prefix, {}, True, [], [], error_msgs)
             if hasattr(module, 'weight'):
+                if module.weight.data.is_meta:
+                    # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                    module.weight = torch.nn.parameter.Parameter(data=torch.empty_like(module.weight.data,
+                                                                                       device="cpu"),
+                                                                 requires_grad=module.weight.data.requires_grad)
                 if 'query_key_value' in prefix:
-                    module.weight = self.mp_replace.qkv_copy(module.weight.data, state_dict[prefix + 'weight'])
+                    module.weight = self.mp_replace.strided_copy(module.weight.data,
+                                                                 state_dict[prefix + 'weight'],
+                                                                 num_splits=3)
                 else:
                     module.weight = self.mp_replace.copy(module.weight.data, state_dict[prefix + 'weight'])
             else:
+                if module.norm.weight.data.is_meta:
+                    # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                    module.norm.weight = torch.nn.parameter.Parameter(
+                        data=torch.empty_like(module.norm.weight.data, device="cpu"),
+                        requires_grad=module.norm.weight.data.requires_grad)
                 module.norm.weight = self.mp_replace.copy(module.norm.weight.data, state_dict[prefix + 'weight'])
             if prefix + 'bias' in self.key_list:
                 if hasattr(module, 'norm'):
+                    if module.norm.bias.data.is_meta:
+                        # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                        module.norm.bias = torch.nn.parameter.Parameter(
+                            data=torch.empty_like(module.norm.bias.data, device="cpu"),
+                            requires_grad=module.norm.bias.data.requires_grad)
                     module.norm.bias = self.mp_replace.copy(module.norm.bias, state_dict[prefix + 'bias'])
                 else:
+                    if module.bias.data.is_meta:
+                        # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                        module.bias = torch.nn.parameter.Parameter(data=torch.empty_like(module.bias.data,
+                                                                                         device="cpu"),
+                                                                   requires_grad=module.bias.data.requires_grad)
                     data = state_dict[prefix + 'bias']
                     data = data.to(get_accelerator().current_device_name())
                     module.bias = self.mp_replace.copy(module.bias, data)
 
         layer_policies = {
             nn.Linear: load,
             nn.Embedding: load,
@@ -377,22 +397,32 @@
                             setattr(module, name, child)
                     load(child, self.sd, prefix + name + '.')
                 else:
                     load_module_recursive(child, prefix if level == 0 else prefix + name + '.', level + 1)
 
         load_module_recursive(r_module)
 
+        embedding_weight = None
+
+        for n, p in r_module.named_parameters():
+            if "word_embeddings." in n or "embed_tokens." in n or "wte." in n:
+                embedding_weight = p
+        if embedding_weight is not None and hasattr(r_module, "lm_head") and hasattr(
+                r_module.lm_head, "weight") and r_module.lm_head.weight.is_meta:
+            r_module.lm_head.weight = embedding_weight
+
     def _apply_injection_policy(self, config, client_module=None):
         # client_module is only passed when using the injection_dict method.
         checkpoint_dir = config.checkpoint
         checkpoint = SDLoaderFactory.get_sd_loader_json(checkpoint_dir,
                                                         self.checkpoint_engine) if checkpoint_dir is not None else None
 
         generic_injection(self.module,
                           fp16=(config.dtype == torch.half) or (config.dtype == torch.int8),
+                          bf16=(config.dtype == torch.bfloat16),
                           enable_cuda_graph=config.enable_cuda_graph)
 
         if isinstance(self.module, torch.nn.Module):
             # config is our DeepSpeedInferenceConfig and self.config is the HF model config
             replace_transformer_layer(client_module, self.module, checkpoint, config, self.config)
 
     def _get_all_ckpt_names(self, checkpoints_path, tag):
@@ -428,24 +458,26 @@
                         tag = fd.read().strip()
 
             ckpt_list = self._get_all_ckpt_names(load_dir, tag)
             sd_loader = SDLoaderFactory.get_sd_loader(ckpt_list, self.checkpoint_engine)
         else:
             sd_loader = SDLoaderFactory.get_sd_loader_json(load_dir, self.checkpoint_engine)
 
-        if type(sd_loader) is list:
-            self.sd = torch.load(sd_loader[0], map_location='cpu')
+        checkpoint = sd_loader['checkpoints']
+
+        if type(checkpoint) is list:
+            self.sd = torch.load(checkpoint[0], map_location='cpu')
             self.key_list = list(self.sd.keys())
 
             self.load_model_with_checkpoint(self.module)
 
-            for i in range(1, len(sd_loader)):
+            for i in range(1, len(checkpoint)):
                 if not dist.is_initialized() or dist.get_rank() == 0:
                     print(f"loading checkpoint ({i})")
-                self.sd = torch.load(sd_loader[i], map_location=get_accelerator().device_name())
+                self.sd = torch.load(checkpoint[i], map_location=get_accelerator().device_name())
                 self.key_list = list(self.sd.keys())
                 self.load_model_with_checkpoint(self.module)
         else:
             mp_rank = 0 if self.mpu is None else self.mpu.get_model_parallel_rank()
 
             load_path, checkpoint, quantize_config = sd_loader.load(self._config.tensor_parallel.tp_size,
                                                                     mp_rank,
@@ -576,15 +608,15 @@
                 self._create_cuda_graph(*inputs, **kwargs)
                 outputs = self._graph_replay(*inputs, **kwargs)
         else:
             outputs = self.module(*inputs, **kwargs)
 
         if self.model_profile_enabled and self._config.enable_cuda_graph:
             get_accelerator().synchronize()
-            duration = time.time() - start
+            duration = (time.time() - start) * 1e3  # convert seconds to ms
             self._model_times.append(duration)
 
         return outputs
 
     def _generate(self, *inputs, **kwargs):
         # Reset KV-cache at the beginning of generate
         if hasattr(self.module, 'reset_cache'):
```

### Comparing `deepspeed-0.9.2/deepspeed/launcher/launch.py` & `deepspeed-0.9.3/deepspeed/launcher/launch.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 import subprocess
 import os
 import json
 import base64
 import time
 import signal
 import psutil
-import distutils
 from collections import defaultdict
 from typing import Dict
 from argparse import ArgumentParser, REMAINDER
 from ..constants import TORCH_DISTRIBUTED_DEFAULT_PORT
 from ..nebula.constants import DLTS_POD_ENV_PATH
-from ..utils import logger
+from ..utils import logger, get_numactl_cmd
 from ..elasticity import is_torch_elastic_compatible
 from .constants import ELASTIC_TRAINING_ID_DEFAULT
 
 PID_FILE_BASEPATH = "/tmp"
 
 
 def parse_args():
@@ -126,97 +125,14 @@
         except psutil.NoSuchProcess:
             pass
     gone, alive = psutil.wait_procs(children, timeout=30)
     for p in alive:
         p.kill()
 
 
-def parse_range(rng):
-    try:
-        value = int(rng)
-        return range(value, value + 1)
-    except ValueError:
-        # value is not a single number
-        parts = rng.split('-')
-        if len(parts) != 2:
-            raise ValueError("Bad range: '%s', range must be either a number or two number separated by dash" %
-                             (rng, ))
-        start = int(parts[0])
-        end = int(parts[1])
-        if start > end:
-            raise ValueError("Bad range: '%s', range end must larger than or equal to start" % (rng, ))
-        return range(start, end + 1)
-
-
-# parse comma and dash separated range list into list
-# i.e. "0,2-4,6" --> [0, 2, 3, 4, 6]
-# rules:
-# 1. Range list numser be comma sepeaated, each item are either a single number,
-#    or a range marked by two numbers (both number are included in the range)
-# 2. Sub ranges must be in ascend order and not overlap with each other
-# 3. No space in the range expression
-def parse_range_list(range_str):
-    number_list = []
-    last = -1
-    range_list = range_str.split(',')
-    for sub_range in range_list:
-        sub_number_list = parse_range(sub_range)
-        if sub_number_list[0] <= last:
-            raise ValueError(
-                "Bad range: '%s', sub ranges must not overlap with each other and should be in ascend order" %
-                (range_str, ))
-        last = sub_number_list[-1]
-        number_list.extend(sub_number_list)
-    return number_list
-
-
-# return a list of list for cores to numa mapping
-# [
-#     [ cores for numa 0 ]
-#     [ cores belong to numa 1 ]
-#     ...
-# ]
-def get_numa_cores():
-    ret = []
-    output = subprocess.check_output(['numactl', '--hardware']).decode("utf-8")
-    lines = output.split('\n')
-    for line in lines:
-        if line.startswith('available:'):
-            num_numas = int(line.split(' ')[1])
-            break
-    for numa in range(num_numas):
-        for line in lines:
-            if line.startswith(f'node {numa} cpus:'):
-                cores = line.split(' ')[3:]
-                ret.append([int(core) for core in cores])
-    return ret
-
-
-def check_for_numactl_pkg():
-    libs = dict(
-        dpkg=["-l", "numactl", "apt"],
-        pacman=["-Q", "numactl", "pacman"],
-        rpm=["-q", "numactl", "yum"],
-    )
-
-    found = False
-    for pkgmgr, data in libs.items():
-        flag, lib, tool = data
-        path = distutils.spawn.find_executable(pkgmgr)
-        if path is not None:
-            cmd = f"{pkgmgr} {flag} {lib}"
-            result = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-            if result.wait() == 0:
-                found = True
-            else:
-                print(f"please install the {lib} package with {tool}")
-            break
-    return found
-
-
 def main():
     args = parse_args()
     current_env = os.environ.copy()
 
     for k in current_env.keys():
         if "NCCL" in k:
             logger.info(f"{args.node_rank} {k}={current_env[k]}")
@@ -304,47 +220,17 @@
             dist_rank = global_rank_mapping[local_node][local_rank]
             current_env["RANK"] = str(dist_rank)
             current_env["LOCAL_RANK"] = str(local_rank)
 
             # spawn the processes
             cmd = []
             if args.bind_cores_to_rank:
-                check_for_numactl_pkg()
-                if 'KMP_AFFINITY' in os.environ.keys():
-                    raise ValueError("Environment variable KMP_AFFINITY conflicts with numactl "
-                                     "because it interfere with how many CPU cores numactl can set. "
-                                     "Unset KMP_AFFINITY before launching deepspeed.\n\n"
-                                     "\t$ unset KMP_AFFINITY\n"
-                                     "\t$ deepspeed <deepspeed command parameters>")
-                if args.bind_core_list != None:
-                    core_list = parse_range_list(args.bind_core_list)
-                    total_cores = len(core_list)
-                else:
-                    total_cores = psutil.cpu_count(logical=False)
-                    core_list = range(total_cores)
-                cores_per_rank = total_cores // num_local_procs
-                assert cores_per_rank >= 1, "At least one core needs to be assigned to each rank"
-                core_list_for_rank = core_list[cores_per_rank * local_rank:cores_per_rank * (local_rank + 1)]
+                cores_per_rank, numactl_cmd = get_numactl_cmd(args.bind_core_list, num_local_procs, local_rank)
                 current_env["OMP_NUM_THREADS"] = f"{cores_per_rank}"
-                cmd.append("numactl")
-
-                # check if all cores belong to same numa, if true, bind process to that numa domain with -m parameter
-                numa_cores = get_numa_cores()
-                num_numas = len(numa_cores)
-                for i in range(num_numas):
-                    if set(core_list_for_rank) <= set(numa_cores[i]):
-                        cmd.append("-m")
-                        cmd.append(f"{i}")
-                        break
-
-                cmd.append("-C")
-                core_list_str = f"{core_list_for_rank[0]}"
-                for core_id in core_list_for_rank[1:]:
-                    core_list_str = f"{core_list_str},{core_id}"
-                cmd.append(f"{core_list_str}")
+                cmd = cmd + numactl_cmd
             if not args.no_python:
                 cmd.append(sys.executable)
                 cmd.append("-u")
                 if args.module:
                     cmd.append("-m")
             else:
                 if args.module:
```

### Comparing `deepspeed-0.9.2/deepspeed/launcher/multinode_runner.py` & `deepspeed-0.9.3/deepspeed/launcher/multinode_runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import shutil
 import subprocess
 import warnings
 from shlex import split
 from abc import ABC, abstractmethod
 from deepspeed.accelerator import get_accelerator
-from ..utils import logger
+from ..utils import logger, get_numactl_cmd
 from .constants import PDSH_MAX_FAN_OUT, MVAPICH_TMP_HOSTFILE
 
 
 class MultiNodeRunner(ABC):
 
     def __init__(self, args, world_info_base64):
         self.args = args
@@ -180,42 +180,138 @@
         if self.args.num_nodes != -1 or self.args.num_gpus != -1:
             raise ValueError(f"{self.name} backend does not support limiting num nodes/gpus")
 
     def get_cmd(self, environment, active_resources):
         devices_per_node = self.resource_pool.values()
         total_process_count = sum(devices_per_node)
         process_per_node = list(devices_per_node)[0]
-        hosts = ""
+        if not all([n == process_per_node for n in devices_per_node]):
+            raise ValueError("MPICH requires same number of devices per node")
 
-        for i, host in enumerate(self.resource_pool.keys()):
+        mpirun_cmd = [
+            'mpirun',
+        ] + split(self.args.launcher_args)
+        export_cmd = []
+
+        for k, v in self.exports.items():
+            export_cmd += ['-genv', "{}={}".format(k, v)]
+
+        export_cmd += ['-genv', 'MASTER_ADDR', str(self.args.master_addr)]
+        export_cmd += ['-genv', 'MASTER_PORT', str(self.args.master_port)]
+        export_cmd += ['-genv', 'WORLD_SIZE', str(total_process_count)]
+        export_cmd += ['-genv', 'LOCAL_SIZE', str(process_per_node)]
+
+        hosts = list(self.resource_pool.keys())
+
+        per_host_cmd = []
+        host_id = 0
+        host_count = 0
+        for i in range(total_process_count):
+            local_rank = i % process_per_node
+            python_exec = []
+            if not self.args.no_python:
+                python_exec += [sys.executable, "-u"]
+                if self.args.module:
+                    python_exec.append("-m")
+            env_mapping = ['-env', 'RANK', str(i)]
+            env_mapping += ['-env', 'LOCAL_RANK', str(local_rank)]
             if i == 0:
-                hosts = f"{host}"
+                per_host_cmd = ['-n', '1', '-host', hosts[host_id]
+                                ] + env_mapping + python_exec + [self.user_script] + self.user_arguments
             else:
-                hosts += f",{host}"
+                per_host_cmd = per_host_cmd + [':', '-n', '1', '-host', hosts[host_id]
+                                               ] + env_mapping + python_exec + [self.user_script] + self.user_arguments
+            host_count = host_count + 1
+            if host_count == process_per_node:
+                host_id = host_id + 1
+                host_count = 0
+
+        return mpirun_cmd + export_cmd + per_host_cmd
+
+
+class IMPIRunner(MultiNodeRunner):
+
+    def __init__(self, args, world_info_base64, resource_pool):
+        super().__init__(args, world_info_base64)
+        self.resource_pool = resource_pool
+
+    def backend_exists(self):
+        #TODO: if IB is available we should suggestion mpich
+        return shutil.which('mpirun')  #mpich_info
+
+    @property
+    def name(self):
+        return "impi"
+
+    def validate_args(self):
+        super().validate_args()
+        #TODO: Allow for include/exclude at node-level but not gpu-level
+        if self.args.include != "" or self.args.exclude != "":
+            raise ValueError(f"{self.name} backend does not support worker include/exclusion")
+
+        if self.args.num_nodes != -1 or self.args.num_gpus != -1:
+            raise ValueError(f"{self.name} backend does not support limiting num nodes/gpus")
+
+    def get_cmd(self, environment, active_resources):
+        devices_per_node = self.resource_pool.values()
+        total_process_count = sum(devices_per_node)
+        process_per_node = list(devices_per_node)[0]
+        if not all([n == process_per_node for n in devices_per_node]):
+            raise ValueError("Intel MPI requires same number of devices per node")
 
         mpirun_cmd = [
             'mpirun',
-            '-n',
-            f'{total_process_count}',
             '-ppn',
             f'{process_per_node}',
-            '-hosts',
-            f'{hosts}',
         ] + split(self.args.launcher_args)
         export_cmd = []
 
         for k, v in self.exports.items():
-            export_cmd += ['-genv', "{}={}".format(k, v)]
+            export_cmd += ['-genv', f'{k}', f'{v}']
 
-        python_exec = []
-        if not self.args.no_python:
-            python_exec = [sys.executable, "-u"]
-            if self.args.module:
-                python_exec.append("-m")
-        return mpirun_cmd + export_cmd + python_exec + [self.user_script] + self.user_arguments
+        if self.args.bind_cores_to_rank:
+            cores_per_rank, _ = get_numactl_cmd(self.args.bind_core_list, process_per_node, 0)
+            export_cmd += ['-genv', 'OMP_NUM_THREADS', str(cores_per_rank)]
+
+        export_cmd += ['-genv', 'MASTER_ADDR', str(self.args.master_addr)]
+        export_cmd += ['-genv', 'MASTER_PORT', str(self.args.master_port)]
+        export_cmd += ['-genv', 'WORLD_SIZE', str(total_process_count)]
+        export_cmd += ['-genv', 'LOCAL_SIZE', str(process_per_node)]
+
+        export_cmd += ['-hosts']
+        hosts = ""
+        for i, host in enumerate(self.resource_pool.keys()):
+            if i == 0:
+                hosts = f"{host}"
+            else:
+                hosts += f",{host}"
+        export_cmd += [hosts]
+
+        per_host_cmd = []
+
+        for i in range(total_process_count):
+            local_rank = i % process_per_node
+            python_exec = []
+            if self.args.bind_cores_to_rank:
+                _, numactl_cmd = get_numactl_cmd(self.args.bind_core_list, process_per_node, local_rank)
+                python_exec += numactl_cmd
+
+            if not self.args.no_python:
+                python_exec += [sys.executable, "-u"]
+                if self.args.module:
+                    python_exec.append("-m")
+            env_mapping = ['-env', 'RANK', str(i)]
+            env_mapping += ['-env', 'LOCAL_RANK', str(local_rank)]
+            if i == 0:
+                per_host_cmd = ['-n', '1'] + env_mapping + python_exec + [self.user_script] + self.user_arguments
+            else:
+                per_host_cmd = per_host_cmd + [':', '-n', '1'] + env_mapping + python_exec + [self.user_script
+                                                                                              ] + self.user_arguments
+        print(mpirun_cmd + export_cmd + per_host_cmd)
+        return mpirun_cmd + export_cmd + per_host_cmd
 
 
 class SlurmRunner(MultiNodeRunner):
 
     def __init__(self, args, world_info_base64, resource_pool):
         super().__init__(args, world_info_base64)
         self.resource_pool = resource_pool
```

### Comparing `deepspeed-0.9.2/deepspeed/launcher/runner.py` & `deepspeed-0.9.3/deepspeed/launcher/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,34 @@
 import argparse
 import subprocess
 import collections
 from copy import deepcopy
 import signal
 import time
 
-from .multinode_runner import PDSHRunner, OpenMPIRunner, MVAPICHRunner, SlurmRunner, MPICHRunner
-from .constants import PDSH_LAUNCHER, OPENMPI_LAUNCHER, MVAPICH_LAUNCHER, SLURM_LAUNCHER, MPICH_LAUNCHER
+from .multinode_runner import PDSHRunner, OpenMPIRunner, MVAPICHRunner, SlurmRunner, MPICHRunner, IMPIRunner
+from .constants import PDSH_LAUNCHER, OPENMPI_LAUNCHER, MVAPICH_LAUNCHER, SLURM_LAUNCHER, MPICH_LAUNCHER, IMPI_LAUNCHER
 from ..constants import TORCH_DISTRIBUTED_DEFAULT_PORT
 from ..nebula.constants import NEBULA_EXPORT_ENVS
 from ..utils import logger
 
 from ..autotuning import Autotuner
 from deepspeed.accelerator import get_accelerator
 
 DLTS_HOSTFILE = "/job/hostfile"
 EXPORT_ENVS = ['MLFLOW', 'NCCL', 'PYTHON', 'MV2', 'UCX']
 EXPORT_ENVS += NEBULA_EXPORT_ENVS
 DEEPSPEED_ENVIRONMENT_NAME = ".deepspeed_env"
 DEEPSPEED_ENVIRONMENT_PATHS = [os.path.expanduser("~"), '.']
 PDSH_MAX_FAN_OUT = 1024
 
+# On AISC compute, each node sets environment variables independently, want to prevent
+# exporting rank-0 env variables in case of heterogeneous compute.
+EXCLUDE_ENVS = {'AISC_JOB_NAME': ['NCCL_IB_HCA', 'UCX_NET_DEVICES']}
+
 
 def parse_args(args=None):
     parser = argparse.ArgumentParser(description="DeepSpeed runner to help launch distributed "
                                      "multi-node/multi-gpu training jobs.",
                                      formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("-H",
@@ -91,14 +95,15 @@
     parser.add_argument("--max_elastic_nodes",
                         type=int,
                         default=-1,
                         help="Maximum number of nodes to run elastic training on. "
                         "Default is num_nodes when elastic training is enabled")
 
     parser.add_argument("--num_gpus",
+                        "--num_accelerators",
                         type=int,
                         default=-1,
                         help="Max number of GPUs to use on each node, will use "
                         "[0:N) GPU ids on each node.")
 
     parser.add_argument("--master_port",
                         default=TORCH_DISTRIBUTED_DEFAULT_PORT,
@@ -112,15 +117,15 @@
                         help="(optional) IP address of node 0, will be "
                         "inferred via 'hostname -I' if not specified.")
 
     parser.add_argument("--launcher",
                         default=PDSH_LAUNCHER,
                         type=str,
                         help="(optional) choose launcher backend for multi-node "
-                        "training. Options currently include PDSH, OpenMPI, MVAPICH, SLURM, MPICH.")
+                        "training. Options currently include PDSH, OpenMPI, MVAPICH, SLURM, MPICH, IMPI.")
 
     parser.add_argument("--launcher_args",
                         default="",
                         type=str,
                         help="(optional) pass launcher specific arguments as a "
                         "single quoted argument.")
 
@@ -500,14 +505,16 @@
         args.launcher = args.launcher.lower()
         if args.launcher == PDSH_LAUNCHER:
             runner = PDSHRunner(args, world_info_base64)
         elif args.launcher == OPENMPI_LAUNCHER:
             runner = OpenMPIRunner(args, world_info_base64, resource_pool)
         elif args.launcher == MPICH_LAUNCHER:
             runner = MPICHRunner(args, world_info_base64, resource_pool)
+        elif args.launcher == IMPI_LAUNCHER:
+            runner = IMPIRunner(args, world_info_base64, resource_pool)
         elif args.launcher == MVAPICH_LAUNCHER:
             runner = MVAPICHRunner(args, world_info_base64, resource_pool)
         elif args.launcher == SLURM_LAUNCHER:
             runner = SlurmRunner(args, world_info_base64, resource_pool)
         else:
             raise NotImplementedError(f"Unknown launcher {args.launcher}")
 
@@ -516,18 +523,25 @@
 
         curr_path = os.path.abspath('.')
         if 'PYTHONPATH' in env:
             env['PYTHONPATH'] = curr_path + ":" + env['PYTHONPATH']
         else:
             env['PYTHONPATH'] = curr_path
 
+        excluded_vars = []
+        for exclude_key, var_list in EXCLUDE_ENVS.items():
+            if exclude_key in env.keys():
+                # key exists in launcher env -> var list should be used
+                excluded_vars += var_list
+
         exports = ""
         for var in env.keys():
             if any([var.startswith(name) for name in EXPORT_ENVS]):
-                runner.add_export(var, env[var])
+                if not any([var == name for name in excluded_vars]):
+                    runner.add_export(var, env[var])
 
         for environ_path in DEEPSPEED_ENVIRONMENT_PATHS:
             environ_file = os.path.join(environ_path, DEEPSPEED_ENVIRONMENT_NAME)
             if os.path.isfile(environ_file):
                 with open(environ_file, 'r') as fd:
                     for var in fd.readlines():
                         key, val = var.split('=', maxsplit=1)
```

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/diffusers/unet.py` & `deepspeed-0.9.3/deepspeed/model_implementations/diffusers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/diffusers/vae.py` & `deepspeed-0.9.3/deepspeed/model_implementations/diffusers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/features/cuda_graph.py` & `deepspeed-0.9.3/deepspeed/model_implementations/features/cuda_graph.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/clip_encoder.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bert.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bloom.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_gpt.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_megatron_gpt.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_opt.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_transformer.py` & `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from deepspeed.utils.logging import log_dist
 
 from deepspeed.ops.transformer.inference.ds_mlp import DeepSpeedMLP
 from deepspeed.ops.transformer.inference.ds_attention import DeepSpeedSelfAttention, BloomSelfAttention
 from deepspeed.accelerator import get_accelerator
 from deepspeed.ops.op_builder import InferenceBuilder
 
-inference_cuda_module = None
+inference_module = None
 
 
 class DeepSpeedTransformerInference(nn.Module):
     """Initialize the DeepSpeed Transformer Layer.
         Arguments:
             layer_id: The layer index starting from 0, e.g. if model has 24 transformer layers,
                 layer_id will be 0,1,2...23 when each layer object is instantiated
@@ -43,19 +43,19 @@
                  mlp_extra_grouping=False):
         super(DeepSpeedTransformerInference, self).__init__()
 
         self.config = config
         self.config.layer_id = DeepSpeedTransformerInference.layer_id
         DeepSpeedTransformerInference.layer_id += 1
 
-        data_type = torch.half if config.fp16 else torch.float
-        global inference_cuda_module
-        if inference_cuda_module is None:
+        data_type = torch.half if self.config.dtype == torch.int8 else self.config.dtype
+        global inference_module
+        if inference_module is None:
             builder = InferenceBuilder()
-            inference_cuda_module = builder.load()
+            inference_module = builder.load()
 
         if DeepSpeedTransformerInference.layer_id == 1:
             log_dist(f"DeepSpeed-Inference config: {self.config.__dict__}", [0])
 
         if self.config.bigscience_bloom:
             self.attention = BloomSelfAttention(self.config, mp_group, quantize_scales, quantize_groups, merge_count)
         else:
@@ -70,22 +70,30 @@
             self.norm_b = None
         else:
             self.norm_w = nn.Parameter(torch.empty(self.config.hidden_size, dtype=data_type, device=device),
                                        requires_grad=False)
             self.norm_b = nn.Parameter(torch.empty(self.config.hidden_size, dtype=data_type, device=device),
                                        requires_grad=False)
         self.layer_past = None
-        self.allocate_workspace = inference_cuda_module.allocate_workspace_fp32 if (not config.fp16) else \
-                                inference_cuda_module.allocate_workspace_fp16
-        self._alloc_workspace = True
+        try:
+            if config.dtype == torch.float32:
+                self.allocate_workspace = inference_module.allocate_workspace_fp32
+            elif config.dtype == torch.bfloat16:
+                self.allocate_workspace = inference_module.allocate_workspace_bf16
+            else:
+                self.allocate_workspace = inference_module.allocate_workspace_fp32
+            self._alloc_workspace = True
+        except AttributeError:
+            self.allocate_workspace = None
+            self._alloc_workspace = False
 
     @classmethod
     def reset_cache(cls):
-        if inference_cuda_module is not None:
-            inference_cuda_module.reset_cache()
+        if inference_module is not None:
+            inference_module.reset_cache()
 
     def forward(
             self,
             input=None,
             input_mask=None,
             attention_mask=None,
             attn_mask=None,
@@ -135,17 +143,19 @@
 
         attn_mask = None
         if isinstance(input, tuple):
             attn_mask = input[1]
             input = input[0]
         input_type = input.dtype
 
-        if (self.config.fp16 or self.config.q_int8) \
+        if (self.config.dtype in [torch.float16, torch.bfloat16, torch.int8]) \
             and input.dtype == torch.float:
-            input = input.half()
+            target_dtype = torch.half if self.dtype == torch.int8 else self.dtype
+            input = input.to(target_dtype)
+
         with torch.no_grad():
             attention_output, key, value, context_outputtn_ctx, inp_norm = \
                                      self.attention(input,
                                               input_mask,
                                               head_mask,
                                               layer_past,
                                               get_present,
@@ -157,15 +167,15 @@
                                               alibi)
 
             presents = (key, value)
             self.layer_past = presents if layer_past is None else None
             output = self.mlp(attention_output, input, inp_norm, self.attention.attn_ob)
 
             if not self.config.pre_layer_norm:
-                output = inference_cuda_module.layer_norm(output, self.norm_w, self.norm_b, self.config.epsilon)
+                output = inference_module.layer_norm(output, self.norm_w, self.norm_b, self.config.epsilon)
 
             output = output.to(input_type)
         if get_present:
             output = (output, presents)
 
         if self.config.return_single_tuple:
             return (output, )
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/auto_tp.py` & `deepspeed-0.9.3/deepspeed/module_inject/auto_tp.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,18 @@
                     layer_list = layer_list + AutoTP.get_layers(key, submodule)
             for i, layer in enumerate(layer_list):
                 if layer == 'ln':
                     if layer_list[i - 1] != 'ln':
                         gem_list = gem_list + [layer_list[i - 1]]
                 elif 'out_proj' in layer:
                     gem_list = gem_list + [layer]
+                elif 'o_proj' in layer:
+                    gem_list = gem_list + [layer]
+                elif 'down_proj' in layer:
+                    gem_list = gem_list + [layer]
             layer_list = []
             if gem_list != []:
                 gem_list = list(set(gem_list))
                 policy_list = AutoTP.update_policy_list(policy_list, module, gem_list)
                 gem_list = []
         assert len(policy_list), "AutoTP not supported for model. Please use kernel injection since container policy for model exists." \
         if AutoTP.kernel_supported(module_list) else "Not able to determine model policy automatically. Please provide policy."
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/__init__.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 from .bert import DS_BERTContainer, HFBertLayerPolicy
 from .bloom import DS_BloomContainer, BLOOMLayerPolicy, supported_models
 from .distil_bert import DS_DistilBERTContainer, HFDistilBertLayerPolicy
 from .gpt2 import DS_GPT2Container, HFGPT2LayerPolicy
 from .gptj import DS_GPTJContainer, HFGPTJLayerPolicy
 from .gptneo import DS_GPTNEOContainer, HFGPTNEOLayerPolicy
 from .gptneox import DS_GPTNEOXContainer, GPTNEOXLayerPolicy
+from .llama import DS_LLAMAContainer, LLAMALayerPolicy
 from .megatron_gpt import DS_MegatronGPTContainer, MegatronLayerPolicy
 from .megatron_gpt_moe import DS_MegatronGPTMoEContainer, MegatronMoELayerPolicy
 from .opt import DS_OPTContainer, HFOPTLayerPolicy
 from .clip import DS_CLIPContainer, HFCLIPLayerPolicy
 from .unet import UNetPolicy
 from .vae import VAEPolicy
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/base_moe.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/base_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/bert.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,16 @@
     def get_hidden_heads(self):
         if self.pre_attn_norm:
             attention_layernorm = self.client_module.PostAttentionLayerNorm
         else:
             attention_layernorm = self.client_module.attention.output.LayerNorm
         return self.client_module.attention.self.query.weight.shape[1], \
                 self.client_module.attention.self.num_attention_heads, \
-                attention_layernorm.eps
-
-    def get_q_k_v(self):
-        return None
+                attention_layernorm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         qw = self.client_module.attention.self.query.weight
         qb = self.client_module.attention.self.query.bias
         kw = self.client_module.attention.self.key.weight
         kb = self.client_module.attention.self.key.bias
         vw = self.client_module.attention.self.value.weight
@@ -67,15 +65,15 @@
         qkvb = Parameter(torch.cat((qb, kb, vb), dim=0), requires_grad=enable_training)
 
         return qkvw, \
                qkvb, \
                self.client_module.attention.output.dense.weight, \
                self.client_module.attention.output.dense.bias, \
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         if self.pre_attn_norm:
             intermediate_ff = self.client_module.intermediate.dense_act
         else:
             intermediate_ff = self.client_module.intermediate.dense
 
         return intermediate_ff.weight, intermediate_ff.bias, \
             self.client_module.output.dense.weight, \
@@ -88,10 +86,7 @@
         else:
             attention_layernorm = self.client_module.attention.output.LayerNorm
             transformer_layernorm = self.client_module.output.LayerNorm
         return attention_layernorm.weight, \
                attention_layernorm.bias, \
                transformer_layernorm.weight, \
                transformer_layernorm.bias
-
-    def get_lora_params(self):
-        return []
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/bloom.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/bloom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from .base import *
 from .features.meta_tensor import MetaTensorContainer
+from .features.hybrid_engine import HybridEngineContainer
 from deepspeed.model_implementations.transformers.ds_bloom import DeepSpeedBloomInference
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 
 from ..policy import maybe_get_lora
 
 supported_models = {None}
 
 
-class DS_BloomContainer(MetaTensorContainer, BaseTransformerContainer):
+class DS_BloomContainer(MetaTensorContainer, HybridEngineContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
         self.bigscience_bloom = True
 
@@ -30,14 +31,25 @@
         self.module.config.scale_attention = self.scale_attention
         return self.module
 
     def attention_qkv_mp(self, mp_replace, reversed_dim=False):
         self.module.attention.attn_qkvw = mp_replace.copy(self.module.attention.attn_qkvw, self.qkvw)
         self.module.attention.attn_qkvb = mp_replace.copy(self.module.attention.attn_qkvb, self.qkvb)
 
+    def set_lora_params(self):
+        """
+        Necessary to implement for `HybridEngineContainer`
+        """
+        self.lora_params = [
+            maybe_get_lora(p) for p in [
+                self.policy.client_module.mlp.dense_h_to_4h, self.policy.client_module.mlp.dense_4h_to_h, self.policy.
+                client_module.self_attention.query_key_value, self.policy.client_module.self_attention.dense
+            ]
+        ]
+
     def load_params(self, module, sd, weight_quantizer, mp_replace, prefix):
         param_names = (
             'self_attention.query_key_value.weight', \
             'self_attention.query_key_value.bias', \
             'self_attention.dense.weight', \
             'self_attention.dense.bias', \
             'mlp.dense_h_to_4h.weight', \
@@ -83,40 +95,27 @@
         except Exception as e:
             print(f"WARNING! Setting BLOOMLayerPolicy._orig_layer_class to None due to Exception: {e}")
             BLOOMLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
         return self.client_module.self_attention.hidden_size, \
                 self.client_module.self_attention.num_heads, \
-                self.client_module.input_layernorm.eps
-
-    def get_q_k_v(self):
-        return None
+                self.client_module.input_layernorm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         return self.client_module.self_attention.query_key_value.weight, \
                 self.client_module.self_attention.query_key_value.bias, \
                 self.client_module.self_attention.dense.weight, \
                 self.client_module.self_attention.dense.bias,
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         return self.client_module.mlp.dense_h_to_4h.weight, \
                self.client_module.mlp.dense_h_to_4h.bias, \
                self.client_module.mlp.dense_4h_to_h.weight, \
                self.client_module.mlp.dense_4h_to_h.bias
 
     def layernorm(self):
         return self.client_module.post_attention_layernorm.weight, \
                self.client_module.post_attention_layernorm.bias, \
                self.client_module.input_layernorm.weight, \
                self.client_module.input_layernorm.bias
-
-    def get_lora_params(self):
-        all_lora_params = []
-        for p in [
-            self.client_module.mlp.dense_h_to_4h, \
-            self.client_module.mlp.dense_4h_to_h, \
-            self.client_module.self_attention.query_key_value, \
-            self.client_module.self_attention.dense
-            ]:
-            all_lora_params.append(maybe_get_lora(p))
-        return all_lora_params
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/clip.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,42 +37,37 @@
                 HFCLIPLayerPolicy._orig_layer_class = transformers.models.clip.modeling_clip.CLIPEncoderLayer
             except:
                 HFCLIPLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
         return self.client_module.self_attn.q_proj.weight.shape[1], \
                 self.client_module.self_attn.num_heads, \
-                self.client_module.layer_norm1.eps
+                self.client_module.layer_norm1.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
-    def get_q_k_v(self):
-        return None
-
-    def attention(self):
+    def attention(self, enable_training=False):
         qw = self.client_module.self_attn.q_proj.weight
         qb = self.client_module.self_attn.q_proj.bias
         kw = self.client_module.self_attn.k_proj.weight
         kb = self.client_module.self_attn.k_proj.bias
         vw = self.client_module.self_attn.v_proj.weight
         vb = self.client_module.self_attn.v_proj.bias
 
-        qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=False)
-        qkvb = Parameter(torch.cat((qb, kb, vb), dim=0), requires_grad=False)
+        qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
+        qkvb = Parameter(torch.cat((qb, kb, vb), dim=0), requires_grad=enable_training)
 
         return qkvw, \
                qkvb, \
                self.client_module.self_attn.out_proj.weight, \
                self.client_module.self_attn.out_proj.bias
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         return self.client_module.mlp.fc1.weight, \
                self.client_module.mlp.fc1.bias, \
                self.client_module.mlp.fc2.weight, \
                self.client_module.mlp.fc2.bias
 
     def layernorm(self):
         return self.client_module.layer_norm2.weight, \
                self.client_module.layer_norm2.bias, \
                self.client_module.layer_norm1.weight, \
                self.client_module.layer_norm1.bias
-
-    def get_lora_params(self):
-        return []
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/distil_bert.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/distil_bert.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,16 @@
                 ]
             except:
                 HFDistilBertLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
         return self.client_module.attention.q_lin.weight.shape[1], \
                 self.client_module.attention.n_heads, \
-                self.client_module.sa_layer_norm.eps
-
-    def get_q_k_v(self):
-        return None
+                self.client_module.sa_layer_norm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         qw = self.client_module.attention.q_lin.weight
         qb = self.client_module.attention.q_lin.bias
         kw = self.client_module.attention.k_lin.weight
         kb = self.client_module.attention.k_lin.bias
         vw = self.client_module.attention.v_lin.weight
@@ -63,24 +61,21 @@
         qkvb = Parameter(torch.cat((qb, kb, vb), dim=0), requires_grad=enable_training)
 
         return qkvw, \
                qkvb, \
                self.client_module.attention.out_lin.weight, \
                self.client_module.attention.out_lin.bias
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         intermediate_ff = self.client_module.ffn.lin1
 
         return intermediate_ff.weight, intermediate_ff.bias, \
             self.client_module.ffn.lin2.weight, \
             self.client_module.ffn.lin2.bias
 
     def layernorm(self):
         attention_layernorm = self.client_module.sa_layer_norm
         transformer_layernorm = self.client_module.output_layer_norm
         return attention_layernorm.weight, \
                attention_layernorm.bias, \
                transformer_layernorm.weight, \
                transformer_layernorm.bias
-
-    def get_lora_params(self):
-        return []
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/features/megatron.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_megatron.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,87 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 import torch
-from abc import ABC
 
+from .hybrid_engine import HybridEngineContainer
+from .megatron import MegatronContainer
 
-class MegatronContainer(ABC):
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.megatron_v2 = self.policy.is_megatron_v2
+class HybridMegatronContainer(MegatronContainer, HybridEngineContainer):
 
-    def _align_qkv_transposed(self, x):
-        attention_head_size = x.shape[-1] // self.num_attention_heads
-        new_x_shape = x.size()[:-1] + (self.num_attention_heads, attention_head_size)
-        x_1 = x.view(*new_x_shape)
-        (q, k, v) = torch.split(x_1, (x_1.shape[-1] // 3), dim=(x_1.dim() - 1))
-        if len(q.shape) > 2:
-            return torch.cat((q.reshape(q.shape[0], -1), k.reshape(q.shape[0], -1), v.reshape(q.shape[0], -1)),
-                             dim=-1).reshape(x.shape)
-        else:
-            return torch.cat((q.reshape(-1), k.reshape(-1), v.reshape(-1)), dim=-1).reshape(x.shape)
-
-    def _align_qkv(self, x):
+    def _align_qkv(self, x: torch.Tensor):
+        """
+        Internal helper for accepting the head-contiguous weight matrix and chunking
+        the query, key, and value components.
+        """
         attention_head_size = x.shape[0] // self.num_attention_heads
         new_x_shape = (self.num_attention_heads, attention_head_size) + x.size()[1:]
         x_1 = x.view(*new_x_shape)
         div_dim = len(x_1.size()) - 2 if len(x.shape) == 2 else -1
         (q, k, v) = torch.split(x_1, (x_1.shape[div_dim] // 3), dim=div_dim)
         if len(q.shape) > 2:
             x.data.copy_(
                 torch.cat((q.reshape(-1, q.shape[-1]), k.reshape(-1, q.shape[-1]), v.reshape(-1, q.shape[-1])),
                           dim=0).reshape(x.shape))
         else:
             x.data.copy_(torch.cat((q.reshape(-1), k.reshape(-1), v.reshape(-1)), dim=-1).reshape(x.shape))
 
-    def _align_merged_qkv(self):
+    def transform_for_inference(self) -> None:
+        """
+        Overrides the HybridEngineContainer implementation.
+
+        The alternative layout of the QKV matrix for Megatron is such that each head's Q, K, and V
+        are sequential in memory. This is different from the default layout in which all of the Qs
+        are sequential, followed by all of the Ks, and then all of the Vs. Here, we take the default
+        layout and transform it to the inference layout.
+        """
         if hasattr(self.qkvw, 'ds_id'):
             from deepspeed.runtime.zero import GatheredParameters
             from deepspeed.runtime.zero.partition_parameters import ZeroParamStatus
             param_list = [self.qkvw, self.qkvb]
             non_active_params = [param for param in param_list if (hasattr(param, 'ds_id') and \
                             param.ds_status == ZeroParamStatus.NOT_AVAILABLE)]
             with GatheredParameters(non_active_params):
                 self._align_qkv(self.qkvw)
                 self._align_qkv(self.qkvb)
         else:
             self._align_qkv(self.qkvw)
             self._align_qkv(self.qkvb)
 
-    def _partition_qkv(self, x):
+    def _partition_qkv(self, x: torch.Tensor):
+        """
+        Internal helper for taking contiguous QKV and partitioning it for contiguous
+        heads.
+        """
         q_k_v = torch.split(x, (x.shape[0] // 3), dim=0)
         attention_head_size = q_k_v[0].shape[0] // self.num_attention_heads
         new_x_shape = (self.num_attention_heads, attention_head_size) + x.size()[1:]
         q, k, v = [data.view(*new_x_shape) for data in q_k_v]
         if len(q.shape) > 2:
             x.data.copy_(torch.cat((q, k, v), dim=-2).reshape(-1, q.shape[-1]))
         else:
             x.data.copy_(torch.cat((q, k, v), dim=-1).reshape(-1))
 
-    def _partition_merged_qkv(self):
+    def transform_for_training(self):
+        """
+        Overrides the HybridEngineContainer implementation.
+
+        The alternative layout of the QKV matrix for Megatron is such that each head's Q, K, and V
+        are sequential in memory. This is different from the default layout in which all of the Qs
+        are sequential, followed by all of the Ks, and then all of the Vs. This function takes the inference format and reverts it back to the default format.
+        """
+        # If parameter is distributed, handle gathering it
         if hasattr(self.qkvw, 'ds_id'):
             from deepspeed.runtime.zero import GatheredParameters
             from deepspeed.runtime.zero.partition_parameters import ZeroParamStatus
             param_list = [self.qkvw, self.qkvb]
             non_active_params = [param for param in param_list if (hasattr(param, 'ds_id') and \
                             param.ds_status == ZeroParamStatus.NOT_AVAILABLE)]
             with GatheredParameters(non_active_params):
                 self._partition_qkv(self.qkvw)
                 self._partition_qkv(self.qkvb)
         else:
             self._partition_qkv(self.qkvw)
             self._partition_qkv(self.qkvb)
-
-    def transpose(self):
-        super().transpose()
-        if self.megatron_v2:
-            self.qkvw = torch.nn.parameter.Parameter(self._align_qkv_transposed(self.qkvw).contiguous())
-            self.qkvb = torch.nn.parameter.Parameter(self._align_qkv_transposed(self.qkvb).contiguous())
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/gpt2.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/gpt2.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,32 +34,27 @@
             HFGPT2LayerPolicy._orig_layer_class = transformers.models.gpt2.modeling_gpt2.GPT2Block
         except:
             HFGPT2LayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
         return self.client_module.attn.embed_dim, \
                 self.client_module.attn.num_heads, \
-                self.client_module.ln_1.eps
-
-    def get_q_k_v(self):
-        return None
+                self.client_module.ln_1.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         return  self.client_module.attn.c_attn.weight, \
                 self.client_module.attn.c_attn.bias, \
                 self.client_module.attn.c_proj.weight, \
                 self.client_module.attn.c_proj.bias
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         return self.client_module.mlp.c_fc.weight, \
                self.client_module.mlp.c_fc.bias, \
                self.client_module.mlp.c_proj.weight, \
                self.client_module.mlp.c_proj.bias
 
     def layernorm(self):
         return self.client_module.ln_2.weight, \
                self.client_module.ln_2.bias, \
                self.client_module.ln_1.weight, \
                self.client_module.ln_1.bias
-
-    def get_lora_params(self):
-        return []
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/gptj.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/gptneo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,125 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from .base import *
 from .features.meta_tensor import MetaTensorContainer
+from .features.hybrid_engine import HybridEngineContainer
 from deepspeed.model_implementations.transformers.ds_gpt import DeepSpeedGPTInference
 import torch
 from torch.nn.parameter import Parameter
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from ..policy import maybe_copy_qkv
 
 from ..policy import maybe_get_lora
 
 
-class DS_GPTJContainer(MetaTensorContainer, BaseTransformerContainer):
+class DS_GPTNEOContainer(MetaTensorContainer, HybridEngineContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
 
     def create_module(self, config=None):
         _config = config if config is not None else self.ds_model_config
         self.module = DeepSpeedGPTInference(_config, mp_group=self.mp_group)
         self.module.config.scale_attention = self.scale_attention
         return self.module
 
+    def set_lora_params(self):
+        """
+        Necessary to implement for `HybridEngineContainer`
+        """
+        self.lora_params = [
+            maybe_get_lora(p) for p in [
+                self.policy.client_module.mlp.c_fc, self.policy.client_module.mlp.c_proj,
+                self.policy.client_module.attn.attention.q_proj, self.policy.client_module.attn.attention.k_proj,
+                self.policy.client_module.attn.attention.v_proj, self.policy.client_module.attn.attention.out_proj
+            ]
+        ]
+
     def load_params(self, module, sd, weight_quantizer, mp_replace, prefix):
         param_names = (
-            'attn.q_proj.weight', \
-            'attn.k_proj.weight', \
-            'attn.v_proj.weight', \
-            'attn.out_proj.weight', \
-            'mlp.fc_in.weight', \
-            'mlp.fc_in.bias', \
-            'mlp.fc_out.weight', \
-            'mlp.fc_out.bias', \
+            'attn.attention.q_proj.weight', \
+            'attn.attention.k_proj.weight', \
+            'attn.attention.v_proj.weight', \
+            'attn.attention.out_proj.weight', \
+            'attn.attention.out_proj.bias', \
+            'mlp.c_fc.weight', \
+            'mlp.c_fc.bias', \
+            'mlp.c_proj.weight', \
+            'mlp.c_proj.bias', \
+            'ln_2.weight', \
+            'ln_2.bias', \
             'ln_1.weight', \
             'ln_1.bias'
         )
         maybe_copy_qkv(module.attention,
                        sd,
                        weight_quantizer,
                        mp_replace,
                        'attn_qkvw', [prefix + param_names[0], prefix + param_names[1], prefix + param_names[2]],
                        split_qkv=self.policy.split_qkv)
-        for i in range(3, 4):
+        for i in range(3, 5):
             maybe_copy(module.attention, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
                        prefix + param_names[i])
-        for i in range(4, 8):
-            maybe_copy(module.mlp, sd, weight_quantizer, mp_replace, transformer_param_names[i],
+        for i in range(5, 11):
+            maybe_copy(module.mlp, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
                        prefix + param_names[i])
-        for i in range(8, 10):
-            maybe_copy(module, sd, weight_quantizer, mp_replace, transformer_param_names[i + 2],
+        for i in range(11, 13):
+            maybe_copy(module, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
                        prefix + param_names[i])
 
 
-class HFGPTJLayerPolicy(TransformerPolicy):
-    _orig_layer_class = None
+class HFGPTNEOLayerPolicy(TransformerPolicy):
 
     def __init__(self, client_module, inference=True):
-        super().__init__(inference, scale_attention=True)
+        super().__init__(inference, scale_attention=False)
         self.client_module = client_module
         try:
             import transformers
-            HFGPTJLayerPolicy._orig_layer_class = transformers.models.gptj.modeling_gptj.GPTJBlock
+            HFGPTNEOLayerPolicy._orig_layer_class = transformers.models.gpt_neo.modeling_gpt_neo.GPTNeoBlock
         except:
-            HFGPTJLayerPolicy._orig_layer_class = None
+            HFGPTNEOLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
-        return self.client_module.attn.embed_dim, \
-                self.client_module.attn.num_attention_heads, \
-                self.client_module.ln_1.eps
+        return self.client_module.attn.attention.embed_dim, \
+                self.client_module.attn.attention.num_heads, \
+                self.client_module.ln_1.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def get_q_k_v(self):
-        return self.client_module.attn.q_proj.weight, \
+        return self.client_module.attn.attention.q_proj.weight, \
                None, \
-               self.client_module.attn.k_proj.weight, \
+               self.client_module.attn.attention.k_proj.weight, \
                None, \
-               self.client_module.attn.v_proj.weight, \
+               self.client_module.attn.attention.v_proj.weight, \
                None
 
     def attention(self, enable_training=False):
-        qw = self.client_module.attn.q_proj.weight
-        kw = self.client_module.attn.k_proj.weight
-        vw = self.client_module.attn.v_proj.weight
+        qw = self.client_module.attn.attention.q_proj.weight
+        kw = self.client_module.attn.attention.k_proj.weight
+        vw = self.client_module.attn.attention.v_proj.weight
 
         qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
 
         return qkvw, \
                None, \
-               self.client_module.attn.out_proj.weight, \
-               None,
+               self.client_module.attn.attention.out_proj.weight, \
+               self.client_module.attn.attention.out_proj.bias
 
-    def mlp(self):
-        return self.client_module.mlp.fc_in.weight, \
-               self.client_module.mlp.fc_in.bias, \
-               self.client_module.mlp.fc_out.weight, \
-               self.client_module.mlp.fc_out.bias
+    def mlp(self, enable_training=False):
+        return self.client_module.mlp.c_fc.weight, \
+               self.client_module.mlp.c_fc.bias, \
+               self.client_module.mlp.c_proj.weight, \
+               self.client_module.mlp.c_proj.bias
 
     def layernorm(self):
-        return None, \
-               None, \
+        return self.client_module.ln_2.weight, \
+               self.client_module.ln_2.bias, \
                self.client_module.ln_1.weight, \
                self.client_module.ln_1.bias
-
-    def get_lora_params(self):
-        all_lora_params = []
-        for p in [
-            self.client_module.mlp.fc_in, \
-            self.client_module.mlp.fc_out, \
-            self.client_module.attn.q_proj, \
-            self.client_module.attn.k_proj, \
-            self.client_module.attn.v_proj, \
-            self.client_module.attn.out_proj, \
-            ]:
-            all_lora_params.append(maybe_get_lora(p))
-        return all_lora_params
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/gptneo.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/opt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,154 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from .base import *
-from .features.meta_tensor import MetaTensorContainer
-from deepspeed.model_implementations.transformers.ds_gpt import DeepSpeedGPTInference
+from .features import MetaTensorContainer, HybridSplitQKVContainer
+from deepspeed.model_implementations.transformers.ds_opt import DeepSpeedOPTInference
 import torch
 from torch.nn.parameter import Parameter
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from ..policy import maybe_copy_qkv
-
 from ..policy import maybe_get_lora
+from deepspeed.utils.types import ActivationFuncType
 
 
-class DS_GPTNEOContainer(MetaTensorContainer, BaseTransformerContainer):
+class DS_OPTContainer(MetaTensorContainer, HybridSplitQKVContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
 
     def create_module(self, config=None):
         _config = config if config is not None else self.ds_model_config
-        self.module = DeepSpeedGPTInference(_config, mp_group=self.mp_group)
+        self.module = DeepSpeedOPTInference(_config, mp_group=self.mp_group)
         self.module.config.scale_attention = self.scale_attention
         return self.module
 
+    def set_lora_params(self):
+        """
+        Necessary to implement for `HybridEngineContainer`
+        """
+        self.lora_params = [
+            maybe_get_lora(p) for p in [
+                self.policy.client_module.fc1,
+                self.policy.client_module.fc2,
+                self.policy.client_module.self_attn.q_proj,
+                self.policy.client_module.self_attn.k_proj,
+                self.policy.client_module.self_attn.v_proj,
+                self.policy.client_module.self_attn.out_proj,
+            ]
+        ]
+
+    def set_q_k_v(self):
+        """
+        Necessary to implement for `HybridSplitQKVContainer`
+        """
+        self.qw = self.policy.client_module.self_attn.q_proj.weight
+        self.qb = self.policy.client_module.self_attn.q_proj.bias
+        self.kw = self.policy.client_module.self_attn.k_proj.weight
+        self.kb = self.policy.client_module.self_attn.k_proj.bias
+        self.vw = self.policy.client_module.self_attn.v_proj.weight
+        self.vb = self.policy.client_module.self_attn.v_proj.bias
+
     def load_params(self, module, sd, weight_quantizer, mp_replace, prefix):
         param_names = (
-            'attn.attention.q_proj.weight', \
-            'attn.attention.k_proj.weight', \
-            'attn.attention.v_proj.weight', \
-            'attn.attention.out_proj.weight', \
-            'attn.attention.out_proj.bias', \
-            'mlp.c_fc.weight', \
-            'mlp.c_fc.bias', \
-            'mlp.c_proj.weight', \
-            'mlp.c_proj.bias', \
-            'ln_2.weight', \
-            'ln_2.bias', \
-            'ln_1.weight', \
-            'ln_1.bias'
+            'self_attn.q_proj.weight', \
+            'self_attn.k_proj.weight', \
+            'self_attn.v_proj.weight', \
+            'self_attn.q_proj.bias', \
+            'self_attn.k_proj.bias', \
+            'self_attn.v_proj.bias', \
+            'self_attn.out_proj.weight', \
+            'self_attn.out_proj.bias', \
+            'fc1.weight', \
+            'fc1.bias', \
+            'fc2.weight', \
+            'fc2.bias', \
+            'final_layer_norm.weight', \
+            'final_layer_norm.bias', \
+            'self_attn_layer_norm.weight', \
+            'self_attn_layer_norm.bias'
         )
-        maybe_copy_qkv(module.attention,
-                       sd,
-                       weight_quantizer,
-                       mp_replace,
-                       'attn_qkvw', [prefix + param_names[0], prefix + param_names[1], prefix + param_names[2]],
-                       split_qkv=self.policy.split_qkv)
-        for i in range(3, 5):
-            maybe_copy(module.attention, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
+
+        for i in range(0, 6, 3):
+            maybe_copy_qkv(module.attention,
+                           sd,
+                           weight_quantizer,
+                           mp_replace,
+                           transformer_param_names[i // 3],
+                           [prefix + param_names[i], prefix + param_names[i + 1], prefix + param_names[i + 2]],
+                           split_qkv=self.policy.split_qkv)
+        for i in range(6, 8):
+            maybe_copy(module.attention, sd, weight_quantizer, mp_replace, transformer_param_names[i - 4],
                        prefix + param_names[i])
-        for i in range(5, 11):
-            maybe_copy(module.mlp, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
+        for i in range(8, 14):
+            maybe_copy(module.mlp, sd, weight_quantizer, mp_replace, transformer_param_names[i - 4],
                        prefix + param_names[i])
-        for i in range(11, 13):
-            maybe_copy(module, sd, weight_quantizer, mp_replace, transformer_param_names[i - 1],
+        for i in range(14, 16):
+            maybe_copy(module, sd, weight_quantizer, mp_replace, transformer_param_names[i - 4],
                        prefix + param_names[i])
 
 
-class HFGPTNEOLayerPolicy(TransformerPolicy):
+class HFOPTLayerPolicy(TransformerPolicy):
+    _orig_layer_class = None
 
-    def __init__(self, client_module, inference=True):
-        super().__init__(inference, scale_attention=False)
+    def __init__(self, client_module, inference=True, use_load_prefix=True):
+        super().__init__(inference, linear_layer=True, pre_attn_norm=True, use_load_prefix=use_load_prefix)
         self.client_module = client_module
         try:
             import transformers
-            HFGPTNEOLayerPolicy._orig_layer_class = transformers.models.gpt_neo.modeling_gpt_neo.GPTNeoBlock
+            HFOPTLayerPolicy._orig_layer_class = transformers.models.opt.modeling_opt.OPTDecoderLayer
         except:
-            HFGPTNEOLayerPolicy._orig_layer_class = None
+            HFOPTLayerPolicy._orig_layer_class = None
+
+        if hasattr(TransformerPolicy, "hf_model_config") and hasattr(TransformerPolicy.hf_model_config,
+                                                                     "activation_function"):
+            if TransformerPolicy.hf_model_config.activation_function == "relu":
+                self.mlp_act_func_type = ActivationFuncType.ReLU
+            elif TransformerPolicy.hf_model_config.activation_function in ["gelu", "gelu_new"]:
+                self.mlp_act_func_type = ActivationFuncType.GELU
+            else:
+                raise ValueError("Unsupported activation function: {}".format(
+                    TransformerPolicy.hf_model_config.activation_function))
+        else:
+            self.mlp_act_func_type = ActivationFuncType.ReLU  # default
 
     def get_hidden_heads(self):
-        return self.client_module.attn.attention.embed_dim, \
-                self.client_module.attn.attention.num_heads, \
-                self.client_module.ln_1.eps
-
-    def get_q_k_v(self):
-        return self.client_module.attn.attention.q_proj.weight, \
-               None, \
-               self.client_module.attn.attention.k_proj.weight, \
-               None, \
-               self.client_module.attn.attention.v_proj.weight, \
-               None
+        return self.client_module.self_attn.embed_dim, \
+                self.client_module.self_attn.num_heads, \
+                self.client_module.self_attn_layer_norm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
-        qw = self.client_module.attn.attention.q_proj.weight
-        kw = self.client_module.attn.attention.k_proj.weight
-        vw = self.client_module.attn.attention.v_proj.weight
+        qw = self.client_module.self_attn.q_proj.weight
+        qb = self.client_module.self_attn.q_proj.bias
 
-        qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
+        kw = self.client_module.self_attn.k_proj.weight
+        kb = self.client_module.self_attn.k_proj.bias
+
+        vw = self.client_module.self_attn.v_proj.weight
+        vb = self.client_module.self_attn.v_proj.bias
 
+        qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
+        qkvb = Parameter(torch.cat((qb, kb, vb), dim=0), requires_grad=enable_training)
         return qkvw, \
-               None, \
-               self.client_module.attn.attention.out_proj.weight, \
-               self.client_module.attn.attention.out_proj.bias
-
-    def mlp(self):
-        return self.client_module.mlp.c_fc.weight, \
-               self.client_module.mlp.c_fc.bias, \
-               self.client_module.mlp.c_proj.weight, \
-               self.client_module.mlp.c_proj.bias
+               qkvb, \
+               self.client_module.self_attn.out_proj.weight, \
+               self.client_module.self_attn.out_proj.bias
+
+    def mlp(self, enable_training=False):
+        return self.client_module.fc1.weight, \
+               self.client_module.fc1.bias, \
+               self.client_module.fc2.weight, \
+               self.client_module.fc2.bias
 
     def layernorm(self):
-        return self.client_module.ln_2.weight, \
-               self.client_module.ln_2.bias, \
-               self.client_module.ln_1.weight, \
-               self.client_module.ln_1.bias
-
-    def get_lora_params(self):
-        all_lora_params = []
-        for p in [
-            self.client_module.mlp.c_fc, \
-            self.client_module.mlp.c_proj, \
-            self.client_module.attn.attention.q_proj, \
-            self.client_module.attn.attention.k_proj, \
-            self.client_module.attn.attention.v_proj, \
-            self.client_module.attn.attention.out_proj, \
-            ]:
-            all_lora_params.append(maybe_get_lora(p))
-        return all_lora_params
+        return self.client_module.final_layer_norm.weight, \
+               self.client_module.final_layer_norm.bias, \
+               self.client_module.self_attn_layer_norm.weight, \
+               self.client_module.self_attn_layer_norm.bias
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/gptneox.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/gptneox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from .base import *
 from .features.meta_tensor import MetaTensorContainer
-from .features.megatron import MegatronContainer
+from .features.hybrid_megatron import HybridMegatronContainer
 from deepspeed.model_implementations.transformers.ds_gpt import DeepSpeedGPTInference
 import torch
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from packaging import version as pkg_version
 
 from ..policy import maybe_get_lora
 
 
-class DS_GPTNEOXContainer(MetaTensorContainer, MegatronContainer, BaseTransformerContainer):
+class DS_GPTNEOXContainer(MetaTensorContainer, HybridMegatronContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
 
     def create_module(self, config=None):
@@ -30,14 +30,30 @@
 
         if self.megatron_v2:
             self.module.config.rotate_half = True
             self.module.config.rotate_every_two = False
 
         return self.module
 
+    def set_lora_params(self):
+        """
+        Necessary to implement for `HybridEngineContainer`
+        """
+        if GPTNEOXLayerPolicy.version == 0:
+            attention = self.policy.client_module.attention
+        else:
+            attention = self.policy.client_module.self_attention
+
+        self.lora_params = [
+            maybe_get_lora(p) for p in [
+                self.policy.client_module.mlp.dense_h_to_4h, self.policy.client_module.mlp.dense_4h_to_h,
+                attention.query_key_value, attention.dense
+            ]
+        ]
+
     def load_params(self, module, sd, weight_quantizer, mp_replace, prefix):
         param_names = (
             'attention.query_key_value.weight', \
             'attention.query_key_value.bias', \
             'attention.dense.weight', \
             'attention.dense.bias', \
             'mlp.dense_h_to_4h.weight', \
@@ -91,50 +107,32 @@
         if GPTNEOXLayerPolicy.version == 0:
             attention = self.client_module.attention
         else:
             attention = self.client_module.self_attention
 
         return self.client_module.attention.hidden_size, \
                 self.client_module.attention.num_attention_heads, \
-                self.client_module.input_layernorm.eps
-
-    def get_q_k_v(self):
-        return None
+                self.client_module.input_layernorm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         if GPTNEOXLayerPolicy.version == 0:
             attention = self.client_module.attention
         else:
             attention = self.client_module.self_attention
 
         return attention.query_key_value.weight, \
                attention.query_key_value.bias, \
                attention.dense.weight, \
                attention.dense.bias
 
-    def mlp(self):
+    def mlp(self, enable_training=False):
         return self.client_module.mlp.dense_h_to_4h.weight, \
                self.client_module.mlp.dense_h_to_4h.bias, \
                self.client_module.mlp.dense_4h_to_h.weight, \
                self.client_module.mlp.dense_4h_to_h.bias
 
     def layernorm(self):
         return self.client_module.post_attention_layernorm.weight, \
                self.client_module.post_attention_layernorm.bias, \
                self.client_module.input_layernorm.weight, \
                self.client_module.input_layernorm.bias
-
-    def get_lora_params(self):
-        if GPTNEOXLayerPolicy.version == 0:
-            attention = self.client_module.attention
-        else:
-            attention = self.client_module.self_attention
-
-        all_lora_params = []
-        for p in [
-            self.client_module.mlp.dense_h_to_4h, \
-            self.client_module.mlp.dense_4h_to_h, \
-            attention.query_key_value, \
-            attention.dense
-            ]:
-            all_lora_params.append(maybe_get_lora(p))
-        return all_lora_params
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,32 +53,30 @@
                     MegatronLayerPolicy._orig_layer_class = ParallelTransformerLayer
                 except ImportError:
                     MegatronLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
         return self.client_module.attention.query_key_value.weight.shape[1], \
                 self.client_module.attention.num_attention_heads, \
-                self.client_module.input_layernorm.eps
-
-    def get_q_k_v(self):
-        return None
+                self.client_module.input_layernorm.eps, \
+                DEFAULT_INTERMEDIATE_SIZE
 
     def attention(self, enable_training=False):
         if self.inference:
             if MegatronLayerPolicy.version == 0:
                 attention = self.client_module.attention
             else:
                 attention = self.client_module.self_attention
 
         return attention.query_key_value.weight, \
                attention.query_key_value.bias, \
                attention.dense.weight, \
                attention.dense.bias
 
-    def mlp(self, moe_type='standard'):
+    def mlp(self, moe_type='standard', enable_training=False):
         from deepspeed.moe.utils import has_moe_layers
         moe, _ = has_moe_layers(self.client_module)
 
         if moe:
             moe_experts = self.client_module.mlp.deepspeed_moe.experts.deepspeed_experts if moe_type == 'standard' else \
                             self.client_module.mlp.moe.deepspeed_moe.experts.deepspeed_experts
             num_experts = len(moe_experts)
@@ -106,10 +104,7 @@
                    self.client_module.mlp.dense_4h_to_h.bias
 
     def layernorm(self):
         return self.client_module.post_attention_layernorm.weight, \
                self.client_module.post_attention_layernorm.bias, \
                self.client_module.input_layernorm.weight, \
                self.client_module.input_layernorm.bias
-
-    def get_lora_params(self):
-        return []
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt_moe.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     MegatronMoELayerPolicy._orig_layer_class = ParallelTransformerLayer
                 except ImportError:
                     MegatronMoELayerPolicy._orig_layer_class = None
 
     def get_num_experts(self):
         return self.num_experts
 
-    def mlp(self, moe_type='standard'):
+    def mlp(self, moe_type='standard', enable_training=False):
         # for now, all of this is tightly coupled to megatron-deepspeed moe implementation
         # todo: think and refactor this to be more general
 
         #from deepspeed.moe.utils import has_moe_layers
         #moe, _ = has_moe_layers(self.client_module)
 
         moe_experts = self.client_module.mlp.deepspeed_moe.experts.deepspeed_experts if moe_type == 'standard' else \
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/unet.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/containers/vae.py` & `deepspeed-0.9.3/deepspeed/module_inject/containers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/inject.py` & `deepspeed-0.9.3/deepspeed/module_inject/inject.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/layers.py` & `deepspeed-0.9.3/deepspeed/module_inject/layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,7 +106,28 @@
         # create positions depending on attention_mask
         positions = (torch.cumsum(attention_mask, dim=1).type_as(attention_mask) * attention_mask).long() - 1
 
         # cut positions if `past_key_values_length` is > 0
         positions = positions[:, past_key_values_length:]
 
         return super().forward(positions + self.offset)
+
+
+class RMSNormalize(nn.Module):
+
+    def __init__(self, dim=None, dtype=torch.float, eps=1e-5, weight=None):
+        super(RMSNormalize, self).__init__()
+        if weight is not None:
+            self.weight = weight
+        else:
+            self.weight = nn.Parameter(torch.ones(dim, dtype=dtype, device=get_accelerator().current_device_name()))
+
+        self.eps = eps
+
+    def forward(self, hidden_states):
+        variance = hidden_states.to(torch.float32).pow(2).mean(-1, keepdim=True)
+        hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
+        print(self.weight)
+        if self.weight.dtype in [torch.float16, torch.bfloat16]:
+            hidden_states = hidden_states.to(self.weight.dtype)
+
+        return hidden_states * self.weight
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/load_checkpoint.py` & `deepspeed-0.9.3/deepspeed/module_inject/load_checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from deepspeed.model_implementations.transformers.ds_bloom import DeepSpeedBloomInference
 from deepspeed.model_implementations.transformers.ds_gpt import DeepSpeedGPTInference
 from deepspeed.model_implementations.transformers.ds_bert import DeepSpeedBERTInference
 from deepspeed.model_implementations.transformers.ds_megatron_gpt import DeepSpeedMegatronGPTInference
 from deepspeed.model_implementations.transformers.ds_opt import DeepSpeedOPTInference
 
 import deepspeed.ops.transformer as transformer_inference
-from .layers import LinearLayer, Normalize, EmbeddingLayer, OPTEmbedding
+from .layers import LinearLayer, Normalize, EmbeddingLayer, OPTEmbedding, RMSNormalize
 import torch
 import gc
 from deepspeed.accelerator import get_accelerator
 import re
 
 
 def load_model_with_checkpoint(r_module,
@@ -171,14 +171,18 @@
                 load_parameters(child, prefix + n + '.')
         else:
             container.load_params(module, sd[0], weight_quantizer, mp_replace, prefix)
 
     try:
         import transformers
         OPTLearnedPositionalEmbedding = transformers.models.opt.modeling_opt.OPTLearnedPositionalEmbedding
+        if hasattr(transformers.models, "llama"):
+            LlamaRMSNorm = transformers.models.llama.modeling_llama.LlamaRMSNorm
+        else:
+            LlamaRMSNorm = None
     except:
         OPTLearnedPositionalEmbedding = None
     layer_policies = {
         nn.Linear: load,
         nn.Embedding: load,
         nn.LayerNorm: load,
         EmbeddingLayer: load,
@@ -187,15 +191,17 @@
         transformer_inference.DeepSpeedTransformerInference: load_transformer_layer,
         DeepSpeedBloomInference: load_transformer_layer,
         DeepSpeedGPTInference: load_transformer_layer,
         DeepSpeedBERTInference: load_transformer_layer,
         DeepSpeedMegatronGPTInference: load_transformer_layer,
         DeepSpeedOPTInference: load_transformer_layer,
         OPTLearnedPositionalEmbedding: load,
-        OPTEmbedding: load
+        OPTEmbedding: load,
+        LlamaRMSNorm: load,
+        RMSNormalize: load
     }
 
     all_ds_ids = {}
 
     def load_module_recursive(module, prefix='', level=0):
         for name, child in module.named_children():
             if child.__class__ in layer_policies:
@@ -220,14 +226,17 @@
                         setattr(module, name, child)
                     elif child.__class__ is nn.Linear:
                         child = LinearLayer(weight_shape=child.weight.shape, bias=child.bias)
                         setattr(module, name, child)
                     elif child.__class__ is OPTLearnedPositionalEmbedding:
                         child = OPTEmbedding(weight_shape=ds_shape)
                         setattr(module, name, child)
+                    elif child.__class__ is LlamaRMSNorm:
+                        child = RMSNormalize(dim=ds_shape[-1], dtype=child.weight.dtype, eps=child.variance_epsilon)
+                        setattr(module, name, child)
                     else:
                         ds_id = None
                         if hasattr(child.weight, 'ds_id'):
                             ds_id = child.weight.ds_id
                         child = EmbeddingLayer(weight_shape=ds_shape, dtype=child.weight.dtype)
                         if ds_id is not None:
                             all_ds_ids[ds_id] = child.weight
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/module_quantize.py` & `deepspeed-0.9.3/deepspeed/module_inject/module_quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/policy.py` & `deepspeed-0.9.3/deepspeed/module_inject/policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 from abc import ABC, abstractmethod
-from deepspeed.utils.types import ActivationFuncType
+from deepspeed.utils.types import ActivationFuncType, NormType
 import torch
 from deepspeed.accelerator import get_accelerator
 
 transformer_param_names = (
         'attn_qkvw', \
         'attn_qkvb', \
         'attn_ow' , \
@@ -54,44 +54,40 @@
             # the type of activation function used in MLP
             mlp_act_func_type=ActivationFuncType.GELU,
             # applies layer norm before attention if `pre_attn_norm` is set to True
             pre_attn_norm=True,
             # this flag shows whether or not using prefix in loading the checkpoint
             use_load_prefix=False,
             # whether or not the qkv is stored in the split-format
-            split_qkv=True):
+            split_qkv=True,
+            # Type of normalization to perform
+            norm_type=NormType.LayerNorm):
         super().__init__()
         self.cuda_graph_supported = False
         self.inference = inference
         self.linear_layer = linear_layer
         self.scale_attention = scale_attention
         self.is_megatron_v2 = megatron_v2
         self.use_mup = use_mup
         self.mlp_act_func_type = mlp_act_func_type
         self.pre_attn_norm = pre_attn_norm
         self.use_load_prefix = use_load_prefix
         self.split_qkv = split_qkv
+        self.norm_type = norm_type
 
     @abstractmethod
-    def attention(self, enable_training=False):
+    def attention(self):
         """
         Returns attention qkv and dense parameters
         weight: (3*hidden, hidden) and (hidden, hidden)
         bias: (3*hidden) and (hidden)
         """
         raise NotImplementedError
 
     @abstractmethod
-    def get_q_k_v(self):
-        """
-        return all q,k,v parameters without merging them together
-        """
-        raise NotImplementedError
-
-    @abstractmethod
     def get_hidden_heads(self):
         """
         return hidden_size and number of heads
         """
         raise NotImplementedError
 
     @abstractmethod
@@ -108,36 +104,28 @@
         """
         Returns LayerNorms used in transformer layer
         Post-Attention and pre/post layer norm
         gamma and beta with shape: (hidden)
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def get_lora_params(self):
-        """
-        Returns lora parameters used in transformer layer
-
-        """
-        raise NotImplementedError
-
 
 # TODO (lekurile): This function exists in base container as well, consolidate as some point
 def transpose(data):
     with torch.no_grad():
         data = data.contiguous()
         data1 = data.transpose(-1, -2).reshape(-1)
         data.reshape(-1).copy_(data1)
         data1 = None
     return data.reshape(data.shape[-1], data.shape[-2])
 
 
 # TODO (lekurile): This function exists in megatron feature container as well, consolidate as some point
 def _transpose(x, heads=1, mp_replace=None):
-    heads = heads // mp_replace.mp_size
+    heads = heads // mp_replace.mp_size  # type: ignore
     outer_dim = -1
     attention_head_size = x.shape[outer_dim] // heads
     new_x_shape = x.size()[:outer_dim] + (heads, attention_head_size)
     x_1 = x.view(*new_x_shape)
     (q, k, v) = torch.split(x_1, (x_1.shape[-1] // 3), dim=-1)
     if len(q.shape) > 2:
         new_shape = (q.shape[0], ) + (-1, )
@@ -160,23 +148,23 @@
                split_qkv=False,
                heads=1):
     if src_name in sd:
         dst = getattr(module, dst_name)
         tmp = sd[src_name]
         if len(dst.shape) == 1:
             if split_qkv:
-                dst = mp_replace.qkv_copy(dst, tmp)
+                dst = mp_replace.strided_copy(dst, tmp, num_splits=3)
             else:
                 dst = mp_replace.copy(dst, tmp)
             if qkv and megatron_v2:
                 dst = torch.nn.parameter.Parameter(_transpose(dst, heads=heads, mp_replace=mp_replace).contiguous())
         else:
             if split_qkv:
-                dst = mp_replace.qkv_copy(dst, weight_quantizer.quantize(tmp if weight_quantizer.q_int8 else \
-                                                (transpose(tmp).contiguous())), int8=weight_quantizer.q_int8)
+                dst = mp_replace.strided_copy(dst, weight_quantizer.quantize(tmp if weight_quantizer.q_int8 else \
+                                                (transpose(tmp).contiguous())), num_splits=3, int8=weight_quantizer.q_int8)
             else:
                 if qkv and megatron_v2:
                     tmp = _transpose(transpose(tmp), heads=heads, mp_replace=mp_replace).contiguous()
                     if weight_quantizer.q_int8:
                         tmp = transpose(tmp)
                 dst = mp_replace.copy(dst, weight_quantizer.quantize(tmp if weight_quantizer.q_int8 else \
                                                 transpose(tmp)), int8=weight_quantizer.q_int8)
@@ -189,27 +177,41 @@
         q = sd[src_names[0]]
         k = sd[src_names[1]]
         v = sd[src_names[2]]
         qkv_data = torch.cat((q, k, v), dim=0)
         dst = getattr(module, dst_name)
         if len(dst.shape) == 1:
             if split_qkv:
-                dst = mp_replace.qkv_copy(dst, qkv_data.contiguous())
+                dst = mp_replace.strided_copy(dst, qkv_data.contiguous(), num_splits=3)
             else:
                 dst = mp_replace.copy(dst, qkv_data)
         else:
             if split_qkv:
-                dst = mp_replace.qkv_copy(dst, weight_quantizer.quantize(qkv_data.to(get_accelerator().device_name()) if weight_quantizer.q_int8 else \
-                                                ((transpose(qkv_data)).contiguous())), int8=weight_quantizer.q_int8)
+                dst = mp_replace.strided_copy(dst, weight_quantizer.quantize(qkv_data.to(get_accelerator().device_name()) if weight_quantizer.q_int8 else \
+                                                ((transpose(qkv_data)).contiguous())), num_splits=3, int8=weight_quantizer.q_int8)
             else:
                 dst = mp_replace.copy(dst, weight_quantizer.quantize(qkv_data.to(get_accelerator().device_name()) if weight_quantizer.q_int8 else \
                                                 transpose(qkv_data)), int8=weight_quantizer.q_int8)
         setattr(module, dst_name, dst)
 
 
+# Extending the `maybe_copy` function for when mlp1 is in separate parameters for GeGLU
+def maybe_copy_geglu(module, sd, weight_quantizer, mp_replace, dst_name, src_names):
+    if src_names[0] in sd:
+        reg_proj = sd[src_names[0]]
+        gate_proj = sd[src_names[1]]
+
+        mlp1_data = torch.cat((reg_proj, gate_proj), dim=0)
+        dst = getattr(module, dst_name)
+
+        dst = mp_replace.strided_copy(dst, weight_quantizer.quantize(mlp1_data.to(get_accelerator().device_name()) if weight_quantizer.q_int8 else \
+                                            transpose(mlp1_data)), num_splits=2, int8=weight_quantizer.q_int8)
+        setattr(module, dst_name, dst)
+
+
 def pack_lora_weights(p):
     return [
         p.lora_right_weight, \
         p.lora_left_weight, \
         p.lora_scaling
     ]
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/replace_module.py` & `deepspeed-0.9.3/deepspeed/module_inject/replace_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 import os
+from typing import Optional
 import torch
 import tqdm
 import deepspeed
 import deepspeed.ops.transformer as transformer_inference
 from deepspeed.ops.transformer.inference.diffusers_attention import DeepSpeedDiffusersAttention
 from deepspeed.ops.transformer.inference.diffusers_transformer_block import DeepSpeedDiffusersTransformerBlock
 from deepspeed.ops.transformer.inference.diffusers_2d_transformer import Diffusers2DTransformerConfig
@@ -20,14 +21,16 @@
 
 from .layers import LinearAllreduce, LinearLayer
 from .load_checkpoint import load_model_with_checkpoint
 import time
 
 from .utils import policy_to_ds_container
 
+import gc
+
 
 class ReplaceWithTensorSlicing:
 
     def __init__(self, mp_group=None, mp_size=1, out_dim=1, in_dim=0):
         if mp_group is not None:
             self.gpu_index = dist.get_rank(group=mp_group)
         else:
@@ -38,60 +41,64 @@
 
     def merge_assert(self, dim1, dim2):
         assert dim1 > dim2, \
             'Merging tensors is not allowed here! Please use deepspeed load_checkpoint\
             for merging your checkpoints before replacing the transformer layer with\
             inference-kernels'
 
-    def qkv_copy(self, dst, src, int8=False, allocat_tensor=False):
+    def strided_copy(self,
+                     dst: Optional[torch.Tensor],
+                     src: Optional[torch.Tensor],
+                     num_splits: int,
+                     int8: bool = False,
+                     allocate_tensor: bool = False):
         if src is None:
             return src
         src_shape = src.shape
         dst_shape = dst.shape
 
         outer_dim = 0 if int8 else -1
-        inner_dim = -1 if int8 else 0
 
-        if allocat_tensor:
+        if allocate_tensor:
             dst = torch.empty_like(dst)
 
-        src_split = torch.split(src.data, src.shape[outer_dim] // 3, dim=outer_dim)
+        src_split = torch.split(src.data, src.shape[outer_dim] // num_splits, dim=outer_dim)
         if (len(src_shape) == 2 and len(dst_shape) == 2):
             if src_shape[outer_dim] == dst_shape[self.out_dim]:
                 dst = dst.reshape(-1).data.copy_(src.data.reshape(-1)).reshape(src.shape)
                 dst = torch.nn.parameter.Parameter(dst, requires_grad=False)
                 if hasattr(src, 'scale'):
                     dst.scale = src.scale
                 return dst
             self.merge_assert(src_shape[outer_dim], dst_shape[self.out_dim])
-            qkv_size = dst_shape[self.out_dim] // 3
+            qkv_size = dst_shape[self.out_dim] // num_splits
             qkv_split = [torch.split(src_s, qkv_size, dim=outer_dim) for src_s in src_split]
             weight_split = [
                 torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=outer_dim) for i in range(len(qkv_split[0]))
             ]
             dst = dst.reshape(-1).data.copy_(weight_split[self.gpu_index].contiguous().reshape(-1)).reshape(
                 weight_split[self.gpu_index].shape)
         else:
             if src_shape[0] == dst_shape[0]:
                 return torch.nn.parameter.Parameter(src)
-            qkv_size = dst_shape[0] // 3
+            qkv_size = dst_shape[0] // num_splits
             qkv_split = [torch.split(src_s, qkv_size, dim=0) for src_s in src_split]
             bias_split = [torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=0) for i in range(len(qkv_split[0]))]
             dst.data.copy_(bias_split[self.gpu_index].contiguous())
 
         dst = torch.nn.parameter.Parameter(dst, requires_grad=False)
         if hasattr(src, 'scale'):
             dst.scale = src.scale
         return dst
 
-    def copy(self, dst, src, int8=False, allocat_tensor=False):
+    def copy(self, dst, src, int8=False, allocate_tensor=False):
         if src is None:
             return src
         assert not dst.data.is_meta  # the torch.Tensor.copy_ method used below will silently fail on meta tensors
-        if allocat_tensor:
+        if allocate_tensor:
             dst = torch.empty_like(dst)
         outer_dim = 0 if int8 else 1
         inner_dim = 1 if int8 else 0
         src_shape = src.shape
         dst_shape = dst.shape
         if (len(src_shape) == 2 and len(dst_shape) == 2):
 
@@ -104,15 +111,15 @@
                                    src[self.gpu_index * dst_shape[self.in_dim]: (self.gpu_index + 1) * dst_shape[self.in_dim], :])
                 else:
                     self.merge_assert(src_shape[outer_dim], dst_shape[self.out_dim])
                     dst.data.copy_(src[:, self.gpu_index * dst_shape[self.out_dim]: (self.gpu_index + 1) * dst_shape[self.out_dim]] if outer_dim == 1 else \
                                    src[self.gpu_index * dst_shape[self.out_dim]: (self.gpu_index + 1) * dst_shape[self.out_dim], :])
         else:
             if src_shape[0] == dst_shape[0]:
-                dst = src
+                dst = src if src.dtype == dst.dtype else dst.data.copy_(src)
             else:
                 dst.data.copy_(src[self.gpu_index * dst_shape[-1]:(self.gpu_index + 1) * dst_shape[-1]])
         dst = torch.nn.parameter.Parameter(dst, requires_grad=False)
         if hasattr(src, 'scale'):
             dst.scale = src.scale
 
         return dst
@@ -173,29 +180,30 @@
     for policy in generic_policies:
         policy = policy()
         if policy.match(module):
             return policy
     return None
 
 
-def generic_injection(module, fp16=False, enable_cuda_graph=True):
+def generic_injection(module, fp16=False, bf16=False, enable_cuda_graph=True):
 
     def replace_attn(child, policy):
         policy_attn = policy.attention(child)
         if policy_attn is None:
             return child
         if len(policy_attn) == 5:
             qkvw, attn_ow, attn_ob, hidden_size, heads = policy_attn
         else:
             qw, kw, vw, attn_ow, attn_ob, hidden_size, heads = policy_attn
 
         config = transformer_inference.DeepSpeedInferenceConfig(
             hidden_size=hidden_size,
             heads=heads,
             fp16=fp16,
+            bf16=bf16,
             triangular_masking=False,
             max_out_tokens=4096,
         )
         attn_module = DeepSpeedDiffusersAttention(config)
 
         def transpose(data):
             data = data.contiguous()
@@ -220,16 +228,16 @@
     def replace_attn_block(child, policy):
         config = Diffusers2DTransformerConfig()
         return DeepSpeedDiffusersTransformerBlock(child, config)
 
     if isinstance(module, torch.nn.Module):
         pass
     else:
-        if fp16 is False:
-            raise ValueError("Generic injection only supported with FP16")
+        if fp16 is False and bf16 is False:
+            raise ValueError("Generic injection only supported with FP16 or BF16")
 
         try:
             import diffusers
             if hasattr(diffusers.models.attention, 'CrossAttention'):
                 cross_attention = diffusers.models.attention.CrossAttention
             else:
                 cross_attention = diffusers.models.attention_processor.Attention
@@ -281,15 +289,14 @@
         checkpoint_dict: Dictionary for checkpoint passed from the Inference Engine
         config: top-level DS Inference config defined in inference/config.py
         model_config: HuggingFace model config passed from the inference/engine.py
     Returns:
         Updated nn.module with replaced transformer layers
     """
     # defining globals as internally defined functions inherit these everywhere
-    fp16 = (config.dtype == torch.float16 or config.dtype == torch.int8)
     quantize = (config.dtype == torch.int8)
     # todo: Refactor later. In future, let's minimize the style used above and use config.** instead
 
     linear_layer_setting = None
     '''
         linear_layer_setting (tuple of modules) [Optional]: shows which two classes are used for linear layers and embedding layers
     '''
@@ -314,30 +321,29 @@
 
         # 1. Create a model-specific container object using the policy object.
         _container = policy_to_ds_container(policy=policy,
                                             config=config,
                                             model_config=model_config,
                                             layer_id=layer_id,
                                             child=child)
-        _container.set_dtype(fp16)
         _container.set_moe(moe)
 
         # 2. Set the tensor parallelism config
         _container.set_tensor_parallel_config(config.tensor_parallel.tp_size, config.tensor_parallel.tp_group)
 
         # 3. Initialize tensors
         _container.initialize_tensors()
 
         # 4. deal with data types -- needs refactor to use dtype instead of fp16
-        if fp16:
-            _container.convert_to_required_dtype(dtype=torch.half)
+        if config.dtype in [torch.float16, torch.bfloat16, torch.int8]:
+            _container.convert_to_required_dtype()
 
         # 5. Set the quantization config
         quantizer = GroupQuantizer(q_int8=quantize)
-        _container.set_quantization_config(quantize, quantizer)
+        _container.set_quantization_config(quantizer)
 
         # 6. create a DS Inference config object
         _container.create_ds_model_config()
 
         # 7. use the config and create the module
         _container.create_module()
 
@@ -354,19 +360,21 @@
         global container_g
 
         if container_g is None:
             container_g = _container
 
         return _container.module
 
-    def replace_wo_policy(module, all_reduce_linears):
+    def replace_wo_policy(module, all_reduce_linears, prefix="", state_dict=None):
         mp_size = config.tensor_parallel.tp_size
         mp_group = config.tensor_parallel.tp_group
 
         def _replace(child, name, conv_linear_layer):
+            if getattr(child, "replaced", False) == True:
+                return
             mp_replace = ReplaceWithTensorSlicing(mp_group=mp_group)
             weight_shape = child.weight.shape
             if name in all_reduce_linears:
                 new_weight = torch.empty((
                     weight_shape[1] if conv_linear_layer else weight_shape[0],
                     (weight_shape[0] if conv_linear_layer else weight_shape[1]) // mp_size,
                 ),
@@ -374,14 +382,15 @@
                                          dtype=child.weight.dtype)
                 if conv_linear_layer:
                     child.weight.data = child.weight.data.transpose(-1, -2).contiguous()
                 data = mp_replace.copy(new_weight, child.weight.data)
                 new_bias = torch.empty((weight_shape[0]), device=child.weight.device, dtype=child.weight.dtype)
                 if child.bias is not None:
                     new_bias.data.copy_(child.bias.data)
+                setattr(child, "replaced", True)
                 return LinearAllreduce(data, child.bias if child.bias is None else \
                             torch.nn.parameter.Parameter(new_bias.to(get_accelerator().current_device_name())), mp_group)
             else:
                 new_weight = torch.empty((
                     (weight_shape[1] if conv_linear_layer else weight_shape[0]) // mp_size,
                     weight_shape[0] // mp_size if conv_linear_layer else weight_shape[1],
                 ),
@@ -392,29 +401,35 @@
                 data = mp_replace.copy(new_weight, child.weight.data)
 
                 new_bias = torch.empty((weight_shape[0] // mp_size),
                                        device=child.weight.device,
                                        dtype=child.weight.dtype)
                 bias_data = None if child.bias is None else mp_replace.copy(new_bias, child.bias.data).to(
                     get_accelerator().current_device_name())
+                setattr(child, "replaced", True)
                 return LinearLayer(weight=data.to(get_accelerator().current_device_name()), bias=bias_data)
 
         def _slice_embedding(child, name, conv_linear_layer):
+            if getattr(child, "replaced", False) == True:
+                return
             mp_replace = ReplaceWithTensorSlicing(mp_group=mp_group)
             new_weight = torch.empty((child.weight.shape[0], child.weight.shape[1] // mp_size),
                                      device=child.weight.device,
                                      dtype=child.weight.dtype)
             data = mp_replace.copy(new_weight,
                                    child.weight.ds_tensor.data if hasattr(child.weight, 'ds_tensor') else \
                                    child.weight.data)
             new_embedding = nn.Embedding(child.weight.shape[0], child.weight.shape[1] // mp_size)
             new_embedding.weight.data.copy_(data)
+            setattr(child, "replaced", True)
             return new_embedding
 
         def update_mp_params(child):
+            if getattr(child, "replaced", False) == True:
+                return
             if hasattr(child, 'n_heads'):
                 assert child.n_heads % mp_size == 0, "n_heads ({}) must be divisible by mp_size ({})".format(
                     child.n_heads, mp_size)
                 child.n_heads = child.n_heads // mp_size
             if hasattr(child, 'inner_dim'):
                 assert child.inner_dim % mp_size == 0, "inner_dim ({}) must be divisible by mp_size ({})".format(
                     child.inner_dim, mp_size)
@@ -439,14 +454,15 @@
                 assert child.embed_dim % mp_size == 0, "embed_dim must ({}) be divisible by mp_size ({})".format(
                     child.embed_dim, mp_size)
                 child.embed_dim = child.embed_dim // mp_size
             if hasattr(child, 'hidden_size'):
                 assert child.hidden_size % mp_size == 0, "hidden_size ({}) must be divisible by mp_size ({})".format(
                     child.hidden_size, mp_size)
                 child.hidden_size = child.hidden_size // mp_size
+            setattr(child, "replaced", True)
 
         conv_linear_layer = False
         if linear_layer_setting is not None:
             linear_policies = {linear_layer_setting[0]: _replace}
             if len(linear_layer_setting) == 2:
                 linear_policies.update({linear_layer_setting[1]: _slice_embedding})
         else:
@@ -456,54 +472,81 @@
                     conv_linear_layer = True
                     linear_policies = {transformers.model_utils.Conv1D: _replace}
                 except ImportError:
                     linear_policies = {nn.Linear: _replace}
             else:
                 linear_policies = {nn.Linear: _replace, nn.Embedding: _slice_embedding}
 
-        def _replace_module(r_module, prev_name=''):
+        def _replace_module(r_module, prev_name='', prev_class_name=''):
             for name, child in r_module.named_children():
+                if prev_class_name == "":
+                    class_name = prev_name
+                elif prev_name == "":
+                    class_name = prev_class_name
+                else:
+                    class_name = prev_class_name + '.' + prev_name
+                checking_key = prefix + '.' + class_name + '.' + name + '.' if class_name != "" else prefix + '.' + name + '.'
+                if child.__class__ in [nn.Linear, nn.Embedding, nn.LayerNorm] and state_dict != None:
+                    if any(checking_key in item for item in state_dict):
+                        load(child, state_dict, checking_key, mp_group)
+                    else:
+                        continue
+                if len(child._buffers) != 0 and state_dict != None:
+                    load_buffer(child, state_dict, checking_key)
                 if child.__class__ in linear_policies:
                     setattr(r_module, name, linear_policies[child.__class__](child, prev_name + '.' + name,
                                                                              conv_linear_layer))
                 else:
                     update_mp_params(child)
-                    _replace_module(child, name)
+                    _replace_module(child, name, class_name)
             return r_module
 
         return _replace_module(module)
 
-    def replace_fn(child, _policy, layer_id=0):
+    def replace_fn(child, _policy, layer_id=0, prefix="", state_dict=None):
         training = False  # todo: refactor this part to go in the config
         if training:
             # copy relevant state from child -> new module
             new_module = replace_with_policy(child, _policy, config.triangular_masking)
 
         else:
             # copy relevant state from child -> new module
             if config.replace_with_kernel_inject:
                 new_module = replace_with_policy(child,
                                                  _policy,
                                                  config.triangular_masking,
                                                  inference=True,
                                                  layer_id=layer_id)
             else:
-                new_module = replace_wo_policy(child, _policy)
+                new_module = replace_wo_policy(child, _policy, prefix=prefix, state_dict=state_dict)
 
         return new_module
 
-    replaced_module = replace_module(model=model,
-                                     orig_class=orig_layer_impl,
-                                     replace_fn=replace_fn,
-                                     _replace_policy=config.injection_policy_tuple)
+    if checkpoint_dict != None and not config.replace_with_kernel_inject:
+        # AutoTP shard loading
+        checkpoint = checkpoint_dict["checkpoints"]
+        pbar = tqdm.tqdm(total=len(checkpoint), desc=f"Loading {len(checkpoint)} checkpoint shards")
+        for i in range(len(checkpoint)):
+            replaced_module = replace_module(model=model,
+                                             orig_class=orig_layer_impl,
+                                             replace_fn=replace_fn,
+                                             _replace_policy=config.injection_policy_tuple,
+                                             checkpoint=checkpoint[i])
+            pbar.update(1)
+            gc.collect()
+    else:
+        replaced_module = replace_module(model=model,
+                                         orig_class=orig_layer_impl,
+                                         replace_fn=replace_fn,
+                                         _replace_policy=config.injection_policy_tuple)
 
     quantizer = GroupQuantizer(q_int8=quantize)
     world_size = dist.get_world_size() if dist.is_initialized() else 1
     rank = dist.get_rank() if dist.is_initialized() else 0
-    if checkpoint_dict is not None:
+    if checkpoint_dict is not None and config.replace_with_kernel_inject:
         assert container_g.ckpt_load_enabled, \
                f"Meta Tensor checkpoint loading not supported in {container_g.__class__.__name__} container"
         start_time = time.time()
         checkpoint = checkpoint_dict['checkpoints']
         ckpt_list = checkpoint["tp"] if type(checkpoint) is dict else checkpoint
         ckpt_type = checkpoint_dict.get('parallelization', 'pp')
         ckpt_mp_size = checkpoint_dict.get('tp_size', len(ckpt_list))
@@ -520,15 +563,14 @@
                                            mp_replace,
                                            ckpt_type,
                                            ckpt_mp_size,
                                            quantizer,
                                            container=container_g)
                 pbar.update(1)
         else:
-            import gc
             num_checkpoints = len(ckpt_list) // ckpt_mp_size
             tp_split_size = (world_size / ckpt_mp_size)
             sd_offset = int(rank / tp_split_size)
             sd_count = int((rank + max(1, tp_split_size)) / tp_split_size) - sd_offset
             pbar = tqdm.tqdm(total=num_checkpoints, desc=f"Loading {num_checkpoints} checkpoint shards")
             for i in range(num_checkpoints):
                 pbar.update(1)
@@ -594,25 +636,33 @@
 
         if not dist.is_initialized() or dist.get_rank() == 0:
             print("Saving tp-sharded checkpoints")
             torch.save(
                 OrderedDict({k: v
                              for k, v in dict(replaced_module.state_dict()).items()
                              if transformer_name not in k}), f'{config.save_mp_checkpoint_path}/{non_tp_ckpt_name}')
+
+            dtype_reprs = {
+                torch.float32: 'float32',
+                torch.float16: 'float16',
+                torch.int8: 'int8',
+                torch.bfloat16: 'bfloat16'
+            }
+
             ckpt_config = json.dumps({
                 'type': ckpt_name,
                 'base_dir': f'{config.save_mp_checkpoint_path}',
                 'checkpoints': {
                     "non_tp": ckpt_files,
                     "tp": [f'tp_{r:0>2d}_{m:0>2d}.pt' for m in range(num_partitions) for r in range(world_size)]
                 },
                 'version': 1.0,
                 'parallelization': 'tp',
                 'tp_size': world_size,
-                'dtype': 'int8' if quantize else ('float16' if fp16 else 'float32')
+                'dtype': dtype_reprs[config.dtype]
             })
             with open(f"{config.save_mp_checkpoint_path}/ds_inference_config.json", "w") as cfg:
                 cfg.write(ckpt_config)
 
         rep_sd = replaced_module.state_dict()
         for n, p in replaced_module.named_parameters():
             if hasattr(p, 'scale'):
@@ -694,24 +744,27 @@
 
     return replace_module(model=model,
                           orig_class=deepspeed.DeepSpeedTransformerLayer,
                           replace_fn=replace_fn,
                           _replace_policy=None)
 
 
-def replace_module(model, orig_class, replace_fn, _replace_policy):
+def replace_module(model, orig_class, replace_fn, _replace_policy, checkpoint=None):
     """ Scan the model for instances of ``orig_clas:`` to replace using ``replace_fn``.
     Arguments:
         model (torch.nn.Module): the model to augment
         orig_class (torch.nn.Module): the module to search for
         replace_fn (method): a method to convert instances of ``orig_class`` to the
                              desired type and return a new instance.
     Returns:
         A modified ``model``.
     """
+    sd = None
+    if checkpoint != None:
+        sd = torch.load(checkpoint, map_location='cpu')
     policy = {}
     if orig_class is not None:
         policy.update({orig_class: (replace_fn, _replace_policy)})
     else:
         for plcy in replace_policies:
             # instantiate a throw-away policy in order to populate the _orig_layer_class
             _ = plcy(None)
@@ -720,37 +773,138 @@
                     policy.update({orig_layer_class: (replace_fn, plcy)})
             elif plcy._orig_layer_class is not None:
                 policy.update({plcy._orig_layer_class: (replace_fn, plcy)})
     assert len(policy.items()) > 0,\
         "No default policy found! Please specify your policy injection_policy (like {BertLayer:HFBEertLayerPolicy})." +\
         "You can find some samples here: https://github.com/microsoft/DeepSpeed/blob/master/deepspeed/module_inject/replace_policy.py"
 
-    replaced_module, _ = _replace_module(model, policy)
+    replaced_module, _ = _replace_module(model, policy, state_dict=sd)
+    if checkpoint != None:
+        embedding_weight = None
+        for n, p in replaced_module.named_parameters():
+            if "word_embeddings." in n or "embed_tokens." in n or "wte." in n:
+                embedding_weight = p
+        if embedding_weight is not None and hasattr(replaced_module, "lm_head") and hasattr(
+                replaced_module.lm_head, "weight") and replaced_module.lm_head.weight.is_meta:
+            replaced_module.lm_head.weight = embedding_weight
     return replaced_module
 
 
 from ..pipe import PipelineModule
 
+import re
+
 
-def _replace_module(model, policies, layer_id=0):
+def skip_level_0_prefix(model, name):
+    model = str(model)
+    key = re.search(r": (.*?)Model", model)
+    if key is None:
+        key = re.search(r": (.*?)Stack", model)
+    if key is None:
+        key = re.match(r"(.*?)Model", model)
+    if key is not None and key.group(1).lower() in "bloom":
+        # if keys start with 'model.', don't skip level 0 prefix
+        if not re.match("^model[.]", name):
+            return True
+    return False
+
+
+def load_buffer(module, state_dict, prefix):
+    for name in module._buffers.keys():
+        if module._buffers[name].data.is_meta:
+            module._buffers[name] = torch.nn.parameter.Parameter(
+                data=torch.empty_like(module._buffers[name].data, device="cpu"),
+                requires_grad=module._buffers[name].data.requires_grad)
+        if prefix + name in state_dict.keys():
+            module._buffers[name].data.copy_(state_dict[prefix + name])
+
+
+def _replace_module(model, policies, prefix='', layer_id=0, level_id=0, state_dict=None):
     """ Traverse model's children recursively and apply any transformations in ``policies``.
     Arguments:
         model (torch.nn.Module): model to augment
         policies (dict): Mapping of source class to replacement function.
     Returns:
         Modified ``model``.
     """
+    try:
+        import transformers
+        OPTLearnedPositionalEmbedding = transformers.models.opt.modeling_opt.OPTLearnedPositionalEmbedding
+    except:
+        OPTLearnedPositionalEmbedding = None
+    load_layers = [nn.Linear, nn.Embedding, nn.LayerNorm, OPTLearnedPositionalEmbedding]
     for name, child in model.named_children():
         if child.__class__ in policies:
-            replaced_module = policies[child.__class__][0](child, policies[child.__class__][-1], layer_id)
+            replaced_module = policies[child.__class__][0](child,
+                                                           policies[child.__class__][-1],
+                                                           layer_id,
+                                                           prefix=prefix + name,
+                                                           state_dict=state_dict)
             setattr(model, name, replaced_module)
             if isinstance(model, PipelineModule):
                 assert hasattr(model, 'forward_funcs'),\
                     "we require pipe-module to have the list of fwd_functions"
                 model.forward_funcs[model.fwd_map[name]] = replaced_module
             layer_id += 1
         else:
-            _, layer_id = _replace_module(child, policies, layer_id=layer_id)
+            checking_key = prefix + name + '.'
+            if child.__class__ in load_layers and state_dict != None:
+                if any(checking_key in item for item in state_dict):
+                    load(
+                        child,
+                        state_dict,
+                        checking_key,
+                    )
+                else:
+                    continue
+            if len(child._buffers) != 0 and state_dict != None:
+                load_buffer(child, state_dict, checking_key)
+            _, layer_id = _replace_module(child,
+                                          policies,
+                                          prefix if level_id == 0 and skip_level_0_prefix(model, name) else \
+                                          prefix + name + '.',
+                                          layer_id=layer_id,
+                                          level_id=level_id + 1,
+                                          state_dict=state_dict)
 
     # Add the reset_cache func to the model, so that it can be called in the beginning of text-generation.
     model.reset_cache = transformer_inference.DeepSpeedTransformerInference.reset_cache
     return model, layer_id
+
+
+def load(module, state_dict, prefix, mp_group=None):
+    mp_replace = ReplaceWithTensorSlicing(mp_group=mp_group)
+    if hasattr(module, 'weight'):
+        if module.weight.data.is_meta:
+            # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+            module.weight = torch.nn.parameter.Parameter(data=torch.empty_like(module.weight.data, device="cpu"),
+                                                         requires_grad=module.weight.data.requires_grad)
+            if 'query_key_value' in prefix:
+                module.weight = mp_replace.strided_copy(module.weight.data,
+                                                        state_dict[prefix + 'weight'],
+                                                        num_splits=3)
+            else:
+                module.weight = mp_replace.copy(module.weight.data, state_dict[prefix + 'weight'])
+    else:
+        if hasattr(module, 'norm') and hasattr(module.norm, 'weight'):
+            if module.norm.weight.data.is_meta:
+                # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                module.norm.weight = torch.nn.parameter.Parameter(data=torch.empty_like(module.norm.weight.data,
+                                                                                        device="cpu"),
+                                                                  requires_grad=module.norm.weight.data.requires_grad)
+            module.norm.weight = mp_replace.copy(module.norm.weight.data, state_dict[prefix + 'weight'])
+
+    if prefix + 'bias' in state_dict.keys():
+        if hasattr(module, 'bias'):
+            if module.bias.data.is_meta:
+                # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                module.bias = torch.nn.parameter.Parameter(data=torch.empty_like(module.bias.data, device="cpu"),
+                                                           requires_grad=module.bias.data.requires_grad)
+            module.bias = mp_replace.copy(module.bias, state_dict[prefix + 'bias'])
+        else:
+            if hasattr(module, 'norm') and hasattr(module.norm, 'bias'):
+                if module.norm.bias.data.is_meta:
+                    # meta tensor cannot be casted or copied to, so we need to replace it with a normal tensor here
+                    module.norm.bias = torch.nn.parameter.Parameter(data=torch.empty_like(module.norm.bias.data,
+                                                                                          device="cpu"),
+                                                                    requires_grad=module.norm.bias.data.requires_grad)
+                module.norm.bias = mp_replace.copy(module.norm.bias, state_dict[prefix + 'bias'])
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/replace_policy.py` & `deepspeed-0.9.3/deepspeed/module_inject/replace_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from .containers import HFGPTJLayerPolicy
 from .containers import HFGPTNEOLayerPolicy
 from .containers import GPTNEOXLayerPolicy
 from .containers import HFOPTLayerPolicy
 from .containers import MegatronLayerPolicy
 from .containers import HFDistilBertLayerPolicy
 from .containers import HFCLIPLayerPolicy
+from .containers import LLAMALayerPolicy
 from .containers import UNetPolicy
 from .containers import VAEPolicy
 
 # transformer-based policies
 replace_policies = [
     HFBertLayerPolicy, HFGPTNEOLayerPolicy, GPTNEOXLayerPolicy, HFGPTJLayerPolicy, MegatronLayerPolicy,
-    HFGPT2LayerPolicy, BLOOMLayerPolicy, HFOPTLayerPolicy, HFCLIPLayerPolicy, HFDistilBertLayerPolicy
+    HFGPT2LayerPolicy, BLOOMLayerPolicy, HFOPTLayerPolicy, HFCLIPLayerPolicy, HFDistilBertLayerPolicy, LLAMALayerPolicy
 ]
 
 # non-transformer-based policies
 generic_policies = [UNetPolicy, VAEPolicy]
```

### Comparing `deepspeed-0.9.2/deepspeed/module_inject/utils.py` & `deepspeed-0.9.3/deepspeed/module_inject/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     from .containers import BLOOMLayerPolicy, DS_BloomContainer
     from .containers import HFGPTJLayerPolicy, DS_GPTJContainer
     from .containers import HFGPTNEOLayerPolicy, DS_GPTNEOContainer
     from .containers import GPTNEOXLayerPolicy, DS_GPTNEOXContainer
     from .containers import HFOPTLayerPolicy, DS_OPTContainer
     from .containers import MegatronLayerPolicy, DS_MegatronGPTContainer
     from .containers import HFDistilBertLayerPolicy, DS_DistilBERTContainer
+    from .containers import LLAMALayerPolicy, DS_LLAMAContainer
 
     policy_to_container = {
         HFGPT2LayerPolicy: DS_GPT2Container,
         HFBertLayerPolicy: DS_BERTContainer,
         BLOOMLayerPolicy: DS_BloomContainer,
         HFGPTJLayerPolicy: DS_GPTJContainer,
         HFGPTNEOLayerPolicy: DS_GPTNEOContainer,
         GPTNEOXLayerPolicy: DS_GPTNEOXContainer,
         HFOPTLayerPolicy: DS_OPTContainer,
         MegatronLayerPolicy: DS_MegatronGPTContainer,
         HFDistilBertLayerPolicy: DS_DistilBERTContainer,
+        LLAMALayerPolicy: DS_LLAMAContainer,
     }
 
     container = None
     policy = kwargs['policy']
     assert policy is not None, "Policy cannot be None"
     policy_type = type(policy)
```

### Comparing `deepspeed-0.9.2/deepspeed/moe/experts.py` & `deepspeed-0.9.3/deepspeed/moe/experts.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/moe/layer.py` & `deepspeed-0.9.3/deepspeed/moe/layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/moe/mappings.py` & `deepspeed-0.9.3/deepspeed/moe/mappings.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/moe/sharded_moe.py` & `deepspeed-0.9.3/deepspeed/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/moe/utils.py` & `deepspeed-0.9.3/deepspeed/moe/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/monitor/config.py` & `deepspeed-0.9.3/deepspeed/monitor/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,11 +70,10 @@
     """ WandB monitor, requires `wandb` package is installed. """
 
     csv_monitor: CSVConfig = {}
     """ Local CSV output of monitoring data. """
 
     @root_validator
     def check_enabled(cls, values):
-        values["enabled"] = False
-        if (values.get("tensorboard").enabled or values.get("wandb").enabled or values.get("csv_monitor").enabled):
-            values["enabled"] = True
+        values["enabled"] = values.get("tensorboard").enabled or values.get("wandb").enabled or values.get(
+            "csv_monitor").enabled
         return values
```

### Comparing `deepspeed-0.9.2/deepspeed/monitor/csv_monitor.py` & `deepspeed-0.9.3/deepspeed/monitor/csv_monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/monitor/monitor.py` & `deepspeed-0.9.3/deepspeed/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/monitor/tensorboard.py` & `deepspeed-0.9.3/deepspeed/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/monitor/utils.py` & `deepspeed-0.9.3/deepspeed/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/monitor/wandb.py` & `deepspeed-0.9.3/deepspeed/monitor/wandb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/nebula/config.py` & `deepspeed-0.9.3/deepspeed/nebula/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/nebula/constants.py` & `deepspeed-0.9.3/deepspeed/nebula/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 NEBULA_ENABLED = "enabled"
 NEBULA_ENABLED_DEFAULT = False
 
 # There is a case where customer want to load the checkpoint saved
 # by raw torch. Because nebula cannot load torch checkpoint directly
 # as they have different folder structures to bring the gap for
-# loading(the data are totaly same in bytes for torch and enbula s
-# aving).
+# loading(the data are totally same in bytes for torch and nebula
+# saving).
 # In this case, we must disable nebula load to use raw torch load.
 # Customer can just set NEBULA_ENABLE_NEBULA_LOAD to False. Then use
 # original way of deepspeed to load, i.e. set the value of "--load".
 NEBULA_ENABLE_NEBULA_LOAD = "enable_nebula_load"
 NEBULA_ENABLE_NEBULA_LOAD_DEFAULT = True
 
 # When you want to resume the previous checkpoint saved by nebula,
@@ -56,15 +56,15 @@
 # Checkpoint number which will be kept in memory. Let us say,
 # if the value is 2. Then we have checkpoints 1 and 2 are ready
 # now. When it comes to checkpoint 3, the 1 will be removed if
 # 1 has been persisted to disk.
 NEBULA_NUM_OF_VERSION_IN_RETENTION = "num_of_version_in_retention"
 NEBULA_NUM_OF_VERSION_IN_RETENTION_DEFAULT = 2
 
-# Neubla envs
+# Nebula envs
 NEBULA_EXPORT_ENVS = [
     'DLTS_JOB_ID', 'DLTS_NUM_WORKER', 'NEBULA_PERSISTENT_STORAGE_PATH', 'NEBULA_PERSISTENT_TIME_INTERVAL',
     'AML_RUN_ID', 'AZUREML_RUN_TOKEN', 'AZUREML_WORKSPACE_SCOPE', 'AZUREML_EXPERIMENT_SCOPE',
     'AZUREML_RUN_HISTORY_SERVICE_ENDPOINT', 'AZUREML_RUN_ID', 'NEBULA_MEMORY_BUFFER_SIZE',
     'AZUREML_PARAMETER_ITPJOB_NAME', 'FC_TASKROLE_NAME', 'FC_TASK_INDEX', 'MASTER_HOST', 'LOCAL_HOST',
     'AZUREML_BLOB_ACCOUNT_NAME', 'AZUREML_BLOB_ACCOUNT_KEY'
 ]
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/adagrad/cpu_adagrad.py` & `deepspeed-0.9.3/deepspeed/ops/adagrad/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/adam/cpu_adam.py` & `deepspeed-0.9.3/deepspeed/ops/adam/cpu_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             eps (float, optional): term added to the denominator to improve
                 numerical stability. (default: 1e-8)
             weight_decay (float, optional): weight decay (L2 penalty) (default: 0)
             amsgrad (boolean, optional): whether to use the AMSGrad variant of this
                 algorithm from the paper `On the Convergence of Adam and Beyond`_
                 (default: False) NOT SUPPORTED in DeepSpeed CPUAdam!
             adamw_mode: select between Adam and AdamW implementations (default: AdamW)
-            full_precision_optimizer_states: creates momementum and variance in full precision regardless of
+            full_precision_optimizer_states: creates momentum and variance in full precision regardless of
                         the precision of the parameters (default: True)
         """
 
         default_args = dict(lr=lr,
                             betas=betas,
                             eps=eps,
                             weight_decay=weight_decay,
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/adam/fused_adam.py` & `deepspeed-0.9.3/deepspeed/ops/adam/fused_adam.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,57 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 """
 Copyright NVIDIA/apex
-This file is adapted from fused adam in NVIDIA/apex, commit a109f85
+This file is adapted from fused adam in NVIDIA/apex, commit 6bd01c4
 """
 
 import torch
 from .multi_tensor_apply import MultiTensorApply
 
 multi_tensor_applier = MultiTensorApply(2048 * 32)
 from deepspeed.accelerator import get_accelerator
 from deepspeed.ops.op_builder import FusedAdamBuilder
 
 
 class FusedAdam(torch.optim.Optimizer):
     """Implements Adam algorithm.
 
-    Currently GPU-only.
+    Currently GPU-only.  Requires Apex to be installed via
+    ``pip install -v --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./``.
 
     This version of fused Adam implements 2 fusions.
 
       * Fusion of the Adam update's elementwise operations
       * A multi-tensor apply launch that batches the elementwise updates applied to all the model's parameters into one or a few kernel launches.
 
+    :class:`apex.optimizers.FusedAdam` may be used as a drop-in replacement for ``torch.optim.AdamW``,
+    or ``torch.optim.Adam`` with ``adam_w_mode=False``::
+
+        opt = apex.optimizers.FusedAdam(model.parameters(), lr = ....)
+        ...
+        opt.step()
+
+    :class:`apex.optimizers.FusedAdam` may be used with or without Amp.  If you wish to use :class:`FusedAdam` with Amp,
+    you may choose any ``opt_level``::
+
+        opt = apex.optimizers.FusedAdam(model.parameters(), lr = ....)
+        model, opt = amp.initialize(model, opt, opt_level="O0" or "O1 or "O2")
+        ...
+        opt.step()
+
+    In general, ``opt_level="O1"`` is recommended.
+
+
+    .. warning::
+        A previous version of :class:`FusedAdam` allowed a number of additional arguments to ``step``.  These additional arguments
+        are now deprecated and unnecessary.
+
     Adam was been proposed in `Adam: A Method for Stochastic Optimization`_.
 
     Arguments:
         params (iterable): iterable of parameters to optimize or dicts defining
             parameter groups.
         lr (float, optional): learning rate. (default: 1e-3)
         betas (Tuple[float, float], optional): coefficients used for computing
@@ -77,15 +100,15 @@
         if self.set_grad_none:
             for group in self.param_groups:
                 for p in group['params']:
                     p.grad = None
         else:
             super(FusedAdam, self).zero_grad()
 
-    def step(self, closure=None, grads=None, output_params=None, scale=None, grad_norms=None):
+    def step(self, closure=None, grads=None, output_params=None, scale=None, grad_norms=None, grad_scaler=None):
         """Performs a single optimization step.
 
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
 
         The remaining arguments are deprecated, and are only retained (for the moment) for error-checking purposes.
@@ -95,61 +118,78 @@
                 'FusedAdam has been updated.  Simply initialize it identically to torch.optim.Adam, and call step() with no arguments.'
             )
         loss = None
         if closure is not None:
             loss = closure()
 
         for group in self.param_groups:
+            if len(group['params']) == 0:
+                continue
             bias_correction = 1 if group['bias_correction'] else 0
             beta1, beta2 = group['betas']
 
+            # assume same step across group now to simplify things
+            # per parameter step can be easily support by making it tensor, or pass list into kernel
             if 'step' not in group:
                 group['step'] = 0
 
             # create lists for multi-tensor apply
             g_16, p_16, m_16, v_16 = [], [], [], []
+            g_bf, p_bf, m_bf, v_bf = [], [], [], []
             g_32, p_32, m_32, v_32 = [], [], [], []
 
             for p in group['params']:
                 if p.grad is None:
                     continue
                 if p.grad.data.is_sparse:
                     raise RuntimeError(
                         'FusedAdam does not support sparse gradients, please consider SparseAdam instead')
 
                 state = self.state[p]
                 # State initialization
                 if len(state) == 0:
                     # DeepSpeed ZeRO 3 processes each subgroup a time, so we need to keep tracking step count for each tensor separately.
-                    # While this is not an issue for ZeRO 1 & 2, since they apply a single optimizatin step to the whole param group at the same time.
+                    # While this is not an issue for ZeRO 1 & 2, since they apply a single optimization step to the whole param group at the same time.
                     # In order to keep backward compatibility for the existing checkpoints, we use group['state'] to initialize state['step'] if it exists.
                     state['step'] = group.get('step', 0)
                     # Exponential moving average of gradient values
                     state['exp_avg'] = torch.zeros_like(p.data)
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p.data)
 
                 if p.dtype == torch.float16:
                     g_16.append(p.grad.data)
                     p_16.append(p.data)
                     m_16.append(state['exp_avg'])
                     v_16.append(state['exp_avg_sq'])
+                elif p.dtype == torch.bfloat16:
+                    g_bf.append(p.grad)
+                    p_bf.append(p)
+                    m_bf.append(state['exp_avg'])
+                    v_bf.append(state['exp_avg_sq'])
                 elif p.dtype == torch.float32:
                     g_32.append(p.grad.data)
                     p_32.append(p.data)
                     m_32.append(state['exp_avg'])
                     v_32.append(state['exp_avg_sq'])
                 else:
-                    raise RuntimeError('FusedAdam only support fp16 and fp32.')
+                    raise RuntimeError('FusedAdam only support fp16, bf16 and fp32.')
 
-            if (len(g_16) > 0):
+            if len(g_16) > 0:
                 state['step'] += 1
                 multi_tensor_applier(self.multi_tensor_adam, self._dummy_overflow_buf, [g_16, p_16, m_16, v_16],
                                      group['lr'], beta1, beta2, group['eps'], state['step'], self.adam_w_mode,
                                      bias_correction, group['weight_decay'])
-            if (len(g_32) > 0):
+
+            if len(g_bf) > 0:
+                state['step'] += 1
+                multi_tensor_applier(self.multi_tensor_adam, self._dummy_overflow_buf, [g_bf, p_bf, m_bf, v_bf],
+                                     group['lr'], beta1, beta2, group['eps'], state['step'], self.adam_w_mode,
+                                     bias_correction, group['weight_decay'])
+
+            if len(g_32) > 0:
                 state['step'] += 1
                 multi_tensor_applier(self.multi_tensor_adam, self._dummy_overflow_buf, [g_32, p_32, m_32, v_32],
                                      group['lr'], beta1, beta2, group['eps'], state['step'], self.adam_w_mode,
                                      bias_correction, group['weight_decay'])
 
         return loss
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/StopWatch.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/Timer.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/context.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/conversion_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adam.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/dropout.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_kernel_utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 #if __CUDA_ARCH__ >= 530
 #define HALF_PRECISION_AVAILABLE = 1
 #define PTX_AVAILABLE
 #endif  // __CUDA_ARCH__ >= 530
 
 #if __CUDA_ARCH__ >= 800
 #define ASYNC_COPY_AVAILABLE
-#define BF16_AVAILABLE
 #endif  // __CUDA_ARCH__ >= 800
 
 #include <cooperative_groups.h>
 
 #endif  //__HIP_PLATFORM_HCC__
 
 inline int next_pow2(const int val)
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/feed_forward.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/gelu.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/gemm_test.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/general_kernels.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/normalize_layer.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/reduction_utils.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/simd.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/softmax.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/includes/type_shim.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/dequantize.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/quantize.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu`

 * *Files 15% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(gelu(data_f + bias_f));
         }
@@ -66,23 +67,22 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_gelu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_gelu<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_GELU(T) \
+    template void launch_bias_gelu<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_GELU(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_gelu<__nv_bfloat16>(__nv_bfloat16*,
-                                              const __nv_bfloat16*,
-                                              int,
-                                              int,
-                                              cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_GELU(__nv_bfloat16)
 #endif
-template void launch_bias_gelu<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_GELU(__half)
 
 /*
 In-place channels-last bias add
 */
 template <typename T>
 __global__ void fused_bias_add(T* input, const T* bias, int total_count, int intermediate_size)
 {
@@ -91,15 +91,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(data_f + bias_f);
         }
@@ -123,23 +124,22 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_add<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_add<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_ADD(T) \
+    template void launch_bias_add<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_ADD(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_add<__nv_bfloat16>(__nv_bfloat16*,
-                                             const __nv_bfloat16*,
-                                             int,
-                                             int,
-                                             cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_ADD(__nv_bfloat16)
 #endif
-template void launch_bias_add<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_ADD(__half)
 
 __global__ void fused_bias_residual(float* residual,
                                     const float* hidden_state,
                                     const float* attn,
                                     const float* bias,
                                     const float* attn_bias,
                                     const int total_count,
@@ -278,52 +278,22 @@
                                                               attn_bias,
                                                               total_count,
                                                               hidden_dim / 4,
                                                               1.0 / mp_size,
                                                               preln);
 }
 
-template void launch_bias_residual<
-    float>(float*, float*, float*, float*, float*, int, int, int, bool, cudaStream_t);
-#ifdef BF16_AVAILABLE
-template void launch_bias_residual<__nv_bfloat16>(__nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  __nv_bfloat16*,
-                                                  int,
-                                                  int,
-                                                  int,
-                                                  bool,
-                                                  cudaStream_t);
-#endif
-template void launch_bias_residual<
-    __half>(__half*, __half*, __half*, __half*, __half*, int, int, int, bool, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_RESIDUAL(T) \
+    template void launch_bias_residual<T>(T*, T*, T*, T*, T*, int, int, int, bool, cudaStream_t);
 
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(float);
 #ifdef BF16_AVAILABLE
-template __global__ void fused_bias_residual(__nv_bfloat16* residual,
-                                             const __nv_bfloat16* hidden_state,
-                                             const __nv_bfloat16* attn,
-                                             const __nv_bfloat16* bias,
-                                             const __nv_bfloat16* attn_bias,
-                                             const int total_count,
-                                             const int intermediate_size,
-                                             const float mp_scale,
-                                             const bool preln);
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(__nv_bfloat16);
 #endif
-
-template __global__ void fused_bias_residual(__half* residual,
-                                             const __half* hidden_state,
-                                             const __half* attn,
-                                             const __half* bias,
-                                             const __half* attn_bias,
-                                             const int total_count,
-                                             const int intermediate_size,
-                                             const float mp_scale,
-                                             const bool preln);
+INSTANTIATE_LAUNCH_BIAS_RESIDUAL(__half);
 
 __global__ void gptj_residual_add(float* residual,
                                   const float* hidden_state,
                                   const float* attn,
                                   const float* bias,
                                   const float* attn_bias,
                                   const int total_count,
@@ -442,66 +412,23 @@
     dim3 block_dims(1024);
     dim3 grid_dims((total_count - 1) / 1024 + 1);  // (batch_size);
 
     gptj_residual_add<<<grid_dims, block_dims, 0, stream>>>(
         residual, hidden_state, attn, bias, attn_bias, total_count, hidden_dim / 4, 1.0 / mp_size);
 }
 
-template void launch_gptj_residual_add<float>(float*,
-                                              float*,
-                                              float*,
-                                              float*,
-                                              float*,
-                                              int,
-                                              int,
-                                              int,
-                                              cudaStream_t);
-
-#ifdef BF16_AVAILABLE
-template void launch_gptj_residual_add<__nv_bfloat16>(__nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      __nv_bfloat16*,
-                                                      int,
-                                                      int,
-                                                      int,
-                                                      cudaStream_t);
-#endif
-
-template void launch_gptj_residual_add<__half>(__half*,
-                                               __half*,
-                                               __half*,
-                                               __half*,
-                                               __half*,
-                                               int,
-                                               int,
-                                               int,
-                                               cudaStream_t);
+#define INSTANTIATE_GPT_RES_ADD(T) \
+    template void launch_gptj_residual_add<T>(T*, T*, T*, T*, T*, int, int, int, cudaStream_t);
 
+INSTANTIATE_GPT_RES_ADD(float);
+INSTANTIATE_GPT_RES_ADD(__half);
 #ifdef BF16_AVAILABLE
-template __global__ void gptj_residual_add(__nv_bfloat16* residual,
-                                           const __nv_bfloat16* hidden_state,
-                                           const __nv_bfloat16* attn,
-                                           const __nv_bfloat16* bias,
-                                           const __nv_bfloat16* attn_bias,
-                                           const int total_count,
-                                           const int intermediate_size,
-                                           const float mp_scale);
+INSTANTIATE_GPT_RES_ADD(__nv_bfloat16);
 #endif
 
-template __global__ void gptj_residual_add(__half* residual,
-                                           const __half* hidden_state,
-                                           const __half* attn,
-                                           const __half* bias,
-                                           const __half* attn_bias,
-                                           const int total_count,
-                                           const int intermediate_size,
-                                           const float mp_scale);
-
 template <typename T>
 __global__ void moe_res_matmul(T* residual, T* coef, T* mlp_out, int seq_len, int hidden_dim)
 {
     constexpr int granularity = 16;
     constexpr int vals_per_access = granularity / sizeof(T);
 
     T* residual_seq = residual + blockIdx.x * hidden_dim;
@@ -538,36 +465,22 @@
 {
     dim3 grid_dim(seq_len);
     dim3 block_dim(1024);
     moe_res_matmul<<<grid_dim, block_dim, 0, stream>>>(
         residual, coef, mlp_out, seq_len, hidden_dim);
 }
 
-template void launch_moe_res_matmul(float* residual,
-                                    float* coef,
-                                    float* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+#define INSTANTIATE_LAUNCH_MOE_RES_MATMUL(T) \
+    template void launch_moe_res_matmul<T>(T*, T*, T*, int, int, cudaStream_t);
 
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(float);
 #ifdef BF16_AVAILABLE
-template void launch_moe_res_matmul(__nv_bfloat16* residual,
-                                    __nv_bfloat16* coef,
-                                    __nv_bfloat16* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(__nv_bfloat16);
 #endif
-
-template void launch_moe_res_matmul(__half* residual,
-                                    __half* coef,
-                                    __half* mlp_out,
-                                    int seq_len,
-                                    int hidden_dim,
-                                    cudaStream_t stream);
+INSTANTIATE_LAUNCH_MOE_RES_MATMUL(__half);
 
 template <typename T>
 __global__ void pad_data_kernel(T* padded_output, T* output, int head_size, int padded_head_size)
 {
     using T2 =
         typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
@@ -603,49 +516,23 @@
               cudaStream_t stream)
 {
     dim3 grid_dim((bsz - 1) / 16 + 1);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_data_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, head_size / 8, padded_head_size / 8);
 }
-template void pad_data(__half* padded_output,
-                       __half* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
 
-#ifdef BF16_AVAILABLE
-template void pad_data(__nv_bfloat16* padded_output,
-                       __nv_bfloat16* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
-#endif
-
-template void pad_data(float* padded_output,
-                       float* output,
-                       int bsz,
-                       int head_size,
-                       int padded_head_size,
-                       cudaStream_t stream);
+#define INSTANTIATE_PAD_DATA(T) template void pad_data(T*, T*, int, int, int, cudaStream_t stream);
 
+INSTANTIATE_PAD_DATA(float);
+INSTANTIATE_PAD_DATA(__half);
 #ifdef BF16_AVAILABLE
-template __global__ void pad_data_kernel(__nv_bfloat16* padded_output,
-                                         __nv_bfloat16* output,
-                                         int head_size,
-                                         int padded_head_size);
+INSTANTIATE_PAD_DATA(__nv_bfloat16);
 #endif
 
-template __global__ void pad_data_kernel(__half* padded_output,
-                                         __half* output,
-                                         int head_size,
-                                         int padded_head_size);
-
 template <typename T>
 __global__ void pad_head_seq_kernel(T* padded_output,
                                     T* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
@@ -692,42 +579,22 @@
 {
     dim3 grid_dim(bsz, padded_seq_len / 16);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_head_seq_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, seq_len, padded_seq_len, head_size / 8, padded_head_size / 8);
 }
 
-template void pad_head_seq(__half* padded_output,
-                           __half* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+#define INSTANTIATE_PAD_HEAD_SEQ(T) \
+    template void pad_head_seq<T>(T*, T*, int, int, int, int, int, cudaStream_t);
 
+INSTANTIATE_PAD_HEAD_SEQ(__half);
 #ifdef BF16_AVAILABLE
-template void pad_head_seq(__nv_bfloat16* padded_output,
-                           __nv_bfloat16* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+INSTANTIATE_PAD_HEAD_SEQ(__nv_bfloat16);
 #endif
-
-template void pad_head_seq(float* padded_output,
-                           float* output,
-                           int bsz,
-                           int seq_len,
-                           int padded_seq_len,
-                           int head_size,
-                           int padded_head_size,
-                           cudaStream_t stream);
+INSTANTIATE_PAD_HEAD_SEQ(float);
 
 // TODO(cmikeh2): evaluate different GeLU performance
 __device__ __forceinline__ float old_gelu(float val)
 {
     // 1 / sqrt(2)
     constexpr float rsqrt_2 = 0.707106769084930419922;
     return val * 0.5f * (1.0f + erff(val * rsqrt_2));
@@ -735,20 +602,23 @@
 
 namespace fused_geglu {
 constexpr int threads = 256;
 constexpr int steps = 2;
 constexpr int granularity = 16;
 }  // namespace fused_geglu
 
-template <typename T>
-__global__ void fused_bias_geglu(T* output,
-                                 const T* activation,
-                                 const T* bias,
-                                 int base_channels,
-                                 int total_elems)
+__device__ __forceinline__ float silu(float val) { return val / (1.0f + expf(-val)); }
+
+template <typename T, bool useGelu>
+__global__ void fused_gate_activation(T* output,
+                                      const T* activation,
+                                      const T* bias,
+                                      int base_channels,
+                                      int output_stride,
+                                      int total_elems)
 {
     constexpr int T_per_access = fused_geglu::granularity / sizeof(T);
     constexpr int T_per_step = T_per_access * fused_geglu::threads;
     constexpr int T_per_block = T_per_step * fused_geglu::steps;
 
     const int id = blockIdx.x * T_per_block + threadIdx.x * T_per_access;
 
@@ -765,41 +635,45 @@
             const int seq_id = iter_id / base_channels;
             const int seq_offset = seq_id * base_channels * 2;
 
             mem_access::load_global<fused_geglu::granularity>(activation_buffer_1,
                                                               activation + seq_offset + channel_id);
             mem_access::load_global<fused_geglu::granularity>(
                 activation_buffer_2, activation + seq_offset + channel_id + base_channels);
-            mem_access::load_global<fused_geglu::granularity>(bias_buffer_1, bias + channel_id);
-            mem_access::load_global<fused_geglu::granularity>(bias_buffer_2,
-                                                              bias + channel_id + base_channels);
+            mem_access::load_global<fused_geglu::granularity>(
+                bias_buffer_1, bias + channel_id, bias != nullptr);
+            mem_access::load_global<fused_geglu::granularity>(
+                bias_buffer_2, bias + channel_id + base_channels, bias != nullptr);
 
             // Since the GeLU is going to happen at float, might as well
             // convert
 #pragma unroll
             for (int v = 0; v < T_per_access; v++) {
                 T hidden_state = activation_buffer_1[v] + bias_buffer_1[v];
                 T pre_gate = activation_buffer_2[v] + bias_buffer_2[v];
-                float gate_f = old_gelu(conversion::to<float>(pre_gate));
+                float pre_gate_f = conversion::to<float>(pre_gate);
+                float gate_f = (useGelu) ? old_gelu(pre_gate_f) : silu(pre_gate_f);
                 T gate = conversion::to<T>(gate_f);
                 activation_buffer_1[v] = hidden_state * gate;
             }
 
-            mem_access::store_global<fused_geglu::granularity>(output + iter_id,
-                                                               activation_buffer_1);
+            mem_access::store_global<fused_geglu::granularity>(
+                output + seq_id * output_stride + channel_id, activation_buffer_1);
         }
     }
 }
 
 template <typename T>
-void launch_fused_bias_geglu(T* output,
+void launch_gated_activation(T* output,
                              const T* activation,
                              const T* bias,
                              int rows,
+                             int output_stride,
                              int elems_per_row,
+                             bool use_gelu,
                              cudaStream_t stream)
 {
     /*
     Fused bias GEGLU is a variant of the gated activation functions.
     The input here is a matrix of [batch, seq_len, 2 * intermediate_dim]
     where the second half of the channels act as GeLU gates for the first
     half.
@@ -812,26 +686,25 @@
 
     const int base_channels = elems_per_row / 2;
     const int total_elems = base_channels * rows;
 
     dim3 block(fused_geglu::threads);
     dim3 grid((total_elems + T_per_block - 1) / T_per_block);
 
-    fused_bias_geglu<<<grid, block, 0, stream>>>(
-        output, activation, bias, base_channels, total_elems);
+    if (use_gelu) {
+        fused_gate_activation<T, true><<<grid, block, 0, stream>>>(
+            output, activation, bias, base_channels, output_stride, total_elems);
+    } else {
+        fused_gate_activation<T, false><<<grid, block, 0, stream>>>(
+            output, activation, bias, base_channels, output_stride, total_elems);
+    }
 }
 
-template void launch_fused_bias_geglu(__half*,
-                                      const __half*,
-                                      const __half*,
-                                      int,
-                                      int,
-                                      cudaStream_t);
+#define INSTANTIATE_LAUNCH_GATED_ACTIVATION(T) \
+    template void launch_gated_activation(     \
+        T*, const T*, const T*, int, int, int, bool, cudaStream_t);
+
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(__half);
 #ifdef BF16_AVAILABLE
-template void launch_fused_bias_geglu(__nv_bfloat16*,
-                                      const __nv_bfloat16*,
-                                      const __nv_bfloat16*,
-                                      int,
-                                      int,
-                                      cudaStream_t);
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(__nv_bfloat16);
 #endif
-template void launch_fused_bias_geglu(float*, const float*, const float*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_GATED_ACTIVATION(float);
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files 12% similar despite different names*

```diff
@@ -42,27 +42,25 @@
     cg::thread_block_tile<hw_warp_size> warp = cg::tiled_partition<hw_warp_size>(tb);
 
     // X-dimension of the block
     const int block_offset = (tb.group_index().x * (maxThreads / threadsPerGroup) * elems_per_row) +
                              (tb.thread_index().y * elems_per_row);
     const int thread_offset = tb.thread_index().x * T_per_load;
     const int base_offset = block_offset + thread_offset;
-    const int stride = tb.size() * T_per_load;
+    const int stride = blockDim.x * T_per_load;
 
     float sum = reduce::init<rop::Add, float>();
 
     const T* input_base = vals + base_offset;
 
     T local_buffer[unRoll * T_per_load];
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
-        T residual_buffer[T_per_load];
-        T bias_buffer[T_per_load];
 
         mem_access::load_global<ln::granularity>(
             iteration_buffer, input_base + i * stride, thread_offset + i * stride < elems_per_row);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
             float vals_up_cast = conversion::to<float>(iteration_buffer[j]);
@@ -87,16 +85,16 @@
         }
     }
 
     reduce::partitioned_block<rop::Add, threadsPerGroup>(tb, warp, mean_diff);
     const float variance = mean_diff / elems_per_row;
     const float denom = __frsqrt_rn(variance + epsilon);
 
-    const T mean_compute = conversion::to<T>(mean);
-    const T denom_compute = conversion::to<T>(denom);
+    // const T mean_compute = conversion::to<T>(mean);
+    // const T denom_compute = conversion::to<T>(denom);
 
     T* block_output = output + block_offset;
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
         const int iter_idx = i * stride + thread_offset;
@@ -105,16 +103,19 @@
         T gamma_local[T_per_load], beta_local[T_per_load];
 
         mem_access::load_global<ln::granularity>(gamma_local, gamma + iter_idx, do_loads);
         mem_access::load_global<ln::granularity>(beta_local, beta + iter_idx, do_loads);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
-            iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
-            iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            float val = conversion::to<float>(iteration_buffer[j]);
+            val = (val - mean) * denom;
+            val =
+                val * conversion::to<float>(gamma_local[j]) + conversion::to<float>(beta_local[j]);
+            iteration_buffer[j] = conversion::to<T>(val);
         }
 
         if (do_loads) {
             mem_access::store_global<ln::granularity>(block_output + iter_idx, iteration_buffer);
         }
     }
 }
@@ -185,34 +186,22 @@
         LAUNCH_FUSED_LN(3 * internal_unRoll, maxThreads, maxThreads);
     } else if (external_unRoll == 4) {
         // 12289 - 16384 elems
         LAUNCH_FUSED_LN(4 * internal_unRoll, maxThreads, maxThreads);
     }
 }
 
-template void launch_fused_ln(__half*,
-                              const __half*,
-                              const __half*,
-                              const __half*,
-                              float,
-                              int,
-                              int,
-                              cudaStream_t);
+#define INSTANTIATE_FUSED_LN(T) \
+    template void launch_fused_ln(T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
+
+INSTANTIATE_FUSED_LN(__half);
 #ifdef BF16_AVAILABLE
-template void launch_fused_ln(__nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              const __nv_bfloat16*,
-                              float,
-                              int,
-                              int,
-                              cudaStream_t);
+INSTANTIATE_FUSED_LN(__nv_bfloat16);
 #endif
-template void
-launch_fused_ln(float*, const float*, const float*, const float*, float, int, int, cudaStream_t);
+INSTANTIATE_FUSED_LN(float);
 
 /*
 Fused resiual + bias + layer norm implementation. Assumes elems_per_row % 8
 is equal to 0.
 
 TODO(cmikeh2): Goal is to deprecate this implementation. The bias + residual
 need to be fused into compute-bound producer operations.
@@ -280,15 +269,15 @@
             bias_buffer, bias_base + i * stride, thread_offset + i * stride < elems_per_row);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
             float vals_up_cast = conversion::to<float>(iteration_buffer[j]);
             float res_up_cast = conversion::to<float>(residual_buffer[j]);
             float bias_up_cast = conversion::to<float>(bias_buffer[j]);
-            vals_up_cast += res_up_cast + bias_up_cast;
+            vals_up_cast = vals_up_cast + bias_up_cast + res_up_cast;
             sum = reduce::element<rop::Add>(sum, vals_up_cast);
             iteration_buffer[j] = conversion::to<T>(vals_up_cast);
         }
 
         if (preLnResidual && (thread_offset + i * stride < elems_per_row)) {
             mem_access::store_global<ln::granularity>(res_output + base_offset + i * stride,
                                                       iteration_buffer);
@@ -311,17 +300,14 @@
         }
     }
 
     reduce::partitioned_block<rop::Add, threadsPerGroup>(tb, warp, mean_diff);
     const float variance = mean_diff / elems_per_row;
     const float denom = __frsqrt_rn(variance + epsilon);
 
-    const T mean_compute = conversion::to<T>(mean);
-    const T denom_compute = conversion::to<T>(denom);
-
     T* block_output = output + block_offset;
 
 #pragma unRoll
     for (int i = 0; i < unRoll; i++) {
         T* iteration_buffer = local_buffer + i * T_per_load;
         const int iter_idx = i * stride + thread_offset;
         const bool do_loads = iter_idx < elems_per_row;
@@ -329,16 +315,21 @@
         T gamma_local[T_per_load], beta_local[T_per_load];
 
         mem_access::load_global<ln::granularity>(gamma_local, gamma + iter_idx, do_loads);
         mem_access::load_global<ln::granularity>(beta_local, beta + iter_idx, do_loads);
 
 #pragma unRoll
         for (int j = 0; j < T_per_load; j++) {
-            iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
-            iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            // iteration_buffer[j] = (iteration_buffer[j] - mean_compute) * denom_compute;
+            // iteration_buffer[j] = iteration_buffer[j] * gamma_local[j] + beta_local[j];
+            float val = conversion::to<float>(iteration_buffer[j]);
+            val = (val - mean) * denom;
+            val =
+                val * conversion::to<float>(gamma_local[j]) + conversion::to<float>(beta_local[j]);
+            iteration_buffer[j] = conversion::to<T>(val);
         }
 
         if (do_loads) {
             mem_access::store_global<ln::granularity>(block_output + iter_idx, iteration_buffer);
         }
     }
 }
@@ -487,81 +478,26 @@
         LAUNCH_FUSED_RES_LN_STORE_PRE_LN_RES(3 * internal_unRoll, maxThreads, maxThreads);
     } else if (external_unRoll == 4) {
         // 12289 - 16384 elems
         LAUNCH_FUSED_RES_LN_STORE_PRE_LN_RES(4 * internal_unRoll, maxThreads, maxThreads);
     }
 }
 
-// No-store specializations
-template void launch_fused_residual_ln(__half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       const __half*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
+#define INSTANTIATE_RES_LN(T)                  \
+    template void launch_fused_residual_ln<T>( \
+        T*, const T*, const T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
+
+#define INSTANTIATE_PRE_LN_RES(T)                               \
+    template void launch_fused_residual_ln_store_pre_ln_res<T>( \
+        T*, T*, const T*, const T*, const T*, const T*, const T*, float, int, int, cudaStream_t);
 
+INSTANTIATE_RES_LN(__half);
+INSTANTIATE_RES_LN(float);
 #ifdef BF16_AVAILABLE
-template void launch_fused_residual_ln(__nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       const __nv_bfloat16*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
+INSTANTIATE_RES_LN(__nv_bfloat16);
 #endif
 
-template void launch_fused_residual_ln(float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       const float*,
-                                       float,
-                                       int,
-                                       int,
-                                       cudaStream_t);
-
-// Store specializations
-template void launch_fused_residual_ln_store_pre_ln_res(__half*,
-                                                        __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        const __half*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
-
+INSTANTIATE_PRE_LN_RES(__half);
+INSTANTIATE_PRE_LN_RES(float);
 #ifdef BF16_AVAILABLE
-template void launch_fused_residual_ln_store_pre_ln_res(__nv_bfloat16*,
-                                                        __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        const __nv_bfloat16*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
+INSTANTIATE_PRE_LN_RES(__nv_bfloat16);
 #endif
-
-template void launch_fused_residual_ln_store_pre_ln_res(float*,
-                                                        float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        const float*,
-                                                        float,
-                                                        int,
-                                                        int,
-                                                        cudaStream_t);
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 #include "inference_cuda_layers.h"
 
 std::array<int, 3> gemm_algos = std::array<int, 3>({99, 99, 99});
 
 // NOTE: This activation function type enum should be always in sync
 // with the python counterpart, otherwise the casting from python binding
 // will be incorrect.
-enum class ActivationFuncType { UNKNOWN = 0, GELU = 1, ReLU = 2 };
+enum class ActivationFuncType { UNKNOWN = 0, GELU = 1, ReLU = 2, GATED_GELU = 3, GATED_SILU = 4 };
+
+enum class NormType { UNKNOWN = 0, LayerNorm = 1, GroupNorm = 2, RMSNorm = 3 };
 
 enum class TransformerType : uint8_t { UNKNOWN = 0, GPTType = 1, BERTType = 2 };
 
 // NOTE: this is a temporary and dodgy solution to distinguish GPT and BERT style models
 // based on the dimensions of the corresponding attention mask.
 inline auto infer_transformer_type(at::Tensor& attn_mask) -> TransformerType
 {
@@ -137,15 +139,15 @@
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     float alpha = 1;
     float gemm_beta = 0.0;
 
     /*
     // Reallocate memory if we received a new prompt
     if (!workspace || input.size(1) != 1) {
-        allocate_workspace<T>(W.size(1), InferenceContext::Instance().GetMaxTokenLenght(),
+        allocate_workspace<T>(W.size(1), InferenceContext::Instance().GetMaxTokenLength(),
     Q.size(0), 1, head_size); workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     }
     */
 
     auto O = at::from_blob(workspace, {Q.size(1), Q.size(2), W.size(1)}, options);
     unsigned m = W.size(1);
     unsigned n = Q.size(1) * Q.size(2);
@@ -378,15 +380,15 @@
                                 &alpha,
                                 &gemm_beta,
                                 (T*)prev_key_cont,
                                 (T*)query_cont,
                                 workspace,
                                 CUBLAS_OP_T,
                                 CUBLAS_OP_N,
-                                InferenceContext::Instance().GetMaxTokenLenght() * k,
+                                InferenceContext::Instance().GetMaxTokenLength() * k,
                                 seq_len * k,
                                 seq_len * soft_len,
                                 bsz * heads,
 #ifdef __HIP_PLATFORM_HCC__
                                 rocblas_gemm_algo_standard);
 #else
                                 CUBLAS_GEMM_DEFAULT_TENSOR_OP);
@@ -411,15 +413,15 @@
                                 &alpha,
                                 &gemm_beta,
                                 (T*)prev_value_cont,
                                 workspace,
                                 (T*)output,
                                 CUBLAS_OP_N,
                                 CUBLAS_OP_N,
-                                InferenceContext::Instance().GetMaxTokenLenght() * k,
+                                InferenceContext::Instance().GetMaxTokenLength() * k,
                                 seq_len * soft_len,
                                 seq_len * k,
                                 bsz * heads,
 #ifdef __HIP_PLATFORM_HCC__
                                 rocblas_gemm_algo_standard);
 #else
                                 CUBLAS_GEMM_DEFAULT_TENSOR_OP);
@@ -462,19 +464,19 @@
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     size_t buf_size = bsz * seq_len * hidden_dim;
     auto output = torch::from_blob(workspace + 4 * buf_size, {bsz, seq_len, hidden_dim}, options);
 
     auto query_cont = workspace + 5 * buf_size;
     size_t offset =
-        10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLenght()) +
-        layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
+        10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLength()) +
+        layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLength() * hidden_dim;
     unsigned all_tokens = soft_len;
     auto kv_cache = workspace + offset + (hidden_dim / heads) * (is_prompt ? 0 : soft_len - 1);
-    size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
+    size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLength() * hidden_dim;
 
     T* temp_buf = (T*)output.data_ptr() + at::numel(output);
     launch_bias_add_transform_0213<T>((T*)query_cont,
                                       kv_cache,
                                       kv_cache + value_offset,
                                       (T*)query_key_value.data_ptr(),
                                       nullptr,
@@ -485,28 +487,26 @@
                                       hidden_dim,
                                       heads,
                                       rotary_dim,
                                       rotate_half,
                                       rotate_every_two,
                                       InferenceContext::Instance().GetCurrentStream(),
                                       3,
-                                      InferenceContext::Instance().GetMaxTokenLenght());
+                                      InferenceContext::Instance().GetMaxTokenLength());
     if (rotary_dim > 0 && rotate_half)
         launch_apply_rotary_pos_emb(query_cont,
                                     kv_cache,
                                     k,
                                     seq_len,
                                     rotary_dim,
                                     (is_prompt ? 0 : soft_len - 1),
                                     heads,
                                     bsz,
-                                    rotate_half,
-                                    rotate_every_two,
                                     InferenceContext::Instance().GetCurrentStream(),
-                                    InferenceContext::Instance().GetMaxTokenLenght());
+                                    InferenceContext::Instance().GetMaxTokenLength());
 
     attention_unfused<T>(workspace + offset,
                          (T*)query_cont,
                          attn_mask,
                          workspace + offset + value_offset,
                          temp_buf,
                          bsz,
@@ -529,25 +529,25 @@
                                output.size(2),
                                InferenceContext::Instance().GetCurrentStream(false),
                                1);
 
     if (layer_id == num_layers - 1) InferenceContext::Instance().advance_tokens();
     auto prev_key = torch::from_blob(workspace + offset,
                                      {bsz, heads, all_tokens, k},
-                                     {hidden_dim * InferenceContext::Instance().GetMaxTokenLenght(),
-                                      k * InferenceContext::Instance().GetMaxTokenLenght(),
+                                     {hidden_dim * InferenceContext::Instance().GetMaxTokenLength(),
+                                      k * InferenceContext::Instance().GetMaxTokenLength(),
                                       k,
                                       1},
                                      options);
 
     auto prev_value =
         torch::from_blob(workspace + offset + value_offset,
                          {bsz, heads, all_tokens, k},
-                         {hidden_dim * InferenceContext::Instance().GetMaxTokenLenght(),
-                          k * InferenceContext::Instance().GetMaxTokenLenght(),
+                         {hidden_dim * InferenceContext::Instance().GetMaxTokenLength(),
+                          k * InferenceContext::Instance().GetMaxTokenLength(),
                           k,
                           1},
                          options);
 
     return {output, prev_key, prev_value};
 }
 
@@ -563,45 +563,52 @@
                      (T*)bias.data_ptr(),
                      intermediate_size,
                      bsz,
                      InferenceContext::Instance().GetCurrentStream());
     return input_cont;
 }
 
-at::Tensor ds_bias_geglu(at::Tensor& activation, at::Tensor& bias)
+#define DISPATCH_GATED_ACT(T_TYPE, C_TYPE)                                         \
+    if (activation.options().dtype() == torch::T_TYPE) {                           \
+        launch_gated_activation((C_TYPE*)output.data_ptr(),                        \
+                                (const C_TYPE*)activation.data_ptr(),              \
+                                (const C_TYPE*)bias.data_ptr(),                    \
+                                rows,                                              \
+                                out_channels,                                      \
+                                channels,                                          \
+                                activation_type == ActivationFuncType::GATED_GELU, \
+                                InferenceContext::Instance().GetCurrentStream());  \
+    }
+
+at::Tensor ds_gated_activation(at::Tensor& activation, at::Tensor& bias, int actFun)
 {
     /*
     Used in FF of Stable diffusion
     */
 
+    const ActivationFuncType activation_type = static_cast<ActivationFuncType>(actFun);
+
+    assert(activation_type == ActivationFuncType::GATED_GELU ||
+           activation_type == ActivationFuncType::GATED_SILU);
+
     const int batch_size = activation.size(0);
     const int seq_len = activation.size(1);
     const int channels = activation.size(2);
 
     const int rows = batch_size * seq_len;
     // Dimensionality is cut in half
     const int out_channels = channels / 2;
 
     auto output = at::empty({batch_size, seq_len, out_channels}, activation.options());
 
-    if (activation.options().dtype() == torch::kFloat32) {
-        launch_fused_bias_geglu((float*)output.data_ptr(),
-                                (const float*)activation.data_ptr(),
-                                (const float*)bias.data_ptr(),
-                                rows,
-                                channels,
-                                InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_bias_geglu((__half*)output.data_ptr(),
-                                (const __half*)activation.data_ptr(),
-                                (const __half*)bias.data_ptr(),
-                                rows,
-                                channels,
-                                InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_GATED_ACT(kFloat, float);
+    DISPATCH_GATED_ACT(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_GATED_ACT(kBFloat16, __nv_bfloat16);
+#endif
 
     return output;
 }
 
 template <typename T>
 at::Tensor ds_bias_relu(at::Tensor& input, at::Tensor& bias)
 {
@@ -647,43 +654,107 @@
     //                      bsz,
     //                      input_cont.size(2),
     //                      (bias.size(0) > 1),
     //                      InferenceContext::Instance().GetCurrentStream());
     return input_cont;
 }
 
+#define DISPATCH_LAYER_NORM(T_TYPE, C_TYPE)                               \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_fused_ln((C_TYPE*)output.data_ptr(),                       \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        (const C_TYPE*)beta.data_ptr(),                   \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 at::Tensor ds_layer_norm(at::Tensor& input, at::Tensor& gamma, at::Tensor& beta, float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_ln((__half*)output.data_ptr(),
-                        (const __half*)input.data_ptr(),
-                        (const __half*)gamma.data_ptr(),
-                        (const __half*)beta.data_ptr(),
-                        epsilon,
-                        rows,
-                        elems_per_row,
-                        InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_ln((float*)output.data_ptr(),
-                        (const float*)input.data_ptr(),
-                        (const float*)gamma.data_ptr(),
-                        (const float*)beta.data_ptr(),
-                        epsilon,
-                        rows,
-                        elems_per_row,
-                        InferenceContext::Instance().GetCurrentStream());
+    DISPATCH_LAYER_NORM(kFloat, float);
+    DISPATCH_LAYER_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_LAYER_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
+    return output;
+}
+
+#define DISPATCH_RMS_NORM(T_TYPE, C_TYPE)                                 \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_rms_norm((C_TYPE*)output.data_ptr(),                       \
+                        (C_TYPE*)nullptr,                                 \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)nullptr,                           \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
     }
 
+at::Tensor ds_rms_norm(at::Tensor& input, at::Tensor& gamma, float epsilon)
+{
+    // Get number of dims of tensor
+    int num_dims = input.dim();
+    const int rows = (num_dims == 2) ? input.size(0) : input.size(0) * input.size(1);
+    const int elems_per_row = (num_dims == 2) ? input.size(1) : input.size(2);
+
+    auto output = at::empty_like(input);
+
+    DISPATCH_RMS_NORM(kFloat, float);
+    DISPATCH_RMS_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_RMS_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
     return output;
 }
 
+#define DISPATCH_PRE_RMS_NORM(T_TYPE, C_TYPE)                             \
+    if (input.options().dtype() == torch::T_TYPE) {                       \
+        launch_rms_norm((C_TYPE*)output.data_ptr(),                       \
+                        (C_TYPE*)res_out.data_ptr(),                      \
+                        (const C_TYPE*)input.data_ptr(),                  \
+                        (const C_TYPE*)residual.data_ptr(),               \
+                        (const C_TYPE*)gamma.data_ptr(),                  \
+                        epsilon,                                          \
+                        rows,                                             \
+                        elems_per_row,                                    \
+                        InferenceContext::Instance().GetCurrentStream()); \
+    }
+
+std::vector<at::Tensor> ds_pre_rms_norm(at::Tensor& input,
+                                        at::Tensor& residual,
+                                        at::Tensor& gamma,
+                                        float epsilon)
+{
+    // Get number of dims of tensor
+    int num_dims = input.dim();
+    const int rows = (num_dims == 2) ? input.size(0) : input.size(0) * input.size(1);
+    const int elems_per_row = (num_dims == 2) ? input.size(1) : input.size(2);
+
+    auto output = at::empty_like(input);
+    auto res_out = at::empty_like(residual);
+
+    DISPATCH_PRE_RMS_NORM(kFloat, float);
+    DISPATCH_PRE_RMS_NORM(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_PRE_RMS_NORM(kBFloat16, __nv_bfloat16);
+#endif
+
+    return {output, res_out};
+}
+
 template <typename T>
 void ds_layer_norm_internal(T* workspace,
                             at::Tensor& input,
                             at::Tensor& gamma,
                             at::Tensor& beta,
                             float epsilon)
 {
@@ -694,91 +765,83 @@
                     (const T*)beta.data_ptr(),
                     epsilon,
                     bsz,
                     input.size(2),
                     InferenceContext::Instance().GetCurrentStream());
 }
 
+#define DISPATCH_LAYER_NORM_RESIDUAL(T_TYPE, C_TYPE)                               \
+    if (input.options().dtype() == torch::T_TYPE) {                                \
+        launch_fused_residual_ln((C_TYPE*)output.data_ptr(),                       \
+                                 (const C_TYPE*)input.data_ptr(),                  \
+                                 (const C_TYPE*)residual.data_ptr(),               \
+                                 (const C_TYPE*)bias.data_ptr(),                   \
+                                 (const C_TYPE*)gamma.data_ptr(),                  \
+                                 (const C_TYPE*)beta.data_ptr(),                   \
+                                 epsilon,                                          \
+                                 rows,                                             \
+                                 elems_per_row,                                    \
+                                 InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 /* Currently only used in unit testing */
 at::Tensor ds_layer_norm_residual(at::Tensor& input,
                                   at::Tensor& bias,
                                   at::Tensor& residual,
                                   at::Tensor& gamma,
                                   at::Tensor& beta,
                                   float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_residual_ln((__half*)output.data_ptr(),
-                                 (const __half*)input.data_ptr(),
-                                 (const __half*)residual.data_ptr(),
-                                 (const __half*)bias.data_ptr(),
-                                 (const __half*)gamma.data_ptr(),
-                                 (const __half*)beta.data_ptr(),
-                                 epsilon,
-                                 rows,
-                                 elems_per_row,
-                                 InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_residual_ln((float*)output.data_ptr(),
-                                 (const float*)input.data_ptr(),
-                                 (const float*)residual.data_ptr(),
-                                 (const float*)bias.data_ptr(),
-                                 (const float*)gamma.data_ptr(),
-                                 (const float*)beta.data_ptr(),
-                                 epsilon,
-                                 rows,
-                                 elems_per_row,
-                                 InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_LAYER_NORM_RESIDUAL(kFloat, float);
+    DISPATCH_LAYER_NORM_RESIDUAL(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_LAYER_NORM_RESIDUAL(kBFloat16, __nv_bfloat16);
+#endif
 
     return output;
 }
 
+#define DISPATCH_PRE_LAYER_NORM_RESIDUAL(T_TYPE, C_TYPE)      \
+    if (input.options().dtype() == torch::T_TYPE) {           \
+        launch_fused_residual_ln_store_pre_ln_res(            \
+            (C_TYPE*)norm_output.data_ptr(),                  \
+            (C_TYPE*)res_output.data_ptr(),                   \
+            (const C_TYPE*)input.data_ptr(),                  \
+            (const C_TYPE*)residual.data_ptr(),               \
+            (const C_TYPE*)bias.data_ptr(),                   \
+            (const C_TYPE*)gamma.data_ptr(),                  \
+            (const C_TYPE*)beta.data_ptr(),                   \
+            epsilon,                                          \
+            rows,                                             \
+            elems_per_row,                                    \
+            InferenceContext::Instance().GetCurrentStream()); \
+    }
+
 /* Currently only used in unit testing */
 std::vector<at::Tensor> ds_layer_norm_residual_store_pre_ln_res(at::Tensor& input,
                                                                 at::Tensor& bias,
                                                                 at::Tensor& residual,
                                                                 at::Tensor& gamma,
                                                                 at::Tensor& beta,
                                                                 float epsilon)
 {
     const int rows = input.size(0) * input.size(1);
     const int elems_per_row = input.size(2);
     auto norm_output = at::empty_like(input);
     auto res_output = at::empty_like(input);
 
-    if (input.options().dtype() == torch::kFloat16) {
-        launch_fused_residual_ln_store_pre_ln_res((__half*)norm_output.data_ptr(),
-                                                  (__half*)res_output.data_ptr(),
-                                                  (const __half*)input.data_ptr(),
-                                                  (const __half*)residual.data_ptr(),
-                                                  (const __half*)bias.data_ptr(),
-                                                  (const __half*)gamma.data_ptr(),
-                                                  (const __half*)beta.data_ptr(),
-                                                  epsilon,
-                                                  rows,
-                                                  elems_per_row,
-                                                  InferenceContext::Instance().GetCurrentStream());
-    } else {
-        launch_fused_residual_ln_store_pre_ln_res((float*)norm_output.data_ptr(),
-                                                  (float*)res_output.data_ptr(),
-                                                  (const float*)input.data_ptr(),
-                                                  (const float*)residual.data_ptr(),
-                                                  (const float*)bias.data_ptr(),
-                                                  (const float*)gamma.data_ptr(),
-                                                  (const float*)beta.data_ptr(),
-                                                  epsilon,
-                                                  rows,
-                                                  elems_per_row,
-                                                  InferenceContext::Instance().GetCurrentStream());
-    }
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kFloat, float);
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kHalf, __half);
+#ifdef BF16_AVAILABLE
+    DISPATCH_PRE_LAYER_NORM_RESIDUAL(kBFloat16, __nv_bfloat16);
+#endif
 
     return {norm_output, res_output};
 }
 
 template <typename T>
 void quantized_gemm(void* output,
                     T* input,
@@ -875,26 +938,89 @@
                         (transposed_mode || q_int8) ? weight.size(0) : weight.size(1),
                         bsz,
                         InferenceContext::Instance().GetCurrentStream());
     return torch::from_blob(workspace, input.sizes(), input.options());
 }
 
 template <typename T>
+std::vector<at::Tensor> ds_rms_qkv(at::Tensor& input,
+                                   at::Tensor& weight,
+                                   at::Tensor& q_scale,
+                                   at::Tensor& gamma,
+                                   const float epsilon,
+                                   bool q_int8,
+                                   bool transposed_mode)
+{
+    const int bsz = input.size(0) * input.size(1);
+    T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
+    T* rms_norm_ptr = workspace + (3 * bsz * input.size(2));
+    int out_size = (transposed_mode || q_int8) ? weight.size(0) : weight.size(1);
+
+    auto options = at::TensorOptions()
+                       .dtype(input.options().dtype())
+                       .layout(at::kStrided)
+                       .device(at::kCUDA)
+                       .requires_grad(false);
+    auto rms_norm = at::from_blob(rms_norm_ptr, input.sizes(), options);
+    auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
+
+    launch_rms_norm((T*)rms_norm.data_ptr(),
+                    (T*)nullptr,
+                    (const T*)input.data_ptr(),
+                    (const T*)nullptr,
+                    (const T*)gamma.data_ptr(),
+                    epsilon,
+                    bsz,
+                    input.size(2),
+                    InferenceContext::Instance().GetCurrentStream());
+
+    if (q_int8) {
+        quantized_gemm<T>((T*)output.data_ptr(),
+                          (T*)rms_norm.data_ptr(),
+                          weight,
+                          q_scale,
+                          q_scale.size(0),
+                          bsz,
+                          input.size(2));
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       weight.size(transposed_mode ? 0 : 1),
+                       bsz,
+                       input.size(2),
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight.data_ptr(),
+                       (T*)rms_norm.data_ptr(),
+                       (T*)output.data_ptr(),
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard);
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP);
+#endif
+    }
+
+    return {output, rms_norm};
+}
+
+template <typename T>
 std::vector<at::Tensor> ds_qkv_gemm(at::Tensor& input,
                                     at::Tensor& weight,
                                     at::Tensor& q_scale,
                                     at::Tensor& bias,
                                     at::Tensor& gamma,
                                     at::Tensor& beta,
                                     const float epsilon,
                                     bool add_bias,
-                                    unsigned num_layers,
-                                    bool external_cache,
-                                    unsigned mp_size,
-                                    unsigned rank,
                                     bool q_int8,
                                     bool transposed_mode)
 {
     int bsz = input.size(0) * input.size(1);
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     int out_size = (transposed_mode || q_int8) ? weight.size(0) : weight.size(1);
 
@@ -962,48 +1088,14 @@
                    rocblas_gemm_algo_standard);
 #else
                    CUBLAS_GEMM_DEFAULT_TENSOR_OP);
 #endif
 }
 
 template <typename T>
-at::Tensor ds_qkv_gemm_int8(at::Tensor& input,
-                            at::Tensor& weight,
-                            at::Tensor& bias,
-                            at::Tensor& gamma,
-                            at::Tensor& beta,
-                            const float epsilon,
-                            at::Tensor& q_scale,
-                            int groups,
-                            bool add_bias)
-{
-    int bsz = input.size(0) * input.size(1);
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    auto inp_norm = ds_layer_norm(input_cont, gamma, beta, epsilon);
-
-    quantized_gemm<T>(output, inp_norm, weight, q_scale, groups, 0);
-    if (add_bias)
-        launch_bias_add((T*)output.data_ptr(),
-                        (T*)bias.data_ptr(),
-                        weight.size(1),
-                        bsz,
-                        InferenceContext::Instance().GetCurrentStream());
-
-    return output;
-}
-
-template <typename T>
 at::Tensor ds_linear_layer(at::Tensor& input,
                            at::Tensor& weight,
                            at::Tensor& bias,
                            bool add_bias,
                            bool do_flash_attn,
                            int num_heads,
                            bool transposed_mode)
@@ -1203,39 +1295,14 @@
         at::from_blob(key_pad_ptr,
                       {query.size(0), heads, key_value_length, padded_head_size},
                       query.options()),
         at::from_blob(value_pad_ptr,
                       {query.size(0), heads, key_value_length, padded_head_size},
                       query.options())};
 }
-template <typename T>
-at::Tensor ds_linear_layer_int8(at::Tensor& input,
-                                at::Tensor& weight,
-                                at::Tensor& bias,
-                                at::Tensor& q_scale,
-                                int groups)
-{
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-    int bsz = input_cont.size(0) * input_cont.size(1);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    quantized_gemm<T>(output, input_cont, weight, q_scale, groups, 0);
-    launch_bias_add((T*)output.data_ptr(),
-                    (T*)bias.data_ptr(),
-                    weight.size(1),
-                    bsz,
-                    InferenceContext::Instance().GetCurrentStream());
-    return output;
-}
 
 template <typename T>
 at::Tensor ds_vector_matmul(at::Tensor& input,
                             at::Tensor& weight,
                             bool async_op,
                             at::Tensor& q_scale,
                             bool q_int8,
@@ -1465,60 +1532,166 @@
                                          act_func_type,
                                          transposed_mode);
 
     return {output, res_add};
 }
 
 template <typename T>
-std::vector<at::Tensor> ds_mlp_gemm_int8(at::Tensor& input,
-                                         at::Tensor& residual,
-                                         at::Tensor& input_bias,
-                                         at::Tensor& weight,
-                                         at::Tensor& bias,
-                                         at::Tensor& gamma,
-                                         at::Tensor& beta,
-                                         const float epsilon,
-                                         at::Tensor& q_scale,
-                                         int groups,
-                                         bool preLayerNorm)
-{
-    auto input_cont = input.contiguous();
+std::vector<at::Tensor> ds_rms_mlp_gemm(at::Tensor& input,
+                                        at::Tensor& residual,
+                                        at::Tensor& weight_interm,
+                                        at::Tensor& weight_out,
+                                        at::Tensor& gamma,
+                                        const float epsilon,
+                                        at::Tensor& q_scale,
+                                        at::Tensor& q_scale1,
+                                        bool q_int8,
+                                        int activation_type,
+                                        bool transposed_mode)
+{
+    const int bsz = input.size(0) * input.size(1);
+    const size_t input_neurons = input.size(2);
+    const size_t mlp_1_out_neurons = transposed_mode ? weight_interm.size(0)
+                                                     : weight_interm.size(1);
+    const size_t mlp_2_in_neurons = transposed_mode ? weight_out.size(1) : weight_out.size(0);
+
     auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
+                       .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
+    T* output_ptr = (T*)InferenceContext::Instance().GetWorkSpace() + torch::numel(input);
+    T* inp_norm_ptr = output_ptr + torch::numel(input);
+    T* intermediate_ptr = inp_norm_ptr + torch::numel(input);
+
+    auto output = at::from_blob(output_ptr, input.sizes(), options);
+    auto inp_norm = at::from_blob(inp_norm_ptr, input.sizes(), options);
+    auto intermediate_gemm =
+        at::from_blob(intermediate_ptr, {input.size(0), input.size(1), mlp_1_out_neurons}, options);
 
-    int bsz = input_cont.size(0) * input_cont.size(1);
-    auto inp_norm = at::empty_like(input_cont);
+    auto act_func_type = static_cast<ActivationFuncType>(activation_type);
 
-    auto residual_add = (preLayerNorm ? at::empty_like(input_cont) : inp_norm);
-    quantized_gemm<T>(output, inp_norm, weight, q_scale, groups, 0);
-    launch_bias_gelu((T*)output.data_ptr(),
-                     (T*)bias.data_ptr(),
-                     weight.size(1),
-                     bsz,
-                     InferenceContext::Instance().GetCurrentStream());
+    // RMS Norm, we'll update the residual in-place
+    launch_rms_norm((T*)inp_norm.data_ptr(),
+                    (T*)residual.data_ptr(),
+                    (const T*)input.data_ptr(),
+                    (const T*)residual.data_ptr(),
+                    (const T*)gamma.data_ptr(),
+                    epsilon,
+                    bsz,
+                    input_neurons,
+                    InferenceContext::Instance().GetCurrentStream());
+
+    if (q_int8) {
+        quantized_gemm<T>(intermediate_ptr,
+                          (T*)inp_norm.data_ptr(),
+                          weight_interm,
+                          q_scale,
+                          q_scale.size(0),
+                          bsz,
+                          input_neurons);
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       mlp_1_out_neurons,
+                       bsz,
+                       input_neurons,
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight_interm.data_ptr(),
+                       (T*)inp_norm.data_ptr(),
+                       intermediate_ptr,
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard);
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP);
+#endif
+    }
+
+    if (act_func_type == ActivationFuncType::GELU) {
+        launch_bias_gelu(intermediate_ptr,
+                         (T*)nullptr,
+                         mlp_1_out_neurons,
+                         bsz,
+                         InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::ReLU) {
+        launch_bias_relu(intermediate_ptr,
+                         (T*)nullptr,
+                         mlp_1_out_neurons,
+                         bsz,
+                         InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::GATED_GELU) {
+        launch_gated_activation(intermediate_ptr,
+                                (const T*)intermediate_ptr,
+                                (const T*)nullptr,
+                                bsz,
+                                mlp_1_out_neurons,
+                                mlp_1_out_neurons,
+                                true,
+                                InferenceContext::Instance().GetCurrentStream());
+    } else if (act_func_type == ActivationFuncType::GATED_SILU) {
+        launch_gated_activation(intermediate_ptr,
+                                (const T*)intermediate_ptr,
+                                (const T*)nullptr,
+                                bsz,
+                                mlp_1_out_neurons,
+                                mlp_1_out_neurons,
+                                false,
+                                InferenceContext::Instance().GetCurrentStream());
+    }
 
-    return {output, residual_add};
+    if (q_int8) {
+        quantized_gemm<T>(output.data_ptr(),
+                          intermediate_ptr,
+                          weight_out,
+                          q_scale1,
+                          q_scale1.size(0),
+                          bsz,
+                          input.size(2));
+    } else {
+        float alpha = (T)1.0;
+        float gemm_beta = (T)0.0;
+        cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
+                        InferenceContext::Instance().GetCurrentStream());
+        cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
+                       (transposed_mode ? CUBLAS_OP_T : CUBLAS_OP_N),
+                       CUBLAS_OP_N,
+                       input_neurons,
+                       bsz,
+                       mlp_2_in_neurons,
+                       &alpha,
+                       &gemm_beta,
+                       (T*)weight_out.data_ptr(),
+                       intermediate_ptr,
+                       (T*)output.data_ptr(),
+#ifdef __HIP_PLATFORM_HCC__
+                       rocblas_gemm_algo_standard,
+#else
+                       CUBLAS_GEMM_DEFAULT_TENSOR_OP,
+#endif
+                       mlp_1_out_neurons);
+    }
+
+    return {output, residual};
 }
 
 template <typename T>
 at::Tensor fused_gemm_gelu(at::Tensor& input,
                            at::Tensor& weight,
                            at::Tensor& weight_scale,
                            at::Tensor& bias,
                            at::Tensor& weight_out,
                            at::Tensor& weight_out_scale,
-                           const float epsilon,
-                           bool preLayerNorm,
                            bool q_int8,
-                           bool async_op,
                            bool transposed_mode)
 {
     auto options = at::TensorOptions()
                        .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
@@ -1637,21 +1810,43 @@
             hidden_size,
             bsz,
             mp_size,
             InferenceContext::Instance().GetCurrentStream());
     return residual;
 }
 
+#define DISPATCH_VECTOR_ADD(T_TYPE, C_TYPE)                                         \
+    if (a.scalar_type() == at::k##T_TYPE) {                                         \
+        launch_vector_add<C_TYPE>((C_TYPE*)(a.data_ptr()),                          \
+                                  (const C_TYPE*)(a.data_ptr()),                    \
+                                  (const C_TYPE*)(b.data_ptr()),                    \
+                                  gamma,                                            \
+                                  total_elems,                                      \
+                                  InferenceContext::Instance().GetCurrentStream()); \
+    }
+
+at::Tensor& _vector_add(at::Tensor& a, at::Tensor& b, float gamma)
+{
+    const int total_elems = a.numel();
+
+    DISPATCH_VECTOR_ADD(Float, float)
+    DISPATCH_VECTOR_ADD(Half, __half)
+#ifdef BF16_AVAILABLE
+    DISPATCH_VECTOR_ADD(BFloat16, __nv_bfloat16)
+#endif
+
+    return a;
+}
+
 std::vector<at::Tensor> apply_rotary_pos_emb(at::Tensor& mixed_query,
                                              at::Tensor& key_layer,
                                              unsigned rotary_dim,
                                              unsigned offset,
                                              unsigned num_heads,
-                                             bool rotate_half,
-                                             bool rotate_every_two)
+                                             bool rotate_half)
 {
     auto query_cont = mixed_query.contiguous();
     auto key_cont = key_layer.contiguous();
 
     unsigned bsz = mixed_query.size(0);
     unsigned head_size = mixed_query.size(2) / num_heads;
     unsigned seq_len = mixed_query.size(1);
@@ -1661,130 +1856,103 @@
                                            (float*)key_cont.data_ptr(),
                                            head_size,
                                            seq_len,
                                            rotary_dim,
                                            offset,
                                            num_heads,
                                            bsz,
-                                           rotate_half,
-                                           rotate_every_two,
                                            InferenceContext::Instance().GetCurrentStream(),
-                                           InferenceContext::Instance().GetMaxTokenLenght());
+                                           InferenceContext::Instance().GetMaxTokenLength());
     else
         launch_apply_rotary_pos_emb<__half>((__half*)query_cont.data_ptr(),
                                             (__half*)key_cont.data_ptr(),
                                             head_size,
                                             seq_len,
                                             rotary_dim,
                                             offset,
                                             num_heads,
                                             bsz,
-                                            rotate_half,
-                                            rotate_every_two,
                                             InferenceContext::Instance().GetCurrentStream(),
-                                            InferenceContext::Instance().GetMaxTokenLenght());
+                                            InferenceContext::Instance().GetMaxTokenLength());
     return {query_cont, key_cont};
 }
 
-template <typename T>
-at::Tensor fused_gemm_gelu_int8(at::Tensor& input,
-                                at::Tensor& weight,
-                                at::Tensor& bias,
-                                const float epsilon,
-                                at::Tensor& q_scale,
-                                int groups,
-                                bool preLayerNorm)
-{
-    auto input_cont = input.contiguous();
-    auto options = at::TensorOptions()
-                       .dtype(input_cont.options().dtype())
-                       .layout(at::kStrided)
-                       .device(at::kCUDA)
-                       .requires_grad(false);
-
-    auto output = at::empty({input_cont.size(0), input_cont.size(1), weight.size(1)}, options);
-
-    int bsz = input_cont.size(0) * input_cont.size(1);
-
-    quantized_gemm<T>(output, input_cont, weight, q_scale, groups, 0);
-    launch_bias_gelu((T*)output.data_ptr(),
-                     (T*)bias.data_ptr(),
-                     weight.size(1),
-                     bsz,
-                     InferenceContext::Instance().GetCurrentStream());
-
-    return output;
-}
+#define DISPATCH_MOE_RESIDUAL(T_TYPE, C_TYPE)                                           \
+    if (moe_res.scalar_type() == torch::T_TYPE) {                                       \
+        launch_moe_res_matmul<C_TYPE>((C_TYPE*)moe_res.data_ptr(),                      \
+                                      (C_TYPE*)coef.data_ptr(),                         \
+                                      (C_TYPE*)output.data_ptr(),                       \
+                                      M,                                                \
+                                      N,                                                \
+                                      InferenceContext::Instance().GetCurrentStream()); \
+    }
 
 at::Tensor moe_res_matmul(at::Tensor& moe_res, at::Tensor& coef, at::Tensor& output)
 {
     int M = moe_res.size(0) * moe_res.size(1);
     int N = moe_res.size(2);
     InferenceContext::Instance().SynchComm();
-    if (moe_res.scalar_type() == at::kFloat) {
-        launch_moe_res_matmul<float>((float*)moe_res.data_ptr(),
-                                     (float*)coef.data_ptr(),
-                                     (float*)output.data_ptr(),
-                                     M,
-                                     N,
-                                     at::cuda::getCurrentCUDAStream());
-    } else {
-        launch_moe_res_matmul<__half>((__half*)moe_res.data_ptr(),
-                                      (__half*)coef.data_ptr(),
-                                      (__half*)output.data_ptr(),
-                                      M,
-                                      N,
-                                      at::cuda::getCurrentCUDAStream());
-    }
+
+    DISPATCH_MOE_RESIDUAL(kFloat, float)
+    DISPATCH_MOE_RESIDUAL(kHalf, __half)
+#ifdef BF16_AVAILABLE
+    DISPATCH_MOE_RESIDUAL(kBFloat16, __nv_bfloat16)
+#endif
+
     return output;
 }
 
 void ds_release_workspace() { InferenceContext::Instance().release_workspace(); }
 
 bool ds_retake_workspace() { return InferenceContext::Instance().retake_workspace(); }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
     m.def("softmax_context_int8",
           &ds_softmax_context1<__half>,
           "DeepSpeed attention with int8 (CUDA)");
-    m.def("bias_geglu", &ds_bias_geglu, "DeepSpeed Bias GEGLU (CUDA)");
+
+    // The following functions handle type dispatching internally
+    m.def("gated_activation", &ds_gated_activation, "DeepSpeed Bias GEGLU (CUDA)");
     m.def("layer_norm", &ds_layer_norm, "DeepSpeed layer norm (CUDA)");
     m.def(
         "_layer_norm_residual", &ds_layer_norm_residual, "DeepSpeed layer norm + residual (CUDA)");
     m.def("layer_norm_residual_store_pre_ln_res",
           &ds_layer_norm_residual_store_pre_ln_res,
           "DeepSpeed layer norm + store pre Layernorm residual (CUDA)");
-    m.def("qkv_gemm_int8", &ds_qkv_gemm_int8<__half>, "DeepSpeed qkv gemm with int8 (CUDA)");
-    m.def("mlp_gemm_int8", &ds_mlp_gemm_int8<__half>, "DeepSpeed mlp with int8 (CUDA)");
-    m.def("vector_matmul_int8",
-          &ds_vector_matmul_int8<__half>,
-          "DeepSpeed vector-MM with int8 (CUDA)");
-    m.def("linear_layer_int8",
-          &ds_linear_layer_int8<__half>,
-          "DeepSpeed linear_layer with int8 (CUDA)");
+    m.def("rms_norm", &ds_rms_norm, "DeepSpeed rms norm (CUDA)");
+    m.def("pre_rms_norm", &ds_pre_rms_norm, "DeepSpeed pre rms norm (CUDA)");
+    m.def("_vector_add", &_vector_add, "DeepSpeed vector add (CUDA)");
     m.def("apply_rotary_pos_emb", &apply_rotary_pos_emb, "DeepSpeed mlp with fp16 (CUDA)");
     m.def("moe_res_matmul", &moe_res_matmul, "DeepSpeed moe residual matmul (CUDA)");
     m.def("reset_cache", &reset_cache, "Reset Cache for generation tasks");
     m.def("release_workspace", &ds_release_workspace, "DeepSpeed Release Workspace");
     m.def("retake_workspace", &ds_retake_workspace, "DeepSpeed Retake Workspace");
 
+    // The following functions are templated and need to be explicitly instantiated and bound
+    // to different python methods
 #define DEF_OPS(_name, _dtype)                                                                    \
     m.def("softmax_" #_name, &ds_softmax<_dtype>, "DeepSpeed SoftMax with " #_name " (CUDA)");    \
     m.def("softmax_context_" #_name,                                                              \
           &ds_softmax_context<_dtype>,                                                            \
-          "DeepSpeed attention with _name (CUDA)");                                               \
+          "DeepSpeed attention with " #_name " (CUDA)");                                          \
     m.def("bias_gelu_" #_name, &ds_bias_gelu<_dtype>, "DeepSpeed Gelu with " #_name " (CUDA)");   \
     m.def("bias_add_" #_name, &ds_bias_add<_dtype>, "DeepSpeed Bias Add with " #_name " (CUDA)"); \
     m.def("bias_relu_" #_name, &ds_bias_relu<_dtype>, "DeepSpeed ReLU with " #_name " (CUDA)");   \
     m.def("bias_residual_" #_name,                                                                \
           &ds_bias_residual<_dtype>,                                                              \
           "DeepSpeed residual-bias add with " #_name " (CUDA)");                                  \
     m.def("qkv_gemm_" #_name, &ds_qkv_gemm<_dtype>, "DeepSpeed qkv gemm with " #_name " (CUDA)"); \
+    m.def("rms_qkv_gemm_" #_name,                                                                 \
+          &ds_rms_qkv<_dtype>,                                                                    \
+          "DeepSpeed rms qkv gemm with " #_name " (CUDA)");                                       \
     m.def("mlp_gemm_" #_name, &ds_mlp_gemm<_dtype>, "DeepSpeed mlp with " #_name " (CUDA)");      \
+    m.def("rms_mlp_gemm_" #_name,                                                                 \
+          &ds_rms_mlp_gemm<_dtype>,                                                               \
+          "DeepSpeed rms mlp gemm with " #_name " (CUDA)");                                       \
     m.def("vector_matmul_" #_name,                                                                \
           &ds_vector_matmul<_dtype>,                                                              \
           "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
     m.def("linear_layer_" #_name,                                                                 \
           &ds_linear_layer<_dtype>,                                                               \
           "DeepSpeed linear_layer with " #_name " (CUDA)");                                       \
     m.def("fused_gemm_gelu_" #_name,                                                              \
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     constexpr int values_per_access = granularity / sizeof(T);
     const int offset = (blockIdx.x * blockDim.x + threadIdx.x) * values_per_access;
 
     if (offset < total_count) {
         T data[values_per_access];
         T data_bias[values_per_access];
         mem_access::load_global<granularity>(data, input + offset);
-        mem_access::load_global<granularity>(data_bias, bias + (offset % intermediate_size));
+        mem_access::load_global<granularity>(
+            data_bias, bias + (offset % intermediate_size), bias != nullptr);
 
 #pragma unroll
         for (int i = 0; i < values_per_access; i++) {
             float data_f = conversion::to<float>(data[i]);
             float bias_f = conversion::to<float>(data_bias[i]);
             data[i] = conversion::to<T>(relu(data_f + bias_f));
         }
@@ -56,16 +57,15 @@
     dim3 block_dims(threads);
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_relu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
-template void launch_bias_relu<float>(float*, const float*, int, int, cudaStream_t);
+#define INSTANTIATE_LAUNCH_BIAS_RELU(T) \
+    template void launch_bias_relu<T>(T*, const T*, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_BIAS_RELU(float)
 #ifdef BF16_AVAILABLE
-template void launch_bias_relu<__nv_bfloat16>(__nv_bfloat16*,
-                                              const __nv_bfloat16*,
-                                              int,
-                                              int,
-                                              cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_RELU(__nv_bfloat16)
 #endif
-template void launch_bias_relu<__half>(__half*, const __half*, int, int, cudaStream_t);
+INSTANTIATE_LAUNCH_BIAS_RELU(__half)
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu`

 * *Files 5% similar despite different names*

```diff
@@ -483,66 +483,37 @@
         } else if (iterations == 64) {
             LAUNCH_ATTN_SOFTMAX_V2(64);
         }
     } else
         throw std::runtime_error("Unsupport Seq_Length!");
 }
 
-template void launch_attn_softmax_v2(float* vals,
-                                     float* mask,
-                                     float* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+#define INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(T)                  \
+    template void launch_attn_softmax_v2(T* vals,              \
+                                         T* mask,              \
+                                         T* alibi,             \
+                                         float layer_scale,    \
+                                         bool triangular,      \
+                                         bool recompute,       \
+                                         bool local_attention, \
+                                         int window_size,      \
+                                         int batch_size,       \
+                                         int heads,            \
+                                         int num_seq,          \
+                                         int sequence_length,  \
+                                         int head_offset,      \
+                                         int mask_stride,      \
+                                         int mp_size,          \
+                                         cudaStream_t stream);
 
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(float);
 #ifdef BF16_AVAILABLE
-template void launch_attn_softmax_v2(__nv_bfloat16* vals,
-                                     __nv_bfloat16* mask,
-                                     __nv_bfloat16* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(__nv_bfloat16);
 #endif
-
-template void launch_attn_softmax_v2(__half* vals,
-                                     __half* mask,
-                                     __half* alibi,
-                                     float layer_scale,
-                                     bool triangular,
-                                     bool recompute,
-                                     bool local_attention,
-                                     int window_size,
-                                     int batch_size,
-                                     int heads,
-                                     int num_seq,
-                                     int sequence_length,
-                                     int head_offset,
-                                     int mask_stride,
-                                     int mp_size,
-                                     cudaStream_t stream);
+INSTANTIATE_LAUNCH_ATTN_SOFTMAX_V2(__half);
 
 #define DEF_ATTN_SOFTMAX_V2_HALF(_iter)                                           \
     template __global__ void attn_softmax_v2<__half, _iter>(__half * vals,        \
                                                             __half * mask,        \
                                                             __half * alibi,       \
                                                             float layer_scale,    \
                                                             bool triangular,      \
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu`

 * *Files 4% similar despite different names*

```diff
@@ -236,51 +236,37 @@
                                                                 rotary_dim >> 3,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
 
+#define INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(T)             \
+    template void launch_bias_add_transform_0213<T>(T*,           \
+                                                    T*,           \
+                                                    T*,           \
+                                                    const T*,     \
+                                                    const T*,     \
+                                                    int,          \
+                                                    int,          \
+                                                    unsigned,     \
+                                                    int,          \
+                                                    int,          \
+                                                    int,          \
+                                                    int,          \
+                                                    bool,         \
+                                                    bool,         \
+                                                    cudaStream_t, \
+                                                    int,          \
+                                                    int)
+
 #ifdef BF16_AVAILABLE
-template void launch_bias_add_transform_0213(__nv_bfloat16* output,
-                                             __nv_bfloat16* k_cache,
-                                             __nv_bfloat16* v_cache,
-                                             const __nv_bfloat16* vals,
-                                             const __nv_bfloat16* bias,
-                                             int batch_size,
-                                             int seq_length,
-                                             unsigned seq_offset,
-                                             int all_tokens,
-                                             int hidden_dim,
-                                             int heads,
-                                             int rotary_dim,
-                                             bool rotate_half,
-                                             bool rotate_every_two,
-                                             cudaStream_t stream,
-                                             int trans_count,
-                                             int max_out_tokens);
+INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(__nv_bfloat16);
 #endif
-
-template void launch_bias_add_transform_0213(__half* output,
-                                             __half* k_cache,
-                                             __half* v_cache,
-                                             const __half* vals,
-                                             const __half* bias,
-                                             int batch_size,
-                                             int seq_length,
-                                             unsigned seq_offset,
-                                             int all_tokens,
-                                             int hidden_dim,
-                                             int heads,
-                                             int rotary_dim,
-                                             bool rotate_half,
-                                             bool rotate_every_two,
-                                             cudaStream_t stream,
-                                             int trans_count,
-                                             int max_out_tokens);
+INSTANTIATE_LAUNCH_BIAS_ADD_TRANSFORM_0213(__half);
 
 // Bias add
 
 __global__ void pad_add_transform_0213(float* output,
                                        const float* vals,
                                        int hidden_dim,
                                        int seq_length,
@@ -364,36 +350,23 @@
     hidden_dim >>= 3;
     dim3 block_dim((padded_head_size >> 3), heads, 2);
     dim3 grid_dim(batch_size, padded_seq_len / 2);
     pad_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(
         output, vals, hidden_dim, seq_length, padded_seq_len, heads, padded_head_size >> 3);
 }
 
+#define INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(T) \
+    template void launch_pad_add_transform_0213<T>(         \
+        T*, const T*, int, int, int, int, int, int, cudaStream_t);
+
+INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(__half);
 #ifdef BF16_AVAILABLE
-template void launch_pad_add_transform_0213(__nv_bfloat16* output,
-                                            const __nv_bfloat16* vals,
-                                            int batch_size,
-                                            int hidden_dim,
-                                            int seq_length,
-                                            int padded_seq_len,
-                                            int heads,
-                                            int padded_head_size,
-                                            cudaStream_t stream);
+INSTANTIATE_LAUNCH_PAD_ADD_TRANSFORM_0213_SIMPLE(__nv_bfloat16);
 #endif
 
-template void launch_pad_add_transform_0213(__half* output,
-                                            const __half* vals,
-                                            int batch_size,
-                                            int hidden_dim,
-                                            int seq_length,
-                                            int padded_seq_len,
-                                            int heads,
-                                            int padded_head_size,
-                                            cudaStream_t stream);
-
 // Bias add
 template <typename T>
 __global__ void bias_add_transform_0213(T* output,
                                         const T* vals,
                                         const T* bias,
                                         int hidden_dim,
                                         int seq_length,
@@ -567,30 +540,14 @@
         int iter_offset =
             (iter_row % blockDim.y) * d2_out_stride + (iter_row / blockDim.y) * matrix_stride;
         output_vec[out_index + iter_offset] =
             in_data[iter_row * d2_stride + d3 + (d2 % 2) * (d1_stride * blockDim.z)];
     }
 }
 
-template __global__ void bias_add_transform_0213_v2(__half* output,
-                                                    const __half* vals,
-                                                    const __half* bias,
-                                                    int hidden_dim,
-                                                    int seq_length,
-                                                    int heads);
-
-#ifdef BF16_AVAILABLE
-template __global__ void bias_add_transform_0213_v2(__nv_bfloat16* output,
-                                                    const __nv_bfloat16* vals,
-                                                    const __nv_bfloat16* bias,
-                                                    int hidden_dim,
-                                                    int seq_length,
-                                                    int heads);
-#endif
-
 template <typename T>
 __global__ void transform4d_0213(T* out,
                                  const T* in,
                                  int heads,
                                  int seq_length,
                                  int hidden_dim,
                                  int head_ext);
@@ -703,28 +660,14 @@
 #pragma unroll
     for (int iter = 0; iter < 2; iter++) {
         int iter_id = iter * iteration_stride + iter_index;
         out_vec[output_offset + iter_id] = in_data[iter_id];
     }
 }
 
-#ifdef BF16_AVAILABLE
-template __global__ void transform4d_0213_v2(__nv_bfloat16* out,
-                                             const __nv_bfloat16* in,
-                                             int heads,
-                                             int seq_length,
-                                             int hidden_dim);
-#endif
-
-template __global__ void transform4d_0213_v2(__half* out,
-                                             const __half* in,
-                                             int heads,
-                                             int seq_length,
-                                             int hidden_dim);
-
 // 3 * [B A S N] - > [B S C*H]
 template <>
 void launch_transform4d_0213<float>(float* out,
                                     const float* in,
                                     int batch_size,
                                     int heads,
                                     int seq_length,
@@ -753,26 +696,14 @@
     int head_ext = (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 grid_dims(batch_size, trans_count, (seq_length * head_ext));
     dim3 block_dims(hidden_dim / heads, (heads / head_ext));
     transform4d_0213<<<grid_dims, block_dims, 0, stream>>>(
         out, in, heads, seq_length, hidden_dim, head_ext);
 }
 
+#define INSTANTIATE_2B_LAUNCH_TRANSFORM4D(T) \
+    template void launch_transform4d_0213<T>(T*, const T*, int, int, int, int, cudaStream_t, int);
+
+INSTANTIATE_2B_LAUNCH_TRANSFORM4D(__half)
 #ifdef BF16_AVAILABLE
-template void launch_transform4d_0213(__nv_bfloat16* out,
-                                      const __nv_bfloat16* in,
-                                      int batch_size,
-                                      int heads,
-                                      int seq_length,
-                                      int hidden_dim,
-                                      cudaStream_t stream,
-                                      int trans_count);
+INSTANTIATE_2B_LAUNCH_TRANSFORM4D(__nv_bfloat16)
 #endif
-
-template void launch_transform4d_0213(__half* out,
-                                      const __half* in,
-                                      int batch_size,
-                                      int heads,
-                                      int seq_length,
-                                      int hidden_dim,
-                                      cudaStream_t stream,
-                                      int trans_count);
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         size_t workSpaceSize = ((external_cache ? (activation_size + temp_size)
                                                 : (activation_size + temp_size + cache_size))) *
                                _max_seq_len * elem_size;
         temp_size *= _max_seq_len * elem_size;
 
         if (_max_seq_len < min_out_tokens) {
             printf(
-                "Allocatable workspace available (%d tokens) is less than minimum requested "
+                "Allocatable workspace available (%ld tokens) is less than minimum requested "
                 "workspace (%d tokens)\n",
                 _max_seq_len,
                 min_out_tokens);
             throw std::runtime_error("Workspace can't be allocated, not enough memory");
         }
 
         if (!_workspace) {
@@ -171,15 +171,15 @@
                    _free_memory_size,
                    total_size);
             throw std::runtime_error("Workspace is null.");
         }
         _workSpaceSize = workSpaceSize;
         _attention_unfused_workspace_offset = workSpaceSize - temp_size;
     }
-    inline size_t GetMaxTokenLenght() const { return _max_seq_len; }
+    inline size_t GetMaxTokenLength() const { return _max_seq_len; }
 
     cudaEvent_t GetCompEvent(int id) { return id == 1 ? _comp1_event : _comp2_event; }
 
     size_t get_workspace_size() const { return _workSpaceSize; }
     void* GetWorkSpace() { return _workspace; }
     void* GetAttentionUnfusedWorkspace()
     {
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 // DeepSpeed Team
 
 #pragma once
 
 #include <assert.h>
 #include <cublas_v2.h>
 #include <cuda.h>
+#ifdef BF16_AVAILABLE
 #include <cuda_bf16.h>
+#endif
 #include <cuda_fp16.h>
 #include <cuda_runtime.h>
 #ifndef __HIP_PLATFORM_HCC__
 #include <mma.h>
 #endif
 #include <stdio.h>
 
@@ -24,44 +26,47 @@
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const float* A,
                    const float* B,
                    float* C,
-                   rocblas_gemm_algo algo)
+                   rocblas_gemm_algo algo,
+                   int b_stride = -1)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const float* A,
                    const float* B,
                    float* C,
-                   cublasGemmAlgo_t algo)
+                   cublasGemmAlgo_t algo,
+                   int b_stride = -1)
 #endif
 {
+    const int ldb = (b_stride == -1) ? ((transb == CUBLAS_OP_N) ? k : n) : b_stride;
 #ifdef __HIP_PLATFORM_HCC__
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
                                             n,
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
                                             rocblas_datatype_f32_r,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
                                             rocblas_datatype_f32_r,
-                                            (transb == rocblas_operation_none) ? k : n,
+                                            ldb,
                                             (const void*)beta,
                                             C,
                                             rocblas_datatype_f32_r,
                                             m,
                                             C,
                                             rocblas_datatype_f32_r,
                                             m,
@@ -78,15 +83,15 @@
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
                                          CUDA_R_32F,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
                                          CUDA_R_32F,
-                                         (transb == CUBLAS_OP_N) ? k : n,
+                                         ldb,
                                          (const void*)beta,
                                          C,
                                          CUDA_R_32F,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
@@ -116,30 +121,33 @@
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const T* A,
                    const T* B,
                    T* C,
-                   rocblas_gemm_algo algo)
+                   rocblas_gemm_algo algo,
+                   int b_stride = -1)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
                    const T* A,
                    const T* B,
                    T* C,
-                   cublasGemmAlgo_t algo)
+                   cublasGemmAlgo_t algo,
+                   int b_stride = -1)
 #endif
 {
+    const int ldb = (b_stride == -1) ? ((transb == CUBLAS_OP_N) ? k : n) : b_stride;
 #ifdef __HIP_PLATFORM_HCC__
     constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
                                                                      : rocblas_datatype_bf16_r;
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
@@ -147,15 +155,15 @@
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
                                             rocblas_dtype_16,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
                                             rocblas_dtype_16,
-                                            (transb == rocblas_operation_none) ? k : n,
+                                            ldb,
                                             (const void*)beta,
                                             (void*)C,
                                             rocblas_dtype_16,
                                             m,
                                             (void*)C,
                                             rocblas_dtype_16,
                                             m,
@@ -173,15 +181,15 @@
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
                                          cublas_dtype_16,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
                                          cublas_dtype_16,
-                                         (transb == CUBLAS_OP_N) ? k : n,
+                                         ldb,
                                          (const void*)beta,
                                          (void*)C,
                                          cublas_dtype_16,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,21 @@
 void launch_bias_gelu(T* input,
                       const T* bias,
                       int intermediate_size,
                       int batch_size,
                       cudaStream_t stream);
 
 template <typename T>
-void launch_fused_bias_geglu(T* output,
+void launch_gated_activation(T* output,
                              const T* activation,
                              const T* bias,
                              int rows,
+                             int output_stride,
                              int elems_per_row,
+                             bool use_gelu,
                              cudaStream_t stream);
 
 // Fused bias add with relu activation
 template <typename T>
 void launch_bias_relu(T* input,
                       const T* bias,
                       int intermediate_size,
@@ -114,14 +116,25 @@
                                                const T* beta,
                                                float epsilon,
                                                int rows,
                                                int elems_per_row,
                                                cudaStream_t stream);
 
 template <typename T>
+void launch_rms_norm(T* norm_output,
+                     T* res_output,
+                     const T* vals,
+                     const T* residual,
+                     const T* gamma,
+                     float epsilon,
+                     int rows,
+                     int elems_per_row,
+                     cudaStream_t stream);
+
+template <typename T>
 void launch_dequantize(T* output,
                        const int8_t* input,
                        const float* qscale,
                        unsigned output_size,
                        unsigned hidden_dim,
                        unsigned groups,
                        unsigned merge_count,
@@ -151,16 +164,14 @@
                                  T* key_layer,
                                  unsigned head_size,
                                  unsigned seq_len,
                                  unsigned rotary_dim,
                                  unsigned offset,
                                  unsigned num_heads,
                                  unsigned batch,
-                                 bool rotate_half,
-                                 bool rotate_every_two,
                                  cudaStream_t stream,
                                  int max_out_tokens);
 
 template <typename T>
 void launch_moe_res_matmul(T* residual,
                            T* coef,
                            T* mlp_out,
@@ -220,7 +231,15 @@
                                    int batch_size,
                                    int hidden_dim,
                                    int seq_length,
                                    int padded_seq_len,
                                    int heads,
                                    int padded_head_size,
                                    cudaStream_t stream);
+
+template <typename T>
+void launch_vector_add(T* out,
+                       const T* a,
+                       const T* b,
+                       float gamma,
+                       int num_elems,
+                       cudaStream_t stream);
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.3/deepspeed/ops/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/lamb/fused_lamb.py` & `deepspeed-0.9.3/deepspeed/ops/lamb/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/__init__.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/all_ops.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/async_io.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/builder.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 cuda_minor_mismatch_ok = {
     10: [
         "10.0",
         "10.1",
         "10.2",
     ],
     11: ["11.0", "11.1", "11.2", "11.3", "11.4", "11.5", "11.6", "11.7", "11.8"],
+    12: ["12.0", "12.1"],
 }
 
 
 def assert_no_cuda_mismatch(name=""):
     cuda_major, cuda_minor = installed_cuda_version(name)
     sys_cuda_version = f'{cuda_major}.{cuda_minor}'
     torch_cuda_version = ".".join(torch.version.cuda.split('.')[:2])
@@ -81,28 +82,36 @@
     if sys_cuda_version != torch_cuda_version:
         if (cuda_major in cuda_minor_mismatch_ok and sys_cuda_version in cuda_minor_mismatch_ok[cuda_major]
                 and torch_cuda_version in cuda_minor_mismatch_ok[cuda_major]):
             print(f"Installed CUDA version {sys_cuda_version} does not match the "
                   f"version torch was compiled with {torch.version.cuda} "
                   "but since the APIs are compatible, accepting this combination")
             return True
+        elif os.getenv("DS_SKIP_CUDA_CHECK", "0") == "1":
+            print(
+                f"{WARNING} DeepSpeed Op Builder: Installed CUDA version {sys_cuda_version} does not match the "
+                f"version torch was compiled with {torch.version.cuda}."
+                "Detected `DS_SKIP_CUDA_CHECK=1`: Allowing this combination of CUDA, but it may result in unexpected behavior."
+            )
+            return True
         raise Exception(f">- DeepSpeed Op Builder: Installed CUDA version {sys_cuda_version} does not match the "
                         f"version torch was compiled with {torch.version.cuda}, unable to compile "
                         "cuda/cpp extensions without a matching cuda version.")
     return True
 
 
 class OpBuilder(ABC):
     _rocm_version = None
     _is_rocm_pytorch = None
 
     def __init__(self, name):
         self.name = name
         self.jit_mode = False
         self.build_for_cpu = False
+        self.enable_bf16 = False
         self.error_log = None
 
     @abstractmethod
     def absolute_name(self):
         '''
         Returns absolute build path for cases where the op is pre-installed, e.g., deepspeed.ops.adam.cpu_adam
         will be installed as something like: deepspeed/ops/adam/cpu_adam.so
@@ -429,15 +438,15 @@
                             sources=self.strip_empty_entries(self.sources()),
                             include_dirs=self.strip_empty_entries(self.include_paths()),
                             extra_compile_args={'cxx': self.strip_empty_entries(self.cxx_args())},
                             extra_link_args=self.strip_empty_entries(self.extra_ldflags()))
 
     def load(self, verbose=True):
         from deepspeed.git_version_info import installed_ops, torch_info
-        if installed_ops[self.name]:
+        if installed_ops.get(self.name, False):
             # Ensure the op we're about to load was compiled with the same
             # torch/cuda versions we are currently using at runtime.
             self.validate_torch_version(torch_info)
             if torch.cuda.is_available() and isinstance(self, CUDAOpBuilder):
                 self.validate_torch_op_version(torch_info)
 
             return importlib.import_module(self.absolute_name())
@@ -473,19 +482,27 @@
         # needed at runtime. This prevents CC collisions such as multiple __half
         # implementations. Stash arch list to reset after build.
         torch_arch_list = None
         if "TORCH_CUDA_ARCH_LIST" in os.environ:
             torch_arch_list = os.environ.get("TORCH_CUDA_ARCH_LIST")
             os.environ["TORCH_CUDA_ARCH_LIST"] = ""
 
+        nvcc_args = self.strip_empty_entries(self.nvcc_args())
+        cxx_args = self.strip_empty_entries(self.cxx_args())
+
+        if isinstance(self, CUDAOpBuilder):
+            if not self.build_for_cpu and self.enable_bf16:
+                cxx_args.append("-DBF16_AVAILABLE")
+                nvcc_args.append("-DBF16_AVAILABLE")
+
         op_module = load(name=self.name,
                          sources=self.strip_empty_entries(sources),
                          extra_include_paths=self.strip_empty_entries(extra_include_paths),
-                         extra_cflags=self.strip_empty_entries(self.cxx_args()),
-                         extra_cuda_cflags=self.strip_empty_entries(self.nvcc_args()),
+                         extra_cflags=cxx_args,
+                         extra_cuda_cflags=nvcc_args,
                          extra_ldflags=self.strip_empty_entries(self.extra_ldflags()),
                          verbose=verbose)
 
         build_duration = time.time() - start_build
         if verbose:
             print(f"Time to load {self.name} op: {build_duration} seconds")
 
@@ -543,20 +560,24 @@
 
         ccs = self.filter_ccs(ccs)
         if len(ccs) == 0:
             raise RuntimeError(
                 f"Unable to load {self.name} op due to no compute capabilities remaining after filtering")
 
         args = []
+        self.enable_bf16 = True
         for cc in ccs:
             num = cc[0] + cc[2]
             args.append(f'-gencode=arch=compute_{num},code=sm_{num}')
             if cc.endswith('+PTX'):
                 args.append(f'-gencode=arch=compute_{num},code=compute_{num}')
 
+            if int(cc[0]) <= 7:
+                self.enable_bf16 = False
+
         return args
 
     def filter_ccs(self, ccs: List[str]):
         """
         Prune any compute capabilities that are not compatible with the builder. Should log
         which CCs have been pruned.
         """
@@ -590,14 +611,17 @@
         else:
             from torch.utils.cpp_extension import CUDAExtension as ExtensionBuilder
 
         compile_args = {'cxx': self.strip_empty_entries(self.cxx_args())} if self.build_for_cpu else \
                        {'cxx': self.strip_empty_entries(self.cxx_args()), \
                            'nvcc': self.strip_empty_entries(self.nvcc_args())}
 
+        if not self.build_for_cpu and self.enable_bf16:
+            compile_args['cxx'].append("-DBF16_AVAILABLE")
+
         cuda_ext = ExtensionBuilder(name=self.absolute_name(),
                                     sources=self.strip_empty_entries(self.sources()),
                                     include_dirs=self.strip_empty_entries(self.include_paths()),
                                     libraries=self.strip_empty_entries(self.libraries_args()),
                                     extra_compile_args=compile_args)
 
         if self.is_rocm_pytorch():
@@ -627,34 +651,34 @@
                 hipify_extra_files_only=True,
             )
 
     def cxx_args(self):
         if sys.platform == "win32":
             return ['-O2']
         else:
-            return ['-O3', '-std=c++14', '-g', '-Wno-reorder']
+            return ['-O3', '-std=c++17', '-g', '-Wno-reorder']
 
     def nvcc_args(self):
         if self.build_for_cpu:
             return []
         args = ['-O3']
         if self.is_rocm_pytorch():
             ROCM_MAJOR, ROCM_MINOR = self.installed_rocm_version()
             args += [
-                '-std=c++14', '-U__HIP_NO_HALF_OPERATORS__', '-U__HIP_NO_HALF_CONVERSIONS__',
+                '-std=c++17', '-U__HIP_NO_HALF_OPERATORS__', '-U__HIP_NO_HALF_CONVERSIONS__',
                 '-U__HIP_NO_HALF2_OPERATORS__',
                 '-DROCM_VERSION_MAJOR=%s' % ROCM_MAJOR,
                 '-DROCM_VERSION_MINOR=%s' % ROCM_MINOR
             ]
         else:
             cuda_major, _ = installed_cuda_version()
             args += [
                 '-allow-unsupported-compiler' if sys.platform == "win32" else '', '--use_fast_math',
-                '-std=c++17' if sys.platform == "win32" and cuda_major > 10 else '-std=c++14',
-                '-U__CUDA_NO_HALF_OPERATORS__', '-U__CUDA_NO_HALF_CONVERSIONS__', '-U__CUDA_NO_HALF2_OPERATORS__'
+                '-std=c++17' if cuda_major > 10 else '-std=c++14', '-U__CUDA_NO_HALF_OPERATORS__',
+                '-U__CUDA_NO_HALF_CONVERSIONS__', '-U__CUDA_NO_HALF2_OPERATORS__'
             ]
             if os.environ.get('DS_DEBUG_CUDA_BUILD', '0') == '1':
                 args.append('--ptxas-options=-v')
             args += self.compute_capability_args()
         return args
 
     def libraries_args(self):
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adagrad.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adam.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/fused_adam.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/fused_lamb.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/quantizer.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/random_ltd.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/sparse_attn.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/spatial_inference.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/stochastic_transformer.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/transformer.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/op_builder/transformer_inference.py` & `deepspeed-0.9.3/deepspeed/ops/op_builder/transformer_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,18 +52,20 @@
 
     def sources(self):
         return [
             'csrc/transformer/inference/csrc/pt_binding.cpp',
             'csrc/transformer/inference/csrc/gelu.cu',
             'csrc/transformer/inference/csrc/relu.cu',
             'csrc/transformer/inference/csrc/layer_norm.cu',
+            'csrc/transformer/inference/csrc/rms_norm.cu',
             'csrc/transformer/inference/csrc/softmax.cu',
             'csrc/transformer/inference/csrc/dequantize.cu',
             'csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu',
             'csrc/transformer/inference/csrc/transform.cu',
+            'csrc/transformer/inference/csrc/pointwise_ops.cu',
         ]
 
     def extra_ldflags(self):
         if not self.is_rocm_pytorch():
             return ['-lcurand']
         else:
             return []
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/quantizer/quantizer.py` & `deepspeed-0.9.3/deepspeed/ops/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/random_ltd/dropping_utils.py` & `deepspeed-0.9.3/deepspeed/ops/random_ltd/dropping_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     sampled_indices = sampled_indices.reshape(layers, batch_size, reserved_length).to(torch.int32)
     global random_ltd_module
     if random_ltd_module is None:
         random_ltd_module = RandomLTDBuilder().load()
     sampled_indices = random_ltd_module.token_sort_(sampled_indices, seq_length)
 
     # Not certain the optimized kernel is actually better here, cause it kind of screws
-    # with alignment right if the sequence length is not divisble by like 16
+    # with alignment right if the sequence length is not divisible by like 16
     # new_mask = random_ltd_module.mask_gather_gpt(attn_mask, reserved_length)
     if attn_mask is not None:
         new_mask = attn_mask[:, :, :reserved_length, :reserved_length]
     else:
         new_mask = None
 
     return sampled_indices, new_mask
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/matmul.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/softmax.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_attention_utils.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_attention_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_self_attention.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparsity_config.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparsity_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
              seq_len: required: an integer determining number of attention heads of the layer.
              different_layout_per_head: optional: this is just for the sake of consistency with other sparsity formats; can ignore it for DenseSparsityConfig
         """
 
         super().__init__(num_heads, block, different_layout_per_head)
 
     def make_layout(self, seq_len):
-        """Set 1 to all blocks of the layout meanins the pattern is dense; not sparse.
+        """Set 1 to all blocks of the layout meaning the pattern is dense; not sparse.
 
         Arguments:
              seq_len: required: an integer determining the underling sequence length; must be <= max sequence length
 
         Return:
              layout: a tensor of dimension (num_heads, num_blocks, num_blocks) containing sparsity layout of all head; for dense everything is 1
         """
@@ -698,15 +698,15 @@
         Return:
              layout: a tensor of dimension (num_heads, num_blocks, num_blocks) containing sparsity layout of all head in which local sliding window layout is set
         """
 
         num_blocks = layout.shape[1]
         if (num_blocks < self.num_sliding_window_blocks):
             raise ValueError(
-                f'Number of sliding window blocks, {self.num_sliding_window_blocks}, must be smaller than overal number of blocks in a row, {num_blocks}!'
+                f'Number of sliding window blocks, {self.num_sliding_window_blocks}, must be smaller than overall number of blocks in a row, {num_blocks}!'
             )
 
         w = self.num_sliding_window_blocks // 2
         for row in range(0, num_blocks):
             start = max(0, row - w)
             end = min(row + w + 1, num_blocks) if self.attention == "bidirectional" else row + 1
             layout[h, row, start:end] = 1
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/__init__.py` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/matmul.tr` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/matmul.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr` & `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/bias_add.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/bias_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/config.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 import json
-from deepspeed.utils.types import ActivationFuncType
+import torch
+from deepspeed.utils.types import ActivationFuncType, NormType
 
 
 class TransformerConfig():
 
     def __init__(self, hidden_size, intermediate_size, heads, num_hidden_layers):
         self.layer_id = -1
         self.hidden_size = hidden_size
@@ -28,14 +29,15 @@
             local_rank: Optional: The rank of GPU running the transformer kernel, it is not required
                 to use if the model already set the current device, otherwise need to set it
                 so that the transformer kernel can work on the right device
             mp_size (optional): This argument is mainly used to create the parameters on the kernel side
                 using model-parallel architecture. If the client model already takes care of this, there is no
                 need to pass this argument.
             fp16: Enable half-precision computation
+            bf16: Enable bf16 floating point computation
             pre_layer_norm: Select between Pre-LN or Post-LN transformer architecture
             stochastic_mode:  Enable for high performance, please note that this flag has some level of
                 non-determinism and can produce different results on different runs.  However, we have seen
                 that by enabling it, the pretraining tasks such as BERT are not affected and can obtain
                 a high accuracy level. On the other hand, for the downstream tasks, such as fine-tuning, we recommend
                 to turn it off in order to be able to reproduce the same result through the regular kernel execution.
 
@@ -48,17 +50,17 @@
                  hidden_size=-1,
                  intermediate_size=-1,
                  heads=-1,
                  num_hidden_layers=-1,
                  layer_norm_eps=1e-12,
                  local_rank=-1,
                  mp_size=1,
-                 fp16=False,
-                 q_int8=False,
+                 dtype=torch.float16,
                  pre_layer_norm=True,
+                 norm_type=NormType.LayerNorm,
                  stochastic_mode=False,
                  scale_attention=True,
                  triangular_masking=True,
                  local_attention=False,
                  window_size=256,
                  rotary_dim=-1,
                  rotate_half=False,
@@ -75,21 +77,21 @@
                  scale_attn_by_inverse_layer_idx=False,
                  return_single_tuple=False,
                  set_empty_params=False,
                  transposed_mode=False):
         super(DeepSpeedInferenceConfig,
               self).__init__(hidden_size, (intermediate_size if intermediate_size > 0 else 4 * hidden_size), heads,
                              num_hidden_layers)
-        self.fp16 = fp16
+        self.dtype = dtype
         self.pre_layer_norm = pre_layer_norm
+        self.norm_type = norm_type
         self.local_rank = local_rank
         self.stochastic_mode = stochastic_mode
         self.epsilon = layer_norm_eps
         self.mp_size = mp_size
-        self.q_int8 = q_int8
         self.scale_attention = scale_attention
         self.triangular_masking = triangular_masking
         self.local_attention = local_attention
         self.window_size = window_size
         self.rotary_dim = rotary_dim
         self.rotate_half = rotate_half
         self.rotate_every_two = rotate_every_two
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_attention.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_attention.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import torch.nn as nn
 from packaging import version as pkg_version
 from deepspeed.utils.logging import log_dist
 from deepspeed.accelerator import get_accelerator
 from deepspeed.ops.op_builder import InferenceBuilder
 
 # Cuda modules will be imported if needed
-inference_cuda_module = None
+inference_module = None
 minus_inf = -10000.0
 triton_flash_attn = None
 
 
 def load_triton_flash_attn():
     global triton_flash_attn
     try:
@@ -73,16 +73,15 @@
                     value = torch.matmul(context, attn_vw)
                 else:
                     qkv = torch.matmul(input, attn_qkvw)
                     query, key, value = qkv.chunk(3, dim=-1)
                     query = query.contiguous()
                     key = key.contiguous()
                     value = value.contiguous()
-                query, key, value = inference_cuda_module.pad_transform_fp16(query, key, value, config.heads,
-                                                                             do_flash_attn)
+                query, key, value = inference_module.pad_transform_fp16(query, key, value, config.heads, do_flash_attn)
                 attention_scores = (torch.matmul(query, key.transpose(-1, -2)) * scale).softmax(dim=-1)
                 context_layer = _transpose_for_context(torch.matmul(attention_scores, value))
 
             output = linear_func(context_layer, attn_ow, attn_ob, do_out_bias, False, config.heads, False)
             return output
 
         output = selfAttention_fp(input, context, input_mask)
@@ -112,20 +111,20 @@
 
         self.config = config
         self.config.layer_id = DeepSpeedDiffusersAttention.layer_id
         DeepSpeedDiffusersAttention.layer_id += 1
         device = get_accelerator().current_device_name() if config.bigscience_bloom else 'cpu'
         qkv_size_per_partition = (self.config.hidden_size // self.config.mp_size) * 3
 
-        data_type = torch.int8 if config.q_int8 else torch.half if config.fp16 else torch.float
-        data_type_fp = torch.half if config.fp16 else torch.float
-        global inference_cuda_module
-        if inference_cuda_module is None:
+        data_type = self.config.dtype
+        data_type_fp = torch.half if self.config.dtype == torch.int8 else self.config.dtype
+        global inference_module
+        if inference_module is None:
             builder = InferenceBuilder()
-            inference_cuda_module = builder.load()
+            inference_module = builder.load()
 
         if DeepSpeedDiffusersAttention.layer_id == 1:
             log_dist(f"DeepSpeed-Attention config: {self.config.__dict__}", [0])
 
         self.attn_qkvw = nn.Parameter(torch.empty(self.config.hidden_size,
                                                   qkv_size_per_partition,
                                                   dtype=data_type,
@@ -168,20 +167,22 @@
 
         self.norm_factor = math.sqrt(math.sqrt(self.config.hidden_size // self.config.heads))
 
         if self.config.scale_attn_by_inverse_layer_idx is True:
             self.norm_factor *= math.sqrt(self.config.layer_id + 1)
             # https://github.com/huggingface/transformers/blob/v4.24.0/src/transformers/models/gpt2/modeling_gpt2.py#L191
 
-        self.score_context_func = inference_cuda_module.softmax_context_fp32 if (not config.fp16) else \
-                                    inference_cuda_module.softmax_context_fp16
-        self.linear_func = inference_cuda_module.linear_layer_fp16 if config.fp16 else \
-                                    inference_cuda_module.linear_layer_fp32
-        self.allocate_workspace = inference_cuda_module.allocate_workspace_fp32 if not (config.fp16) else \
-                                    inference_cuda_module.allocate_workspace_fp16
+        if self.config.dtype in [torch.float16, torch.int8]:
+            self.score_context_func = inference_module.softmax_context_fp16
+            self.linear_func = inference_module.linear_layer_fp16
+            self.allocate_workspace = inference_module.allocate_workspace_fp16
+        else:
+            self.score_context_func = inference_module.softmax_context_fp32
+            self.linear_func = inference_module.linear_layer_fp32
+            self.allocate_workspace = inference_module.allocate_workspace_fp32
 
     def forward(self, input, context=None, input_mask=None):
         if self.config.layer_id == 0:
             self.allocate_workspace(self.config.hidden_size, self.config.heads,
                                     input.size()[1],
                                     input.size()[0], DeepSpeedDiffusersAttention.layer_id, self.config.mp_size, False,
                                     0, self.config.max_out_tokens, self.config.min_out_tokens)
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_transformer_block.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_transformer_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import torch.nn as nn
 
 from deepspeed import module_inject
 from .diffusers_attention import DeepSpeedDiffusersAttention
 from .bias_add import nhwc_bias_add
 from .diffusers_2d_transformer import Diffusers2DTransformerConfig
 from deepspeed.ops.op_builder import InferenceBuilder, SpatialInferenceBuilder
+from deepspeed.utils.types import ActivationFuncType
 
 # Ops will be loaded on demand
 transformer_cuda_module = None
 spatial_cuda_module = None
 
 
 def load_transformer_module():
@@ -93,11 +94,11 @@
         out_norm_2, out_attn_1 = self.transformer_cuda_module.layer_norm_residual_store_pre_ln_res(
             out_attn_1, self.attn_1_bias, hidden_states, self.norm2_g, self.norm2_b, self.norm2_eps)
         out_attn_2 = self.attn_2(out_norm_2, context=context)
         out_norm_3, out_attn_2 = self.transformer_cuda_module.layer_norm_residual_store_pre_ln_res(
             out_attn_2, self.attn_2_bias, out_attn_1, self.norm3_g, self.norm3_b, self.norm3_eps)
 
         out_ff1 = nn.functional.linear(out_norm_3, self.ff1_w)
-        out_geglu = self.transformer_cuda_module.bias_geglu(out_ff1, self.ff1_b)
+        out_geglu = self.transformer_cuda_module.gated_activation(out_ff1, self.ff1_b, ActivationFuncType.GATED_GELU)
 
         out_ff2 = nn.functional.linear(out_geglu, self.ff2_w)
         return nhwc_bias_add(out_ff2, self.ff2_b, other=out_attn_2)
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_attention.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 class DeepSpeedSelfAttention(nn.Module):
     num_layers = 0
     _qkv_buffers = []
 
     def __init__(self, config, mp_group=None, q_scales=None, q_groups=1, merge_count=1):
         super(DeepSpeedSelfAttention, self).__init__()
         self.config = config
-        data_type = torch.int8 if config.q_int8 else torch.half if config.fp16 else torch.float
-        data_type_fp = torch.half if config.fp16 else torch.float
+        data_type = self.config.dtype
+        data_type_fp = torch.half if self.config.dtype == torch.int8 else self.config.dtype
         self.config.layer_id = DeepSpeedSelfAttention.num_layers
         DeepSpeedSelfAttention.num_layers = DeepSpeedSelfAttention.num_layers + 1
         device = get_accelerator().current_device_name()  #if config.bigscience_bloom else 'cpu'
         if self.config.set_empty_params:
             self.attn_qw = None
             self.attn_qb = None
             self.attn_kw = None
@@ -84,15 +84,15 @@
                             self.config.hidden_size,
                             dtype=data_type_fp,
                             device=device),
                 torch.empty(self.hidden_size_per_partition * 3, dtype=data_type_fp, device=device)
             ]
 
     def compute_attention(self, qkv_out, input_mask, layer_past, alibi):
-        if isinstance(qkv_out, list):
+        if isinstance(qkv_out, list) or isinstance(qkv_out, tuple):
             qkv_out = qkv_out[0]
 
         no_masking = input_mask is None
 
         if no_masking:
             input_mask = torch.empty(1)
 
@@ -108,22 +108,22 @@
             alibi=alibi)
 
         context_layer, key_layer, value_layer = attn_key_value
         return context_layer, key_layer, value_layer
 
     def _merge_qkv(self):
         qvkw = DeepSpeedSelfAttention._qkv_buffers[0]
-        qvkw[:self.hidden_size_per_partition, :] = self.attn_qw
-        qvkw[self.hidden_size_per_partition:2 * self.hidden_size_per_partition, :] = self.attn_kw
-        qvkw[2 * self.hidden_size_per_partition:, :] = self.attn_vw
+        qvkw[:self.hidden_size_per_partition, :] = self.attn_qw  # type: ignore
+        qvkw[self.hidden_size_per_partition:2 * self.hidden_size_per_partition, :] = self.attn_kw  # type: ignore
+        qvkw[2 * self.hidden_size_per_partition:, :] = self.attn_vw  # type: ignore
         if self.attn_qb is not None:
             qvkb = DeepSpeedSelfAttention._qkv_buffers[1]
             qvkb[:self.hidden_size_per_partition] = self.attn_qb
-            qvkb[self.hidden_size_per_partition:2 * self.hidden_size_per_partition] = self.attn_kb
-            qvkb[2 * self.hidden_size_per_partition:] = self.attn_vb
+            qvkb[self.hidden_size_per_partition:2 * self.hidden_size_per_partition] = self.attn_kb  # type: ignore
+            qvkb[2 * self.hidden_size_per_partition:] = self.attn_vb  # type: ignore
         return DeepSpeedSelfAttention._qkv_buffers
 
     def forward(self,
                 input,
                 input_mask,
                 head_mask=None,
                 layer_past=None,
@@ -147,20 +147,18 @@
                                        add_bias=self.attn_qkvb is not None,
                                        do_flash_attn=False,
                                        num_heads=self.num_attention_heads_per_partition,
                                        num_layers=DeepSpeedSelfAttention.num_layers)
         else:
             qkv_out = self.qkv_func(input=input,
                                     weight=self._attn_qkvw,
-                                    bias=(self._attn_qkvb if self._attn_qkvb is not None else norm_b),
+                                    bias=self._attn_qkvb,
                                     gamma=norm_w,
-                                    beta=norm_b,
-                                    add_bias=(self.attn_qkvb is not None),
-                                    num_layers=DeepSpeedSelfAttention.num_layers,
-                                    num_heads=self.num_attention_heads_per_partition)
+                                    beta=norm_b)
+
         context_layer, key_layer, value_layer = self.compute_attention(qkv_out=qkv_out,
                                                                        input_mask=input_mask,
                                                                        layer_past=layer_past,
                                                                        alibi=alibi)
         output = self.vector_matmul_func(input=context_layer, weight=self.attn_ow)
         inp_norm = qkv_out[-1]
 
@@ -207,15 +205,15 @@
         # Note: torch.split does not create contiguous tensors by default.
         if contiguous_split_chunks:
             return tuple(chunk.contiguous() for chunk in tensor_list)
 
         return tensor_list
 
     def compute_attention(self, qkv_out, input_mask, layer_past, alibi):
-        if isinstance(qkv_out, list):
+        if isinstance(qkv_out, list) or isinstance(qkv_out, tuple):
             qkv_out = qkv_out[0]
 
         no_masking = input_mask is None
 
         if no_masking:
             input_mask = torch.empty(1)
 
@@ -244,16 +242,17 @@
         presents = (key_layer, value_layer)
         # Raw attention scores. [batch_size * num_heads, q_length, k_length]
         matmul_result = torch.matmul(query_layer, key_layer)
         # change view to [batch_size, num_heads, q_length, k_length]
         attention_scores = matmul_result.view(output_size[0], output_size[1], output_size[2], -1)
 
         offset = dist.get_rank() * self.num_attention_heads_per_partition if dist.is_initialized() else 0
+        target_dtype = torch.float16 if self.config.dtype == torch.int8 else self.config.dtype
         attention_probs = self.softmax_func(attn_scores=attention_scores,
-                                            attn_mask=((1 - input_mask).half() * minus_inf),
+                                            attn_mask=((1 - input_mask).to(target_dtype) * minus_inf),
                                             alibi=alibi,
                                             triangular=(self.config.triangular_masking
                                                         and (attention_scores.shape[-2] > 1)),
                                             recompute=False,
                                             local_attention=False,
                                             window_size=1,
                                             async_op=False,
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/moe_inference.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/moe_inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 # DeepSpeed Team
 
 import json
 import math
 import torch
 from torch.autograd import Function
-#from ...inference.engine import inference_cuda_module, specialized_mode
-# Cuda modules will be imported if needed
-inference_cuda_module = None
+# accelerator modules will be imported if needed
+inference_module = None
 specialized_mode = None
 import torch.nn as nn
 from .ds_attention import DeepSpeedSelfAttention
 from .config import DeepSpeedInferenceConfig
 from ....moe.sharded_moe import TopKGate
 from deepspeed import comm as dist
 from deepspeed.accelerator import get_accelerator
@@ -31,14 +30,15 @@
             local_rank: Optional: The rank of GPU running the transformer kernel, it is not required
                 to use if the model already set the current device, otherwise need to set it
                 so that the transformer kernel can work on the right device
             mp_size (optional): This argument is mainly used to create the parameters on the kernel side
                 using model-parallel architecture. If the client model already takes care of this, there is no
                 need to pass this argument.
             fp16: Enable half-precision computation
+            bf16: Enable bf16 floating point computation
             pre_layer_norm: Select between Pre-LN or Post-LN transformer architecture
             stochastic_mode:  Enable for high performance, please note that this flag has some level of
                 non-determinism and can produce different results on different runs.  However, we have seen
                 that by enabling it, the pretraining tasks such as BERT are not affected and can obtain
                 a high accuracy level. On the other hand, for the downstream tasks, such as fine-tuning, we recommend
                 to turn it off in order to be able to reproduce the same result through the regular kernel execution.
 
@@ -51,14 +51,15 @@
                  intermediate_size=-1,
                  heads=-1,
                  num_hidden_layers=-1,
                  layer_norm_eps=1e-12,
                  local_rank=-1,
                  mp_size=1,
                  fp16=False,
+                 bf16=False,
                  q_int8=False,
                  pre_layer_norm=True,
                  stochastic_mode=False,
                  scale_attention=True,
                  triangular_masking=True,
                  local_attention=False,
                  window_size=256,
@@ -72,17 +73,17 @@
                  noisy_gate_policy=None,
                  drop_tokens=True,
                  use_rts=False,
                  mlp_type='standard',
                  scale_attn_by_inverse_layer_idx=False):
         super(DeepSpeedMoEInferenceConfig,
               self).__init__(hidden_size, (intermediate_size if intermediate_size > 0 else 4 * hidden_size), heads,
-                             num_hidden_layers, layer_norm_eps, local_rank, mp_size, fp16, q_int8, pre_layer_norm,
-                             stochastic_mode, scale_attention, triangular_masking, local_attention, window_size,
-                             return_tuple)
+                             num_hidden_layers, layer_norm_eps, local_rank, mp_size, fp16, bf16, q_int8,
+                             pre_layer_norm, stochastic_mode, scale_attention, triangular_masking, local_attention,
+                             window_size, return_tuple)
         self.moe_experts = moe_experts
         self.k = k
         self.capacity_factor = capacity_factor
         self.eval_capacity_factor = eval_capacity_factor
         self.min_capacity = min_capacity
         self.noisy_gate_policy = noisy_gate_policy
         self.drop_tokens = drop_tokens
@@ -107,22 +108,20 @@
 
 class DeepSpeedMLPFunction(Function):
 
     @staticmethod
     def forward(ctx, input, inter_w, inter_b, config, output_b, output_w, q_scales, q_groups, merge_count, mp_group,
                 async_op):
         if config.q_int8:
-            intermediate = inference_cuda_module.fused_gemm_gelu_int8(input, inter_w, inter_b, config.epsilon,
-                                                                      q_scales[2], (q_groups * (2**merge_count)),
-                                                                      config.pre_layer_norm)
-            output = inference_cuda_module.vector_matmul_int8(intermediate, output_w, q_scales[3], q_groups,
-                                                              (merge_count))
+            intermediate = inference_module.fused_gemm_gelu_int8(input, inter_w, inter_b, config.epsilon, q_scales[2],
+                                                                 (q_groups * (2**merge_count)), config.pre_layer_norm)
+            output = inference_module.vector_matmul_int8(intermediate, output_w, q_scales[3], q_groups, (merge_count))
         else:
-            mlp_gemm_func = inference_cuda_module.fused_gemm_gelu_fp16 if config.fp16 else \
-                                    inference_cuda_module.fused_gemm_gelu_fp32
+            mlp_gemm_func = inference_module.fused_gemm_gelu_fp16 if config.fp16 else \
+                                    inference_module.fused_gemm_gelu_fp32
 
             output = mlp_gemm_func(input, inter_w, inter_b, output_w, config.epsilon, config.pre_layer_norm, async_op)
         if mp_group is not None and dist.get_world_size(group=mp_group) > 1:
             dist.all_reduce(output, group=mp_group, async_op=async_op)
 
         return output + output_b
 
@@ -184,43 +183,44 @@
                  quantize_groups=1,
                  merge_count=1,
                  mlp_extra_grouping=False):
         super(DeepSpeedMoEInference, self).__init__()
 
         self.config = config
         self.config.layer_id = DeepSpeedMoEInference.layer_id
-        global inference_cuda_module
+        global inference_module
         global specialized_mode
-        if inference_cuda_module is None:
+        if inference_module is None:
             specialized_mode = False
             # InferenceSpecializedBuilder is not among DeepSpeed provided builder yet, so we infer by builder name string
             builder = get_accelerator().create_op_builder("InferenceSpecializedBuilder")
             if builder != None and builder.is_compatible():
-                inference_cuda_module = builder.load()
+                inference_module = builder.load()
                 specialized_mode = True
             else:
-                inference_cuda_module = InferenceBuilder().load()
+                inference_module = InferenceBuilder().load()
         self.config.specialized_mode = specialized_mode
+        assert self.config.dtype != torch.bfloat16, "DeepSpeed MoE Transformer Inference not yet tested for bfloat support"
 
         DeepSpeedMoEInference.layer_id += 1
         self.attention = DeepSpeedSelfAttention(self.config, mp_group, quantize_scales, quantize_groups, merge_count)
         self.attn_nw = nn.Parameter(torch.Tensor(self.config.hidden_size))
         self.attn_nb = nn.Parameter(torch.Tensor(self.config.hidden_size))
 
         self.norm_w = nn.Parameter(torch.Tensor(self.config.hidden_size))
         self.norm_b = nn.Parameter(torch.Tensor(self.config.hidden_size))
 
         if config.mlp_type == 'residual':
             self.res_mlp = DeepSpeedMoEMLP(config, quantize_scales, quantize_groups, merge_count, mlp_extra_grouping,
                                            mp_group)
             self.res_coef = nn.Parameter(torch.Tensor(self.config.hidden_size, 2))
-            self.coef_func = inference_cuda_module.softmax_fp16 if self.config.fp16 or self.config.q_int8 else \
-                                        inference_cuda_module.softmax_fp32
-            self.vector_matmul_func = inference_cuda_module.vector_matmul_fp16 if config.fp16 else \
-                                    inference_cuda_module.vector_matmul_fp32
+            self.coef_func = inference_module.softmax_fp16 if self.config.dtype in [torch.float16, torch.int8] else \
+                                        inference_module.softmax_fp32
+            self.vector_matmul_func = inference_module.vector_matmul_fp16 if self.config.dtype == torch.float16 else \
+                                    inference_module.vector_matmul_fp32
 
         config.mp_size = 1
         self.mlp = nn.ModuleList(
             DeepSpeedMoEMLP(config, quantize_scales, quantize_groups, merge_count, mlp_extra_grouping, expert_mp_group)
             for i in range(self.config.moe_experts))
 
         self.moe_gate = TopKGate(self.config.hidden_size, self.config.global_experts, self.config.k,
@@ -230,20 +230,20 @@
 
         self.ep_group = ep_group
         self.mp_group = mp_group
         self.expert_mp_group = expert_mp_group
 
         print("DeepSpeed MoE Transformer Inference config is ", self.config.__dict__)
 
-        self.bias_residual_func = inference_cuda_module.bias_residual_fp16 if config.fp16 or config.q_int8 else \
-                                        inference_cuda_module.bias_residual_fp32
-        self.ds_layernorm = inference_cuda_module.layer_norm_fp16 if self.config.fp16 or self.config.q_int8 else \
-                                        inference_cuda_module.layer_norm_fp32
-        self.einsum_sec_sm_ecm = inference_cuda_module.einsum_sec_sm_ecm_fp16 if self.config.fp16 or self.config.q_int8 else \
-                                        inference_cuda_module.einsum_sec_sm_ecm_fp32
+        self.bias_residual_func = inference_module.bias_residual_fp16 if self.config.dtype in [torch.float16, torch.int8] else \
+                                        inference_module.bias_residual_fp32
+        self.ds_layernorm = inference_module.layer_norm_fp16 if self.config.dtype in [torch.float16, torch.int8] else \
+                                        inference_module.layer_norm_fp32
+        self.einsum_sec_sm_ecm = inference_module.einsum_sec_sm_ecm_fp16 if self.config.dtype in [torch.float16, torch.int8] else \
+                                        inference_module.einsum_sec_sm_ecm_fp32
 
     def res_coef_func(self, inp, async_op):
         inp = self.vector_matmul_func(inp, self.res_coef, async_op)
         return self.coef_func(inp, torch.empty(1), False, False, False, 256, async_op)
 
     def moe_gate_einsum(self, attention_output):
         _, combined_weights, dispatch_mask, _ = self.moe_gate(
@@ -298,16 +298,15 @@
                 encoder_attention_mask=None,
                 use_cache=False,
                 output_attentions=False):
         get_present = (get_present or get_key_value or use_cache)
         input_mask = input_mask if attention_mask is None else attention_mask
         input_type = input.dtype
 
-        if (self.config.fp16 or self.config.q_int8) \
-            and input.dtype == torch.float:
+        if (self.config.dtype in [torch.float16, torch.int8]) and input_type == torch.float:
             input = input.half()
 
         with torch.no_grad():
             attention_output = self.attention(input, input_mask, head_mask, layer_past, get_present,
                                               encoder_hidden_states, encoder_attention_mask, output_attentions,
                                               self.norm_w, self.norm_b)
 
@@ -343,15 +342,15 @@
             ################################################
 
             if self.expert_mp_group is not None:
                 output = output.split(output.shape[0] // dist.get_world_size(group=self.expert_mp_group),
                                       dim=0)[dist.get_rank(group=self.expert_mp_group)]
 
             if self.config.mlp_type == 'residual':
-                inference_cuda_module.moe_res_matmul(res_mlp_out, res_coef_out, output)
+                inference_module.moe_res_matmul(res_mlp_out, res_coef_out, output)
 
             output = self.bias_residual_func(output, residual_add, torch.empty(1))
 
             if not self.config.pre_layer_norm:
                 output = self.ds_layernorm(output, self.norm_w, self.norm_b, self.config.epsilon)
 
             if input_type != output.dtype:
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/base.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch
 from ..config import DeepSpeedInferenceConfig
 
 from deepspeed.ops.op_builder import InferenceBuilder
 
 
 class BaseOp(torch.nn.Module):
-    inference_cuda_module = None
+    inference_module = None
 
     def __init__(self, config: DeepSpeedInferenceConfig):
         super(BaseOp, self).__init__()
         self.config = config
-        if BaseOp.inference_cuda_module is None:
+        if BaseOp.inference_module is None:
             builder = InferenceBuilder()
-            BaseOp.inference_cuda_module = builder.load()
+            BaseOp.inference_module = builder.load()
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,33 @@
 from .base import BaseOp
 
 
 class GELUGemmOp(BaseOp):
 
     def __init__(self, config: DeepSpeedInferenceConfig):
         super(GELUGemmOp, self).__init__(config)
-        if self.config.fp16:
-            self.fused_gemm_gelu = self.inference_cuda_module.fused_gemm_gelu_fp16
-        else:
-            self.fused_gemm_gelu = self.inference_cuda_module.fused_gemm_gelu_fp32
-
-    def forward(self,
-                input: torch.Tensor,
-                weight: torch.Tensor,
-                bias: torch.Tensor,
-                weight_out: torch.Tensor,
-                async_op: bool = False):
-        output = self.fused_gemm_gelu(input, weight, weight.scale if hasattr(weight, 'scale') else torch.empty(1),
-                                      bias, weight_out,
-                                      weight_out.scale if hasattr(weight_out, 'scale') else torch.empty(1),
-                                      self.config.epsilon, self.config.pre_layer_norm, self.config.q_int8, async_op,
-                                      self.config.transposed_mode)
+        try:
+            if self.config.dtype in [torch.float16, torch.int8]:
+                self.fused_gemm_gelu = self.inference_module.fused_gemm_gelu_fp16  # type: ignore
+            elif self.config.dtype == torch.bfloat16:
+                self.fused_gemm_gelu = self.inference_module.fused_gemm_gelu_bf16
+            else:
+                self.fused_gemm_gelu = self.inference_module.fused_gemm_gelu_fp32  # type: ignore
+        except AttributeError:
+            self.fused_gemm_gelu = self.gelu_gemm_fallback
+
+    def gelu_gemm_fallback(self, input, weight, scale, bias, out, out_scale, dtype, transpose):
+        raise NotImplementedError
+
+    def forward(self, input: torch.Tensor, weight: torch.Tensor, bias: torch.Tensor, weight_out: torch.Tensor):
+
+        output = self.fused_gemm_gelu(
+            input,
+            weight,
+            weight.scale if hasattr(weight, 'scale') else torch.empty(1),  # type: ignore
+            bias,
+            weight_out,
+            weight_out.scale if hasattr(weight_out, 'scale') else torch.empty(1),  # type: ignore
+            self.config.dtype == torch.int8,
+            self.config.transposed_mode)
+
         return output
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/linear.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/linear.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,26 @@
 from .base import BaseOp
 
 
 class LinearOp(BaseOp):
 
     def __init__(self, config: DeepSpeedInferenceConfig):
         super(LinearOp, self).__init__(config)
-        if self.config.fp16:
-            self.linear_func = self.inference_cuda_module.linear_layer_fp16
-        else:
-            self.linear_func = self.inference_cuda_module.linear_layer_fp32
+        try:
+            if self.config.dtype in [torch.float16, torch.int8]:
+                self.linear_func = self.inference_module.linear_layer_fp16
+            elif self.config.dtype == torch.bfloat16:
+                self.linear_func = self.inference_module.linear_layer_bf16
+            else:
+                self.linear_func = self.inference_module.linear_layer_fp32
+        except AttributeError:
+            self.linear_func = self.linear_fallback
+
+    def linear_fallback(self, input, weight, bias, add_bias, do_flash_attn, num_heads, transpose):
+        raise NotImplementedError
 
     def forward(self,
                 input: torch.Tensor,
                 weight: torch.Tensor,
                 bias: torch.Tensor,
                 add_bias: bool,
                 do_flash_attn: bool,
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
+import os
 import torch
 from ..config import DeepSpeedInferenceConfig
 from .base import BaseOp
 
 
-class MLPGemmOp(BaseOp):
+class VectorMatMulOp(BaseOp):
 
     def __init__(self, config: DeepSpeedInferenceConfig):
-        super(MLPGemmOp, self).__init__(config)
-        if self.config.fp16:
-            self.mlp_gemm_func = self.inference_cuda_module.mlp_gemm_fp16
+        super(VectorMatMulOp, self).__init__(config)
+        try:
+            if self.config.dtype in [torch.float16, torch.int8]:
+                self.vector_matmul_func = self.inference_module.vector_matmul_fp16
+            elif self.config.dtype == torch.bfloat16:
+                self.vector_matmul_func = self.inference_module.vector_matmul_bf16
+            else:
+                self.vector_matmul_func = self.inference_module.vector_matmul_fp32
+        except AttributeError:
+            self.vector_matmul_func = self.vector_matmul_fallback
+
+    def vector_matmul_fallback(self, input, weight, async_op, q_scale, q_int8, transpose):
+        if os.environ.get('DS_KI_FALLBACK') == 'True' and not transpose:
+            return torch.matmul(input, weight)
         else:
-            self.mlp_gemm_func = self.inference_cuda_module.mlp_gemm_fp32
+            raise NotImplementedError
 
-    def forward(self, input: torch.Tensor, residual: torch.Tensor, input_bias: torch.Tensor,
-                weight_interm: torch.Tensor, weight_out: torch.Tensor, bias: torch.Tensor, gamma: torch.Tensor,
-                beta: torch.Tensor):
-        output, residual_add = self.mlp_gemm_func(
-            input, residual, input_bias, weight_interm, weight_out, bias, gamma, beta, self.config.epsilon,
-            self.config.pre_layer_norm, self.config.mlp_after_attn,
-            weight_interm.scale if hasattr(weight_interm, 'scale') else torch.empty(1),
-            weight_out.scale if hasattr(weight_out, 'scale') else torch.empty(1), self.config.q_int8,
-            self.config.mlp_act_func_type, self.config.transposed_mode)
-        return output, residual_add
+    def forward(self, input: torch.Tensor, weight: torch.Tensor, async_op: bool = False):
+        q_scale = weight.scale if hasattr(weight, 'scale') else torch.empty(1)
+        q_int8 = self.config.dtype == torch.int8
+        output = self.vector_matmul_func(input, weight, async_op, q_scale, q_int8, self.config.transposed_mode)
+        return output
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax_context.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,28 @@
 from .base import BaseOp
 
 
 class SoftmaxContextOp(BaseOp):
 
     def __init__(self, config: DeepSpeedInferenceConfig):
         super(SoftmaxContextOp, self).__init__(config)
-        if self.config.fp16:
-            self.softmax_context_func = self.inference_cuda_module.softmax_context_fp16
-        else:
-            self.softmax_context_func = self.inference_cuda_module.softmax_context_fp32
+        try:
+            if self.config.dtype in [torch.float16, torch.int8]:
+                self.softmax_context_func = self.inference_module.softmax_context_fp16
+            elif self.config.dtype == torch.bfloat16:
+                self.softmax_context_func = self.inference_module.softmax_context_bf16
+            else:
+                self.softmax_context_func = self.inference_module.softmax_context_fp32
+        except AttributeError:
+            self.softmax_context_func = self.softmax_context_fallback
+
+    def softmax_context_fallback(self, query_key_value, attn_mask, rotary_dim, rotate_half, roteate_every_two, heads,
+                                 norm_factor, triangular_masking, local_attention, window_size, no_masking, layer_id,
+                                 num_layers, alibi):
+        raise NotImplementedError
 
     def forward(self, query_key_value: torch.Tensor, attn_mask: torch.Tensor, heads: int, norm_factor: float,
                 no_masking: bool, layer_id: int, num_layers: int, alibi: torch.Tensor):
 
         if alibi is not None:
             batch_heads = query_key_value.shape[0] * heads
             offset = dist.get_rank() * batch_heads if dist.is_initialized() else 0
@@ -28,8 +38,9 @@
         else:
             alibi = torch.empty(1)
 
         output = self.softmax_context_func(query_key_value, attn_mask, self.config.rotary_dim, self.config.rotate_half,
                                            self.config.rotate_every_two, heads, norm_factor,
                                            self.config.triangular_masking, self.config.local_attention,
                                            self.config.window_size, no_masking, layer_id, num_layers, alibi)
+
         return output
```

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/inference/triton_ops.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/inference/triton_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/ops/transformer/transformer.py` & `deepspeed-0.9.3/deepspeed/ops/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/profiling/config.py` & `deepspeed-0.9.3/deepspeed/profiling/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 
 class DeepSpeedFlopsProfilerConfig(DeepSpeedConfigObject):
 
     def __init__(self, param_dict):
         super(DeepSpeedFlopsProfilerConfig, self).__init__()
 
         self.enabled = None
+        self.recompute_fwd_factor = None
         self.profile_step = None
         self.module_depth = None
         self.top_modules = None
 
         if FLOPS_PROFILER in param_dict.keys():
             flops_profiler_dict = param_dict[FLOPS_PROFILER]
         else:
             flops_profiler_dict = {}
 
         self._initialize(flops_profiler_dict)
 
     def _initialize(self, flops_profiler_dict):
         self.enabled = get_scalar_param(flops_profiler_dict, FLOPS_PROFILER_ENABLED, FLOPS_PROFILER_ENABLED_DEFAULT)
 
+        self.recompute_fwd_factor = get_scalar_param(flops_profiler_dict, FLOPS_PROFILER_RECOMPUTE_FWD_FACTOR,
+                                                     FLOPS_PROFILER_RECOMPUTE_FWD_FACTOR_DEFAULT)
+
         self.profile_step = get_scalar_param(flops_profiler_dict, FLOPS_PROFILER_PROFILE_STEP,
                                              FLOPS_PROFILER_PROFILE_STEP_DEFAULT)
 
         self.module_depth = get_scalar_param(flops_profiler_dict, FLOPS_PROFILER_MODULE_DEPTH,
                                              FLOPS_PROFILER_MODULE_DEPTH_DEFAULT)
 
         self.top_modules = get_scalar_param(flops_profiler_dict, FLOPS_PROFILER_TOP_MODULES,
```

### Comparing `deepspeed-0.9.2/deepspeed/profiling/constants.py` & `deepspeed-0.9.3/deepspeed/profiling/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 # Flops profiler. By default, this feature is not enabled.
 # Users can configure in ds_config.json as below example:
 FLOPS_PROFILER_FORMAT = '''
 flops profiler should be enabled as:
 "session_params": {
   "flops_profiler": {
     "enabled": true,
+    "recompute_fwd_factor": 0.0,
     "profile_step": 1,
     "module_depth": -1,
     "top_modules": 3,
     "detailed": true,
     "output_file": null
     }
 }
 '''
 
 FLOPS_PROFILER = "flops_profiler"
 
 FLOPS_PROFILER_ENABLED = "enabled"
 FLOPS_PROFILER_ENABLED_DEFAULT = False
 
+FLOPS_PROFILER_RECOMPUTE_FWD_FACTOR = "recompute_fwd_factor"
+FLOPS_PROFILER_RECOMPUTE_FWD_FACTOR_DEFAULT = 0.0
+
 FLOPS_PROFILER_PROFILE_STEP = "profile_step"
 FLOPS_PROFILER_PROFILE_STEP_DEFAULT = 1
 
 FLOPS_PROFILER_MODULE_DEPTH = "module_depth"
 FLOPS_PROFILER_MODULE_DEPTH_DEFAULT = -1
 
 FLOPS_PROFILER_TOP_MODULES = "top_modules"
```

### Comparing `deepspeed-0.9.2/deepspeed/profiling/flops_profiler/profiler.py` & `deepspeed-0.9.3/deepspeed/profiling/flops_profiler/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,18 @@
 
     To profile a trained model in inference, use the `get_model_profile` API.
 
     Args:
         object (torch.nn.Module): The PyTorch model to profile.
     """
 
-    def __init__(self, model, ds_engine=None):
+    def __init__(self, model, ds_engine=None, recompute_fwd_factor=0.0):
         self.model = model
         self.ds_engine = ds_engine
+        self.recompute_fwd_factor = recompute_fwd_factor
         self.started = False
         self.func_patched = False
 
     def start_profile(self, ignore_list=None):
         """Starts profiling.
 
         Extra attributes are added recursively to all the modules and the profiled torch.nn.functionals are monkey patched.
@@ -297,28 +298,30 @@
         if self.ds_engine and self.ds_engine.wall_clock_breakdown():
             fwd_latency = self.ds_engine.timers('forward').elapsed(False) / 1000.0
         print('{:<60}  {:<8}'.format('fwd latency: ', duration_to_string(fwd_latency)))
         print('{:<60}  {:<8}'.format('fwd FLOPS per GPU = fwd flops per GPU / fwd latency: ',
                                      flops_to_string(total_flops / fwd_latency)))
 
         if self.ds_engine and self.ds_engine.wall_clock_breakdown():
+            bwd_factor = 2 + self.recompute_fwd_factor
             bwd_latency = self.ds_engine.timers('backward').elapsed(False) / 1000.0
             step_latency = self.ds_engine.timers('step').elapsed(False) / 1000.0
             print('{:<60}  {:<8}'.format('bwd latency: ', duration_to_string(bwd_latency)))
-            print('{:<60}  {:<8}'.format('bwd FLOPS per GPU = 2 * fwd flops per GPU / bwd latency: ',
-                                         flops_to_string(2 * total_flops / bwd_latency)))
-            print('{:<60}  {:<8}'.format('fwd+bwd FLOPS per GPU = 3 * fwd flops per GPU / (fwd+bwd latency): ',
-                                         flops_to_string(3 * total_flops / (fwd_latency + bwd_latency))))
+            print('{:<60}  {:<8}'.format(f'bwd FLOPS per GPU = {bwd_factor} * fwd flops per GPU / bwd latency: ',
+                                         flops_to_string(bwd_factor * total_flops / bwd_latency)))
+            print('{:<60}  {:<8}'.format(
+                f'fwd+bwd FLOPS per GPU = {bwd_factor+1} * fwd flops per GPU / (fwd+bwd latency): ',
+                flops_to_string((bwd_factor + 1) * total_flops / (fwd_latency + bwd_latency))))
 
             print('{:<60}  {:<8}'.format('step latency: ', duration_to_string(step_latency)))
 
             iter_latency = fwd_latency + bwd_latency + step_latency
             print('{:<60}  {:<8}'.format('iter latency: ', duration_to_string(iter_latency)))
-            print('{:<60}  {:<8}'.format('FLOPS per GPU = 3 * fwd flops per GPU / iter latency: ',
-                                         flops_to_string(3 * total_flops / iter_latency)))
+            print('{:<60}  {:<8}'.format(f'FLOPS per GPU = {bwd_factor+1} * fwd flops per GPU / iter latency: ',
+                                         flops_to_string((bwd_factor + 1) * total_flops / iter_latency)))
 
             samples_per_iter = self.ds_engine.train_micro_batch_size_per_gpu() * self.ds_engine.world_size
             print('{:<60}  {:<8.2f}'.format('samples/second: ', samples_per_iter / iter_latency))
 
         def flops_repr(module):
             params = module.__params__
             flops = get_module_flops(module)
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/checkpointing.py` & `deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/checkpointing.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/config.py` & `deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/bf16_optimizer.py` & `deepspeed-0.9.3/deepspeed/runtime/bf16_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py` & `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     def save(self, state_dict, path: str):
         pass
 
     def load(self, path: str, map_location=None):
         pass
 
     def commit(self, tag):
-        # to tell checkpoint services if all files are readys.
+        # to tell checkpoint services if all files are ready.
         pass
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py` & `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             NEBULA_NUM_OF_VERSION_IN_RETENTION: config_params.num_of_version_in_retention,
         }
         torch_nebula.init(**nebula_config_params)
 
     def create(self, tag):
         log_dist(f"[Nebula] Start Checkpoint for tag:{tag}", ranks=[0])
         # -2 means: customer needs to  explicitly tell nebula
-        # current checkpoint is complete by commit methond.
+        # current checkpoint is complete by commit method.
         self.checkpoint = torch_nebula.Checkpoint(tag, -2)
 
     def save(self, state_dict, path: str):
         log_dist(f"[Nebula] Create dummy files for loading.")
         torch.save("", path)
 
         tag = _get_tag_from_path(path)
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py` & `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/comm/coalesced_collectives.py` & `deepspeed-0.9.3/deepspeed/runtime/comm/coalesced_collectives.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/comm/mpi.py` & `deepspeed-0.9.3/deepspeed/runtime/comm/mpi.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/comm/nccl.py` & `deepspeed-0.9.3/deepspeed/runtime/comm/nccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/compression/cupy.py` & `deepspeed-0.9.3/deepspeed/runtime/compression/cupy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/config.py` & `deepspeed-0.9.3/deepspeed/runtime/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import base64
 
 from .constants import *
 from .fp16.loss_scaler import (
     INITIAL_LOSS_SCALE,
     SCALE_WINDOW,
     DELAYED_SHIFT,
+    CONSECUTIVE_HYSTERESIS,
     MIN_LOSS_SCALE,
 )
 from .config_utils import (
     get_scalar_param,
     dict_raise_error_on_duplicate_keys,
     ScientificNotationEncoder,
 )
@@ -42,16 +43,16 @@
     ensure_immutable_elastic_config,
 )
 from ..elasticity.config import ElasticityConfigError
 from ..elasticity.constants import (
     ELASTICITY,
     IGNORE_NON_ELASTIC_BATCH_INFO,
     IGNORE_NON_ELASTIC_BATCH_INFO_DEFAULT,
-    MODEL_PARLLEL_SIZE,
-    MODEL_PARLLEL_SIZE_DEFAULT,
+    MODEL_PARALLEL_SIZE,
+    MODEL_PARALLEL_SIZE_DEFAULT,
     NUM_GPUS_PER_NODE,
     NUM_GPUS_PER_NODE_DEFAULT,
 )
 
 from ..profiling.config import DeepSpeedFlopsProfilerConfig
 from ..autotuning.config import DeepSpeedAutotuningConfig
 from ..nebula.config import DeepSpeedNebulaConfig
@@ -200,24 +201,28 @@
     if get_fp16_enabled(param_dict):
         fp16_dict = param_dict[FP16]
         dynamic_loss_args = [
             FP16_INITIAL_SCALE_POWER,
             FP16_LOSS_SCALE_WINDOW,
             FP16_MIN_LOSS_SCALE,
             FP16_HYSTERESIS,
+            FP16_CONSECUTIVE_HYSTERESIS,
         ]
         if any(arg in list(fp16_dict.keys()) for arg in dynamic_loss_args):
             init_scale = get_scalar_param(fp16_dict, FP16_INITIAL_SCALE_POWER, FP16_INITIAL_SCALE_POWER_DEFAULT)
             scale_window = get_scalar_param(fp16_dict, FP16_LOSS_SCALE_WINDOW, FP16_LOSS_SCALE_WINDOW_DEFAULT)
             delayed_shift = get_scalar_param(fp16_dict, FP16_HYSTERESIS, FP16_HYSTERESIS_DEFAULT)
+            consecutive_hysteresis = get_scalar_param(fp16_dict, FP16_CONSECUTIVE_HYSTERESIS,
+                                                      FP16_CONSECUTIVE_HYSTERESIS_DEFAULT)
             min_loss_scale = get_scalar_param(fp16_dict, FP16_MIN_LOSS_SCALE, FP16_MIN_LOSS_SCALE_DEFAULT)
             loss_scale_args = {
                 INITIAL_LOSS_SCALE: 2**init_scale,
                 SCALE_WINDOW: scale_window,
                 DELAYED_SHIFT: delayed_shift,
+                CONSECUTIVE_HYSTERESIS: consecutive_hysteresis,
                 MIN_LOSS_SCALE: min_loss_scale,
             }
 
     return loss_scale_args
 
 
 def get_gradient_accumulation_steps(param_dict):
@@ -708,15 +713,15 @@
             )
 
             elastic_dict = self._param_dict[ELASTICITY]
 
             # Ensure the resource scheduler saw the same elastic config we are using at runtime
             ensure_immutable_elastic_config(runtime_elastic_config_dict=elastic_dict)
 
-            self.elastic_model_parallel_size = elastic_dict.get(MODEL_PARLLEL_SIZE, MODEL_PARLLEL_SIZE_DEFAULT)
+            self.elastic_model_parallel_size = elastic_dict.get(MODEL_PARALLEL_SIZE, MODEL_PARALLEL_SIZE_DEFAULT)
             if self.elastic_model_parallel_size < 1:
                 raise ElasticityConfigError("Model-Parallel size cannot be less than 1, "
                                             f"given model-parallel size: {self.elastic_model_parallel_size}")
 
             self.num_gpus_per_node = elastic_dict.get(NUM_GPUS_PER_NODE, NUM_GPUS_PER_NODE_DEFAULT)
             if self.num_gpus_per_node < 1:
                 raise ElasticityConfigError("NUmber of GPUs per node cannot be less than 1, "
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/config_utils.py` & `deepspeed-0.9.3/deepspeed/runtime/config_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/constants.py` & `deepspeed-0.9.3/deepspeed/runtime/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 "fp16": {
   "enabled": true,
   "auto_cast": false,
   "loss_scale": 0,
   "initial_scale_power": 16,
   "loss_scale_window": 1000,
   "hysteresis": 2,
+  "consecutive_hysteresis": false,
   "min_loss_scale": 1
 }
 '''
 FP16 = "fp16"
 
 FP16_ENABLED = "enabled"
 FP16_ENABLED_DEFAULT = False
@@ -163,14 +164,18 @@
 FP16_LOSS_SCALE_WINDOW = "loss_scale_window"
 FP16_LOSS_SCALE_WINDOW_DEFAULT = 1000
 
 # FP16 hysteresis
 FP16_HYSTERESIS = "hysteresis"
 FP16_HYSTERESIS_DEFAULT = 2
 
+# FP16 consecutive hysteresis
+FP16_CONSECUTIVE_HYSTERESIS = "consecutive_hysteresis"
+FP16_CONSECUTIVE_HYSTERESIS_DEFAULT = False
+
 # FP16 min loss scale
 FP16_MIN_LOSS_SCALE = "min_loss_scale"
 FP16_MIN_LOSS_SCALE_DEFAULT = 1
 
 # FP16 master and grads
 FP16_MASTER_WEIGHTS_AND_GRADS = "fp16_master_weights_and_grads"
 FP16_MASTER_WEIGHTS_AND_GRADS_DEFAULT = False
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/config.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/constants.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/curriculum_scheduler.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/curriculum_scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/helper.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/scheduler.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/utils.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
                 index_to_sample_merged_builder = create_mmap_dataset_builder(index_to_sample_merged_fname,
                                                                              sample_idx_dtype)
                 for v_idx in range(len(index_to_sample)):
                     if v_idx > 0:
                         assert index_to_metric[v_idx] > index_to_metric[v_idx - 1]
                     num_sample_per_value[index_to_metric[v_idx][0]] = len(index_to_sample[v_idx])
                 assert sum(num_sample_per_value.values()) == total_num_samples
-                merge_step = len(index_to_sample) // 100
+                merge_step = max(1, len(index_to_sample) // 100)
                 for v_idx in range(0, len(index_to_sample), merge_step):
                     merged_samples = np.copy(
                         np.concatenate(index_to_sample[v_idx:min(len(index_to_sample), (v_idx + merge_step))],
                                        axis=None))
                     index_to_sample_merged_builder.add_item(
                         torch.tensor(merged_samples.astype(np.int64), dtype=torch.long))
                     logger.info(f"Finished merging index_to_sample {v_idx} to {v_idx+merge_step}.")
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/utils.py` & `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/dataloader.py` & `deepspeed-0.9.3/deepspeed/runtime/dataloader.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/eigenvalue.py` & `deepspeed-0.9.3/deepspeed/runtime/eigenvalue.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/engine.py` & `deepspeed-0.9.3/deepspeed/runtime/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,15 @@
         self._global_grad_norm = None
         self.use_ds_comm = False  # False --> Use torch.dist, True --> Use ds.comm backend.
 
         self.checkpoint_engine = None
 
         self._is_gradient_accumulation_boundary = None
         self.scale_wrt_gas = None
+        self.losses = []
 
         # for debug purposes - can then debug print: debug_get_module_name(module)
         debug_extract_module_and_param_names(model)
 
         # needed for zero_to_fp32 weights reconstruction to remap nameless data to state_dict
         self.param_names = {param: name for name, param in model.named_parameters()}
 
@@ -277,15 +278,15 @@
             steps_per_output=self.steps_per_print(),
             monitor_memory=False,
         )
 
         log_dist(f"DeepSpeed Flops Profiler Enabled: {self.flops_profiler_enabled()}", ranks=[0])
 
         if self.flops_profiler_enabled():
-            self.flops_profiler = FlopsProfiler(self.module, self)
+            self.flops_profiler = FlopsProfiler(self.module, self, self.flops_profiler_recompute_fwd_factor())
 
         if training_data:
             self.training_dataloader = self.deepspeed_io(training_data)
         else:
             self.training_dataloader = None
 
         # Configure optimizer and scheduler
@@ -310,14 +311,20 @@
             self._report_progress(0)
         elif self.zero_optimization():
             # no optim selected but zero is enabled
             self.optimizer = self._configure_zero_optimizer(optimizer=None)
         elif self.bfloat16_enabled():
             self.optimizer = self._configure_bf16_optimizer(optimizer=None)
 
+        # Hook optimizer for snip_momentum pruning
+        if hasattr(model, 'pruners'):
+            from ..compression.helper import rewrite_optimizer_step
+            self.optimizer.pruners = model.pruners
+            rewrite_optimizer_step(self.optimizer)
+
         # Bookkeeping for sparse support
         self.sparse_tensor_module_names = set()
         # if self.sparse_gradients_enabled():
         for name, module in self.module.named_modules():
             if isinstance(module, (torch.nn.Embedding, torch.nn.EmbeddingBag)) and self.sparse_gradients_enabled():
                 self.sparse_tensor_module_names.add(name + ".weight")
                 logger.info("Will convert {} to sparse tensor during training".format(name))
@@ -365,15 +372,15 @@
     def _get_model_parameters(self):
         if self.autotuning_profile_model_info():
             self.autotuning_model_info = {}
             num_params = 0
             trainable_num_params = 0
 
             for p in self.module.parameters():
-                # since user code might call deepspeed.zero.Init() before deepspeed.initialize(), need to check the attrbuite to check if the parameter is partitioned in zero 3 already or not
+                # since user code might call deepspeed.zero.Init() before deepspeed.initialize(), need to check the attribute to check if the parameter is partitioned in zero 3 already or not
                 n = 0
                 if hasattr(p, "ds_tensor"):  # if the parameter is partitioned in zero 3
                     n += p.ds_numel
                 else:  # if the parameter is not partitioned in zero 3 yet
                     n += p.numel()
                 num_params += n
                 if p.requires_grad:
@@ -559,14 +566,17 @@
 
     def wall_clock_breakdown(self):
         return self._config.wall_clock_breakdown
 
     def flops_profiler_enabled(self):
         return self._config.flops_profiler_config.enabled or self.autotuning_enabled()
 
+    def flops_profiler_recompute_fwd_factor(self):
+        return self._config.flops_profiler_config.recompute_fwd_factor
+
     def flops_profiler_profile_step(self):
         step = self._config.flops_profiler_config.profile_step
         if self._config.autotuning_config.enabled:
             step = self.autotuning_start_profile_step()
         return step
 
     def flops_profiler_module_depth(self):
@@ -1016,28 +1026,30 @@
         modules['module'] = model
         # register module attribute in engine but avoid getattr
         self.__dict__['module'] = model
 
     def _configure_distributed_model(self, model):
         self._set_client_model(model)
 
+        is_zero3_model = self.zero_optimization_partition_weights() and any(
+            [hasattr(param, "ds_id") for param in self.module.parameters()])
+
         if self.fp16_enabled():
-            if self.zero_optimization_partition_weights() and any(
-                [hasattr(param, "ds_id") for param in self.module.parameters()]):
+            if is_zero3_model:
                 self.__check_params(self.module, torch.half)
             self.module.half()
         elif self.bfloat16_enabled():
-            if self.zero_optimization_partition_weights() and any(
-                    hasattr(param, 'ds_id') for param in self.module.parameters()):
+            if is_zero3_model:
                 self.__check_params(self.module, torch.bfloat16)
             self.module.bfloat16()
         else:
             self.__check_params(self.module, torch.float)
 
-        if not self.dont_change_device:
+        # zero.Init() handles device placement of model
+        if not (self.dont_change_device or is_zero3_model):
             self.module.to(self.device)
 
         # MoE related initialization
         for _, module in self.module.named_modules():
             if isinstance(module, MoE):
                 self.has_moe_layers = True
                 self.num_experts.append(module.num_experts)
@@ -1065,30 +1077,30 @@
         # Query the groups module to get information about various parallel groups
         self.data_parallel_group = groups._get_data_parallel_group()
         self.dp_world_size = groups._get_data_parallel_world_size()
         self.mp_world_size = groups._get_model_parallel_world_size()
         self.expert_parallel_group = groups._get_expert_parallel_group_dict()
         self.expert_data_parallel_group = groups._get_expert_data_parallel_group_dict()
 
-        if not self.amp_enabled():
+        if not (self.amp_enabled() or is_zero3_model):
             self._broadcast_model()
 
     # check if parameters are duplicated in optimizer param_groups
     def _check_for_duplicates(self, optimizer):
         for name, param in self.module.named_parameters():
             param_id = id(param)
 
             def ids_list(group):
                 return [id(param) for param in group]
 
             occurrence = sum([
                 ids_list(group['params']).count(param_id) if param_id in ids_list(group['params']) else 0
                 for group in optimizer.param_groups
             ])
-            assert occurrence <= 1, f"Parameter with name: {name} occurs multiple times in optimizer.param_groups. Make sure it only appears once to prevent undefined behaviour."
+            assert occurrence <= 1, f"Parameter with name: {name} occurs multiple times in optimizer.param_groups. Make sure it only appears once to prevent undefined behavior."
 
     def _do_optimizer_sanity_check(self, basic_optimizer):
         model_dtype, grad_accum_dtype = self.get_data_types()
         zero_enabled = self.zero_optimization()
         amp_enabled = self.amp_enabled()
         # config based assertions
         assert (
@@ -1131,15 +1143,15 @@
                 )
             if model_dtype == torch.float16:
                 return FP16
             # else optimizer_wrapper = None
         elif model_dtype == torch.bfloat16 and grad_accum_dtype == torch.float32:
             return BFLOAT16
         else:
-            raise NotImplementedError("unsupported mix of model dtype and gradient accummulation type")
+            raise NotImplementedError("unsupported mix of model dtype and gradient accumulation type")
 
         return None
 
     # Configure optimizer
     def _configure_optimizer(self, client_optimizer, model_parameters):
         if client_optimizer is not None:
             if isinstance(client_optimizer, tuple(self._supported_optims())):
@@ -1824,19 +1836,24 @@
 
         # Log training Loss
         if self.monitor.enabled:
             if self.is_gradient_accumulation_boundary():
                 if self.global_rank == 0:
                     self.summary_events = [(
                         f"Train/Samples/train_loss",
-                        loss.mean().item() * self.gradient_accumulation_steps(),
+                        sum(self.losses) / self.gradient_accumulation_steps(),
                         self.global_samples,
                     )]
                     self.monitor.write_events(self.summary_events)
 
+        if self.is_gradient_accumulation_boundary():
+            self.losses = []
+        else:
+            self.losses.append(loss.mean().item())
+
         self._start_timers(self.engine_timers.backward_timers)
 
         assert self.optimizer is not None and not isinstance(self.optimizer, DummyOptim), \
             "must provide optimizer during init in order to use backward"
 
         self._start_timers(self.engine_timers.backward_inner_timers)
 
@@ -1898,15 +1915,15 @@
         else:
             return self._is_gradient_accumulation_boundary
 
     def set_gradient_accumulation_boundary(self, is_boundary):
         """
         Manually overrides the DeepSpeed engine's gradient accumulation boundary state, this is an optional
         feature and should be used with care. The state should be set before to the intended
-        value before each forward/backward. The final fordward/backward should have the
+        value before each forward/backward. The final forward/backward should have the
         boundary state set to True. This style allows client code to only call engine.step() once after all
         the gradient accumulation passes are complete. See example below:
         .. code-block:: python
         engine.set_gradient_accumulation_boundary(False)
         for _ in range(gradient_accumulation_steps - 1):
             micro_batch = next(data_loader)
             loss = engine(micro_batch)
@@ -1954,15 +1971,15 @@
                 self.quantizer.quantize(
                     tensor_to_quantize,
                     (self.optimizer.overflow if self.fp16_enabled() else False),
                     self.eigenvalue_enabled(),
                     block_eigenvalue,
                 )
         # zero grad in basic optimizer could be unreliable and may not exhibit
-        # the behaviour that we want
+        # the behavior that we want
         if self.bfloat16_enabled():
             # TODO: Temporary until bf16_optimizer and zero_optimizer are integrated
             if self.zero_optimization() and hasattr(self.optimizer, "zero_grad"):
                 self.optimizer.zero_grad()
             else:
                 pass
         elif self.zero_optimization() or self.fp16_enabled() or self.amp_enabled():
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/fused_optimizer.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/loss_scaler.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/loss_scaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import torch
 from deepspeed import comm as dist
 from deepspeed.utils import logger
 
 INITIAL_LOSS_SCALE = 'init_scale'
 SCALE_WINDOW = 'scale_window'
 DELAYED_SHIFT = 'delayed_shift'
+CONSECUTIVE_HYSTERESIS = 'consecutive_hysteresis'
 MIN_LOSS_SCALE = 'min_scale'
 
 
 # item() is a recent addition, so this helps with backward compatibility.
 def to_python_float(t):
     if hasattr(t, 'item'):
         return t.item()
@@ -107,14 +108,15 @@
     In this way :class:`DynamicLossScaler` attempts to "ride the edge" of
     always using the highest loss scale possible without incurring overflow.
 
     Args:
         init_scale (float, optional, default=2**32):  Initial loss scale attempted by :class:`DynamicLossScaler.`
         scale_factor (float, optional, default=2.0):  Factor used when adjusting the loss scale. If an overflow is encountered, the loss scale is readjusted to loss scale/``scale_factor``.  If ``scale_window`` consecutive iterations take place without an overflow, the loss scale is readjusted to loss_scale*``scale_factor``.
         scale_window (int, optional, default=1000):  Number of consecutive iterations without an overflow to wait before increasing the loss scale.
+        consecutive_hysteresis (bool, optional, default=False): Whether to refill hysteresis if we reach an iteration that doesn't overflow
     """
 
     def __init__(self,
                  init_scale=2**32,
                  scale_factor=2.,
                  scale_window=1000,
                  min_scale=1,
@@ -186,14 +188,17 @@
                     if self.dtype == torch.half:
                         overflow_msg += f" Attempted loss scale: {int(self.cur_scale)}, but hysteresis is {self.cur_hysteresis}. Reducing hysteresis to {self.cur_hysteresis-1}"
                     logger.info(overflow_msg)
                 self.cur_hysteresis -= 1
             self.last_overflow_iter = self.cur_iter
         else:
             if self.consecutive_hysteresis:
+                if dist.get_rank() == 0:
+                    hysteresis_msg = f"Consecutive hysteresis is enabled. Restoring hysteresis to {self.delayed_shift}"
+                    logger.info(hysteresis_msg)
                 self.cur_hysteresis = self.delayed_shift
             if (self.cur_iter - self.last_overflow_iter) % self.scale_window == 0:
                 if not self.consecutive_hysteresis:
                     self.cur_hysteresis = self.delayed_shift
                 self.cur_scale *= self.scale_factor
         self.cur_iter += 1
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/adam.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/lamb.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/zoadam.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/zoadam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/fp16/unfused_optimizer.py` & `deepspeed-0.9.3/deepspeed/runtime/fp16/unfused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/hybrid_engine.py` & `deepspeed-0.9.3/deepspeed/runtime/hybrid_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,22 +81,24 @@
 
         _replace_linear_layer(model)
 
     def new_inference_container(self, orig_layer, policy_cls, layer_id):
         policy = policy_cls(orig_layer, inference=True)
         _container = policy_to_ds_container(
             policy=policy,
-            config=DeepSpeedInferenceConfig(set_empty_params=True,
-                                            max_out_tokens=self._config.hybrid_engine.max_out_tokens,
-                                            min_out_tokens=self._config.hybrid_engine.max_out_tokens,
-                                            transposed_mode=True),
+            config=DeepSpeedInferenceConfig(
+                set_empty_params=True,
+                dtype=torch.float16 if self._config.fp16_enabled else torch.float32,
+                max_out_tokens=self._config.hybrid_engine.max_out_tokens,
+                min_out_tokens=self._config.hybrid_engine.max_out_tokens,
+                transposed_mode=True,
+            ),
             model_config=self.module.config if hasattr(self.module, 'config') else None,
             layer_id=layer_id,
             child=orig_layer)
-        _container.set_dtype(self._config.fp16_enabled)
 
         if self.mpu is not None:
             if hasattr(self.mpu, 'get_model_parallel_world_size'):
                 _container.set_tensor_parallel_config(self.mpu.get_model_parallel_world_size(),
                                                       self.mpu.get_model_parallel_group())
             else:
                 _container.set_tensor_parallel_config(self.mpu.get_tensor_model_parallel_world_size(),
@@ -161,15 +163,15 @@
                 self._unfuse_lora(self.layer_params[layer_id], self.lora_params[layer_id])
 
     def retake_inference_cache(self):
         if self._config.hybrid_engine.release_inference_cache:
             retake_success = inference_cuda_module.retake_workspace()
 
             if not retake_success:
-                logger.warning("Unable to acquire workspace on first attempt, emtpying cache and retrying.")
+                logger.warning("Unable to acquire workspace on first attempt, emptying cache and retrying.")
                 gc.collect()
                 get_accelerator().empty_cache()
                 retake_success = inference_cuda_module.retake_workspace()
 
                 if not retake_success:
                     raise RuntimeError("Unable to retake inference workspace.")
 
@@ -201,16 +203,16 @@
                     with GatheredParameters(non_active_params):
                         for layer_id in range(lg * partition_size,
                                               min(len(self.layer_params), (lg + 1) * partition_size), 1):
                             if len(self.all_lora_params) > 0:
                                 self._fuse_lora(self.layer_params[layer_id], self.lora_params[layer_id])
 
                             if self.mpu is not None:
-                                self._inference_containers[layer_id].apply_tensor_parallelism(
-                                    mp_group=self.mp_group, tp_size=self._config.hybrid_engine.inference_tp_size)
+                                self._inference_containers[layer_id].apply_tensor_parallelism(self.mp_replace,
+                                                                                              reversed_dim=True)
 
                 # TODO(cmikeh2) Evaluate if this can be deferred when release_inference_cache
                 # is enabled.
                 gc.collect()
                 get_accelerator().empty_cache()
 
                 self._gather_latency = time.time() - self._t0
@@ -312,33 +314,50 @@
         self.all_lora_params = []
 
         self._other_layers = []
         self._orig_modules_others = []
         self._orig_fwds_others = []
 
         if self._config.hybrid_engine.inference_tp_size > 1:
-            if self.mpu is not None:
+            if self.mpu is None:
                 global_rank = dist.get_rank()
                 world_size = dist.get_world_size()
                 mp_group_id = global_rank // self._config.hybrid_engine.inference_tp_size
                 num_mp_groups = world_size // self._config.hybrid_engine.inference_tp_size
                 for mp_group_id in range(num_mp_groups):
                     ranks = list(
                         range(mp_group_id * self._config.hybrid_engine.inference_tp_size, \
                             (mp_group_id + 1) * self._config.hybrid_engine.inference_tp_size, \
                             1)
                     )
                     mp_group = dist.new_group(ranks)
                     if global_rank in ranks:
+                        # mp_group is used for broader collective
                         self.mp_group = mp_group
+
+                        # mp_replace is used for container tensor slicing
+                        from deepspeed.module_inject import ReplaceWithTensorSlicing
+                        self.mp_replace = ReplaceWithTensorSlicing(
+                            mp_group=self.mp_group,
+                            mp_size=self._config.hybrid_engine.inference_tp_size,
+                            out_dim=0,
+                            in_dim=1)
+
             else:
                 self.mp_group = self.mpu.get_model_parallel_group() if hasattr(self.mpu, 'get_model_parallel_group') else \
                     self.mpu.get_tensor_model_parallel_group()
+
+                from deepspeed.module_inject import ReplaceWithTensorSlicing
+                self.mp_replace = ReplaceWithTensorSlicing(mp_group=self.mp_group,
+                                                           mp_size=self._config.hybrid_engine.inference_tp_size,
+                                                           out_dim=0,
+                                                           in_dim=1)
         else:
             self.mp_group = None
+            self.mp_replace = None
         self.populate_all_inference_policies()
         self.all_layers_params = list(self.module.parameters())
         self.create_inference_containers(self.module)
 
         if len(self._inference_containers) > 0:
             self._generate = self.module.generate
             self.module.generate = self.generate
@@ -385,42 +404,40 @@
             for i, (orig_module, inference_container) in enumerate(zip(self._orig_modules,
                                                                        self._inference_containers)):
                 if self.Z3_enabled and not self.gather_all_layers:
                     orig_module.forward = self._zero3_forward(i)
                 else:
                     orig_module.forward = inference_container.module.forward
 
-                inference_container.align_merged_qkv()
+                inference_container.transform_for_inference()
 
             if not self.Z3_enabled or self.gather_all_layers:
                 for orig_module, inference_layer in zip(self._orig_modules_others, self._other_layers):
                     orig_module.forward = inference_layer.forward
         if self.Z3_enabled:
             gc.collect()
             get_accelerator().empty_cache()
         if self._t_start is None:
             self._t_start = time.time()
 
     def train(self, mode=True):
         if mode and len(self._orig_modules) > 0:
             for inference_container, orig_module, orig_fwd in zip(self._inference_containers, self._orig_modules,
                                                                   self._orig_fwds):
-                inference_container.partition_merged_qkv()
+                inference_container.transform_for_training()
                 orig_module.forward = orig_fwd
             for orig_module, orig_fwd in zip(self._orig_modules_others, self._orig_fwds_others):
                 orig_module.forward = orig_fwd
         super().train(mode)
         if mode:
             self._training_start_time = time.time()
 
     def step(self, lr_kwargs=None):
         super().step(lr_kwargs=lr_kwargs)
 
         if len(self._inference_containers) > 0:
-            if(self._inference_containers[0].module.attention.attn_qkvw is not None and \
-                self._inference_containers[0].q_k_v is not None):
-                for inference_container in self._inference_containers:
-                    inference_container.reset_qkv()
+            for inference_container in self._inference_containers:
+                inference_container.reset_params()
 
         if self._training_start_time is not None:
             self._training_latency += (time.time() - self._training_start_time)
             self._training_start_time = time.time()
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/lr_schedules.py` & `deepspeed-0.9.3/deepspeed/runtime/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/pipe/engine.py` & `deepspeed-0.9.3/deepspeed/runtime/pipe/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
             grad = weight._hp_grad if self.bfloat16_enabled() else weight.grad
             dist.all_reduce(grad, group=group)
 
     def _exec_reduce_grads(self):
         self._force_grad_boundary = True
         if self.pipeline_enable_backward_allreduce:
             if self.bfloat16_enabled():
-                if self.zero_optimization_stage() < ZeroStageEnum().gradients:
+                if self.zero_optimization_stage() < ZeroStageEnum.gradients:
                     self._bf16_reduce_grads()
                 else:
                     raise NotImplementedError("PP+BF16 only work for ZeRO Stage 1")
             else:
                 self.allreduce_gradients(bucket_size=MEMORY_OPT_ALLREDUCE_SIZE)
         self._force_grad_boundary = False
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/pipe/module.py` & `deepspeed-0.9.3/deepspeed/runtime/pipe/module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/pipe/p2p.py` & `deepspeed-0.9.3/deepspeed/runtime/pipe/p2p.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/pipe/schedule.py` & `deepspeed-0.9.3/deepspeed/runtime/pipe/schedule.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/pipe/topology.py` & `deepspeed-0.9.3/deepspeed/runtime/pipe/topology.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/progressive_layer_drop.py` & `deepspeed-0.9.3/deepspeed/runtime/progressive_layer_drop.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/quantize.py` & `deepspeed-0.9.3/deepspeed/runtime/quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/sparse_tensor.py` & `deepspeed-0.9.3/deepspeed/runtime/sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/state_dict_factory.py` & `deepspeed-0.9.3/deepspeed/runtime/state_dict_factory.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/aio_config.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/aio_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/async_swapper.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/async_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/constants.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/optimizer_utils.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/utils.py` & `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/utils.py` & `deepspeed-0.9.3/deepspeed/runtime/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     def has_overflow(self, params, has_moe_params=None):
         if has_moe_params is None:
             has_moe_params = self.has_moe_params
         overflow = self.has_overflow_serial(params)
         # Since each model parallel GPU carries only part of the model,
         # make sure overflow flag is synced across all the model parallel GPUs
         overflow_gpu = get_accelerator().ByteTensor([overflow])
-        # deepspeeed.comm.all_reduce(overflow_gpu,
+        # deepspeed.comm.all_reduce(overflow_gpu,
         #                             op=deepspeed.comm.ReduceOp.MAX,
         #                             group=mpu.get_model_parallel_group())
         if has_moe_params:
             # All reduce this across expert_parallel_group, so that if an expert
             # overflows, we detect it here
             dist.all_reduce(overflow_gpu, op=dist.ReduceOp.MAX, group=groups._get_max_expert_parallel_group())
         if self.zero_reduce_scatter:
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/weight_quantizer.py` & `deepspeed-0.9.3/deepspeed/runtime/weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/config.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/contiguous_memory_allocator.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/contiguous_memory_allocator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/linear.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/mics.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/mics.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/mics_utils.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/mics_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/offload_config.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/offload_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/parameter_offload.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/parameter_offload.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import torch
 from collections import OrderedDict
 from deepspeed.runtime.utils import see_memory_usage
 from deepspeed.runtime.zero.offload_config import OffloadDeviceEnum
 from deepspeed.runtime.zero.partition_parameters import _init_external_params
 from deepspeed.runtime.zero.partition_parameters import *
-from deepspeed.runtime.zero.partitioned_param_coordinator import PartitionedParameterCoordinator, iter_params
+from deepspeed.runtime.zero.partitioned_param_coordinator import PartitionedParameterCoordinator, InflightParamRegistry, iter_params
 from deepspeed import comm as dist
 from deepspeed.accelerator import get_accelerator
 
 FWD_MODULE_STACK = list()
 
 
 def is_builtin_type(obj):
@@ -240,14 +240,18 @@
 
         self.param_coordinators = {}
         self._prefetch_bucket_sz = int(prefetch_bucket_size)
         self._max_reuse_distance_in_numel = int(max_reuse_distance)
         self._max_available_parameters_in_numel = int(max_live_parameters)
         self.__allgather_stream = get_accelerator().Stream() if overlap_comm else get_accelerator().default_stream()
 
+        if not hasattr(module, "ds_inflight_param_registry"):
+            module.ds_inflight_param_registry = InflightParamRegistry()
+        self.__inflight_param_registry = module.ds_inflight_param_registry
+
         self.forward_hooks = []
         self.backward_hooks = []
         self.setup_zero_stage3_hooks()
         print_rank_0(
             f'Created module hooks: forward = {len(self.forward_hooks)}, backward = {len(self.backward_hooks)}',
             force=False)
 
@@ -266,14 +270,15 @@
     def get_param_coordinator(self, training):
         if not training in self.param_coordinators:
             self.param_coordinators[training] = PartitionedParameterCoordinator(
                 prefetch_bucket_sz=self._prefetch_bucket_sz,
                 max_reuse_distance_in_numel=self._max_reuse_distance_in_numel,
                 max_available_parameters_in_numel=self._max_available_parameters_in_numel,
                 allgather_stream=self.__allgather_stream,
+                inflight_param_registry=self.__inflight_param_registry,
                 prefetch_nvme=self.offload_device == OffloadDeviceEnum.nvme,
             )
 
         return self.param_coordinators[training]
 
     def empty_partition_cache(self):
         self.partition_all_parameters()
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/partition_parameters.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/partition_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -796,36 +796,40 @@
                 assert ds_config.zero_config.offload_param is not None, \
                 f'"offload_param" must be defined in DeepSpeed Config if remote device is {OffloadDeviceEnum.nvme}.'
 
                 assert ds_config.zero_config.offload_param.nvme_path is not None, \
                 f'"nvme_path" in DeepSpeed Config cannot be None if remote device is {OffloadDeviceEnum.nvme}'
 
     def _post_init_method(self, module):
-        #see_memory_usage(f"Before converting parmas in {module.__class__.__name__}", force=False)
+        #see_memory_usage(f"Before converting params in {module.__class__.__name__}", force=False)
         print_rank_0(f'Converting Params in {module.__class__.__name__}', force=False)
-        see_memory_usage(f"Before converting and partitioning parmas in {module.__class__.__name__}", force=False)
+        see_memory_usage(f"Before converting and partitioning params in {module.__class__.__name__}", force=False)
 
         global param_count
         for name, param in module.named_parameters(recurse=False):
             param_count += param.numel()
             if not is_zero_param(param):
                 self._convert_to_deepspeed_param(param)
                 print_rank_0(
                     f"Partitioning param {debug_param2name_id_shape(param)} module={debug_module2name(module)}")
 
                 if get_accelerator().on_accelerator(param):
-                    dist.broadcast(param, 0, self.get_dp_process_group())
+                    if dist.get_world_group() == self.get_dp_process_group():
+                        dist.broadcast(param, 0, self.get_dp_process_group())
+                    else:
+                        dist.broadcast(param, dist.get_global_rank(self.get_dp_process_group(), 0),
+                                       self.get_dp_process_group())
                 else:
                     if dist.get_rank() == 0:
                         logger.warn(f"param `{name}` in {module.__class__.__name__} "
                                     f"not on GPU so was not broadcasted from rank 0")
 
                 param.partition()
         see_memory_usage(
-            f"Param count {param_count}. After converting and partitioning parmas in {module.__class__.__name__}",
+            f"Param count {param_count}. After converting and partitioning params in {module.__class__.__name__}",
             force=False)
 
     def _convert_to_deepspeed_param(self, param):
 
         # Partitioned, Normal, Remote
         param.ds_param_type = ZeroParamType.PARTITIONED
 
@@ -1396,15 +1400,15 @@
 
             # some ranks may have partitions that are padded to go beyond the grad size.
             # For these ranks the output of reduce scatter is a separate buffer and needs
             # to be copied in
             partition_size = param.ds_tensor.ds_numel
             start = self.get_partition_rank() * partition_size
             end = start + partition_size
-            #print_rank_0("REduce scatter was executed for praam {param.ds_id}")
+            #print_rank_0("REduce scatter was executed for param {param.ds_id}")
             if start < param.ds_numel and end > param.ds_numel:
                 elements = param.ds_numel - start
                 param.grad.view(-1).narrow(0, start, elements).copy_(reduced_partition.narrow(0, 0, elements))
 
     def _reduce_scatter_gradient(self, param):
 
         partition_size = param.ds_tensor.ds_numel
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/partitioned_param_coordinator.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/partitioned_param_coordinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,42 +36,44 @@
     RECORD = 1
     # Use recorded network trace to optimize current forward+backward or forward
     COMPLETE = 2
     # Recorded trace does not match current forward+backward or forward pass.
     INVALID = 3
 
 
-class PartitionedParameterCoordinator:
-    """Handles partitioning and gathering of parameters."""
+class InflightParamRegistry(UserDict):
+    """registry for parameters in flight"""
+
+    def __setitem__(self, param: Parameter, handle: AllGatherCoalescedHandle) -> None:
+        if param in self.data:
+            raise RuntimeError(f"{param.ds_summary()} already in registry")
+        if param.ds_status != ZeroParamStatus.INFLIGHT:
+            raise RuntimeError(f"attempted to add non-inflight parameter to registry {param.ds_summary()}")
+        self.data[param] = handle
 
-    class __InflightParamRegistry(UserDict):
-        """registry for parameters in flight"""
 
-        def __setitem__(self, param: Parameter, handle: AllGatherCoalescedHandle) -> None:
-            if param in self.data:
-                raise RuntimeError(f"{param.ds_summary()} already in registry")
-            if param.ds_status != ZeroParamStatus.INFLIGHT:
-                raise RuntimeError(f"attempted to add non-inflight parameter to registry {param.ds_summary()}")
-            self.data[param] = handle
+class PartitionedParameterCoordinator:
+    """Handles partitioning and gathering of parameters."""
 
     @dataclass
     class __ParamInTrace:
         param: Parameter
         step_id_last_used_at: int
 
     def __init__(
         self,
         prefetch_bucket_sz: int,
         max_reuse_distance_in_numel: int,
         max_available_parameters_in_numel: int,
         allgather_stream: get_accelerator().Stream,
+        inflight_param_registry: InflightParamRegistry,
         prefetch_nvme: bool = False,
     ) -> None:
         # mapping of param -> handle for each param that is currently in flight
-        self.__inflight_param_registry = __class__.__InflightParamRegistry()
+        self.__inflight_param_registry = inflight_param_registry
         # keeps track of the number of submodules invoked so far.
         self.__step_id: int = 0
         # network tracing mode
         self.__trace_mode: ZeRoTraceMode = ZeRoTraceMode.RECORD
         # sequence of submodules/parameters in forward pass + backward pass
         self.__submodule_order: Iterable[Module] = []
         self.__param_order: Iterable[__class__.__ParamInTrace] = []
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/stage3.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/stage3.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                                                             ds_config=ds_config,
                                                             overlap_comm=overlap_comm,
                                                             prefetch_bucket_size=prefetch_bucket_size,
                                                             max_reuse_distance=max_reuse_distance,
                                                             max_live_parameters=max_live_parameters,
                                                             param_persistence_threshold=param_persistence_threshold,
                                                             model_persistence_threshold=model_persistence_threshold,
-                                                            offload_optimizer_config=offload_optimizer_config,
+                                                            offload_param_config=offload_param_config,
                                                             mpu=mpu)
 
         self.persistent_parameters = self.parameter_offload.persistent_parameters
         self._configure_offloading(offload_optimizer_config, offload_param_config)
 
         self.module = module
         self.elastic_checkpoint = elastic_checkpoint
@@ -347,27 +347,27 @@
         ds_config,
         overlap_comm,
         prefetch_bucket_size,
         max_reuse_distance,
         max_live_parameters,
         param_persistence_threshold,
         model_persistence_threshold,
-        offload_optimizer_config,
+        offload_param_config,
         mpu,
     ):
         return DeepSpeedZeRoOffload(module=module,
                                     timers=timers,
                                     ds_config=ds_config,
                                     overlap_comm=overlap_comm,
                                     prefetch_bucket_size=prefetch_bucket_size,
                                     max_reuse_distance=max_reuse_distance,
                                     max_live_parameters=max_live_parameters,
                                     param_persistence_threshold=param_persistence_threshold,
                                     model_persistence_threshold=model_persistence_threshold,
-                                    offload_param_config=offload_optimizer_config,
+                                    offload_param_config=offload_param_config,
                                     mpu=mpu)
 
     def _get_trainable_parameter_groups(self):
         param_groups = []
         for param_group in self.optimizer.param_groups:
             trainable_params = {"params": [p for p in param_group["params"] if p.requires_grad]}
             param_groups.append(trainable_params)
@@ -888,29 +888,29 @@
                 if self.offload_optimizer_pin_memory:
                     subgroup_gradient_buffer = get_accelerator().pin_memory(subgroup_gradient_buffer)
 
                 self.fp32_partitioned_groups_flat[i].grad = subgroup_gradient_buffer
             else:
                 self.fp32_partitioned_groups_flat[i].grad = gradient_buffer.narrow(0, 0, num_elements)
 
-            # Initialize the optimizer states with the flattended fp32 partition.
+            # Initialize the optimizer states with the flattened fp32 partition.
             if not is_adagrad:
                 self._optimizer_step(i)
 
             if swappable_param_subgroup:
                 self._partitioned_params_swap_out(i)
 
             if swappable_optimizer_subgroup:
                 self._optimizer_states_and_gradient_swap_out(i, timer_names)
 
             see_memory_usage(
                 f'[End] Initialize optimizer states {i} / {num_subgroups} subgroups, num_elems: {num_elements}, swappable opt/param:{swappable_optimizer_subgroup}/{swappable_param_subgroup}',
                 force=False)
 
-        # Initialize the optimizer states with the flattended fp32 partition.
+        # Initialize the optimizer states with the flattened fp32 partition.
         if is_adagrad:
             self.optimizer = torch.optim.Adagrad(self.fp32_partitioned_groups_flat, **self.optimizer.defaults)
 
         self.stop_timers([INIT_OPTIMIZER_TIMER])
         self.log_timers(timer_names)
 
         if self.swap_optimizer:
@@ -1032,15 +1032,15 @@
     def report_ipg_memory_usage(self, tag, param_elems):
         elem_count = self.elements_in_ipg_bucket + param_elems
         percent_of_bucket_size = (100.0 * elem_count) // self.reduce_bucket_size
         see_memory_usage(
             f"{tag}: elems in_bucket {self.elements_in_ipg_bucket} param {param_elems} max_percent {percent_of_bucket_size}",
             force=False)
 
-    ###############Idependent Partition Gradient ########################
+    ###############Independent Partition Gradient ########################
     def reduce_independent_p_g_buckets_and_remove_grads(self, param, i):
         #print_rank_0(f"Inside reduce ipg buckets. {debug_param2name_id_shape(param)}, ipg elements {self.elements_in_ipg_bucket}, reduce bucket size {self.reduce_bucket_size}", force=True)
 
         # Because the ipg bucket is initialized with a random place holder tensor, we must
         # explicitly check that the bucket has any real data in it (self.elements_in_ipg_bucket >
         # 0). Otherwise if the incoming param.ds_numel is large, this branch may get triggered on a
         # garbage data and `self.average_tensor()` will crash because its params_to_reduce will be
@@ -1118,15 +1118,16 @@
             full_grads_for_rank = [g.to(self.communication_data_type) for g in full_grads_for_rank]
 
         if self.postscale_gradients and self.gradient_predivide_factor != 1.0:
             full_grads_for_rank = [g.div(self.gradient_predivide_factor) for g in full_grads_for_rank]
 
         grad_partitions_for_rank = reduce_scatter_coalesced(full_grads_for_rank, self.dp_process_group)
 
-        if self.postscale_gradients and self.gradient_predivide_factor != dist.get_world_size(self.dp_process_group):
+        if self.postscale_gradients and self.gradient_predivide_factor != 1.0 and self.gradient_predivide_factor != dist.get_world_size(
+                self.dp_process_group):
             grad_partitions_for_rank = [g.mul(self.gradient_predivide_factor) for g in grad_partitions_for_rank]
 
         if self.communication_data_type != self.dtype:
             grad_partitions_for_rank = [g.to(self.dtype) for g in grad_partitions_for_rank]
 
         return grad_partitions_for_rank
 
@@ -1494,15 +1495,20 @@
             #    logger.info(f"Total Norm beginning {total_norm}")
             grad_norms = []
             for g, p in zip(gradients, params):
                 if is_model_parallel_parameter(p) or (self.model_parallel_rank == 0):
                     grad_norms.append(g.to(get_accelerator().device_name(), non_blocking=True).double().norm(2))
 
             # Sum across all model parallel GPUs.
-            total_norm_cuda = torch.sum(torch.pow(torch.stack(grad_norms), 2))
+            if len(grad_norms) == 0:
+                # FIX https://github.com/microsoft/DeepSpeed/issues/3564
+                total_norm_cuda = torch.tensor(0,
+                                               dtype=gradients[0].dtype).to(get_accelerator().device_name()).double()
+            else:
+                total_norm_cuda = torch.sum(torch.pow(torch.stack(grad_norms), 2))
 
             dist.all_reduce(total_norm_cuda, op=dist.ReduceOp.SUM, group=self.dp_process_group)
 
             self._model_parallel_all_reduce(tensor=total_norm_cuda, op=dist.ReduceOp.SUM)
 
             total_norm = total_norm_cuda.item()**(1. / norm_type)
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/stage_1_and_2.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/stage_1_and_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
         for i, group in enumerate(self.bit16_groups):
             single_grad_partition = torch.zeros(int(self.partition_size[i]),
                                                 dtype=self.single_partition_of_fp32_groups[i].dtype,
                                                 device=self.device)
             self.single_partition_of_fp32_groups[i].grad = get_accelerator().pin_memory(
                 single_grad_partition) if self.cpu_offload else single_grad_partition
 
-        # Initialize the optimizer states with the flattended fp32 partition.
+        # Initialize the optimizer states with the flattened fp32 partition.
         # State initialization for the Adagrad optimizer occurs at construction as opposed to other optimizers
         # which do lazy initialization of the state at the first call to step.
         if isinstance(self.optimizer, torch.optim.Adagrad):
             self.optimizer = torch.optim.Adagrad(self.single_partition_of_fp32_groups, **self.optimizer.defaults)
         else:
             self.optimizer.step()
 
@@ -1626,15 +1626,15 @@
         bit16_partitions = self.parallel_partitioned_bit16_groups[group_no]
         partition_id = dist.get_rank(group=self.real_dp_process_group[group_no])
         return [bit16_partitions[dist.get_rank(group=self.real_dp_process_group[group_no])]]
 
     def _optimizer_step(self, group_no):
         original_param_groups = self.optimizer.param_groups
         self.optimizer.param_groups = [original_param_groups[group_no]]
-        # Disabling this as the C++ side copy & synchornize is not working correctly
+        # Disabling this as the C++ side copy & synchronize is not working correctly
         #from deepspeed.ops.adam import DeepSpeedCPUAdam
         #if type(self.optimizer) == DeepSpeedCPUAdam and self.dtype == torch.half:
         #    self.optimizer.step(fp16_param_groups=[self.get_bit16_param_group(group_no)])
         #else:
         #    self.optimizer.step()
         self.optimizer.step()
         self.optimizer.param_groups = original_param_groups
```

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/test.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/test.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/tiling.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/tiling.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/runtime/zero/utils.py` & `deepspeed-0.9.3/deepspeed/runtime/zero/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/__init__.py` & `deepspeed-0.9.3/deepspeed/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 from .groups import *
 from .nvtx import instrument_w_nvtx
 # TODO: Move tensor fragment and mixed precision to zero utils
 from .tensor_fragment import tensor_fragment, get_full_hp_param, get_hp_fragment_mapping, fragment_address, get_full_hp_grad
 from .tensor_fragment import safe_get_full_fp32_param, safe_get_full_grad, safe_get_full_optimizer_state
 from .mixed_precision_linkage import link_hp_params
 from deepspeed.runtime.dataloader import RepeatingLoader
+from .numa import get_numactl_cmd
```

### Comparing `deepspeed-0.9.2/deepspeed/utils/comms_logging.py` & `deepspeed-0.9.3/deepspeed/utils/comms_logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/debug.py` & `deepspeed-0.9.3/deepspeed/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/groups.py` & `deepspeed-0.9.3/deepspeed/utils/groups.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/init_on_device.py` & `deepspeed-0.9.3/deepspeed/utils/init_on_device.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/logging.py` & `deepspeed-0.9.3/deepspeed/utils/logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/mixed_precision_linkage.py` & `deepspeed-0.9.3/deepspeed/utils/mixed_precision_linkage.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/tensor_fragment.py` & `deepspeed-0.9.3/deepspeed/utils/tensor_fragment.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed/utils/timer.py` & `deepspeed-0.9.3/deepspeed/utils/timer.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,35 +36,51 @@
     class Timer:
         """Timer."""
 
         def __init__(self, name):
             self.name_ = name
             self.started_ = False
             self.event_timers = []
+            self.use_host_timer = get_accelerator().is_synchronized_device()
             self.start_event = None
             self.elapsed_records = None
+            self.start_time = 0.0
+            self.end_time = 0.0
 
         def start(self):
             """Start the timer."""
             assert not self.started_, f"{self.name_} timer has already been started"
-            self.start_event = get_accelerator().Event(enable_timing=True)
-            self.start_event.record()
+            if self.use_host_timer:
+                self.start_time = time.time()
+            else:
+                event_class = get_accelerator().Event
+                self.start_event = event_class(enable_timing=True)
+                self.start_event.record()
             self.started_ = True
 
         def stop(self, reset=False, record=False):
             """Stop the timer."""
             assert self.started_, "timer is not started"
-            end_event = get_accelerator().Event(enable_timing=True)
-            end_event.record()
-            self.event_timers.append(CudaEventTimer(self.start_event, end_event))
-            self.start_event = None
+            event_class = get_accelerator().Event
+            if self.use_host_timer:
+                self.end_time = time.time()
+                self.event_timers.append(self.end_time - self.start_time)
+            else:
+                event_class = get_accelerator().Event
+                end_event = event_class(enable_timing=True)
+                end_event.record()
+                self.event_timers.append(CudaEventTimer(self.start_event, end_event))
+                self.start_event = None
             self.started_ = False
 
         def _get_elapsed_msec(self):
-            self.elapsed_records = [et.get_elapsed_msec() for et in self.event_timers]
+            if self.use_host_timer:
+                self.elapsed_records = [et * 1000.0 for et in self.event_timers]
+            else:
+                self.elapsed_records = [et.get_elapsed_msec() for et in self.event_timers]
             self.event_timers.clear()
             return sum(self.elapsed_records)
 
         def reset(self):
             """Reset timer."""
             self.started_ = False
             self.start_event = None
```

### Comparing `deepspeed-0.9.2/deepspeed/utils/zero_to_fp32.py` & `deepspeed-0.9.3/deepspeed/utils/zero_to_fp32.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/deepspeed.egg-info/PKG-INFO` & `deepspeed-0.9.3/deepspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.2
+Version: 0.9.3
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
-License: MIT
+License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,15 @@
 Provides-Extra: 1bit
 Provides-Extra: 1bit_mpi
 Provides-Extra: readthedocs
 Provides-Extra: dev
 Provides-Extra: autotuning
 Provides-Extra: autotuning_ml
 Provides-Extra: sparse_attn
+Provides-Extra: sparse
 Provides-Extra: inf
 Provides-Extra: sd
 Provides-Extra: all
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
```

### Comparing `deepspeed-0.9.2/deepspeed.egg-info/SOURCES.txt` & `deepspeed-0.9.3/deepspeed.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 README.md
 build.txt
 setup.cfg
 setup.py
 version.txt
 accelerator/__init__.py
 accelerator/abstract_accelerator.py
+accelerator/cpu_accelerator.py
 accelerator/cuda_accelerator.py
+accelerator/npu_accelerator.py
 accelerator/real_accelerator.py
 bin/deepspeed
 bin/deepspeed.pt
 bin/ds
 bin/ds_bench
 bin/ds_elastic
 bin/ds_report
@@ -36,14 +38,15 @@
 csrc/aio/py_lib/deepspeed_py_aio.h
 csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
 csrc/aio/py_lib/deepspeed_py_aio_handle.h
 csrc/aio/py_lib/deepspeed_py_copy.cpp
 csrc/aio/py_lib/deepspeed_py_copy.h
 csrc/aio/py_lib/py_ds_aio.cpp
 csrc/common/custom_cuda_kernel.cu
+csrc/cpu/comm/ccl.cpp
 csrc/includes/StopWatch.h
 csrc/includes/Timer.h
 csrc/includes/compat.h
 csrc/includes/context.h
 csrc/includes/conversion_utils.h
 csrc/includes/cpu_adagrad.h
 csrc/includes/cpu_adam.h
@@ -89,16 +92,18 @@
 csrc/transformer/normalize_kernels.cu
 csrc/transformer/softmax_kernels.cu
 csrc/transformer/transform_kernels.cu
 csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
 csrc/transformer/inference/csrc/dequantize.cu
 csrc/transformer/inference/csrc/gelu.cu
 csrc/transformer/inference/csrc/layer_norm.cu
+csrc/transformer/inference/csrc/pointwise_ops.cu
 csrc/transformer/inference/csrc/pt_binding.cpp
 csrc/transformer/inference/csrc/relu.cu
+csrc/transformer/inference/csrc/rms_norm.cu
 csrc/transformer/inference/csrc/softmax.cu
 csrc/transformer/inference/csrc/transform.cu
 csrc/transformer/inference/includes/inference_context.h
 csrc/transformer/inference/includes/inference_cublas_wrappers.h
 csrc/transformer/inference/includes/inference_cuda_layers.h
 csrc/utils/flatten_unflatten.cpp
 deepspeed/__init__.py
@@ -110,15 +115,17 @@
 deepspeed.egg-info/SOURCES.txt
 deepspeed.egg-info/dependency_links.txt
 deepspeed.egg-info/entry_points.txt
 deepspeed.egg-info/requires.txt
 deepspeed.egg-info/top_level.txt
 deepspeed/accelerator/__init__.py
 deepspeed/accelerator/abstract_accelerator.py
+deepspeed/accelerator/cpu_accelerator.py
 deepspeed/accelerator/cuda_accelerator.py
+deepspeed/accelerator/npu_accelerator.py
 deepspeed/accelerator/real_accelerator.py
 deepspeed/autotuning/__init__.py
 deepspeed/autotuning/autotuner.py
 deepspeed/autotuning/config.py
 deepspeed/autotuning/constants.py
 deepspeed/autotuning/scheduler.py
 deepspeed/autotuning/utils.py
@@ -139,17 +146,19 @@
 deepspeed/checkpoint/reshape_meg_2d.py
 deepspeed/checkpoint/reshape_utils.py
 deepspeed/checkpoint/universal_checkpoint.py
 deepspeed/checkpoint/utils.py
 deepspeed/checkpoint/zero_checkpoint.py
 deepspeed/comm/__init__.py
 deepspeed/comm/backend.py
+deepspeed/comm/ccl.py
 deepspeed/comm/comm.py
 deepspeed/comm/config.py
 deepspeed/comm/constants.py
+deepspeed/comm/reduce_op.py
 deepspeed/comm/torch.py
 deepspeed/comm/utils.py
 deepspeed/compression/__init__.py
 deepspeed/compression/basic_layer.py
 deepspeed/compression/compress.py
 deepspeed/compression/config.py
 deepspeed/compression/constants.py
@@ -202,22 +211,27 @@
 deepspeed/module_inject/containers/bloom.py
 deepspeed/module_inject/containers/clip.py
 deepspeed/module_inject/containers/distil_bert.py
 deepspeed/module_inject/containers/gpt2.py
 deepspeed/module_inject/containers/gptj.py
 deepspeed/module_inject/containers/gptneo.py
 deepspeed/module_inject/containers/gptneox.py
+deepspeed/module_inject/containers/llama.py
 deepspeed/module_inject/containers/megatron_gpt.py
 deepspeed/module_inject/containers/megatron_gpt_moe.py
 deepspeed/module_inject/containers/opt.py
 deepspeed/module_inject/containers/unet.py
 deepspeed/module_inject/containers/vae.py
 deepspeed/module_inject/containers/features/__init__.py
+deepspeed/module_inject/containers/features/gated_mlp.py
+deepspeed/module_inject/containers/features/hybrid_engine.py
+deepspeed/module_inject/containers/features/hybrid_megatron.py
 deepspeed/module_inject/containers/features/megatron.py
 deepspeed/module_inject/containers/features/meta_tensor.py
+deepspeed/module_inject/containers/features/split_qkv.py
 deepspeed/moe/__init__.py
 deepspeed/moe/experts.py
 deepspeed/moe/layer.py
 deepspeed/moe/mappings.py
 deepspeed/moe/sharded_moe.py
 deepspeed/moe/utils.py
 deepspeed/monitor/__init__.py
@@ -258,14 +272,15 @@
 deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
 deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
 deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
 deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
 deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
 deepspeed/ops/csrc/aio/py_test/single_process_config.json
 deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+deepspeed/ops/csrc/cpu/comm/ccl.cpp
 deepspeed/ops/csrc/includes/StopWatch.h
 deepspeed/ops/csrc/includes/Timer.h
 deepspeed/ops/csrc/includes/compat.h
 deepspeed/ops/csrc/includes/context.h
 deepspeed/ops/csrc/includes/conversion_utils.h
 deepspeed/ops/csrc/includes/cpu_adagrad.h
 deepspeed/ops/csrc/includes/cpu_adam.h
@@ -311,16 +326,18 @@
 deepspeed/ops/csrc/transformer/normalize_kernels.cu
 deepspeed/ops/csrc/transformer/softmax_kernels.cu
 deepspeed/ops/csrc/transformer/transform_kernels.cu
 deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
 deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
 deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
 deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
 deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
 deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
 deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
 deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
 deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
 deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
 deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
 deepspeed/ops/csrc/utils/flatten_unflatten.cpp
 deepspeed/ops/lamb/__init__.py
@@ -337,14 +354,18 @@
 deepspeed/ops/op_builder/random_ltd.py
 deepspeed/ops/op_builder/sparse_attn.py
 deepspeed/ops/op_builder/spatial_inference.py
 deepspeed/ops/op_builder/stochastic_transformer.py
 deepspeed/ops/op_builder/transformer.py
 deepspeed/ops/op_builder/transformer_inference.py
 deepspeed/ops/op_builder/utils.py
+deepspeed/ops/op_builder/cpu/__init__.py
+deepspeed/ops/op_builder/cpu/builder.py
+deepspeed/ops/op_builder/cpu/comm.py
+deepspeed/ops/op_builder/cpu/no_impl.py
 deepspeed/ops/quantizer/__init__.py
 deepspeed/ops/quantizer/quantizer.py
 deepspeed/ops/random_ltd/__init__.py
 deepspeed/ops/random_ltd/dropping_utils.py
 deepspeed/ops/sparse_attention/__init__.py
 deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
 deepspeed/ops/sparse_attention/matmul.py
@@ -469,14 +490,15 @@
 deepspeed/utils/comms_logging.py
 deepspeed/utils/debug.py
 deepspeed/utils/exceptions.py
 deepspeed/utils/groups.py
 deepspeed/utils/init_on_device.py
 deepspeed/utils/logging.py
 deepspeed/utils/mixed_precision_linkage.py
+deepspeed/utils/numa.py
 deepspeed/utils/nvtx.py
 deepspeed/utils/tensor_fragment.py
 deepspeed/utils/timer.py
 deepspeed/utils/types.py
 deepspeed/utils/zero_to_fp32.py
 op_builder/__init__.py
 op_builder/all_ops.py
@@ -490,16 +512,22 @@
 op_builder/random_ltd.py
 op_builder/sparse_attn.py
 op_builder/spatial_inference.py
 op_builder/stochastic_transformer.py
 op_builder/transformer.py
 op_builder/transformer_inference.py
 op_builder/utils.py
+op_builder/cpu/__init__.py
+op_builder/cpu/builder.py
+op_builder/cpu/comm.py
+op_builder/cpu/no_impl.py
 requirements/requirements-1bit-mpi.txt
 requirements/requirements-autotuning-ml.txt
 requirements/requirements-autotuning.txt
+requirements/requirements-cpu.txt
 requirements/requirements-dev.txt
 requirements/requirements-inf.txt
 requirements/requirements-readthedocs.txt
 requirements/requirements-sd.txt
 requirements/requirements-sparse_attn.txt
+requirements/requirements-sparse_pruning.txt
 requirements/requirements.txt
```

### Comparing `deepspeed-0.9.2/deepspeed.egg-info/requires.txt` & `deepspeed-0.9.3/deepspeed.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,48 +10,49 @@
 
 [1bit]
 
 [1bit_mpi]
 mpi4py
 
 [all]
-diffusers
+packaging
+neural-compressor==2.1.0
+tensorboard
+torchvision
+mpi4py
+transformers
+pytest-forked
+protobuf
+xgboost
 pytest
-sphinx
-future
-sphinx-rtd-theme
-psutil
-lm-eval==0.3.0
 triton==1.0.0
-torch
 transformers[sentencepiece]
-recommonmark
-protobuf
-tqdm
-google
-pydantic<2.0.0
-mpi4py
+tabulate
 clang-format==16.0.2
-pytest-forked
 docutils<0.18
+psutil
+py-cpuinfo
+triton==2.0.0.dev20221202
+pre-commit>=2.20.0
+sphinx-rtd-theme
+sphinx
+autodoc_pydantic<2.0.0
 wandb
+pydantic<2.0.0
 pytest-xdist
-packaging
 importlib-metadata>=4
-xgboost
-autodoc_pydantic<2.0.0
-torchvision
-tabulate
-py-cpuinfo
-pytest-randomly
-triton==2.0.0.dev20221202
 hjson
-transformers
-tensorboard
-pre-commit>=2.20.0
+google
+recommonmark
+tqdm
+torch
+lm-eval==0.3.0
+future
+diffusers
+pytest-randomly
 
 [autotuning]
 tabulate
 
 [autotuning_ml]
 hjson
 tabulate
@@ -93,9 +94,12 @@
 torch
 tqdm
 
 [sd]
 diffusers
 triton==2.0.0.dev20221202
 
+[sparse]
+neural-compressor==2.1.0
+
 [sparse_attn]
 triton==1.0.0
```

### Comparing `deepspeed-0.9.2/op_builder/__init__.py` & `deepspeed-0.9.3/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/all_ops.py` & `deepspeed-0.9.3/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/async_io.py` & `deepspeed-0.9.3/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/builder.py` & `deepspeed-0.9.3/op_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 cuda_minor_mismatch_ok = {
     10: [
         "10.0",
         "10.1",
         "10.2",
     ],
     11: ["11.0", "11.1", "11.2", "11.3", "11.4", "11.5", "11.6", "11.7", "11.8"],
+    12: ["12.0", "12.1"],
 }
 
 
 def assert_no_cuda_mismatch(name=""):
     cuda_major, cuda_minor = installed_cuda_version(name)
     sys_cuda_version = f'{cuda_major}.{cuda_minor}'
     torch_cuda_version = ".".join(torch.version.cuda.split('.')[:2])
@@ -81,28 +82,36 @@
     if sys_cuda_version != torch_cuda_version:
         if (cuda_major in cuda_minor_mismatch_ok and sys_cuda_version in cuda_minor_mismatch_ok[cuda_major]
                 and torch_cuda_version in cuda_minor_mismatch_ok[cuda_major]):
             print(f"Installed CUDA version {sys_cuda_version} does not match the "
                   f"version torch was compiled with {torch.version.cuda} "
                   "but since the APIs are compatible, accepting this combination")
             return True
+        elif os.getenv("DS_SKIP_CUDA_CHECK", "0") == "1":
+            print(
+                f"{WARNING} DeepSpeed Op Builder: Installed CUDA version {sys_cuda_version} does not match the "
+                f"version torch was compiled with {torch.version.cuda}."
+                "Detected `DS_SKIP_CUDA_CHECK=1`: Allowing this combination of CUDA, but it may result in unexpected behavior."
+            )
+            return True
         raise Exception(f">- DeepSpeed Op Builder: Installed CUDA version {sys_cuda_version} does not match the "
                         f"version torch was compiled with {torch.version.cuda}, unable to compile "
                         "cuda/cpp extensions without a matching cuda version.")
     return True
 
 
 class OpBuilder(ABC):
     _rocm_version = None
     _is_rocm_pytorch = None
 
     def __init__(self, name):
         self.name = name
         self.jit_mode = False
         self.build_for_cpu = False
+        self.enable_bf16 = False
         self.error_log = None
 
     @abstractmethod
     def absolute_name(self):
         '''
         Returns absolute build path for cases where the op is pre-installed, e.g., deepspeed.ops.adam.cpu_adam
         will be installed as something like: deepspeed/ops/adam/cpu_adam.so
@@ -429,15 +438,15 @@
                             sources=self.strip_empty_entries(self.sources()),
                             include_dirs=self.strip_empty_entries(self.include_paths()),
                             extra_compile_args={'cxx': self.strip_empty_entries(self.cxx_args())},
                             extra_link_args=self.strip_empty_entries(self.extra_ldflags()))
 
     def load(self, verbose=True):
         from deepspeed.git_version_info import installed_ops, torch_info
-        if installed_ops[self.name]:
+        if installed_ops.get(self.name, False):
             # Ensure the op we're about to load was compiled with the same
             # torch/cuda versions we are currently using at runtime.
             self.validate_torch_version(torch_info)
             if torch.cuda.is_available() and isinstance(self, CUDAOpBuilder):
                 self.validate_torch_op_version(torch_info)
 
             return importlib.import_module(self.absolute_name())
@@ -473,19 +482,27 @@
         # needed at runtime. This prevents CC collisions such as multiple __half
         # implementations. Stash arch list to reset after build.
         torch_arch_list = None
         if "TORCH_CUDA_ARCH_LIST" in os.environ:
             torch_arch_list = os.environ.get("TORCH_CUDA_ARCH_LIST")
             os.environ["TORCH_CUDA_ARCH_LIST"] = ""
 
+        nvcc_args = self.strip_empty_entries(self.nvcc_args())
+        cxx_args = self.strip_empty_entries(self.cxx_args())
+
+        if isinstance(self, CUDAOpBuilder):
+            if not self.build_for_cpu and self.enable_bf16:
+                cxx_args.append("-DBF16_AVAILABLE")
+                nvcc_args.append("-DBF16_AVAILABLE")
+
         op_module = load(name=self.name,
                          sources=self.strip_empty_entries(sources),
                          extra_include_paths=self.strip_empty_entries(extra_include_paths),
-                         extra_cflags=self.strip_empty_entries(self.cxx_args()),
-                         extra_cuda_cflags=self.strip_empty_entries(self.nvcc_args()),
+                         extra_cflags=cxx_args,
+                         extra_cuda_cflags=nvcc_args,
                          extra_ldflags=self.strip_empty_entries(self.extra_ldflags()),
                          verbose=verbose)
 
         build_duration = time.time() - start_build
         if verbose:
             print(f"Time to load {self.name} op: {build_duration} seconds")
 
@@ -543,20 +560,24 @@
 
         ccs = self.filter_ccs(ccs)
         if len(ccs) == 0:
             raise RuntimeError(
                 f"Unable to load {self.name} op due to no compute capabilities remaining after filtering")
 
         args = []
+        self.enable_bf16 = True
         for cc in ccs:
             num = cc[0] + cc[2]
             args.append(f'-gencode=arch=compute_{num},code=sm_{num}')
             if cc.endswith('+PTX'):
                 args.append(f'-gencode=arch=compute_{num},code=compute_{num}')
 
+            if int(cc[0]) <= 7:
+                self.enable_bf16 = False
+
         return args
 
     def filter_ccs(self, ccs: List[str]):
         """
         Prune any compute capabilities that are not compatible with the builder. Should log
         which CCs have been pruned.
         """
@@ -590,14 +611,17 @@
         else:
             from torch.utils.cpp_extension import CUDAExtension as ExtensionBuilder
 
         compile_args = {'cxx': self.strip_empty_entries(self.cxx_args())} if self.build_for_cpu else \
                        {'cxx': self.strip_empty_entries(self.cxx_args()), \
                            'nvcc': self.strip_empty_entries(self.nvcc_args())}
 
+        if not self.build_for_cpu and self.enable_bf16:
+            compile_args['cxx'].append("-DBF16_AVAILABLE")
+
         cuda_ext = ExtensionBuilder(name=self.absolute_name(),
                                     sources=self.strip_empty_entries(self.sources()),
                                     include_dirs=self.strip_empty_entries(self.include_paths()),
                                     libraries=self.strip_empty_entries(self.libraries_args()),
                                     extra_compile_args=compile_args)
 
         if self.is_rocm_pytorch():
@@ -627,34 +651,34 @@
                 hipify_extra_files_only=True,
             )
 
     def cxx_args(self):
         if sys.platform == "win32":
             return ['-O2']
         else:
-            return ['-O3', '-std=c++14', '-g', '-Wno-reorder']
+            return ['-O3', '-std=c++17', '-g', '-Wno-reorder']
 
     def nvcc_args(self):
         if self.build_for_cpu:
             return []
         args = ['-O3']
         if self.is_rocm_pytorch():
             ROCM_MAJOR, ROCM_MINOR = self.installed_rocm_version()
             args += [
-                '-std=c++14', '-U__HIP_NO_HALF_OPERATORS__', '-U__HIP_NO_HALF_CONVERSIONS__',
+                '-std=c++17', '-U__HIP_NO_HALF_OPERATORS__', '-U__HIP_NO_HALF_CONVERSIONS__',
                 '-U__HIP_NO_HALF2_OPERATORS__',
                 '-DROCM_VERSION_MAJOR=%s' % ROCM_MAJOR,
                 '-DROCM_VERSION_MINOR=%s' % ROCM_MINOR
             ]
         else:
             cuda_major, _ = installed_cuda_version()
             args += [
                 '-allow-unsupported-compiler' if sys.platform == "win32" else '', '--use_fast_math',
-                '-std=c++17' if sys.platform == "win32" and cuda_major > 10 else '-std=c++14',
-                '-U__CUDA_NO_HALF_OPERATORS__', '-U__CUDA_NO_HALF_CONVERSIONS__', '-U__CUDA_NO_HALF2_OPERATORS__'
+                '-std=c++17' if cuda_major > 10 else '-std=c++14', '-U__CUDA_NO_HALF_OPERATORS__',
+                '-U__CUDA_NO_HALF_CONVERSIONS__', '-U__CUDA_NO_HALF2_OPERATORS__'
             ]
             if os.environ.get('DS_DEBUG_CUDA_BUILD', '0') == '1':
                 args.append('--ptxas-options=-v')
             args += self.compute_capability_args()
         return args
 
     def libraries_args(self):
```

### Comparing `deepspeed-0.9.2/op_builder/cpu_adagrad.py` & `deepspeed-0.9.3/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/cpu_adam.py` & `deepspeed-0.9.3/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/fused_adam.py` & `deepspeed-0.9.3/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/fused_lamb.py` & `deepspeed-0.9.3/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/quantizer.py` & `deepspeed-0.9.3/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/random_ltd.py` & `deepspeed-0.9.3/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/sparse_attn.py` & `deepspeed-0.9.3/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/spatial_inference.py` & `deepspeed-0.9.3/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/stochastic_transformer.py` & `deepspeed-0.9.3/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/transformer.py` & `deepspeed-0.9.3/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.2/op_builder/transformer_inference.py` & `deepspeed-0.9.3/op_builder/transformer_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,18 +52,20 @@
 
     def sources(self):
         return [
             'csrc/transformer/inference/csrc/pt_binding.cpp',
             'csrc/transformer/inference/csrc/gelu.cu',
             'csrc/transformer/inference/csrc/relu.cu',
             'csrc/transformer/inference/csrc/layer_norm.cu',
+            'csrc/transformer/inference/csrc/rms_norm.cu',
             'csrc/transformer/inference/csrc/softmax.cu',
             'csrc/transformer/inference/csrc/dequantize.cu',
             'csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu',
             'csrc/transformer/inference/csrc/transform.cu',
+            'csrc/transformer/inference/csrc/pointwise_ops.cu',
         ]
 
     def extra_ldflags(self):
         if not self.is_rocm_pytorch():
             return ['-lcurand']
         else:
             return []
```

### Comparing `deepspeed-0.9.2/setup.py` & `deepspeed-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     '1bit': [],  # add cupy based on cuda/rocm version
     '1bit_mpi': fetch_requirements('requirements/requirements-1bit-mpi.txt'),
     'readthedocs': fetch_requirements('requirements/requirements-readthedocs.txt'),
     'dev': fetch_requirements('requirements/requirements-dev.txt'),
     'autotuning': fetch_requirements('requirements/requirements-autotuning.txt'),
     'autotuning_ml': fetch_requirements('requirements/requirements-autotuning-ml.txt'),
     'sparse_attn': fetch_requirements('requirements/requirements-sparse_attn.txt'),
+    'sparse': fetch_requirements('requirements/requirements-sparse_pruning.txt'),
     'inf': fetch_requirements('requirements/requirements-inf.txt'),
     'sd': fetch_requirements('requirements/requirements-sd.txt')
 }
 
 # Add specific cupy version to both onebit extension variants.
 if torch_available and torch.cuda.is_available():
     cupy = None
@@ -294,13 +295,13 @@
           'bin/ds_elastic'
       ],
       classifiers=[
           'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10'
       ],
-      license='MIT',
+      license='Apache Software License 2.0',
       ext_modules=ext_modules,
       cmdclass=cmdclass)
 
 end_time = time.time()
 print(f'deepspeed build time = {end_time - start_time} secs')
```

