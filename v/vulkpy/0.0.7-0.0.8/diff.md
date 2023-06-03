# Comparing `tmp/vulkpy-0.0.7.tar.gz` & `tmp/vulkpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulkpy-0.0.7.tar", last modified: Sun Mar 12 09:34:45 2023, max compression
+gzip compressed data, was "vulkpy-0.0.8.tar", last modified: Sat Jun  3 05:15:47 2023, max compression
```

## Comparing `vulkpy-0.0.7.tar` & `vulkpy-0.0.8.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 09:34:45.653705 vulkpy-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-12 09:33:37.000000 vulkpy-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-12 09:33:37.000000 vulkpy-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4264 2023-03-12 09:34:45.653705 vulkpy-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3694 2023-03-12 09:33:37.000000 vulkpy-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       62 2023-03-12 09:33:37.000000 vulkpy-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 09:34:45.653705 vulkpy-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4330 2023-03-12 09:33:37.000000 vulkpy-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 09:34:45.561701 vulkpy-0.0.7/vulkpy/
--rw-r--r--   0 root         (0) root         (0)      519 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27783 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/_vkarray.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 09:34:45.573702 vulkpy-0.0.7/vulkpy/nn/
--rw-r--r--   0 root         (0) root         (0)      974 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/core.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/initializers.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/layers.py
--rw-r--r--   0 root         (0) root         (0)    10818 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/losses.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/models.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/optimizers.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/parameters.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/nn/regularizers.py
--rw-r--r--   0 root         (0) root         (0)     9975 2023-03-12 09:33:37.000000 vulkpy-0.0.7/vulkpy/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 09:34:45.653705 vulkpy-0.0.7/vulkpy/shader/
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:28.000000 vulkpy-0.0.7/vulkpy/shader/abs.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/acos.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:32.000000 vulkpy-0.0.7/vulkpy/shader/acosh.spv
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-12 09:34:19.000000 vulkpy-0.0.7/vulkpy/shader/add.spv
--rw-r--r--   0 root         (0) root         (0)     3596 2023-03-12 09:34:23.000000 vulkpy-0.0.7/vulkpy/shader/add_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:21.000000 vulkpy-0.0.7/vulkpy/shader/add_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/asin.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:32.000000 vulkpy-0.0.7/vulkpy/shader/asinh.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:30.000000 vulkpy-0.0.7/vulkpy/shader/atan.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:32.000000 vulkpy-0.0.7/vulkpy/shader/atanh.spv
--rw-r--r--   0 root         (0) root         (0)     3120 2023-03-12 09:34:44.000000 vulkpy-0.0.7/vulkpy/shader/batch_affine.spv
--rw-r--r--   0 root         (0) root         (0)     3024 2023-03-12 09:34:43.000000 vulkpy-0.0.7/vulkpy/shader/broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1932 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/clamp.spv
--rw-r--r--   0 root         (0) root         (0)     1640 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/clamp_ss.spv
--rw-r--r--   0 root         (0) root         (0)     1796 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/clamp_sv.spv
--rw-r--r--   0 root         (0) root         (0)     1796 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/clamp_vs.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/cos.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:32.000000 vulkpy-0.0.7/vulkpy/shader/cosh.spv
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-12 09:34:20.000000 vulkpy-0.0.7/vulkpy/shader/div.spv
--rw-r--r--   0 root         (0) root         (0)     3596 2023-03-12 09:34:24.000000 vulkpy-0.0.7/vulkpy/shader/div_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:22.000000 vulkpy-0.0.7/vulkpy/shader/div_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:34.000000 vulkpy-0.0.7/vulkpy/shader/exp.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:34.000000 vulkpy-0.0.7/vulkpy/shader/exp2.spv
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-12 09:34:44.000000 vulkpy-0.0.7/vulkpy/shader/gather.spv
--rw-r--r--   0 root         (0) root         (0)     3076 2023-03-12 09:34:44.000000 vulkpy-0.0.7/vulkpy/shader/gather_axis.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:28.000000 vulkpy-0.0.7/vulkpy/shader/iabs.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:31.000000 vulkpy-0.0.7/vulkpy/shader/iacos.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/iacosh.spv
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-12 09:34:20.000000 vulkpy-0.0.7/vulkpy/shader/iadd.spv
--rw-r--r--   0 root         (0) root         (0)     3004 2023-03-12 09:34:24.000000 vulkpy-0.0.7/vulkpy/shader/iadd_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-12 09:34:22.000000 vulkpy-0.0.7/vulkpy/shader/iadd_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:31.000000 vulkpy-0.0.7/vulkpy/shader/iasin.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/iasinh.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:31.000000 vulkpy-0.0.7/vulkpy/shader/iatan.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/iatanh.spv
--rw-r--r--   0 root         (0) root         (0)     1724 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/iclamp.spv
--rw-r--r--   0 root         (0) root         (0)     1432 2023-03-12 09:34:39.000000 vulkpy-0.0.7/vulkpy/shader/iclamp_ss.spv
--rw-r--r--   0 root         (0) root         (0)     1588 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/iclamp_sv.spv
--rw-r--r--   0 root         (0) root         (0)     1588 2023-03-12 09:34:39.000000 vulkpy-0.0.7/vulkpy/shader/iclamp_vs.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:30.000000 vulkpy-0.0.7/vulkpy/shader/icos.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/icosh.spv
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-12 09:34:21.000000 vulkpy-0.0.7/vulkpy/shader/idiv.spv
--rw-r--r--   0 root         (0) root         (0)     3004 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/idiv_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-12 09:34:23.000000 vulkpy-0.0.7/vulkpy/shader/idiv_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:35.000000 vulkpy-0.0.7/vulkpy/shader/iexp.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:35.000000 vulkpy-0.0.7/vulkpy/shader/iexp2.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:36.000000 vulkpy-0.0.7/vulkpy/shader/iinvsqrt.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:35.000000 vulkpy-0.0.7/vulkpy/shader/ilog.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:35.000000 vulkpy-0.0.7/vulkpy/shader/ilog2.spv
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/imax.spv
--rw-r--r--   0 root         (0) root         (0)     3028 2023-03-12 09:34:27.000000 vulkpy-0.0.7/vulkpy/shader/imax_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1336 2023-03-12 09:34:26.000000 vulkpy-0.0.7/vulkpy/shader/imax_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-12 09:34:26.000000 vulkpy-0.0.7/vulkpy/shader/imin.spv
--rw-r--r--   0 root         (0) root         (0)     3028 2023-03-12 09:34:28.000000 vulkpy-0.0.7/vulkpy/shader/imin_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1336 2023-03-12 09:34:27.000000 vulkpy-0.0.7/vulkpy/shader/imin_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-12 09:34:21.000000 vulkpy-0.0.7/vulkpy/shader/imul.spv
--rw-r--r--   0 root         (0) root         (0)     3004 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/imul_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-12 09:34:22.000000 vulkpy-0.0.7/vulkpy/shader/imul_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:36.000000 vulkpy-0.0.7/vulkpy/shader/invsqrt.spv
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-12 09:34:36.000000 vulkpy-0.0.7/vulkpy/shader/ipow.spv
--rw-r--r--   0 root         (0) root         (0)     3028 2023-03-12 09:34:38.000000 vulkpy-0.0.7/vulkpy/shader/ipow_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1336 2023-03-12 09:34:37.000000 vulkpy-0.0.7/vulkpy/shader/ipow_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/isign.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:30.000000 vulkpy-0.0.7/vulkpy/shader/isin.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/isinh.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:36.000000 vulkpy-0.0.7/vulkpy/shader/isqrt.spv
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-12 09:34:20.000000 vulkpy-0.0.7/vulkpy/shader/isub.spv
--rw-r--r--   0 root         (0) root         (0)     3004 2023-03-12 09:34:24.000000 vulkpy-0.0.7/vulkpy/shader/isub_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-12 09:34:22.000000 vulkpy-0.0.7/vulkpy/shader/isub_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:30.000000 vulkpy-0.0.7/vulkpy/shader/itan.spv
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-12 09:34:33.000000 vulkpy-0.0.7/vulkpy/shader/itanh.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:34.000000 vulkpy-0.0.7/vulkpy/shader/log.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:34.000000 vulkpy-0.0.7/vulkpy/shader/log2.spv
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/matmul.spv
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/max.spv
--rw-r--r--   0 root         (0) root         (0)     3604 2023-03-12 09:34:27.000000 vulkpy-0.0.7/vulkpy/shader/max_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1544 2023-03-12 09:34:26.000000 vulkpy-0.0.7/vulkpy/shader/max_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     2084 2023-03-12 09:34:42.000000 vulkpy-0.0.7/vulkpy/shader/maximum.spv
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-12 09:34:42.000000 vulkpy-0.0.7/vulkpy/shader/maximum_axis.spv
--rw-r--r--   0 root         (0) root         (0)     2888 2023-03-12 09:34:43.000000 vulkpy-0.0.7/vulkpy/shader/maximum_axis_rebroadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-12 09:34:42.000000 vulkpy-0.0.7/vulkpy/shader/maximum_v1.3.spv
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-12 09:34:25.000000 vulkpy-0.0.7/vulkpy/shader/min.spv
--rw-r--r--   0 root         (0) root         (0)     3604 2023-03-12 09:34:27.000000 vulkpy-0.0.7/vulkpy/shader/min_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1544 2023-03-12 09:34:26.000000 vulkpy-0.0.7/vulkpy/shader/min_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     2084 2023-03-12 09:34:42.000000 vulkpy-0.0.7/vulkpy/shader/minimum.spv
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-12 09:34:43.000000 vulkpy-0.0.7/vulkpy/shader/minimum_axis.spv
--rw-r--r--   0 root         (0) root         (0)     2888 2023-03-12 09:34:43.000000 vulkpy-0.0.7/vulkpy/shader/minimum_axis_rebroadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-12 09:34:43.000000 vulkpy-0.0.7/vulkpy/shader/minimum_v1.3.spv
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-12 09:34:20.000000 vulkpy-0.0.7/vulkpy/shader/mul.spv
--rw-r--r--   0 root         (0) root         (0)     3596 2023-03-12 09:34:24.000000 vulkpy-0.0.7/vulkpy/shader/mul_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:22.000000 vulkpy-0.0.7/vulkpy/shader/mul_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1752 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy/shader/nn_cross_entropy.spv
--rw-r--r--   0 root         (0) root         (0)     1724 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy/shader/nn_cross_entropy_backward.spv
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-12 09:34:36.000000 vulkpy-0.0.7/vulkpy/shader/pow.spv
--rw-r--r--   0 root         (0) root         (0)     3604 2023-03-12 09:34:37.000000 vulkpy-0.0.7/vulkpy/shader/pow_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1544 2023-03-12 09:34:37.000000 vulkpy-0.0.7/vulkpy/shader/pow_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-12 09:34:39.000000 vulkpy-0.0.7/vulkpy/shader/prng_box_muller.spv
--rw-r--r--   0 root         (0) root         (0)     2168 2023-03-12 09:34:40.000000 vulkpy-0.0.7/vulkpy/shader/prng_ibox_muller.spv
--rw-r--r--   0 root         (0) root         (0)     1816 2023-03-12 09:34:40.000000 vulkpy-0.0.7/vulkpy/shader/prng_randrange.spv
--rw-r--r--   0 root         (0) root         (0)     3848 2023-03-12 09:34:39.000000 vulkpy-0.0.7/vulkpy/shader/prng_xoshiro128pp_float.spv
--rw-r--r--   0 root         (0) root         (0)     3652 2023-03-12 09:34:39.000000 vulkpy-0.0.7/vulkpy/shader/prng_xoshiro128pp_uint32.spv
--rw-r--r--   0 root         (0) root         (0)     2040 2023-03-12 09:34:41.000000 vulkpy-0.0.7/vulkpy/shader/prod.spv
--rw-r--r--   0 root         (0) root         (0)     2580 2023-03-12 09:34:41.000000 vulkpy-0.0.7/vulkpy/shader/prod_axis.spv
--rw-r--r--   0 root         (0) root         (0)     2844 2023-03-12 09:34:41.000000 vulkpy-0.0.7/vulkpy/shader/prod_axis_rebroadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1748 2023-03-12 09:34:41.000000 vulkpy-0.0.7/vulkpy/shader/prod_v1.3.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:23.000000 vulkpy-0.0.7/vulkpy/shader/rdiv_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1544 2023-03-12 09:34:37.000000 vulkpy-0.0.7/vulkpy/shader/rpow_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:23.000000 vulkpy-0.0.7/vulkpy/shader/rsub_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:28.000000 vulkpy-0.0.7/vulkpy/shader/sign.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/sin.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:31.000000 vulkpy-0.0.7/vulkpy/shader/sinh.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:35.000000 vulkpy-0.0.7/vulkpy/shader/sqrt.spv
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-12 09:34:20.000000 vulkpy-0.0.7/vulkpy/shader/sub.spv
--rw-r--r--   0 root         (0) root         (0)     3596 2023-03-12 09:34:23.000000 vulkpy-0.0.7/vulkpy/shader/sub_broadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-12 09:34:21.000000 vulkpy-0.0.7/vulkpy/shader/sub_scalar.spv
--rw-r--r--   0 root         (0) root         (0)     2036 2023-03-12 09:34:40.000000 vulkpy-0.0.7/vulkpy/shader/sum.spv
--rw-r--r--   0 root         (0) root         (0)     2576 2023-03-12 09:34:40.000000 vulkpy-0.0.7/vulkpy/shader/sum_axis.spv
--rw-r--r--   0 root         (0) root         (0)     2840 2023-03-12 09:34:41.000000 vulkpy-0.0.7/vulkpy/shader/sum_axis_rebroadcast.spv
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-12 09:34:40.000000 vulkpy-0.0.7/vulkpy/shader/sum_v1.3.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:29.000000 vulkpy-0.0.7/vulkpy/shader/tan.spv
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-12 09:34:32.000000 vulkpy-0.0.7/vulkpy/shader/tanh.spv
--rw-r--r--   0 root         (0) root         (0)     1701 2023-03-12 09:33:38.000000 vulkpy-0.0.7/vulkpy/util.py
--rw-r--r--   0 root         (0) root         (0)    44889 2023-03-12 09:33:38.000000 vulkpy-0.0.7/vulkpy/vkarray.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-03-12 09:33:38.000000 vulkpy-0.0.7/vulkpy/vktyping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 09:34:45.565701 vulkpy-0.0.7/vulkpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4264 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3837 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-12 09:34:45.000000 vulkpy-0.0.7/vulkpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 05:15:47.531827 vulkpy-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-03 05:14:46.000000 vulkpy-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-03 05:14:46.000000 vulkpy-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-03 05:15:47.531827 vulkpy-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-06-03 05:14:46.000000 vulkpy-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-03 05:14:46.000000 vulkpy-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 05:15:47.531827 vulkpy-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-06-03 05:14:46.000000 vulkpy-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 05:15:47.439825 vulkpy-0.0.8/vulkpy/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28364 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/_vkarray.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 05:15:47.447825 vulkpy-0.0.8/vulkpy/nn/
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/core.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/initializers.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/layers.py
+-rw-r--r--   0 root         (0) root         (0)    10876 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/losses.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/models.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/optimizers.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/parameters.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/nn/regularizers.py
+-rw-r--r--   0 root         (0) root         (0)     9975 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 05:15:47.531827 vulkpy-0.0.8/vulkpy/shader/
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:29.000000 vulkpy-0.0.8/vulkpy/shader/abs.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/acos.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:33.000000 vulkpy-0.0.8/vulkpy/shader/acosh.spv
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-03 05:15:22.000000 vulkpy-0.0.8/vulkpy/shader/add.spv
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-03 05:15:26.000000 vulkpy-0.0.8/vulkpy/shader/add_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:24.000000 vulkpy-0.0.8/vulkpy/shader/add_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/asin.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:33.000000 vulkpy-0.0.8/vulkpy/shader/asinh.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/atan.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:33.000000 vulkpy-0.0.8/vulkpy/shader/atanh.spv
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-03 05:15:46.000000 vulkpy-0.0.8/vulkpy/shader/batch_affine.spv
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-06-03 05:15:46.000000 vulkpy-0.0.8/vulkpy/shader/broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-06-03 05:15:39.000000 vulkpy-0.0.8/vulkpy/shader/clamp.spv
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-03 05:15:40.000000 vulkpy-0.0.8/vulkpy/shader/clamp_ss.spv
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-06-03 05:15:39.000000 vulkpy-0.0.8/vulkpy/shader/clamp_sv.spv
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-06-03 05:15:39.000000 vulkpy-0.0.8/vulkpy/shader/clamp_vs.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/cos.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:32.000000 vulkpy-0.0.8/vulkpy/shader/cosh.spv
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/div.spv
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-03 05:15:26.000000 vulkpy-0.0.8/vulkpy/shader/div_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:24.000000 vulkpy-0.0.8/vulkpy/shader/div_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:35.000000 vulkpy-0.0.8/vulkpy/shader/exp.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:35.000000 vulkpy-0.0.8/vulkpy/shader/exp2.spv
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-03 05:15:46.000000 vulkpy-0.0.8/vulkpy/shader/gather.spv
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-06-03 05:15:46.000000 vulkpy-0.0.8/vulkpy/shader/gather_axis.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/iabs.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:32.000000 vulkpy-0.0.8/vulkpy/shader/iacos.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:34.000000 vulkpy-0.0.8/vulkpy/shader/iacosh.spv
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/iadd.spv
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-06-03 05:15:26.000000 vulkpy-0.0.8/vulkpy/shader/iadd_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/iadd_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/iasin.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:34.000000 vulkpy-0.0.8/vulkpy/shader/iasinh.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:32.000000 vulkpy-0.0.8/vulkpy/shader/iatan.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:35.000000 vulkpy-0.0.8/vulkpy/shader/iatanh.spv
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-06-03 05:15:40.000000 vulkpy-0.0.8/vulkpy/shader/iclamp.spv
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-06-03 05:15:41.000000 vulkpy-0.0.8/vulkpy/shader/iclamp_ss.spv
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-03 05:15:40.000000 vulkpy-0.0.8/vulkpy/shader/iclamp_sv.spv
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-03 05:15:40.000000 vulkpy-0.0.8/vulkpy/shader/iclamp_vs.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/icos.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:34.000000 vulkpy-0.0.8/vulkpy/shader/icosh.spv
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-03 05:15:24.000000 vulkpy-0.0.8/vulkpy/shader/idiv.spv
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/idiv_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/idiv_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:36.000000 vulkpy-0.0.8/vulkpy/shader/iexp.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:36.000000 vulkpy-0.0.8/vulkpy/shader/iexp2.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:37.000000 vulkpy-0.0.8/vulkpy/shader/iinvsqrt.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:36.000000 vulkpy-0.0.8/vulkpy/shader/ilog.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:36.000000 vulkpy-0.0.8/vulkpy/shader/ilog2.spv
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/imax.spv
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-03 05:15:29.000000 vulkpy-0.0.8/vulkpy/shader/imax_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/imax_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/imin.spv
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-03 05:15:29.000000 vulkpy-0.0.8/vulkpy/shader/imin_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/imin_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/imul.spv
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/imul_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/imul_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:37.000000 vulkpy-0.0.8/vulkpy/shader/invsqrt.spv
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/ipow.spv
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-03 05:15:39.000000 vulkpy-0.0.8/vulkpy/shader/ipow_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/ipow_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/isign.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/isin.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:33.000000 vulkpy-0.0.8/vulkpy/shader/isinh.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:37.000000 vulkpy-0.0.8/vulkpy/shader/isqrt.spv
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/isub.spv
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/isub_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/isub_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:31.000000 vulkpy-0.0.8/vulkpy/shader/itan.spv
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-03 05:15:34.000000 vulkpy-0.0.8/vulkpy/shader/itanh.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:35.000000 vulkpy-0.0.8/vulkpy/shader/log.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:36.000000 vulkpy-0.0.8/vulkpy/shader/log2.spv
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/matmul.spv
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/max.spv
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/max_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/max_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-06-03 05:15:44.000000 vulkpy-0.0.8/vulkpy/shader/maximum.spv
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-06-03 05:15:44.000000 vulkpy-0.0.8/vulkpy/shader/maximum_axis.spv
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-03 05:15:45.000000 vulkpy-0.0.8/vulkpy/shader/maximum_axis_rebroadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-06-03 05:15:44.000000 vulkpy-0.0.8/vulkpy/shader/maximum_v1.3.spv
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-03 05:15:27.000000 vulkpy-0.0.8/vulkpy/shader/min.spv
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-06-03 05:15:29.000000 vulkpy-0.0.8/vulkpy/shader/min_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-03 05:15:28.000000 vulkpy-0.0.8/vulkpy/shader/min_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-06-03 05:15:45.000000 vulkpy-0.0.8/vulkpy/shader/minimum.spv
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-06-03 05:15:45.000000 vulkpy-0.0.8/vulkpy/shader/minimum_axis.spv
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-03 05:15:46.000000 vulkpy-0.0.8/vulkpy/shader/minimum_axis_rebroadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-06-03 05:15:45.000000 vulkpy-0.0.8/vulkpy/shader/minimum_v1.3.spv
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/mul.spv
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-03 05:15:26.000000 vulkpy-0.0.8/vulkpy/shader/mul_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:24.000000 vulkpy-0.0.8/vulkpy/shader/mul_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy/shader/nn_cross_entropy.spv
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy/shader/nn_cross_entropy_backward.spv
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/pow.spv
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/pow_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/pow_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-06-03 05:15:41.000000 vulkpy-0.0.8/vulkpy/shader/prng_box_muller.spv
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-03 05:15:41.000000 vulkpy-0.0.8/vulkpy/shader/prng_ibox_muller.spv
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-06-03 05:15:42.000000 vulkpy-0.0.8/vulkpy/shader/prng_randrange.spv
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-06-03 05:15:41.000000 vulkpy-0.0.8/vulkpy/shader/prng_xoshiro128pp_float.spv
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-06-03 05:15:41.000000 vulkpy-0.0.8/vulkpy/shader/prng_xoshiro128pp_uint32.spv
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-03 05:15:43.000000 vulkpy-0.0.8/vulkpy/shader/prod.spv
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-06-03 05:15:43.000000 vulkpy-0.0.8/vulkpy/shader/prod_axis.spv
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-06-03 05:15:44.000000 vulkpy-0.0.8/vulkpy/shader/prod_axis_rebroadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-03 05:15:43.000000 vulkpy-0.0.8/vulkpy/shader/prod_v1.3.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/rdiv_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-03 05:15:38.000000 vulkpy-0.0.8/vulkpy/shader/rpow_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:25.000000 vulkpy-0.0.8/vulkpy/shader/rsub_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/sign.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/sin.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:32.000000 vulkpy-0.0.8/vulkpy/shader/sinh.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:37.000000 vulkpy-0.0.8/vulkpy/shader/sqrt.spv
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-03 05:15:23.000000 vulkpy-0.0.8/vulkpy/shader/sub.spv
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-06-03 05:15:26.000000 vulkpy-0.0.8/vulkpy/shader/sub_broadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-03 05:15:24.000000 vulkpy-0.0.8/vulkpy/shader/sub_scalar.spv
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-06-03 05:15:42.000000 vulkpy-0.0.8/vulkpy/shader/sum.spv
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-06-03 05:15:42.000000 vulkpy-0.0.8/vulkpy/shader/sum_axis.spv
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-03 05:15:43.000000 vulkpy-0.0.8/vulkpy/shader/sum_axis_rebroadcast.spv
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-06-03 05:15:42.000000 vulkpy-0.0.8/vulkpy/shader/sum_v1.3.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:30.000000 vulkpy-0.0.8/vulkpy/shader/tan.spv
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-03 05:15:33.000000 vulkpy-0.0.8/vulkpy/shader/tanh.spv
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/util.py
+-rw-r--r--   0 root         (0) root         (0)    45911 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/vkarray.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-03 05:14:46.000000 vulkpy-0.0.8/vulkpy/vktyping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 05:15:47.443825 vulkpy-0.0.8/vulkpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-03 05:15:47.000000 vulkpy-0.0.8/vulkpy.egg-info/top_level.txt
```

### Comparing `vulkpy-0.0.7/LICENSE` & `vulkpy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/PKG-INFO` & `vulkpy-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulkpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: GPGPU array on Vulkan
 Home-page: https://github.com/ymd-h/vulkpy
 Author: H. Yamada
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -106,16 +106,16 @@
     * Gaussian with Box-Muller (`.normal(shape=None, buffer=None, mean=0.0, stddev=1.0)`)
   * [ ] pcg32
 * Neural Network
   * Layers
     * [x] `Dense`, `ReLU`, `Sigmoid`, `Softmax`
     * [ ] conv, batch norm, layer norm, ...
   * Optimizers
-    * [x] `SGD`, `Adam`
-    * [ ] rmsprop, adagrad, ...
+    * [x] `SGD`, `Adam`, `AdaGrad`
+    * [ ] rmsprop, ...
   * Losses
     * [x] `CrossEntropyLoss`, `SoftmaxCrossEntropyLoss`, `MSELoss`, `HuberLoss`
     * [ ] ...
   * Initializers
     * [x] `Constant`, `HeNormal`
     * [ ] ...
   * Models
```

### Comparing `vulkpy-0.0.7/README.md` & `vulkpy-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     * Gaussian with Box-Muller (`.normal(shape=None, buffer=None, mean=0.0, stddev=1.0)`)
   * [ ] pcg32
 * Neural Network
   * Layers
     * [x] `Dense`, `ReLU`, `Sigmoid`, `Softmax`
     * [ ] conv, batch norm, layer norm, ...
   * Optimizers
-    * [x] `SGD`, `Adam`
-    * [ ] rmsprop, adagrad, ...
+    * [x] `SGD`, `Adam`, `AdaGrad`
+    * [ ] rmsprop, ...
   * Losses
     * [x] `CrossEntropyLoss`, `SoftmaxCrossEntropyLoss`, `MSELoss`, `HuberLoss`
     * [ ] ...
   * Initializers
     * [x] `Constant`, `HeNormal`
     * [ ] ...
   * Models
```

### Comparing `vulkpy-0.0.7/setup.py` & `vulkpy-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 README = "README.md"
 if os.path.exists(README):
     with open(README) as f:
         desc["long_description"] = f.read()
         desc["long_description_content_type"] = "text/markdown"
 
 setup(name="vulkpy",
-      version="0.0.7",
+      version="0.0.8",
       author="H. Yamada",
       description="GPGPU array on Vulkan",
       **desc,
       url="https://github.com/ymd-h/vulkpy",
       packages=find_packages(),
       ext_modules=ext,
       include_package_data=True,
```

### Comparing `vulkpy-0.0.7/vulkpy/_vkarray.cc` & `vulkpy-0.0.8/vulkpy/_vkarray.cc`

 * *Files 2% similar despite different names*

```diff
@@ -466,15 +466,26 @@
   vk::DeviceQueueCreateInfo queueInfo;
   vk::DeviceCreateInfo deviceInfo;
   vk::UniqueDevice device;
   vk::Queue queue;
   std::unordered_map<std::string_view, OpVariant_t> opMap;
 public:
   GPU(std::size_t id, float priority = 0.0f): priority(priority) {
+#if defined(__APPLE__)
+    std::vector<const char *> extensionNames;
+    extensionNames.push_back(VK_KHR_GET_PHYSICAL_DEVICE_PROPERTIES_2_EXTENSION_NAME);
+    extensionNames.push_back(VK_KHR_PORTABILITY_ENUMERATION_EXTENSION_NAME);
+    vk::InstanceCreateInfo instanceInfo{};
+    instanceInfo.flags = vk::InstanceCreateFlagBits::eEnumeratePortabilityKHR;
+    instanceInfo.enabledExtensionCount = static_cast<uint32_t>(extensionNames.size());
+    instanceInfo.ppEnabledExtensionNames = extensionNames.data();
+    this->instance = vk::createInstanceUnique(instanceInfo);
+#else
     this->instance = vk::createInstanceUnique(vk::InstanceCreateInfo{});
+#endif
     this->physical = this->instance->enumeratePhysicalDevices()[id];
 
     this->queueFamilyIndex = this->findQueueFamilyIndex(vk::QueueFlagBits::eCompute);
 
     this->queueInfo = vk::DeviceQueueCreateInfo{
       .queueFamilyIndex=this->queueFamilyIndex,
       .queueCount=1,
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/__init__.py` & `vulkpy-0.0.8/vulkpy/nn/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,16 +28,27 @@
 >>> pred_y, loss = net.train(x, y)
 
 Predict with Model
 
 >>> pred_y = net.predict(x)
 """
 
+from .core import (
+    Optimizer,
+    OptimizerState,
+    Loss,
+    Regularizer,
+    Module,
+)
 from .initializers import Constant, HeNormal
-from .optimizers import SGD, Adam
+from .optimizers import (
+    SGD, SGDState,
+    Adam, AdamState,
+    AdaGrad, AdaGradState,
+)
 from .layers import Dense, ReLU, Sigmoid, Softmax
 from .losses import (
     CrossEntropyLoss,
     SoftmaxCrossEntropyLoss,
     MSELoss,
     HuberLoss,
 )
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/core.py` & `vulkpy-0.0.8/vulkpy/nn/initializers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,89 @@
+"""
+Neural Network Initializer Module (:mod:`vulkpy.nn.initializers`)
+=================================================================
+"""
 from __future__ import annotations
-from typing import Iterable
+from typing import Iterable, Optional
 
-from vulkpy.vkarray import GPU, Array
-
-
-__all__ = [
-    "OptimizerState",
-    "Optimizer",
-    "Module",
-    "Loss",
-]
-
-
-class OptimizerState:
-    def grad2diff(self, grad: Array) -> Array:
-        raise NotImplementedError
+import numpy as np
 
-class Optimizer:
-    def init_state(self, shape: Iterable[int]) -> OptimizerState:
-        raise NotImplementedError
+from vulkpy.vkarray import GPU, Array
+from vulkpy.random import Xoshiro128pp
 
-class Loss:
-    def __call__(self, x: Array, y: Array) -> Array:
-        raise NotImplementedError
 
-    def grad(self) -> Array:
-        raise NotImplementedError
+__all__ = ["Constant", "HeNormal"]
 
-class Regularizer:
-    def loss(self, param: Array) -> Array:
+class Initializer:
+    def __call__(self, gpu: GPU, shape: Iterable[int]) -> Array:
         raise NotImplementedError
 
-    def grad(self, param: Array) -> Array:
-        raise NotImplementedError
 
+class Constant(Initializer):
+    """
+    Constant Initializer
+    """
+    def __init__(self, value: float):
+        """
+        Initialize Constant Initializer
 
-class Module:
-    def __init__(self):
-        pass
+        Parameters
+        ----------
+        value : float
+            Constant value
+        """
+        self.value = value
 
-    def __call__(self, x: Array) -> Array:
+    def __call__(self, gpu: GPU, shape: Iterable[int]) -> Array:
         """
-        Call Module
+        Initialize new parameters
 
         Parameters
         ----------
-        x : vulkpy.Array
-            Input
+        gpu : vulkpy.GPU
+            GPU
+        shape : iterable of ints
+            Parameter shape
+        """
+        p = Array(gpu, shape=shape)
+        p[:] = self.value
+        return p
 
-        Returns
-        -------
-        y : vulkpy.Array
-            Output
-
-        Raises
-        ------
-        ValueError
-            If input (``x``) shape doesn't have at least 2-dimensions.
-
-        Notes
-        -----
-        This function stores input (``x``) and output (``y``) for training.
-        """
-        if len(x.shape) < 2:
-            raise ValueError("Input must have at least 2-dimensions.")
-
-        self._x = x
-        self._y = self.forward(x)
-        return self._y
 
-    def forward(self, x: Array) -> Array:
-        raise NotImplementedError
+class HeNormal(Initializer):
+    r"""
+    He Normal Initializer
 
-    def backward(self, dy: Array) -> Array:
-        raise NotImplementedError
+    Note
+    ----
+    Standard deviation :math:`\sigma` is following;
 
-    def zero_grad(self):
+    .. math:: \sigma = \sqrt{2/d_{\text{in}}}
+    """
+    def __init__(self, gpu: GPU, input_dim: int, *, seed: Optional[int] = None):
         """
-        Reset accumulated gradients to 0.
+        Initialize He Normal Initializer
+
+        Parameters
+        ----------
+        gpu : vulkpy.GPU
+            GPU
+        input_dim : int
+            Input dimension
+        seed : int, optional
+            Initial seed for PRNG
         """
-        pass
+        self.rng = Xoshiro128pp(gpu, seed=seed)
+        self.stddev = np.sqrt(2 / input_dim)
 
-    def update(self):
+    def __call__(self, gpu: GPU, shape: Iterable[int]):
         """
-        Update parameters based on accumulated gradients
+        Initialize new parameters
+
+        Parameters
+        ----------
+        gpu : vulkpy.GPU
+            GPU
+        shape : iterable of ints
+            Parameter shape
         """
-        pass
+        return self.rng.normal(shape=shape, stddev=self.stddev)
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/layers.py` & `vulkpy-0.0.8/vulkpy/nn/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 
 __all__ = ["Dense", "ReLU", "Sigmoid", "Softmax"]
 
 
 class Dense(Module):
     """
-    Dense
+    Fully connected Dense Layer
     """
+
     _batch_affine = getShader("batch_affine.spv")
 
     def __init__(self, gpu: GPU, input_dim: int, output_dim: int, *,
                  w_init: Optional[Callable[[GPU, Iterable[int]], Array]] = None,
                  b_init: Optional[Callable[[GPU, Iterable[int]], Array]] = None,
                  w_opt: Optional[Optimizer] = None,
                  b_opt: Optional[Optimizer] = None,
@@ -114,15 +115,15 @@
         vulkpy.Array
             Batch grad
 
         Notes
         -----
         .. math::
 
-            dx = dy @ W\\
+            dx = dy W\\
             dW = dy ^T \cdot x\\
             db = dy
         """
         db = dy.sum(axis=0) # Allocate
         self.b.add_grad(db)
 
         x_shape = self._x.shape
@@ -195,15 +196,15 @@
         Returns
         -------
         vulkpy.Array
             Batch grad
 
         Notes
         -----
-        .. math:: dx = dy \times \max(sign(y), 0)
+        .. math:: dx = dy \cdot \max(\rm{sign}(y), 0)
 
         if x == 0, dy/dx => 0
         """
         dx = self._y.sign() # Allocate
         dx.max(0.0, inplace=True)
         dx *= dy
         return dx
@@ -254,15 +255,15 @@
         Returns
         -------
         vulkpy.Array
             Batch grad
 
         Notes
         -----
-        .. math:: dx = dy \times y(1 - y)
+        .. math:: dx = dy \cdot y(1 - y)
         """
         dx = 1.0 - self._y
         dx *= self._y
         dx *= dy
         return dx
 
 
@@ -310,13 +311,13 @@
         Returns
         -------
         vulkpy.Array
             Batch grad
 
         Notes
         -----
-        .. math:: dx = dy \times y(1 - y)
+        .. math:: dx = dy \cdot y(1 - y)
         """
         dx = 1.0 - self._y
         dx *= self._y
         dx *= dy
         return dx
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/losses.py` & `vulkpy-0.0.8/vulkpy/nn/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         loss : vulkpy.Array
             Cross Entropy Loss
 
         Notes
         -----
         .. math::
 
-             L = - Reduce _i ( y_i \times \log (x_i) )
+             L = - f _{\text{reduce}} ( y_i \log (x_i) )
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``__call__`` instead, where input / output are stored for training.
         """
         size = x.buffer.size()
@@ -178,16 +178,16 @@
 
 class SoftmaxCrossEntropyLoss(CrossEntropyLoss):
     """
     Softmax Cross Entropy Loss
 
     See Also
     --------
-    Softmax : Softmax layer
-    CrossEntropyLoss : Cross Entropy loss without Softmax
+    vulkpy.nn.Softmax : Softmax layer
+    vulkpy.nn.CrossEntropyLoss : Cross Entropy loss without Softmax
     """
     def __init__(self, *args, **kwargs):
         """
         Initialize Softmax Cross Entropy Loss
 
         Parameters
         ----------
@@ -213,15 +213,15 @@
         loss : vulkpy.Array
             Loss
 
         Notes
         -----
         .. math::
 
-             L = - Reduce _i (y_i \times \log (softmax(x) _i))
+             L = - f _{\text{reduce}} (y_i \log (\rm{softmax}(x) _i))
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``__call__`` instead, where input / output are stored for training.
         """
         return super().forward(self._sm(x), y)
@@ -235,15 +235,15 @@
         loss : vulkpy.Array
            Batch gradients
 
         Notes
         -----
         .. math::
 
-             dx = softmax(x) - y
+             dx = \rm{softmax}(x) - y
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``grad()`` instead, where reduction scale is corrected.
         """
         return cast(Array, self._sm._y) - self._y
@@ -280,15 +280,15 @@
         loss : vulkpy.Array
             Loss
 
         Notes
         -----
         .. math::
 
-             L = Reduce _i |x - y|^2
+             L = f _{\text{reduce}} |x - y|^2
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``__call__`` instead, where input / output are stored for training.
         """
         L = (y - x)          # Allocate
@@ -304,15 +304,15 @@
         loss : vulkpy.Array
            Batch gradients
 
         Notes
         -----
         .. math::
 
-             dx = 2 * (x - y)
+             dx = 2 (x - y)
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``grad()`` instead, where reduction scale is corrected.
         """
         dx = self._x - self._y # Allocate
@@ -351,15 +351,15 @@
         loss : vulkpy.Array
             Loss
 
         Notes
         -----
         .. math::
 
-             L = 0.5 Reduce _i min(|x - y|^2, |x - y|)
+             L = 0.5 f _{\text{reduce}} \min(|x - y|^2, |x - y|)
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``__call__`` instead, where input / output are stored for training.
         """
         delta = y - x # Allocate
@@ -377,15 +377,15 @@
         loss : vulkpy.Array
            Batch gradients
 
         Notes
         -----
         .. math::
 
-             dx = clamp(x - y, -1.0, 1.0)
+             dx = \text{clamp}(x - y, -1.0, 1.0)
 
         .. warning::
 
              Generally, users should not call this method directly.
              Use ``grad()`` instead, where reduction scale is corrected.
         """
         delta = self._x - self._y
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/models.py` & `vulkpy-0.0.8/vulkpy/nn/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 
 __all__ = ["Sequence"]
 
 
 class Sequence:
     """
     Sequential Model
+
+    All layers sequentially connceted.
     """
     def __init__(self,
                  layers: Iterable[Module],
-                 loss: Loss, *,
-                 regularizer: Optional[Regularizer] = None):
+                 loss: Loss):
         """
         Initialize Sequence
 
         Parameters
         ----------
         layers : iterable of vulkpy.nn.Module
             Layers to be called sequentially
         loss : vulkpy.nn.Loss
             Loss layer
-        regularizer : vulkpy.nn.Regularizer, optional
-            Regularizer
         """
         self.L: Tuple[Module, ...] = tuple(layers)
         self.loss: Loss = loss
 
     def _forward(self, x: Array) -> Array:
         for _L in self.L:
             x = _L(x)
@@ -60,17 +59,17 @@
         Parameters
         ----------
         x, y : vulkpy.Array
             Features and Labels/Targets
 
         Returns
         -------
-        vulkpy.Array
+        y : vulkpy.Array
             Predicted Labels/Targets
-        vulkpy.Array
+        loss : vulkpy.Array
             Loss
         """
         _y = self._forward(x)
         _loss = self.loss(_y, y)
 
         self._zero_grad()
         self._backward()
@@ -89,17 +88,17 @@
         x : vulkpy.Array
             Features
         y : vulkpy.Array, optional
             Labels/Targets.
 
         Returns
         -------
-        vulkpy.Array
+        pred_y : vulkpy.Array
             Predicted Labels/Targets
-        vulkpy.Array
+        loss : vulkpy.Array
             Loss. Return only if ``y`` is specified.
         """
         _y = self._forward(x)
         if y is None:
             return _y
 
         _loss = self.loss(_y, y)
```

### Comparing `vulkpy-0.0.7/vulkpy/nn/parameters.py` & `vulkpy-0.0.8/vulkpy/nn/parameters.py`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/nn/regularizers.py` & `vulkpy-0.0.8/vulkpy/nn/regularizers.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     r"""
     Lasso (L1) Regularization
 
     Notes
     -----
     .. math::
 
-         L = coeff \times \sum_i |W_i|\
-         dL/dW_i = coeff \times sign(W_i)
+         L = \text{coeff} \times \sum_i |W_i|\\
+         dL/dW_i = \text{coeff} \times \rm{sign}(W_i)
     """
     def __init__(self, coeff: float = 1.0):
         """
         Initialize Lasso Regularizer
 
         Parameters
         ----------
@@ -81,16 +81,16 @@
     r"""
     Ridge (L2) Regularization
 
     Notes
     -----
     .. math::
 
-         L = coeff \times \sum_i |W_i|^2\
-         dL/dW_i = 2 coeff \times W_i
+         L = \text{coeff} \times \sum_i |W_i|^2\\
+         dL/dW_i = 2 \cdot \text{coeff} \times W_i
     """
     def __init__(self, coeff: float = 1.0):
         """
         Initialize Ridge Regularizer
 
         Parameters
         ----------
@@ -131,23 +131,30 @@
         -------
         dW : vulkpy.Array
             Gradient for L2 Regularization Loss
         """
         return (2 * self.coeff) * param
 
 class Elastic(Regularizer):
-    """
+    r"""
     Elastic (L1 + L2) Regularization
+
+    Notes
+    -----
+    .. math::
+
+         L = \alpha \sum _i |W_i| + \beta \sum _i |W_i|^2\\
+         dL/dW_i = \alpha \rm{sign}(W_i) + 2 \beta W_i
     """
     def __init__(self, L1: float = 1.0, L2: float = 1.0):
         """
         Initialize Elastic Regularizer
 
-        Paramters
-        ---------
+        Parameters
+        ----------
         L1 : float, optional
             L1 Coefficient
         L2 : float, optional
             L2 Coefficient
         """
         self.L1 = Lasso(L1)
         self.L2 = Ridge(L2)
```

### Comparing `vulkpy-0.0.7/vulkpy/random.py` & `vulkpy-0.0.8/vulkpy/random.py`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/abs.spv` & `vulkpy-0.0.8/vulkpy/shader/abs.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/acos.spv` & `vulkpy-0.0.8/vulkpy/shader/acos.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/acosh.spv` & `vulkpy-0.0.8/vulkpy/shader/acosh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/add.spv` & `vulkpy-0.0.8/vulkpy/shader/add.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/add_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/add_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/add_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/add_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/asin.spv` & `vulkpy-0.0.8/vulkpy/shader/asin.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/asinh.spv` & `vulkpy-0.0.8/vulkpy/shader/asinh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/atan.spv` & `vulkpy-0.0.8/vulkpy/shader/atan.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/atanh.spv` & `vulkpy-0.0.8/vulkpy/shader/atanh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/batch_affine.spv` & `vulkpy-0.0.8/vulkpy/shader/batch_affine.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/clamp.spv` & `vulkpy-0.0.8/vulkpy/shader/clamp.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/clamp_ss.spv` & `vulkpy-0.0.8/vulkpy/shader/clamp_ss.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/clamp_sv.spv` & `vulkpy-0.0.8/vulkpy/shader/clamp_sv.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/clamp_vs.spv` & `vulkpy-0.0.8/vulkpy/shader/clamp_vs.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/cos.spv` & `vulkpy-0.0.8/vulkpy/shader/cos.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/cosh.spv` & `vulkpy-0.0.8/vulkpy/shader/cosh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/div.spv` & `vulkpy-0.0.8/vulkpy/shader/div.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/div_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/div_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/div_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/div_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/exp.spv` & `vulkpy-0.0.8/vulkpy/shader/exp.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/exp2.spv` & `vulkpy-0.0.8/vulkpy/shader/exp2.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/gather.spv` & `vulkpy-0.0.8/vulkpy/shader/gather.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/gather_axis.spv` & `vulkpy-0.0.8/vulkpy/shader/gather_axis.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iabs.spv` & `vulkpy-0.0.8/vulkpy/shader/iabs.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iacos.spv` & `vulkpy-0.0.8/vulkpy/shader/iacos.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iacosh.spv` & `vulkpy-0.0.8/vulkpy/shader/iacosh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iadd.spv` & `vulkpy-0.0.8/vulkpy/shader/iadd.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iadd_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/iadd_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iadd_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/iadd_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iasin.spv` & `vulkpy-0.0.8/vulkpy/shader/iasin.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iasinh.spv` & `vulkpy-0.0.8/vulkpy/shader/iasinh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iatan.spv` & `vulkpy-0.0.8/vulkpy/shader/iatan.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iatanh.spv` & `vulkpy-0.0.8/vulkpy/shader/iatanh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iclamp.spv` & `vulkpy-0.0.8/vulkpy/shader/iclamp.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iclamp_ss.spv` & `vulkpy-0.0.8/vulkpy/shader/iclamp_ss.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iclamp_sv.spv` & `vulkpy-0.0.8/vulkpy/shader/iclamp_sv.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iclamp_vs.spv` & `vulkpy-0.0.8/vulkpy/shader/iclamp_vs.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/icos.spv` & `vulkpy-0.0.8/vulkpy/shader/icos.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/icosh.spv` & `vulkpy-0.0.8/vulkpy/shader/icosh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/idiv.spv` & `vulkpy-0.0.8/vulkpy/shader/idiv.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/idiv_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/idiv_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/idiv_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/idiv_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iexp.spv` & `vulkpy-0.0.8/vulkpy/shader/iexp.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iexp2.spv` & `vulkpy-0.0.8/vulkpy/shader/iexp2.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/iinvsqrt.spv` & `vulkpy-0.0.8/vulkpy/shader/iinvsqrt.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/ilog.spv` & `vulkpy-0.0.8/vulkpy/shader/ilog.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/ilog2.spv` & `vulkpy-0.0.8/vulkpy/shader/ilog2.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imax.spv` & `vulkpy-0.0.8/vulkpy/shader/imax.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imax_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/imax_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imax_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/imax_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imin.spv` & `vulkpy-0.0.8/vulkpy/shader/imin.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imin_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/imin_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imin_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/imin_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imul.spv` & `vulkpy-0.0.8/vulkpy/shader/imul.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imul_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/imul_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/imul_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/imul_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/invsqrt.spv` & `vulkpy-0.0.8/vulkpy/shader/invsqrt.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/ipow.spv` & `vulkpy-0.0.8/vulkpy/shader/ipow.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/ipow_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/ipow_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/ipow_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/ipow_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isign.spv` & `vulkpy-0.0.8/vulkpy/shader/isign.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isin.spv` & `vulkpy-0.0.8/vulkpy/shader/isin.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isinh.spv` & `vulkpy-0.0.8/vulkpy/shader/isinh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isqrt.spv` & `vulkpy-0.0.8/vulkpy/shader/isqrt.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isub.spv` & `vulkpy-0.0.8/vulkpy/shader/isub.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isub_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/isub_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/isub_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/isub_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/itan.spv` & `vulkpy-0.0.8/vulkpy/shader/itan.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/itanh.spv` & `vulkpy-0.0.8/vulkpy/shader/itanh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/log.spv` & `vulkpy-0.0.8/vulkpy/shader/log.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/log2.spv` & `vulkpy-0.0.8/vulkpy/shader/log2.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/matmul.spv` & `vulkpy-0.0.8/vulkpy/shader/matmul.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/max.spv` & `vulkpy-0.0.8/vulkpy/shader/max.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/max_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/max_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/max_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/max_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/maximum.spv` & `vulkpy-0.0.8/vulkpy/shader/maximum.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/maximum_axis.spv` & `vulkpy-0.0.8/vulkpy/shader/maximum_axis.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/maximum_axis_rebroadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/maximum_axis_rebroadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/maximum_v1.3.spv` & `vulkpy-0.0.8/vulkpy/shader/maximum_v1.3.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/min.spv` & `vulkpy-0.0.8/vulkpy/shader/min.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/min_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/min_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/min_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/min_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/minimum.spv` & `vulkpy-0.0.8/vulkpy/shader/minimum.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/minimum_axis.spv` & `vulkpy-0.0.8/vulkpy/shader/minimum_axis.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/minimum_axis_rebroadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/minimum_axis_rebroadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/minimum_v1.3.spv` & `vulkpy-0.0.8/vulkpy/shader/minimum_v1.3.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/mul.spv` & `vulkpy-0.0.8/vulkpy/shader/mul.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/mul_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/mul_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/mul_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/mul_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/nn_cross_entropy.spv` & `vulkpy-0.0.8/vulkpy/shader/nn_cross_entropy.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/nn_cross_entropy_backward.spv` & `vulkpy-0.0.8/vulkpy/shader/nn_cross_entropy_backward.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/pow.spv` & `vulkpy-0.0.8/vulkpy/shader/pow.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/pow_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/pow_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/pow_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/pow_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prng_box_muller.spv` & `vulkpy-0.0.8/vulkpy/shader/prng_box_muller.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prng_ibox_muller.spv` & `vulkpy-0.0.8/vulkpy/shader/prng_ibox_muller.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prng_randrange.spv` & `vulkpy-0.0.8/vulkpy/shader/prng_randrange.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prng_xoshiro128pp_float.spv` & `vulkpy-0.0.8/vulkpy/shader/prng_xoshiro128pp_float.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prng_xoshiro128pp_uint32.spv` & `vulkpy-0.0.8/vulkpy/shader/prng_xoshiro128pp_uint32.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prod.spv` & `vulkpy-0.0.8/vulkpy/shader/prod.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prod_axis.spv` & `vulkpy-0.0.8/vulkpy/shader/prod_axis.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prod_axis_rebroadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/prod_axis_rebroadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/prod_v1.3.spv` & `vulkpy-0.0.8/vulkpy/shader/prod_v1.3.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/rdiv_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/rdiv_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/rpow_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/rpow_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/rsub_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/rsub_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sign.spv` & `vulkpy-0.0.8/vulkpy/shader/sign.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sin.spv` & `vulkpy-0.0.8/vulkpy/shader/sin.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sinh.spv` & `vulkpy-0.0.8/vulkpy/shader/sinh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sqrt.spv` & `vulkpy-0.0.8/vulkpy/shader/sqrt.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sub.spv` & `vulkpy-0.0.8/vulkpy/shader/sub.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sub_broadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/sub_broadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sub_scalar.spv` & `vulkpy-0.0.8/vulkpy/shader/sub_scalar.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sum.spv` & `vulkpy-0.0.8/vulkpy/shader/sum.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sum_axis.spv` & `vulkpy-0.0.8/vulkpy/shader/sum_axis.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sum_axis_rebroadcast.spv` & `vulkpy-0.0.8/vulkpy/shader/sum_axis_rebroadcast.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/sum_v1.3.spv` & `vulkpy-0.0.8/vulkpy/shader/sum_v1.3.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/tan.spv` & `vulkpy-0.0.8/vulkpy/shader/tan.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/shader/tanh.spv` & `vulkpy-0.0.8/vulkpy/shader/tanh.spv`

 * *Files identical despite different names*

### Comparing `vulkpy-0.0.7/vulkpy/util.py` & `vulkpy-0.0.8/vulkpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def enable_debug(*, validation: bool = True, api_dump: bool = True):
     """
     Enable debug message
 
     Parameters
     ----------
     validation : bool, optional
-        If ``True`` (default), enable vulkan validation.
+        If ``True`` (default), enable Vulkan validation.
     api_dump : bool, optional
         If ``True`` (default), enable Vulkan API dump.
 
     Notes
     -----
     ``validation`` requires validation layer [1]_.
     ``api_dump`` requires LunarG API dump layer [2]_.
```

### Comparing `vulkpy-0.0.7/vulkpy/vkarray.py` & `vulkpy-0.0.8/vulkpy/vkarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,31 @@
 ]
 
 logger = wblog.getLogger()
 
 class GPU:
     """
     GPU instance
+
+    Examples
+    --------
+    >>> import vulkpy as vk
+    >>> gpu = vk.GPU()
+
+    If you have multiple GPUs, you can specify GPU index
+
+    >>> gpu1 = vk.GPU(1)
+
+    GPU equality is checked by GPU index
+
+    >>> gpu == gpu1
+    False
+
+    >>> gpu == vk.GPU()
+    True
     """
     def __init__(self, idx: int=0, priority: float=0.0):
         """
         Initialize GPU
 
         Parameters
         ----------
@@ -170,18 +187,43 @@
         self.wait()
         return self.array
 
 
 class U32Array(_GPUArray):
     """
     GPU Array of uint (32bit) for shape or indices
+
+    See Also
+    --------
+    vulkpy.Array : float (32bit) array supporing mathematical operation
+
+    Warnings
+    --------
+    U32Array doesn't support any mathematical operation.
+    This class is designed for indexing and class label.
     """
     def __init__(self, gpu: GPU, *,
                  data: Optional[Iterable[int]] = None,
                  shape: Optional[Iterable[int]] = None):
+        """
+        Initialize U32Array
+
+        Parameters
+        ----------
+        data : iterable of ints, optional
+            Data to be copied.
+        shape : iterable of ints, optional
+            Shape for uninitialized array.
+            If ``data`` is not ``None``, ``shape`` is ignored.
+
+        Raises
+        ------
+        ValueError
+            If neither ``data`` nor ``shape`` is specified.
+        """
         super().__init__(gpu)
 
         if data is not None:
             data = np.asarray(data, dtype=np.uint32)
             self.shape = data.shape
             self.buffer = self._gpu.gpu.toU32Buffer(np.ravel(data))
         else:
@@ -583,14 +625,15 @@
             inplace: bool = False) -> Array:
         """
         Element-wise Max
 
         Parameters
         ----------
         other : Array or float
+            Other value
         inplace : bool
             If ``True``, update inplace, otherwise returns new array.
             Default value is ``False``.
 
         Returns
         -------
         Array
@@ -610,14 +653,15 @@
             inplace: bool = False) -> Array:
         """
         Element-wise Min
 
         Parameters
         ----------
         other : Array or float
+            Other value
         inplace : bool
             If ``True``, update inplace, otherwise returns new array.
             Default value is ``False``.
 
         Returns
         -------
         Array
@@ -1066,16 +1110,18 @@
     def clamp(self, min: Union[Array, float], max: Union[Array, float],
               inplace: bool = False) -> Array:
         """
         Element-wise clamp()
 
         Parameters
         ----------
-        min, max : Array or float
-            Minimum/Maximum value
+        min : Array or float
+            Minimum value
+        max : Array or float
+            Maximum value
         inplace : bool
             If ``True``, update inplace, otherwise returns new array.
             Default value is ``False``.
 
         Returns
         -------
         Array
```

### Comparing `vulkpy-0.0.7/vulkpy.egg-info/PKG-INFO` & `vulkpy-0.0.8/vulkpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulkpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: GPGPU array on Vulkan
 Home-page: https://github.com/ymd-h/vulkpy
 Author: H. Yamada
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -106,16 +106,16 @@
     * Gaussian with Box-Muller (`.normal(shape=None, buffer=None, mean=0.0, stddev=1.0)`)
   * [ ] pcg32
 * Neural Network
   * Layers
     * [x] `Dense`, `ReLU`, `Sigmoid`, `Softmax`
     * [ ] conv, batch norm, layer norm, ...
   * Optimizers
-    * [x] `SGD`, `Adam`
-    * [ ] rmsprop, adagrad, ...
+    * [x] `SGD`, `Adam`, `AdaGrad`
+    * [ ] rmsprop, ...
   * Losses
     * [x] `CrossEntropyLoss`, `SoftmaxCrossEntropyLoss`, `MSELoss`, `HuberLoss`
     * [ ] ...
   * Initializers
     * [x] `Constant`, `HeNormal`
     * [ ] ...
   * Models
```

### Comparing `vulkpy-0.0.7/vulkpy.egg-info/SOURCES.txt` & `vulkpy-0.0.8/vulkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

