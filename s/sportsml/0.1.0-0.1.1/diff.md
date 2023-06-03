# Comparing `tmp/sportsml-0.1.0.tar.gz` & `tmp/sportsml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportsml-0.1.0.tar", last modified: Sat Jun  3 16:19:31 2023, max compression
+gzip compressed data, was "sportsml-0.1.1.tar", last modified: Sat Jun  3 16:56:10 2023, max compression
```

## Comparing `sportsml-0.1.0.tar` & `sportsml-0.1.1.tar`

### file list

```diff
@@ -1,81 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.779678 sportsml-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:19:31.778678 sportsml-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-03 16:19:24.000000 sportsml-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-03 16:19:24.000000 sportsml-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 16:19:31.779678 sportsml-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-03 16:19:24.000000 sportsml-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.770678 sportsml-0.1.0/sportsml/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.771678 sportsml-0.1.0/sportsml/cbb/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cbb/data/
--rw-rw-rw-   0 root         (0) root         (0)     4374 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/datamodule.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)     8378 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/predict/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/predict/conf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/predict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/cli/train/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/cli/train/conf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/layers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/layers/gnn/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.774678 sportsml-0.1.0/sportsml/layers/gnn/encoder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/gcn.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/mean.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/nn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.774678 sportsml-0.1.0/sportsml/layers/gnn/predictor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/predictor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/predictor/nn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/gnn.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/mlp.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/mongo/
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/averages.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/client.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/model_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/nba/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.776678 sportsml-0.1.0/sportsml/nba/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7363 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/datamodule.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     5442 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.777678 sportsml-0.1.0/sportsml/nfl/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.777678 sportsml-0.1.0/sportsml/nfl/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4363 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.778678 sportsml-0.1.0/sportsml/odds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/client.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.778678 sportsml-0.1.0/sportsml/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/utils/ensemble.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.771678 sportsml-0.1.0/sportsml.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1627 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.573093 sportsml-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-03 16:56:03.000000 sportsml-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:56:10.573093 sportsml-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-03 16:56:03.000000 sportsml-0.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-03 16:56:03.000000 sportsml-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 16:56:10.573093 sportsml-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-03 16:56:03.000000 sportsml-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.560093 sportsml-0.1.1/sportsml/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.561093 sportsml-0.1.1/sportsml/cbb/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.562093 sportsml-0.1.1/sportsml/cbb/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     8378 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cbb/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.562093 sportsml-0.1.1/sportsml/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.563093 sportsml-0.1.1/sportsml/cli/predict/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.563093 sportsml-0.1.1/sportsml/cli/predict/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/conf.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.563093 sportsml-0.1.1/sportsml/cli/predict/conf/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/graph/cbb.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/graph/nba.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.564093 sportsml-0.1.1/sportsml/cli/predict/conf/team_map/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/team_map/cbb.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/conf/team_map/nba.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/predict/predict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.564093 sportsml-0.1.1/sportsml/cli/train/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.564093 sportsml-0.1.1/sportsml/cli/train/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/conf.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.565093 sportsml-0.1.1/sportsml/cli/train/conf/dm/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/dm/cbb.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/dm/nba.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.565093 sportsml-0.1.1/sportsml/cli/train/conf/model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.565093 sportsml-0.1.1/sportsml/cli/train/conf/model/encoder/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/model/encoder/gcn.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/model/encoder/mean.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/model/encoder/nn.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/model/gnn.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.565093 sportsml-0.1.1/sportsml/cli/train/conf/model/predictor/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/model/predictor/nn.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.566093 sportsml-0.1.1/sportsml/cli/train/conf/trainer/
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/trainer/early_stopping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/conf/trainer/prod.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/cli/train/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.566093 sportsml-0.1.1/sportsml/layers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.566093 sportsml-0.1.1/sportsml/layers/gnn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.567093 sportsml-0.1.1/sportsml/layers/gnn/encoder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/encoder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/encoder/gcn.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/encoder/mean.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/encoder/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.567093 sportsml-0.1.1/sportsml/layers/gnn/predictor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/predictor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/layers/gnn/predictor/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.568093 sportsml-0.1.1/sportsml/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/models/gnn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/models/mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/models/rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.569093 sportsml-0.1.1/sportsml/mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/mongo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/mongo/averages.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/mongo/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/mongo/model_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.569093 sportsml-0.1.1/sportsml/nba/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.570093 sportsml-0.1.1/sportsml/nba/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5442 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nba/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.570093 sportsml-0.1.1/sportsml/nfl/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.571093 sportsml-0.1.1/sportsml/nfl/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/data/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/nfl/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.572093 sportsml-0.1.1/sportsml/odds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/odds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/odds/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/odds/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.573093 sportsml-0.1.1/sportsml/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-06-03 16:56:03.000000 sportsml-0.1.1/sportsml/utils/ensemble.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:56:10.561093 sportsml-0.1.1/sportsml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-03 16:56:10.000000 sportsml-0.1.1/sportsml.egg-info/top_level.txt
```

### Comparing `sportsml-0.1.0/pyproject.toml` & `sportsml-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sportsml"
-version = "0.1.0"
+version = "0.1.1"
 description = "ML for sports"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT license"}
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
```

### Comparing `sportsml-0.1.0/sportsml/cbb/data/datamodule.py` & `sportsml-0.1.1/sportsml/cbb/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/cbb/data/download.py` & `sportsml-0.1.1/sportsml/cbb/data/download.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/cbb/data/nodes.py` & `sportsml-0.1.1/sportsml/cbb/data/nodes.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/cli/predict/predict.py` & `sportsml-0.1.1/sportsml/cli/predict/predict.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/cli/train/train.py` & `sportsml-0.1.1/sportsml/cli/train/train.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/layers/gnn/encoder/gcn.py` & `sportsml-0.1.1/sportsml/layers/gnn/encoder/gcn.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/layers/gnn/predictor/nn.py` & `sportsml-0.1.1/sportsml/layers/gnn/predictor/nn.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/models/gnn.py` & `sportsml-0.1.1/sportsml/models/gnn.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/models/mlp.py` & `sportsml-0.1.1/sportsml/models/mlp.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/mongo/averages.py` & `sportsml-0.1.1/sportsml/mongo/averages.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/mongo/model_store.py` & `sportsml-0.1.1/sportsml/mongo/model_store.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nba/data/datamodule.py` & `sportsml-0.1.1/sportsml/nba/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nba/data/download.py` & `sportsml-0.1.1/sportsml/nba/data/download.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nba/data/features.py` & `sportsml-0.1.1/sportsml/nba/data/features.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nba/data/nodes.py` & `sportsml-0.1.1/sportsml/nba/data/nodes.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nba/data/utils.py` & `sportsml-0.1.1/sportsml/nba/data/utils.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nfl/data/download.py` & `sportsml-0.1.1/sportsml/nfl/data/download.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nfl/data/features.py` & `sportsml-0.1.1/sportsml/nfl/data/features.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/nfl/data/utils.py` & `sportsml-0.1.1/sportsml/nfl/data/utils.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/odds/client.py` & `sportsml-0.1.1/sportsml/odds/client.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/odds/utils.py` & `sportsml-0.1.1/sportsml/odds/utils.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml/utils/ensemble.py` & `sportsml-0.1.1/sportsml/utils/ensemble.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.1.0/sportsml.egg-info/SOURCES.txt` & `sportsml-0.1.1/sportsml.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 sportsml/__init__.py
 sportsml.egg-info/PKG-INFO
 sportsml.egg-info/SOURCES.txt
 sportsml.egg-info/dependency_links.txt
@@ -14,17 +15,32 @@
 sportsml/cbb/data/features.py
 sportsml/cbb/data/nodes.py
 sportsml/cbb/data/utils.py
 sportsml/cli/__init__.py
 sportsml/cli/predict/__init__.py
 sportsml/cli/predict/predict.py
 sportsml/cli/predict/conf/__init__.py
+sportsml/cli/predict/conf/conf.yaml
+sportsml/cli/predict/conf/graph/cbb.yaml
+sportsml/cli/predict/conf/graph/nba.yaml
+sportsml/cli/predict/conf/team_map/cbb.yaml
+sportsml/cli/predict/conf/team_map/nba.yaml
 sportsml/cli/train/__init__.py
 sportsml/cli/train/train.py
 sportsml/cli/train/conf/__init__.py
+sportsml/cli/train/conf/conf.yaml
+sportsml/cli/train/conf/dm/cbb.yaml
+sportsml/cli/train/conf/dm/nba.yaml
+sportsml/cli/train/conf/model/gnn.yaml
+sportsml/cli/train/conf/model/encoder/gcn.yaml
+sportsml/cli/train/conf/model/encoder/mean.yaml
+sportsml/cli/train/conf/model/encoder/nn.yaml
+sportsml/cli/train/conf/model/predictor/nn.yaml
+sportsml/cli/train/conf/trainer/early_stopping.yaml
+sportsml/cli/train/conf/trainer/prod.yaml
 sportsml/layers/__init__.py
 sportsml/layers/gnn/__init__.py
 sportsml/layers/gnn/encoder/__init__.py
 sportsml/layers/gnn/encoder/gcn.py
 sportsml/layers/gnn/encoder/mean.py
 sportsml/layers/gnn/encoder/nn.py
 sportsml/layers/gnn/predictor/__init__.py
```

