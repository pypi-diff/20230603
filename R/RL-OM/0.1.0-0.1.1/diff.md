# Comparing `tmp/RL_OM-0.1.0.tar.gz` & `tmp/RL_OM-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.1.0.tar", last modified: Thu Jun  1 16:44:22 2023, max compression
+gzip compressed data, was "RL_OM-0.1.1.tar", last modified: Sat Jun  3 18:14:17 2023, max compression
```

## Comparing `RL_OM-0.1.0.tar` & `RL_OM-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.092641 RL_OM-0.1.0/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.1.0/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.1.0/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:44:22.092503 RL_OM-0.1.0/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.1.0/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.085722 RL_OM-0.1.0/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   131239 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.086952 RL_OM-0.1.0/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.087206 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.087806 RL_OM-0.1.0/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.088282 RL_OM-0.1.0/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      929 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.089241 RL_OM-0.1.0/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.090152 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.090971 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.091759 RL_OM-0.1.0/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     3783 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.092268 RL_OM-0.1.0/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.086804 RL_OM-0.1.0/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.1.0/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-01 16:43:27.000000 RL_OM-0.1.0/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-01 16:44:22.092695 RL_OM-0.1.0/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.1.0/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.791353 RL_OM-0.1.1/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.1.1/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.1.1/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-03 18:14:17.791202 RL_OM-0.1.1/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.1.1/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.783570 RL_OM-0.1.1/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   131239 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.785835 RL_OM-0.1.1/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.786090 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5975 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.786625 RL_OM-0.1.1/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.787040 RL_OM-0.1.1/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1141 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.787961 RL_OM-0.1.1/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.789135 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.789989 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.790714 RL_OM-0.1.1/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4407 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    11345 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.791001 RL_OM-0.1.1/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     7822 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.785680 RL_OM-0.1.1/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.1.1/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-03 18:13:53.000000 RL_OM-0.1.1/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-03 18:14:17.791396 RL_OM-0.1.1/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.1.1/setup.py
```

### Comparing `RL_OM-0.1.0/LICENSE` & `RL_OM-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/PKG-INFO` & `RL_OM-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.1.0/RL_OM/_modidx.py` & `RL_OM-0.1.1/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.1.1/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """
     Agent implementing the Economic Order Quantity (EOQ) policy.
 
     Args:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
         s (numpy.ndarray): The fixed ordering cost.
         h (numpy.ndarray): The holding cost per unit per period.
+        l (numpy.ndarray): The lead time per product.
         preprocessors (list): List of preprocessors to be applied to the state.
         postprocessors (list): List of postprocessors to be applied to the policy.
         agent_name (str): Name of the agent. If set to None will use some default name.
         precision (int): Number of decimal places to round the demand input to.
 
     Attributes:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
@@ -34,24 +35,26 @@
     """
 
 
     def __init__(self,
                   mdp_info,
                   s, # fixed ordering cost
                   h, # holding cost per unit per period
+                  l = None, # lead time
                   preprocessors = None,
                   postprocessors = None,
                   agent_name = None,
                   precision = 5
         ):
 
         policy = EOQPolicy(
             d = None,
             s = s,
             h = h,
+            l = l,
             preprocessors = preprocessors,
             postprocessors = postprocessors
         )
 
         self.precision=precision
 
         if agent_name is None:
@@ -91,36 +94,40 @@
 
     Notethat d, s, and h must all have the shape (num_products,)
 
     Args:
         d (numpy.ndarray): The (average) demand per period for each product.
         s (numpy.ndarray): The fixed ordering cost for each product.
         h (numpy.ndarray): The holding cost per unit per period for each product.
+        l (numpy.ndarray): The lead time per product.
         postprocessors (list): List of postprocessors to be applied to the action.
 
     Attributes:
         d (numpy.ndarray): The (average) demand per period for each product.
         s (numpy.ndarray): The fixed ordering cost for each product.
         h (numpy.ndarray): The holding cost per unit per period for each product.
+        l (numpy.ndarray): The lead time per product.
         num_products (int): The number of products.
         q_star (numpy.ndarray): The optimal order quantity per product.
         postprocessors (list): List of postprocessors to be applied to the action.
 
     """
 
     def __init__(self,
                  d, 
                  s, 
                  h, 
+                 l = None,
                  preprocessors = None,
                  postprocessors = None
                  ):
         self.d = d
         self.s = s
         self.h = h
+        self.l = l
         self.num_products = len(s)
         self.q_star = None
         if preprocessors is None:
             self.preprocessors = []
         else:
             self.preprocessors = (preprocessors)
         if postprocessors is None:
@@ -138,38 +145,47 @@
         Returns:
             None
 
         """
 
         self.q_star = np.sqrt((2*self.s*self.d)/self.h)
 
-    def draw_action(self, inventory_level):
+    def draw_action(self, input):
 
         """
         Generate an action based on the current state.
 
         Returns zero for products which have still sufficient inventory, and the optimal order quantity for products which are running out of stock.
 
         Parameters:
-            inventory_level (numpy.ndarray): The current inventory level for each product. Shape must be (num_products,).
+            input (numpy.ndarray): The current inventory level and potentially order pipeline for each product.
 
         Returns:
             numpy.ndarray: The action to be taken, indicating the quantity to order for each product.
 
         """
 
         assert self.q_star is not None, "q_star is not set"
 
         action = np.zeros(self.num_products)
 
         for preprocessor in self.preprocessors:
-            inventory_level = preprocessor(inventory_level)
+            input = preprocessor(input)
 
         # TODO account for lead time
-        action = np.where(inventory_level >= self.d, 0, self.q_star)
+
+        if self.l is None:
+            action = np.where(input >= self.d, 0, self.q_star)
+
+        else:
+            pipeline_vector = input[self.num_products:]
+            pipeline = np.reshape(pipeline_vector, (self.num_products, max(self.l)))
+            pipeline_sum = np.sum(pipeline, axis=1)
+            input = input[:self.num_products]
+            action = np.where((input >= self.d + (self.d * self.l)) or (pipeline_sum != 0), 0, self.q_star)
 
         for postprocessor in self.postprocessors:
             action = postprocessor(action)
 
         return action
     
     def reset(self):
```

### Comparing `RL_OM-0.1.0/RL_OM/agents/networks/actors.py` & `RL_OM-0.1.1/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/networks/base.py` & `RL_OM-0.1.1/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/networks/critics.py` & `RL_OM-0.1.1/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.1.1/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,16 +15,20 @@
     Args:
         num_features (int): Number of features in the state.
         num_products (int): Number of products in the state.
 
     """
     
 
-    def __init__(self, num_features, num_products):
+    def __init__(self, num_features, num_products, max_l = None):
         self.num_features = num_features
         self.num_products = num_products
+        self.max_l = max_l
     
     def __call__(self, input):
-        assert len(input) == self.num_features + self.num_products
+        #assert len(input) == self.num_features + self.num_products
         assert len(input.shape) == 1
         
-        return input[self.num_features:self.num_features+self.num_products]
+        if self.max_l is not None:
+            return input[self.num_features:self.num_features+self.num_products+np.max(self.max_l)*self.num_products]
+        else:
+            return input[self.num_features:self.num_features+self.num_products]
```

### Comparing `RL_OM-0.1.0/RL_OM/agents/processors/processors.py` & `RL_OM-0.1.1/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/environments/calculation_functions.py` & `RL_OM-0.1.1/RL_OM/environments/calculation_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,23 @@
 
     fixed_ordering_cost_step = get_fixed_ordering_cost(self, action, positive_only = True)
 
     # todo: add variable ordering cost:
         # variable cost positive order ...
         # variable cost negative order would build on overage cost
 
-    self.inventory += action # first, the order will be added to inventory (meaning lead-time is 0)
+    if self.use_order_pipeline:
+        orders_arriving = self.order_pipeline[:,-1]
+            # Move elements one slot to the right in order_pipeline
+        self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
+        self.order_pipeline[:, 0] = action
+    else:
+        orders_arriving = action
+
+    self.inventory += orders_arriving # first, the order will be added to inventory (meaning lead-time is 0)
 
     self.inventory = np.maximum(self.inventory, 0) # inventory cannot be negative
 
     self.inventory = np.minimum(self.inventory, self.inventory_cap) # inventory cannot be higher than inventory_cap
 
     self.inventory -= self.demand[self.period, :] # Then demand is subtracted from inventory
 
@@ -37,32 +45,39 @@
 
     info = dict()
 
     self.period += 1
 
     return reward, info
 
-
 # %% ../../nbs/environments/10_calculation_functions.ipynb 8
 def rq_calculations(self, action):
 
     # TODO Think about naming of the function
     
     r = action[0]
     q = action[1]
 
     order = np.where(self.inventory <= r, q, 0)
 
     fixed_ordering_cost_step = get_fixed_ordering_cost(self, order, positive_only = True)
 
+    if self.use_order_pipeline:
+        orders_arriving = self.order_pipeline[:,-1]
+            # Move elements one slot to the right in order_pipeline
+        self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
+        self.order_pipeline[:, 0] = order
+    else:
+        orders_arriving = order
+
     # todo: add variable ordering cost:
         # variable cost positive order ...
         # variable cost negative order would build on overage cost
 
-    self.inventory += order # first, the order will be added to inventory (meaning lead-time is 0)
+    self.inventory += orders_arriving # first, the order will be added to inventory (meaning lead-time is 0)
 
     self.inventory = np.maximum(self.inventory, 0) # inventory cannot be negative
 
     self.inventory = np.minimum(self.inventory, self.inventory_cap) # inventory cannot be higher than inventory_cap
 
     self.inventory -= self.demand[self.period, :] # Then demand is subtracted from inventory
```

### Comparing `RL_OM-0.1.0/RL_OM/environments/data_generators.py` & `RL_OM-0.1.1/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/environments/feature_converters.py` & `RL_OM-0.1.1/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.1.1/RL_OM/environments/multi_period_inventory.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,16 @@
 
         if not self.inventory_allowed:
             assert holding_cost is None, "If inventory is not allowed, holding_cost must be None"
         self.holding_cost = holding_cost
 
         if np.all(lead_time == 0):
             self.use_order_pipeline = False
+        else:
+            self.use_order_pipeline = True
 
         self.lead_time = lead_time
         self.lead_time_variance = lead_time_variance
 
         if np.all(lead_time_variance == 0):
             self.max_lead_time = self.lead_time
         else:
@@ -207,48 +209,57 @@
         if demand_backlog:
             low_limit[self.num_features+inventory_space+order_pipeline_space:self.num_features+inventory_space+order_pipeline_space+demand_backlog_space] = 0
             high_limit[self.num_features+inventory_space+order_pipeline_space:self.num_features+inventory_space+order_pipeline_space+demand_backlog_space] = self.max_demand_backlog
 
         self.observation_space = Box(low_limit, high_limit, shape=(total_obs_space_lenght,))
 
     def reset(self, state = None):
-        
+
         # TODO: Check in mushroom where state would come from and implement here
-        self.period = np.random.choice(self.num_observations-self._mdp_info.horizon)
+        if self.num_observations == self._mdp_info.horizon:
+            self.period = 0
+        else:
+            self.period = np.random.choice(self.num_observations-self._mdp_info.horizon)
+        print("reset with period {}".format(self.period))
         self.demand_backlog = np.zeros(self.num_products)
         self.inventory = self.start_inventory.copy()
-        self.order_pipeline = np.zeros(sum((self.num_products*self.max_lead_time)))
+        self.order_pipeline = np.zeros((self.num_products,np.max(self.max_lead_time)))
 
         self.set_observation_state()
 
         return self.observation_state
 
     def set_observation_state(self):
         
         # TODO: check if this is computationally expensive
         # TODO: make sure this is consistent if some elements are there but not tracked in state
 
-        self.observation_state = np.zeros(self.observation_space.shape)
+        if self.period >= self.num_observations:
+            self.observation_state = np.zeros(self.observation_space.shape)
+        
+        else:
+
+            self.observation_state = np.zeros(self.observation_space.shape)
 
-        if self.num_features > 0:
-            self.observation_state[:self.num_features] = self.features[self.period]
+            if self.num_features > 0:
+                self.observation_state[:self.num_features] = self.features[self.period]
 
-        if self.inventory_allowed:
-            self.observation_state[self.num_features:self.num_features+self.num_products] = self.inventory
+            if self.inventory_allowed:
+                self.observation_state[self.num_features:self.num_features+self.num_products] = self.inventory
 
-        if self.use_order_pipeline:
-            slots_occupied = 0
-            for product in range(self.num_products):
-                self.observation_state[self.num_features+self.num_products+slots_occupied:self.num_features+self.num_products+slots_occupied+self.max_lead_time[product]] = self.order_pipeline[product]
-                slots_occupied += self.max_lead_time[product]
+            if self.use_order_pipeline:
+                slots_occupied = 0
+                for product in range(self.num_products):
+                    self.observation_state[self.num_features+self.num_products+slots_occupied:self.num_features+self.num_products+slots_occupied+self.max_lead_time[product]] = self.order_pipeline[product]
+                    slots_occupied += self.max_lead_time[product]
 
-        if self.max_demand_backlog > 0:
-            self.observation_state[self.num_features+self.num_products+np.sum(self.num_products * self.lead_time):] = self.demand_backlog
+            if self.max_demand_backlog > 0:
+                self.observation_state[self.num_features+self.num_products+np.sum(self.num_products * self.lead_time):] = self.demand_backlog
 
-        self.observation_state = np.round(self.observation_state, self.precision)
+            self.observation_state = np.round(self.observation_state, self.precision)
 
 
     def step(self, action):
 
         absorbing = False
 
         reward, info = self.calculations(self, action)
```

### Comparing `RL_OM-0.1.0/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.1.1/RL_OM/experiment_functions/run_experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 # %% ../../nbs/experiment_functions/01_run_experiment.ipynb 6
 def experiment_stepwise(mdp,
                         run_params,
                         n_epochs,
                         n_steps,
                         n_episodes_test,
+                        mdp_test = None,
                         rand_seed = None,
                         logger_dir = "./results/loggers",
                         results_dir = "./results",
                         dataset_log_freq = None):
 
     """
     TODO 1: Add function to (deep)save the entire agent to be able to reloead it later and potentially continue training.
@@ -64,31 +65,41 @@
     filename = f"{logger_dir}/logger_{agent.name}_{run}.pkl"
     os.makedirs(os.path.dirname(filename), exist_ok=True)
     pickle.dump(logger, open(f"{logger_dir}/logger_{agent.name}_{run}.pkl", "wb"))
 
     # ensure mdp starts from the same state
     mdp.reset()
 
+    if mdp_test is not None:
+        mdp_test.reset(state=0)
+
     # Start training
 
     logger.strong_line()
     logger.info('Experiment Algorithm: ' + agent.name)
 
+    core = Core(agent, mdp)
+    if mdp_test is not None:
+        core_test = Core(agent, mdp_test)
+
     try:
         if agent.train_directly:
             agent.fit(mdp.demand)
-            core = Core(agent, mdp)
 
-    
     except:
    
-        core = Core(agent, mdp)
+        if mdp_test is not None:
+            core_test = Core(agent, mdp_test)
+        
 
         ### Initial evaluation
-        dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+        if mdp_test is not None:
+            dataset = core_test.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+        else:
+            dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
         s, *_ = parse_dataset(dataset)
 
         J = np.mean(compute_J(dataset, mdp.info.gamma))
         R = np.mean(compute_J(dataset))
         try:
             E = agent.policy.entropy(s)
         except:
@@ -100,15 +111,18 @@
 
         ### Training
         initial_replay_size = agent._replay_memory._initial_size
         core.learn(n_steps=initial_replay_size, n_steps_per_fit=initial_replay_size, quiet=True)
 
         for n in trange(n_epochs, leave=False):
             core.learn(n_steps=n_steps, n_steps_per_fit=1, quiet = True)
-            dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+            if mdp_test is not None:
+                dataset = core_test.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+            else:
+                dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
             s, *_ = parse_dataset(dataset)
 
             J = np.mean(compute_J(dataset, mdp.info.gamma))
             R = np.mean(compute_J(dataset))
             try:
                 E = agent.policy.entropy(s)
             except:
@@ -119,15 +133,18 @@
 
             if dataset_log_freq is not None:
                 if n % dataset_log_freq == 0:
                     logger.log_dataset(dataset, name_addition = f"_epoch_{n+1}")
         
         ### Final evaluation
     
-    dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet=True)
+    if mdp_test is not None:
+        dataset = core_test.evaluate(n_episodes=n_episodes_test, render=False, quiet=True)
+    else:
+        dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet=True)
     
     s, *_ = parse_dataset(dataset)
 
     J = np.mean(compute_J(dataset, mdp.info.gamma))
     R = np.mean(compute_J(dataset))
     try:
         E = agent.policy.entropy(s)
@@ -142,14 +159,15 @@
 
 # %% ../../nbs/experiment_functions/01_run_experiment.ipynb 7
 def experiment_stepwise_no_log(mdp,
                         agent,
                         n_epochs,
                         n_steps,
                         n_episodes_test,
+                        mdp_test = None,
                         rand_seed = None,
                         dataset_log_freq = None):
 
     """
     TODO 1: Add function to (deep)save the entire agent to be able to reloead it later and potentially continue training.
     TODO 2: Provide functionalita to turn of exploration during evaluation (e.g., epsilon=0 for DQN, sample_mean for SAC)
 
@@ -169,26 +187,34 @@
     """
 
     if rand_seed is not None:
         np.random.seed(rand_seed)
         torch.manual_seed(rand_seed)
 
     # ensure mdp starts from the same state
-    mdp.reset()
+    if mdp_test is not None:
+        mdp_test.reset()
+    else:
+        mdp.reset()
 
     core = Core(agent, mdp)
+    if mdp_test is not None:
+        core_test = Core(agent, mdp_test)
 
     ### Training
     initial_replay_size = agent._replay_memory._initial_size
     core.learn(n_steps=initial_replay_size, n_steps_per_fit=initial_replay_size, quiet=True)
 
     R_hist = []
 
     for n in trange(n_epochs, leave=False):
         core.learn(n_steps=n_steps, n_steps_per_fit=1, quiet = True)
-        dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+        if mdp_test is not None:
+            dataset = core_test.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+        else:
+            dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
 
         R = np.mean(compute_J(dataset))
 
         R_hist.append(R)
         
     return R_hist
```

### Comparing `RL_OM-0.1.0/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.1.1/RL_OM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.1.0/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.1.1/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.0/settings.ini` & `RL_OM-0.1.1/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.1.0/setup.py` & `RL_OM-0.1.1/setup.py`

 * *Files identical despite different names*

