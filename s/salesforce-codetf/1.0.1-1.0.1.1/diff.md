# Comparing `tmp/salesforce-codetf-1.0.1.tar.gz` & `tmp/salesforce-codetf-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-1.0.1.tar", last modified: Fri Jun  2 21:59:45 2023, max compression
+gzip compressed data, was "salesforce-codetf-1.0.1.1.tar", last modified: Sat Jun  3 04:14:00 2023, max compression
```

## Comparing `salesforce-codetf-1.0.1.tar` & `salesforce-codetf-1.0.1.1.tar`

### file list

```diff
@@ -1,93 +1,143 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.682083 salesforce-codetf-1.0.1/
--rw-r--r--   0 nghi.bui   (503) staff       (20)       39 2023-06-02 21:30:18.000000 salesforce-codetf-1.0.1/MANIFEST.in
--rw-r--r--   0 nghi.bui   (503) staff       (20)    26341 2023-06-02 21:59:45.682619 salesforce-codetf-1.0.1/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    22981 2023-06-02 21:58:59.000000 salesforce-codetf-1.0.1/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.643151 salesforce-codetf-1.0.1/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.644958 salesforce-codetf-1.0.1/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.645824 salesforce-codetf-1.0.1/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.646788 salesforce-codetf-1.0.1/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.647639 salesforce-codetf-1.0.1/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.648650 salesforce-codetf-1.0.1/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-1.0.1/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.649652 salesforce-codetf-1.0.1/codetf/configs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:28:24.000000 salesforce-codetf-1.0.1/codetf/configs/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.650183 salesforce-codetf-1.0.1/codetf/configs/dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      328 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/dataset/dataset.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)      131 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1/codetf/configs/default.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.651670 salesforce-codetf-1.0.1/codetf/configs/inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      480 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/configs/inference/bert.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2852 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/configs/inference/causal_lm.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/configs/inference/codet5.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.652687 salesforce-codetf-1.0.1/codetf/configs/training/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      766 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/training/causal_lm.yaml
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1020 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/configs/training/codet5.yaml
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.656076 salesforce-codetf-1.0.1/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.657425 salesforce-codetf-1.0.1/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.657940 salesforce-codetf-1.0.1/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.658427 salesforce-codetf-1.0.1/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3375 2023-06-02 21:54:25.000000 salesforce-codetf-1.0.1/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.658911 salesforce-codetf-1.0.1/codetf/models/seq2seq_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/codetf/models/seq2seq_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.660425 salesforce-codetf-1.0.1/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.662016 salesforce-codetf-1.0.1/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.662568 salesforce-codetf-1.0.1/docs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-1.0.1/docs/conf.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.666782 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    26341 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2385 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      319 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       42 2023-06-02 21:59:45.000000 salesforce-codetf-1.0.1/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 21:59:45.683694 salesforce-codetf-1.0.1/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1644 2023-06-02 21:59:34.000000 salesforce-codetf-1.0.1/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.670413 salesforce-codetf-1.0.1/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.671177 salesforce-codetf-1.0.1/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.672833 salesforce-codetf-1.0.1/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.678767 salesforce-codetf-1.0.1/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      448 2023-06-02 21:55:53.000000 salesforce-codetf-1.0.1/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 21:47:19.000000 salesforce-codetf-1.0.1/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_inference/test_load_model_zoo.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:59:45.681365 salesforce-codetf-1.0.1/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 21:34:03.000000 salesforce-codetf-1.0.1/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-1.0.1/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.718792 salesforce-codetf-1.0.1.1/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       91 2023-06-03 04:13:13.000000 salesforce-codetf-1.0.1.1/MANIFEST.in
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    26343 2023-06-03 04:14:00.719313 salesforce-codetf-1.0.1.1/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    22981 2023-06-02 22:06:30.000000 salesforce-codetf-1.0.1.1/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.404484 salesforce-codetf-1.0.1.1/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1.1/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.407239 salesforce-codetf-1.0.1.1/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.408446 salesforce-codetf-1.0.1.1/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.409667 salesforce-codetf-1.0.1.1/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.410745 salesforce-codetf-1.0.1.1/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.412152 salesforce-codetf-1.0.1.1/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-1.0.1.1/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1.1/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.413814 salesforce-codetf-1.0.1.1/codetf/configs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:28:24.000000 salesforce-codetf-1.0.1.1/codetf/configs/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.414652 salesforce-codetf-1.0.1.1/codetf/configs/dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      328 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/configs/dataset/dataset.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      131 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.1.1/codetf/configs/default.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.416710 salesforce-codetf-1.0.1.1/codetf/configs/inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      480 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/codetf/configs/inference/bert.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2852 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/configs/inference/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/configs/inference/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.418192 salesforce-codetf-1.0.1.1/codetf/configs/training/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      766 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/configs/training/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1020 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/configs/training/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.422337 salesforce-codetf-1.0.1.1/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1.1/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.423733 salesforce-codetf-1.0.1.1/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.424533 salesforce-codetf-1.0.1.1/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.425458 salesforce-codetf-1.0.1.1/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3375 2023-06-02 21:54:25.000000 salesforce-codetf-1.0.1.1/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.426445 salesforce-codetf-1.0.1.1/codetf/models/seq2seq_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.428743 salesforce-codetf-1.0.1.1/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1.1/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.1.1/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.431457 salesforce-codetf-1.0.1.1/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.400014 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.548279 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   623752 2023-04-02 14:02:02.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/apex.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   517568 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/bash.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   361144 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/c.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  3032464 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/c_sharp.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  1217512 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/cpp.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    99680 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/css.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   236232 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/elm.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   230128 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/go.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  8532424 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/haskell.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   149608 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/html.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   262848 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/java.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   280160 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/javascript.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  4604424 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/kotlin.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   198688 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/lua.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   432360 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/php.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   254160 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/python.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  1098880 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/ruby.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   804520 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/rust.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   263848 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/scala.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   590536 2023-02-08 02:55:51.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/solidity.so
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   164488 2023-04-02 14:04:27.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/soql.so
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   180872 2023-04-02 14:02:15.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Darwin/sosl.so
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.690712 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   533096 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/apex.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   160688 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/asm.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   704688 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/bash.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   442184 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/c.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  3112856 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/c_sharp.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  1512216 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/cpp.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   137144 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/css.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   442568 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/elm.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   301056 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/go.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  4731648 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/haskell.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   950536 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/html.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   315720 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/java.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   343560 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/javascript.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  4924440 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/kotlin.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   234240 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/lua.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   623208 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/php.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   352352 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/python.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)  1364728 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/ruby.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   902504 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/rust.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   309752 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/scala.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   727704 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/solidity.so
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   127040 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/soql.so
+-rwxr-xr-x   0 nghi.bui   (503) staff       (20)   139328 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/sosl.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20) 18164400 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/verilog.so
+-rw-r--r--   0 nghi.bui   (503) staff       (20)   445224 2023-04-11 11:45:20.000000 salesforce-codetf-1.0.1.1/codetf/tree-sitter-prebuilts/Linux/yaml.so
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.695288 salesforce-codetf-1.0.1.1/docs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-1.0.1.1/docs/conf.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.700232 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    26343 2023-06-03 04:14:00.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4452 2023-06-03 04:14:00.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-03 04:14:00.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      319 2023-06-03 04:14:00.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       42 2023-06-03 04:14:00.000000 salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-03 04:14:00.720394 salesforce-codetf-1.0.1.1/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1646 2023-06-03 04:13:51.000000 salesforce-codetf-1.0.1.1/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.704329 salesforce-codetf-1.0.1.1/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1.1/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.705148 salesforce-codetf-1.0.1.1/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.706879 salesforce-codetf-1.0.1.1/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.1.1/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.1.1/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.713843 salesforce-codetf-1.0.1.1/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.1.1/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      479 2023-06-02 22:05:23.000000 salesforce-codetf-1.0.1.1/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 22:00:11.000000 salesforce-codetf-1.0.1.1/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 21:47:19.000000 salesforce-codetf-1.0.1.1/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-03 04:14:00.717549 salesforce-codetf-1.0.1.1/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.1.1/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 21:34:03.000000 salesforce-codetf-1.0.1.1/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-1.0.1.1/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-1.0.1/PKG-INFO` & `salesforce-codetf-1.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.1
+Version: 1.0.1.1
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
@@ -90,15 +90,15 @@
         ```bash
         conda create -n codetf python=3.8
         conda activate codetf
         ```
         
         2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
         ```bash
-        pip install salesforce-codetf==1.0.0
+        pip install salesforce-codetf==1.0.1
         ```
             
         3. Alternatively, build CodeTF from source:
         
         ```bash
         git clone https://github.com/salesforce/CodeTF.git
         cd CodeTF
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1 Summary: CodeTF: A
-Transformer-based Library for Code Intelligence Home-page: https://github.com/
-Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1.1 Summary: CodeTF:
+A Transformer-based Library for Code Intelligence Home-page: https://
+github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
+Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
 (#installation-guide) - [Getting Started](#getting-started) - [Inferencing
 Pipeline](#inferencing-pipeline) - [Model Zoo](#model-zoo) - [Fine-Tuning Your
@@ -64,15 +65,15 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+codetf==1.0.1 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
 https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
 Additionally, to make sure the quantization feature works well, also install
 these dependencies: ```bash pip install -q -U git+https://github.com/
 huggingface/transformers.git pip install -q -U git+https://github.com/
 huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
 accelerate.git ``` For some models, such as [StarCoder](https://github.com/
 bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
```

### Comparing `salesforce-codetf-1.0.1/README.md` & `salesforce-codetf-1.0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 ```bash
 conda create -n codetf python=3.8
 conda activate codetf
 ```
 
 2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
 ```bash
-pip install salesforce-codetf==1.0.0
+pip install salesforce-codetf==1.0.1
 ```
     
 3. Alternatively, build CodeTF from source:
 
 ```bash
 git clone https://github.com/salesforce/CodeTF.git
 cd CodeTF
```

#### html2text {}

```diff
@@ -61,15 +61,15 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+codetf==1.0.1 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
 https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
 Additionally, to make sure the quantization feature works well, also install
 these dependencies: ```bash pip install -q -U git+https://github.com/
 huggingface/transformers.git pip install -q -U git+https://github.com/
 huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
 accelerate.git ``` For some models, such as [StarCoder](https://github.com/
 bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
```

### Comparing `salesforce-codetf-1.0.1/codetf/__init__.py` & `salesforce-codetf-1.0.1.1/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-1.0.1.1/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/code_utility/ast_parser.py` & `salesforce-codetf-1.0.1.1/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/code_utility/base_utility.py` & `salesforce-codetf-1.0.1.1/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-1.0.1.1/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-1.0.1.1/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/common/registry.py` & `salesforce-codetf-1.0.1.1/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/common/utils.py` & `salesforce-codetf-1.0.1.1/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/configs/inference/causal_lm.yaml` & `salesforce-codetf-1.0.1.1/codetf/configs/inference/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/configs/inference/codet5.yaml` & `salesforce-codetf-1.0.1.1/codetf/configs/inference/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/configs/training/causal_lm.yaml` & `salesforce-codetf-1.0.1.1/codetf/configs/training/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/configs/training/codet5.yaml` & `salesforce-codetf-1.0.1.1/codetf/configs/training/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/base_dataset.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/data_utility/util.py` & `salesforce-codetf-1.0.1.1/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/models/__init__.py` & `salesforce-codetf-1.0.1.1/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/models/base_model.py` & `salesforce-codetf-1.0.1.1/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/models/bert_models/__init__.py` & `salesforce-codetf-1.0.1.1/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-1.0.1.1/codetf/models/causal_lm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/models/seq2seq_models/__init__.py` & `salesforce-codetf-1.0.1.1/codetf/models/seq2seq_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/performance/evaluation_metric.py` & `salesforce-codetf-1.0.1.1/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/performance/model_evaluator.py` & `salesforce-codetf-1.0.1.1/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/trainer/base_trainer.py` & `salesforce-codetf-1.0.1.1/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-1.0.1.1/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-1.0.1.1/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/docs/conf.py` & `salesforce-codetf-1.0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-1.0.1.1/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.1
+Version: 1.0.1.1
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
@@ -90,15 +90,15 @@
         ```bash
         conda create -n codetf python=3.8
         conda activate codetf
         ```
         
         2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
         ```bash
-        pip install salesforce-codetf==1.0.0
+        pip install salesforce-codetf==1.0.1
         ```
             
         3. Alternatively, build CodeTF from source:
         
         ```bash
         git clone https://github.com/salesforce/CodeTF.git
         cd CodeTF
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1 Summary: CodeTF: A
-Transformer-based Library for Code Intelligence Home-page: https://github.com/
-Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.1.1 Summary: CodeTF:
+A Transformer-based Library for Code Intelligence Home-page: https://
+github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
+Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
 (#installation-guide) - [Getting Started](#getting-started) - [Inferencing
 Pipeline](#inferencing-pipeline) - [Model Zoo](#model-zoo) - [Fine-Tuning Your
@@ -64,15 +65,15 @@
 1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
 Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
 CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
 CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
 Installation Guide 1. (Optional) Creating conda environment ```bash conda
 create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
 (https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
-codetf==1.0.0 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
+codetf==1.0.1 ``` 3. Alternatively, build CodeTF from source: ```bash git clone
 https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
 Additionally, to make sure the quantization feature works well, also install
 these dependencies: ```bash pip install -q -U git+https://github.com/
 huggingface/transformers.git pip install -q -U git+https://github.com/
 huggingface/peft.git pip install -q -U git+https://github.com/huggingface/
 accelerate.git ``` For some models, such as [StarCoder](https://github.com/
 bigcode-project/starcoder), it is required to log in Huggingface. Please obtain
```

### Comparing `salesforce-codetf-1.0.1/setup.py` & `salesforce-codetf-1.0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/transformers.git")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/peft.git")
     
 setup(
   name = 'salesforce-codetf',
-  version = "1.0.1",
+  version = "1.0.1.1",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   package_dir={"codeff": "codetf"},
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
```

### Comparing `salesforce-codetf-1.0.1/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-1.0.1.1/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_code_utilities/test_parse_code.py` & `salesforce-codetf-1.0.1.1/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-1.0.1.1/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-1.0.1.1/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-1.0.1.1/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-1.0.1.1/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_inference/test_codet5_multitask.py` & `salesforce-codetf-1.0.1.1/test_inference/test_codet5_multitask.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-1.0.1.1/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-1.0.1.1/test_trainer/test_codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.1/test_trainer/test_t5_trainer.py` & `salesforce-codetf-1.0.1.1/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

