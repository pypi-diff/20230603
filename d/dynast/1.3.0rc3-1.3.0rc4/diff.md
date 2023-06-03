# Comparing `tmp/dynast-1.3.0rc3.tar.gz` & `tmp/dynast-1.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynast-1.3.0rc3.tar", last modified: Fri Jun  2 22:06:08 2023, max compression
+gzip compressed data, was "dynast-1.3.0rc4.tar", last modified: Sat Jun  3 16:58:05 2023, max compression
```

## Comparing `dynast-1.3.0rc3.tar` & `dynast-1.3.0rc4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/LICENSE.md
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/README.md
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.238978 dynast-1.3.0rc3/dynast/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/analytics/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/analytics/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3111 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/analytics/results.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4596 2023-06-02 03:42:21.000000 dynast-1.3.0rc3/dynast/analytics/visualize.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4860 2023-06-02 22:03:53.000000 dynast-1.3.0rc3/dynast/cli.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/common.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/dynast_manager.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/measure/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/measure/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/measure/latency.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/predictors/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/predictors/__init__.py
--rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6751 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/predictors/dynamic_predictor.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/predictors/predictor_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/python.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/search/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/search/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/search/encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-06-02 03:42:21.000000 dynast-1.3.0rc3/dynast/search/evaluation_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16397 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/search/evolutionary.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41296 2023-06-02 22:03:53.000000 dynast-1.3.0rc3/dynast/search/search_tactic.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/supernetwork/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14923 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14561 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12721 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.246977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8793 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8312 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.250977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16147 2023-05-05 17:45:18.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-06-02 19:59:33.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.250977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4971 2023-06-02 22:03:30.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.250977 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6955 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2235 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15297 2023-06-01 18:29:08.000000 dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa_interface.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.250977 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/modules_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7752 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22141 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43472 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_supernetwork.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.250977 dynast-1.3.0rc3/dynast/supernetwork/recommendation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/recommendation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-06-02 22:03:53.000000 dynast-1.3.0rc3/dynast/supernetwork/supernetwork_registry.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/dynast/supernetwork/text_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/text_classification/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12528 2023-06-01 18:51:42.000000 dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7282 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3595 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/supernetwork/text_classification/sst2_dataloader.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/dynast/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8884 2023-06-01 18:29:08.000000 dynast-1.3.0rc3/dynast/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/utils/cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10458 2023-05-30 18:27:20.000000 dynast-1.3.0rc3/dynast/utils/datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/dynast/utils/distributed.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6423 2023-05-18 21:41:10.000000 dynast-1.3.0rc3/dynast/utils/nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6734 2023-05-05 17:45:18.000000 dynast-1.3.0rc3/dynast/utils/reference.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.242977 dynast-1.3.0rc3/dynast.egg-info/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4794 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/SOURCES.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/dependency_links.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/entry_points.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      295 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/requires.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-06-02 22:06:08.000000 dynast-1.3.0rc3/dynast.egg-info/top_level.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      361 2023-06-01 18:50:40.000000 dynast-1.3.0rc3/pyproject.toml
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/setup.cfg
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-06-02 22:04:05.000000 dynast-1.3.0rc3/setup.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/tests/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/tests/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 22:06:08.254977 dynast-1.3.0rc3/tests/checks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/tests/checks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/tests/checks/check_license.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1168 2023-05-05 17:45:18.000000 dynast-1.3.0rc3/tests/checks/helpers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/tests/functional_reference.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-05-01 19:25:12.000000 dynast-1.3.0rc3/tests/test_dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/LICENSE.md
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/README.md
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.114081 dynast-1.3.0rc4/dynast/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.114081 dynast-1.3.0rc4/dynast/analytics/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/analytics/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3111 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/analytics/results.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4596 2023-06-02 03:42:21.000000 dynast-1.3.0rc4/dynast/analytics/visualize.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4860 2023-06-02 22:03:53.000000 dynast-1.3.0rc4/dynast/cli.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/common.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.114081 dynast-1.3.0rc4/dynast/measure/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/measure/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/measure/latency.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/predictors/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/predictors/__init__.py
+-rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6751 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/predictors/dynamic_predictor.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/predictors/predictor_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/python.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/search/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/search/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/search/encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-06-02 03:42:21.000000 dynast-1.3.0rc4/dynast/search/evaluation_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16397 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/search/evolutionary.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41296 2023-06-02 22:03:53.000000 dynast-1.3.0rc4/dynast/search/search_tactic.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.118081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.122081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.122081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.122081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14923 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14561 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12721 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.122081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8793 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8312 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.122081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16147 2023-05-05 17:45:18.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-06-02 19:59:33.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.126081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5029 2023-06-03 16:56:03.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.126081 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6955 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2235 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15297 2023-06-01 18:29:08.000000 dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa_interface.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.126081 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/modules_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7752 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22141 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43472 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_supernetwork.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.126081 dynast-1.3.0rc4/dynast/supernetwork/recommendation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/recommendation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-06-02 22:03:53.000000 dynast-1.3.0rc4/dynast/supernetwork/supernetwork_registry.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.126081 dynast-1.3.0rc4/dynast/supernetwork/text_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/text_classification/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12528 2023-06-01 18:51:42.000000 dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7282 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3595 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/supernetwork/text_classification/sst2_dataloader.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/dynast/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8884 2023-06-01 18:29:08.000000 dynast-1.3.0rc4/dynast/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/utils/cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10458 2023-05-30 18:27:20.000000 dynast-1.3.0rc4/dynast/utils/datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/dynast/utils/distributed.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6423 2023-05-18 21:41:10.000000 dynast-1.3.0rc4/dynast/utils/nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6734 2023-05-05 17:45:18.000000 dynast-1.3.0rc4/dynast/utils/reference.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.114081 dynast-1.3.0rc4/dynast.egg-info/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4794 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/SOURCES.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/dependency_links.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/entry_points.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      295 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/requires.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-06-03 16:58:05.000000 dynast-1.3.0rc4/dynast.egg-info/top_level.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      361 2023-06-01 18:50:40.000000 dynast-1.3.0rc4/pyproject.toml
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/setup.cfg
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-06-03 16:58:00.000000 dynast-1.3.0rc4/setup.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/tests/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/tests/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-03 16:58:05.130081 dynast-1.3.0rc4/tests/checks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/tests/checks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/tests/checks/check_license.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1168 2023-05-05 17:45:18.000000 dynast-1.3.0rc4/tests/checks/helpers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/tests/functional_reference.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-05-01 19:25:12.000000 dynast-1.3.0rc4/tests/test_dynast_manager.py
```

### Comparing `dynast-1.3.0rc3/LICENSE.md` & `dynast-1.3.0rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/PKG-INFO` & `dynast-1.3.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.3.0rc3
+Version: 1.3.0rc4
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.3.0rc3/README.md` & `dynast-1.3.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/__init__.py` & `dynast-1.3.0rc4/dynast/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/analytics/__init__.py` & `dynast-1.3.0rc4/dynast/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/analytics/results.py` & `dynast-1.3.0rc4/dynast/analytics/results.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/analytics/visualize.py` & `dynast-1.3.0rc4/dynast/analytics/visualize.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/cli.py` & `dynast-1.3.0rc4/dynast/cli.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/common.py` & `dynast-1.3.0rc4/dynast/common.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/dynast_manager.py` & `dynast-1.3.0rc4/dynast/dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/measure/__init__.py` & `dynast-1.3.0rc4/dynast/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/measure/latency.py` & `dynast-1.3.0rc4/dynast/measure/latency.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/predictors/__init__.py` & `dynast-1.3.0rc4/dynast/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/predictors/dynamic_predictor.py` & `dynast-1.3.0rc4/dynast/predictors/dynamic_predictor.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/predictors/predictor_manager.py` & `dynast-1.3.0rc4/dynast/predictors/predictor_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/python.py` & `dynast-1.3.0rc4/dynast/python.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/search/__init__.py` & `dynast-1.3.0rc4/dynast/search/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/search/encoding.py` & `dynast-1.3.0rc4/dynast/search/encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/search/evaluation_interface.py` & `dynast-1.3.0rc4/dynast/search/evaluation_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/search/evolutionary.py` & `dynast-1.3.0rc4/dynast/search/evolutionary.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/search/search_tactic.py` & `dynast-1.3.0rc4/dynast/search/search_tactic.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,18 @@
             # Currenly HAN Lab's server has misconfigured SSL certificate
             # and there is no other workaround available right now...
             with open(cached_file, 'wb') as f:
                 f.write(req_file.content)
         return cached_file
     except Exception as e:
         # remove lock file so download can be executed next time.
-        os.remove(os.path.join(model_dir, "download.lock"))
+        try:
+            os.remove(os.path.join(model_dir, "download.lock"))
+        except OSError:
+            pass
         sys.stderr.write("Failed to download from url %s" % url + "\n" + str(e) + "\n")
         return None
 
 
 def write_log(logs_path, log_str, prefix="valid", should_print=True, mode="a"):
     if not os.path.exists(logs_path):
         os.makedirs(logs_path, exist_ok=True)
```

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa_encoding.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/image_classification/ofa/ofa_interface.py` & `dynast-1.3.0rc4/dynast/supernetwork/image_classification/ofa/ofa_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/machine_translation/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/machine_translation/modules_supernetwork.py` & `dynast-1.3.0rc4/dynast/supernetwork/machine_translation/modules_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_encoding.py` & `dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_interface.py` & `dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/machine_translation/transformer_supernetwork.py` & `dynast-1.3.0rc4/dynast/supernetwork/machine_translation/transformer_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/recommendation/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/supernetwork_registry.py` & `dynast-1.3.0rc4/dynast/supernetwork/supernetwork_registry.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/text_classification/__init__.py` & `dynast-1.3.0rc4/dynast/supernetwork/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_encoding.py` & `dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_interface.py` & `dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/text_classification/bert_supernetwork.py` & `dynast-1.3.0rc4/dynast/supernetwork/text_classification/bert_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/supernetwork/text_classification/sst2_dataloader.py` & `dynast-1.3.0rc4/dynast/supernetwork/text_classification/sst2_dataloader.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/__init__.py` & `dynast-1.3.0rc4/dynast/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/cache.py` & `dynast-1.3.0rc4/dynast/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/datasets.py` & `dynast-1.3.0rc4/dynast/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/distributed.py` & `dynast-1.3.0rc4/dynast/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/nn.py` & `dynast-1.3.0rc4/dynast/utils/nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast/utils/reference.py` & `dynast-1.3.0rc4/dynast/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/dynast.egg-info/PKG-INFO` & `dynast-1.3.0rc4/dynast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.3.0rc3
+Version: 1.3.0rc4
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.3.0rc3/dynast.egg-info/SOURCES.txt` & `dynast-1.3.0rc4/dynast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/setup.py` & `dynast-1.3.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import datetime
 
 from setuptools import find_packages, setup
 
 
 def get_version():
     # TODO(macsz) Replace with __version__
-    return '1.3.0rc3'
+    return '1.3.0rc4'
 
 
 def get_dependencies():
     deps = []
     with open('requirements.txt') as f:
         lines = f.readlines()
         for line in lines:
```

### Comparing `dynast-1.3.0rc3/tests/__init__.py` & `dynast-1.3.0rc4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/tests/checks/__init__.py` & `dynast-1.3.0rc4/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/tests/checks/check_license.py` & `dynast-1.3.0rc4/tests/checks/check_license.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/tests/checks/helpers.py` & `dynast-1.3.0rc4/tests/checks/helpers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/tests/functional_reference.py` & `dynast-1.3.0rc4/tests/functional_reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc3/tests/test_dynast_manager.py` & `dynast-1.3.0rc4/tests/test_dynast_manager.py`

 * *Files identical despite different names*

