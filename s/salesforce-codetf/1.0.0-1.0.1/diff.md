# Comparing `tmp/salesforce-codetf-1.0.0.tar.gz` & `tmp/salesforce-codetf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-1.0.0.tar", last modified: Fri Jun  2 21:45:46 2023, max compression
+gzip compressed data, was "salesforce-codetf-1.0.1.tar", last modified: Fri Jun  2 21:59:45 2023, max compression
```

## Comparing `salesforce-codetf-1.0.0.tar` & `salesforce-codetf-1.0.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.673999 salesforce-codetf-1.0.0/
--rw-r--r--   0 nghi.bui   (503) staff       (20)       39 2023-06-02 21:30:18.000000 salesforce-codetf-1.0.0/MANIFEST.in
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25728 2023-06-02 21:45:46.674499 salesforce-codetf-1.0.0/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.630022 salesforce-codetf-1.0.0/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.0/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.632290 salesforce-codetf-1.0.0/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.633576 salesforce-codetf-1.0.0/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.634248 salesforce-codetf-1.0.0/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.635436 salesforce-codetf-1.0.0/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.636526 salesforce-codetf-1.0.0/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-1.0.0/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.637521 salesforce-codetf-1.0.0/codetf/configs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:28:24.000000 salesforce-codetf-1.0.0/codetf/configs/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.637972 salesforce-codetf-1.0.0/codetf/configs/dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      328 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/dataset/dataset.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)      131 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.0/codetf/configs/default.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.639390 salesforce-codetf-1.0.0/codetf/configs/inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      480 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/configs/inference/bert.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2852 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/configs/inference/causal_lm.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/configs/inference/codet5.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.640306 salesforce-codetf-1.0.0/codetf/configs/training/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      766 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/training/causal_lm.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1020 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/training/codet5.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.644650 salesforce-codetf-1.0.0/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.646035 salesforce-codetf-1.0.0/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.646898 salesforce-codetf-1.0.0/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.647652 salesforce-codetf-1.0.0/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.648401 salesforce-codetf-1.0.0/codetf/models/seq2seq_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/seq2seq_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.650601 salesforce-codetf-1.0.0/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.652963 salesforce-codetf-1.0.0/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.653779 salesforce-codetf-1.0.0/docs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-1.0.0/docs/conf.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.660054 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25728 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2385 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      319 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       42 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 21:45:46.675522 salesforce-codetf-1.0.0/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1644 2023-06-02 21:45:35.000000 salesforce-codetf-1.0.0/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.664961 salesforce-codetf-1.0.0/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.665714 salesforce-codetf-1.0.0/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.667183 salesforce-codetf-1.0.0/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.671255 salesforce-codetf-1.0.0/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1098 2023-06-02 21:45:21.000000 salesforce-codetf-1.0.0/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_load_model_zoo.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.673349 salesforce-codetf-1.0.0/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 21:34:03.000000 salesforce-codetf-1.0.0/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-1.0.0/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.682083 salesforce-codetf-1.0.1/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       39 2023-06-02 21:30:18.000000 salesforce-codetf-1.0.1/MANIFEST.in
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    26341 2023-06-02 21:59:45.682619 salesforce-codetf-1.0.1/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    22981 2023-06-02 21:58:59.000000 salesforce-codetf-1.0.1/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.643151 salesforce-codetf-1.0.1/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.644958 salesforce-codetf-1.0.1/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.645824 salesforce-codetf-1.0.1/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.646788 salesforce-codetf-1.0.1/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.647639 salesforce-codetf-1.0.1/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.648650 salesforce-codetf-1.0.1/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-1.0.1/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.649652 salesforce-codetf-1.0.1/codetf/configs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:28:24.000000 salesforce-codetf-1.0.1/codetf/configs/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.650183 salesforce-codetf-1.0.1/codetf/configs/dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      328 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/dataset/dataset.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      131 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1/codetf/configs/default.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.651670 salesforce-codetf-1.0.1/codetf/configs/inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      480 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/configs/inference/bert.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2852 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/configs/inference/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/configs/inference/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.652687 salesforce-codetf-1.0.1/codetf/configs/training/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      766 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/training/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1020 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/training/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.656076 salesforce-codetf-1.0.1/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.657425 salesforce-codetf-1.0.1/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.657940 salesforce-codetf-1.0.1/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.658427 salesforce-codetf-1.0.1/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3375 2023-06-02 21:54:25.000000 salesforce-codetf-1.0.1/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.658911 salesforce-codetf-1.0.1/codetf/models/seq2seq_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.660425 salesforce-codetf-1.0.1/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.662016 salesforce-codetf-1.0.1/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.662568 salesforce-codetf-1.0.1/docs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-1.0.1/docs/conf.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.666782 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    26341 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2385 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      319 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       42 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 21:59:45.683694 salesforce-codetf-1.0.1/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1644 2023-06-02 21:59:34.000000 salesforce-codetf-1.0.1/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.670413 salesforce-codetf-1.0.1/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.671177 salesforce-codetf-1.0.1/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.672833 salesforce-codetf-1.0.1/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.678767 salesforce-codetf-1.0.1/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      448 2023-06-02 21:55:53.000000 salesforce-codetf-1.0.1/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 21:47:19.000000 salesforce-codetf-1.0.1/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.681365 salesforce-codetf-1.0.1/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 21:34:03.000000 salesforce-codetf-1.0.1/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-1.0.1/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-1.0.0/PKG-INFO` & `salesforce-codetf-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.0
+Version: 1.0.1
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
@@ -90,25 +90,37 @@
         ```bash
         conda create -n codetf python=3.8
         conda activate codetf
         ```
         
         2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
         ```bash
-        pip install salesforce-codetf
+        pip install salesforce-codetf==1.0.0
         ```
             
         3. Alternatively, build CodeTF from source:
         
         ```bash
         git clone https://github.com/salesforce/CodeTF.git
         cd CodeTF
         pip install -e .
         ```
         
+        Additionally, to make sure the quantization feature works well, also install these dependencies:
+        ```bash
+        pip install -q -U git+https://github.com/huggingface/transformers.git
+        pip install -q -U git+https://github.com/huggingface/peft.git
+        pip install -q -U git+https://github.com/huggingface/accelerate.git
+        ```
+        
+        For some models, such as [StarCoder](https://github.com/bigcode-project/starcoder), it is required to log in Huggingface. Please obtain the HuggingFace token and login:
+        ```
+        huggingface-cli login
+        ```
+        
         ## Getting Started
         ### Inferencing Pipeline
             
         Getting started with CodeTF is simple and quick with our model loading pipeline function ``load_model_pipeline()``. Here's an example showing how to load codet5+ model and perform inference on code generation task:
             
         ```python
         from codetf.models import load_model_pipeline
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.0 Summary: CodeTF: A
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1 Summary: CodeTF: A
 Transformer-based Library for Code Intelligence Home-page: https://github.com/
 Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
@@ -64,16 +64,23 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf ``` 3. Alternatively, build CodeTF from source: ```bash git clone https:
-//github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ``` ## Getting
+codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
+Additionally, to make sure the quantization feature works well, also install
+these dependencies: ```bash pip install -q -U git+https://github.com/
+huggingface/transformers.git pip install -q -U git+https://github.com/
+huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
+accelerate.git ``` For some models, such as [StarCoder](https://github.com/
+bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
+the HuggingFace token and login: ``` huggingface-cli login ``` ## Getting
 Started ### Inferencing Pipeline Getting started with CodeTF is simple and
 quick with our model loading pipeline function ``load_model_pipeline()``.
 Here's an example showing how to load codet5+ model and perform inference on
 code generation task: ```python from codetf.models import load_model_pipeline
 code_generation_model = load_model_pipeline(model_name="codet5",
 task="pretrained", model_type="plus-220M", is_eval=True, load_in_8bit=True,
 weight_sharding=False) result = code_generation_model.predict(["def
```

### Comparing `salesforce-codetf-1.0.0/README.md` & `salesforce-codetf-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,25 +83,37 @@
 ```bash
 conda create -n codetf python=3.8
 conda activate codetf
 ```
 
 2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
 ```bash
-pip install salesforce-codetf
+pip install salesforce-codetf==1.0.0
 ```
     
 3. Alternatively, build CodeTF from source:
 
 ```bash
 git clone https://github.com/salesforce/CodeTF.git
 cd CodeTF
 pip install -e .
 ```
 
+Additionally, to make sure the quantization feature works well, also install these dependencies:
+```bash
+pip install -q -U git+https://github.com/huggingface/transformers.git
+pip install -q -U git+https://github.com/huggingface/peft.git
+pip install -q -U git+https://github.com/huggingface/accelerate.git
+```
+
+For some models, such as [StarCoder](https://github.com/bigcode-project/starcoder), it is required to log in Huggingface. Please obtain the HuggingFace token and login:
+```
+huggingface-cli login
+```
+
 ## Getting Started
 ### Inferencing Pipeline
     
 Getting started with CodeTF is simple and quick with our model loading pipeline function ``load_model_pipeline()``. Here's an example showing how to load codet5+ model and perform inference on code generation task:
     
 ```python
 from codetf.models import load_model_pipeline
```

#### html2text {}

```diff
@@ -61,16 +61,23 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf ``` 3. Alternatively, build CodeTF from source: ```bash git clone https:
-//github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ``` ## Getting
+codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
+Additionally, to make sure the quantization feature works well, also install
+these dependencies: ```bash pip install -q -U git+https://github.com/
+huggingface/transformers.git pip install -q -U git+https://github.com/
+huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
+accelerate.git ``` For some models, such as [StarCoder](https://github.com/
+bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
+the HuggingFace token and login: ``` huggingface-cli login ``` ## Getting
 Started ### Inferencing Pipeline Getting started with CodeTF is simple and
 quick with our model loading pipeline function ``load_model_pipeline()``.
 Here's an example showing how to load codet5+ model and perform inference on
 code generation task: ```python from codetf.models import load_model_pipeline
 code_generation_model = load_model_pipeline(model_name="codet5",
 task="pretrained", model_type="plus-220M", is_eval=True, load_in_8bit=True,
 weight_sharding=False) result = code_generation_model.predict(["def
```

### Comparing `salesforce-codetf-1.0.0/codetf/__init__.py` & `salesforce-codetf-1.0.1/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-1.0.1/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/code_utility/ast_parser.py` & `salesforce-codetf-1.0.1/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/code_utility/base_utility.py` & `salesforce-codetf-1.0.1/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-1.0.1/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-1.0.1/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/common/registry.py` & `salesforce-codetf-1.0.1/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/common/utils.py` & `salesforce-codetf-1.0.1/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/configs/inference/causal_lm.yaml` & `salesforce-codetf-1.0.1/codetf/configs/inference/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/configs/inference/codet5.yaml` & `salesforce-codetf-1.0.1/codetf/configs/inference/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/configs/training/causal_lm.yaml` & `salesforce-codetf-1.0.1/codetf/configs/training/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/configs/training/codet5.yaml` & `salesforce-codetf-1.0.1/codetf/configs/training/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-1.0.1/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/base_dataset.py` & `salesforce-codetf-1.0.1/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-1.0.1/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-1.0.1/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-1.0.1/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/data_utility/util.py` & `salesforce-codetf-1.0.1/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/models/__init__.py` & `salesforce-codetf-1.0.1/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/models/base_model.py` & `salesforce-codetf-1.0.1/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/models/bert_models/__init__.py` & `salesforce-codetf-1.0.1/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-1.0.1/codetf/models/causal_lm_models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         )
    
     def forward(self, sources):
         encoding = self.tokenizer(sources, return_tensors='pt')
         input_ids = encoding.input_ids.to(self.device)
         attention_mask = encoding.attention_mask.to(self.device)
         generated_ids = self.model.generate(input_ids, attention_mask=attention_mask, 
-                                            max_length=self.max_prediction_length,
-                                            num_beams=self.beam_size)
+                                            max_length=self.max_prediction_length)
 
         predictions = self.tokenizer.batch_decode(generated_ids, truncate_before_pattern=[r"\n\n^#", "^'''", "\n\n\n"])
         return predictions
 
     def predict(self, sources):
         input_for_net = [' '.join(source.strip().split()).replace('\n', ' ') for source in sources]
         output = self.forward(input_for_net)
```

### Comparing `salesforce-codetf-1.0.0/codetf/models/seq2seq_models/__init__.py` & `salesforce-codetf-1.0.1/codetf/models/seq2seq_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/performance/evaluation_metric.py` & `salesforce-codetf-1.0.1/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/performance/model_evaluator.py` & `salesforce-codetf-1.0.1/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/trainer/base_trainer.py` & `salesforce-codetf-1.0.1/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-1.0.1/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-1.0.1/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/docs/conf.py` & `salesforce-codetf-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-1.0.1/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.0
+Version: 1.0.1
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
@@ -90,25 +90,37 @@
         ```bash
         conda create -n codetf python=3.8
         conda activate codetf
         ```
         
         2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
         ```bash
-        pip install salesforce-codetf
+        pip install salesforce-codetf==1.0.0
         ```
             
         3. Alternatively, build CodeTF from source:
         
         ```bash
         git clone https://github.com/salesforce/CodeTF.git
         cd CodeTF
         pip install -e .
         ```
         
+        Additionally, to make sure the quantization feature works well, also install these dependencies:
+        ```bash
+        pip install -q -U git+https://github.com/huggingface/transformers.git
+        pip install -q -U git+https://github.com/huggingface/peft.git
+        pip install -q -U git+https://github.com/huggingface/accelerate.git
+        ```
+        
+        For some models, such as [StarCoder](https://github.com/bigcode-project/starcoder), it is required to log in Huggingface. Please obtain the HuggingFace token and login:
+        ```
+        huggingface-cli login
+        ```
+        
         ## Getting Started
         ### Inferencing Pipeline
             
         Getting started with CodeTF is simple and quick with our model loading pipeline function ``load_model_pipeline()``. Here's an example showing how to load codet5+ model and perform inference on code generation task:
             
         ```python
         from codetf.models import load_model_pipeline
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.0 Summary: CodeTF: A
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1 Summary: CodeTF: A
 Transformer-based Library for Code Intelligence Home-page: https://github.com/
 Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
@@ -64,16 +64,23 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf ``` 3. Alternatively, build CodeTF from source: ```bash git clone https:
-//github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ``` ## Getting
+codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
+Additionally, to make sure the quantization feature works well, also install
+these dependencies: ```bash pip install -q -U git+https://github.com/
+huggingface/transformers.git pip install -q -U git+https://github.com/
+huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
+accelerate.git ``` For some models, such as [StarCoder](https://github.com/
+bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
+the HuggingFace token and login: ``` huggingface-cli login ``` ## Getting
 Started ### Inferencing Pipeline Getting started with CodeTF is simple and
 quick with our model loading pipeline function ``load_model_pipeline()``.
 Here's an example showing how to load codet5+ model and perform inference on
 code generation task: ```python from codetf.models import load_model_pipeline
 code_generation_model = load_model_pipeline(model_name="codet5",
 task="pretrained", model_type="plus-220M", is_eval=True, load_in_8bit=True,
 weight_sharding=False) result = code_generation_model.predict(["def
```

### Comparing `salesforce-codetf-1.0.0/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-1.0.1/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/setup.py` & `salesforce-codetf-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/transformers.git")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/peft.git")
     
 setup(
   name = 'salesforce-codetf',
-  version = "1.0.0",
+  version = "1.0.1",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   package_dir={"codeff": "codetf"},
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
```

### Comparing `salesforce-codetf-1.0.0/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-1.0.1/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_code_utilities/test_parse_code.py` & `salesforce-codetf-1.0.1/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-1.0.1/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-1.0.1/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_inference/test_codet5_multitask.py` & `salesforce-codetf-1.0.1/test_inference/test_codet5_multitask.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# import sys
-# from pathlib import Path
-# sys.path.append(str(Path(".").absolute().parent))
+import sys
+from pathlib import Path
+sys.path.append(str(Path(".").absolute().parent))
 from codetf.models import load_model_pipeline
 
 translation_model = load_model_pipeline(model_name="codet5", task="translate_cs_java",
             model_type="base", is_eval=True, 
             load_in_4bit=True, weight_sharding=False)
 
 summarization_model = load_model_pipeline(model_name="codet5", task="sum_python",
```

### Comparing `salesforce-codetf-1.0.0/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-1.0.1/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-1.0.1/test_trainer/test_codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.0/test_trainer/test_t5_trainer.py` & `salesforce-codetf-1.0.1/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

