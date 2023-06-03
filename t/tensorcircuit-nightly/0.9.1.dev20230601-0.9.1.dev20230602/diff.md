# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230601.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230601.tar", last modified: Thu Jun  1 12:40:52 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230602.tar", last modified: Fri Jun  2 12:39:29 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230601.tar` & `tensorcircuit-nightly-0.9.1.dev20230602.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.181338 tensorcircuit-nightly-0.9.1.dev20230601/
--rw-r--r--   0 runner    (1001) docker     (122)    25659 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-01 12:40:52.181338 tensorcircuit-nightly-0.9.1.dev20230601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19131 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6535 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.161337 tensorcircuit-nightly-0.9.1.dev20230601/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.169338 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6356 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     5839 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 12:40:52.181338 tensorcircuit-nightly-0.9.1.dev20230601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-01 12:40:45.000000 tensorcircuit-nightly-0.9.1.dev20230601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.173338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-01 12:40:45.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    43480 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.173338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14325 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11518 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.177338 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-01 12:40:51.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-06-01 12:40:51.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 12:40:51.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-01 12:40:51.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-01 12:40:51.000000 tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:40:52.181338 tensorcircuit-nightly-0.9.1.dev20230601/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47707 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5606 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-06-01 12:17:50.000000 tensorcircuit-nightly-0.9.1.dev20230601/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.511187 tensorcircuit-nightly-0.9.1.dev20230602/
+-rw-r--r--   0 runner    (1001) docker     (122)    25759 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-02 12:39:29.511187 tensorcircuit-nightly-0.9.1.dev20230602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19131 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6535 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.483187 tensorcircuit-nightly-0.9.1.dev20230602/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.491187 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6356 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5839 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:39:29.511187 tensorcircuit-nightly-0.9.1.dev20230602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-02 12:39:23.000000 tensorcircuit-nightly-0.9.1.dev20230602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.495187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-02 12:39:23.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43480 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.499187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.503187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.503187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14325 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11518 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.503187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17600 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.503187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.503187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.507187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.507187 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-02 12:39:29.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-06-02 12:39:29.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:39:29.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-02 12:39:29.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-02 12:39:29.000000 tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:39:29.507187 tensorcircuit-nightly-0.9.1.dev20230602/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47707 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5606 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-06-02 12:16:58.000000 tensorcircuit-nightly-0.9.1.dev20230602/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230602/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 - Task management via group tag (when `submit_task` and `list_tasks`)
 
 - `batch_expectation_ps` now supports local device without topology and thus unify the interface for numerical exact simulation, numerical simulation with measurement shots and QPU experiments
 
 - introduce two stage compiling for `batch_expectation_ps` to save some compiling overhead
 
+- Add experimental support for ODE backend pulse level control simulation/analog quantum computing
+
 ### Fixed
 
 - `tc.results.counts.plot_histogram` now can dispatch kws to corresponding qiskit method
 
 - New implementation for `c.inverse()` to partially avoid unrecognized gate name issue
 
 - Fixed bug for `batch_expectation_ps` for jax backend
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230602/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230602/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230602/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230601
+Version: 0.9.1.dev20230602
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/README.md` & `tensorcircuit-nightly-0.9.1.dev20230602/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230602/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230602/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230602/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230601"
+__version__ = "0.9.1.dev20230602"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/experimental.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 """
 
 from functools import partial
 from typing import Any, Callable, Optional, Tuple, Sequence, Union
 
 import numpy as np
 
-from .cons import backend, dtypestr
+from .cons import backend, dtypestr, contractor, rdtypestr
+from .gates import Gate, array_to_tensor
 
 Tensor = Any
+Circuit = Any
 
 
 def adaptive_vmap(
     f: Callable[..., Any],
     vectorized_argnums: Union[int, Sequence[int]] = 0,
     chunk_size: Optional[int] = None,
 ) -> Callable[..., Any]:
@@ -429,7 +431,90 @@
         psi_exact = backend.reshape(psi_exact, [-1])
         psi_exact = psi_exact / backend.norm(psi_exact)
         if callback is None:
             return psi_exact
         return callback(psi_exact)
 
     return backend.stack([_evol(t) for t in tlist])
+
+
+def evol_local(
+    c: Circuit,
+    index: Sequence[int],
+    h_fun: Callable[..., Tensor],
+    t: float,
+    *args: Any,
+    **solver_kws: Any
+) -> Circuit:
+    """
+    ode evolution of time dependent Hamiltonian on circuit of given indices
+    [only jax backend support for now]
+
+    :param c: _description_
+    :type c: Circuit
+    :param index: _description_
+    :type index: Sequence[int]
+    :param h_fun: h_fun should return a dense Hamiltonian matrix
+        with input arguments time and *args
+    :type h_fun: Callable[..., Tensor]
+    :param t: evolution time
+    :type t: float
+    :return: _description_
+    :rtype: Circuit
+    """
+    from jax.experimental.ode import odeint
+
+    s = c.state()
+    n = c._nqubits
+    l = len(index)
+
+    def f(y: Tensor, t: Tensor, *args: Any) -> Tensor:
+        y = backend.reshape2(y)
+        y = Gate(y)
+        h = -1.0j * h_fun(t, *args)
+        h = backend.reshape2(h)
+        h = Gate(h)
+        edges = []
+        for i in range(n):
+            if i not in index:
+                edges.append(y[i])
+            else:
+                j = index.index(i)
+                edges.append(h[j])
+                h[j + l] ^ y[i]
+        y = contractor([y, h], output_edge_order=edges)
+        return backend.reshape(y.tensor, [-1])
+
+    t = array_to_tensor([0, t], dtype=rdtypestr)
+    s1 = odeint(f, s, t, *args, **solver_kws)
+    return type(c)(n, inputs=s1[-1])
+
+
+def evol_global(
+    c: Circuit, h_fun: Callable[..., Tensor], t: float, *args: Any, **solver_kws: Any
+) -> Circuit:
+    """
+    ode evolution of time dependent Hamiltonian on circuit of all qubits
+    [only jax backend support for now]
+
+    :param c: _description_
+    :type c: Circuit
+    :param h_fun: h_fun should return a **SPARSE** Hamiltonian matrix
+        with input arguments time and *args
+    :type h_fun: Callable[..., Tensor]
+    :param t: _description_
+    :type t: float
+    :return: _description_
+    :rtype: Circuit
+    """
+    from jax.experimental.ode import odeint
+
+    s = c.state()
+    n = c._nqubits
+
+    def f(y: Tensor, t: Tensor, *args: Any) -> Tensor:
+        h = -1.0j * h_fun(t, *args)
+        return backend.sparse_dense_matmul(h, y)
+
+    t = array_to_tensor([0, t], dtype=rdtypestr)
+    s1 = odeint(f, s, t, *args, **solver_kws)
+    return type(c)(n, inputs=s1[-1])
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230601
+Version: 0.9.1.dev20230602
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230602/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_miscs.py`

 * *Files 7% similar despite different names*

```diff
@@ -214,7 +214,37 @@
     def fsum1(param1, param2):
         return tc.backend.mean(f1(param1, param2))
 
     g3, g4 = tc.backend.value_and_grad(fsum1)(p1, p2)
 
     np.testing.assert_allclose(g1, g3, atol=1e-5)
     np.testing.assert_allclose(g2, g4, atol=1e-5)
+
+
+def test_evol(jaxb):
+    def h_square(t, b):
+        return (tc.backend.sign(t - 1.0) + 1) / 2 * b * tc.gates.x().tensor
+
+    c = tc.Circuit(3)
+    c.x(0)
+    c.cx(0, 1)
+    c.h(2)
+    c = experimental.evol_local(
+        c, [1], h_square, 2.0, tc.backend.convert_to_tensor(0.2)
+    )
+    c.rx(1, theta=np.pi - 0.4)
+    np.testing.assert_allclose(c.expectation_ps(z=[1]), 1.0, atol=1e-5)
+
+    ixi = tc.quantum.PauliStringSum2COO([[0, 1, 0]])
+
+    def h_square_sparse(t, b):
+        return (tc.backend.sign(t - 1.0) + 1) / 2 * b * ixi
+
+    c = tc.Circuit(3)
+    c.x(0)
+    c.cx(0, 1)
+    c.h(2)
+    c = experimental.evol_global(
+        c, h_square_sparse, 2.0, tc.backend.convert_to_tensor(0.2)
+    )
+    c.rx(1, theta=np.pi - 0.4)
+    np.testing.assert_allclose(c.expectation_ps(z=[1]), 1.0, atol=1e-5)
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230601/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230602/tests/test_van.py`

 * *Files identical despite different names*

