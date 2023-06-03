# Comparing `tmp/sportsml-0.0.9.tar.gz` & `tmp/sportsml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportsml-0.0.9.tar", last modified: Sat Mar 18 14:52:03 2023, max compression
+gzip compressed data, was "sportsml-0.1.0.tar", last modified: Sat Jun  3 16:19:31 2023, max compression
```

## Comparing `sportsml-0.0.9.tar` & `sportsml-0.1.0.tar`

### file list

```diff
@@ -1,65 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.054054 sportsml-0.0.9/
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-18 14:52:03.053054 sportsml-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-18 14:51:53.000000 sportsml-0.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-03-18 14:51:53.000000 sportsml-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-18 14:52:03.054054 sportsml-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-18 14:51:53.000000 sportsml-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.041053 sportsml-0.0.9/sportsml/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.043053 sportsml-0.0.9/sportsml/cbb/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.044053 sportsml-0.0.9/sportsml/cbb/data/
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/datamodule.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/cli/conf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/layers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.046054 sportsml-0.0.9/sportsml/layers/gnn/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.047053 sportsml-0.0.9/sportsml/layers/gnn/encoder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/mean.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/nn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.047053 sportsml-0.0.9/sportsml/layers/gnn/predictor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/predictor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/predictor/nn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.048054 sportsml-0.0.9/sportsml/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2768 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/gnn.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/mlp.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.049054 sportsml-0.0.9/sportsml/mongo/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/averages.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.050054 sportsml-0.0.9/sportsml/nba/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.051054 sportsml-0.0.9/sportsml/nba/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5902 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/datamodule.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)     1126 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4572 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.052054 sportsml-0.0.9/sportsml/nfl/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.053054 sportsml-0.0.9/sportsml/nfl/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.043053 sportsml-0.0.9/sportsml.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.779678 sportsml-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:19:31.778678 sportsml-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-03 16:19:24.000000 sportsml-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-03 16:19:24.000000 sportsml-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 16:19:31.779678 sportsml-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-03 16:19:24.000000 sportsml-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.770678 sportsml-0.1.0/sportsml/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.771678 sportsml-0.1.0/sportsml/cbb/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cbb/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     8378 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cbb/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/predict/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.772678 sportsml-0.1.0/sportsml/cli/predict/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/predict/predict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/cli/train/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/cli/train/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/cli/train/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/layers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.773678 sportsml-0.1.0/sportsml/layers/gnn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.774678 sportsml-0.1.0/sportsml/layers/gnn/encoder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/gcn.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/mean.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/encoder/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.774678 sportsml-0.1.0/sportsml/layers/gnn/predictor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/predictor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/layers/gnn/predictor/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/gnn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/models/rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/averages.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/mongo/model_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.775678 sportsml-0.1.0/sportsml/nba/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.776678 sportsml-0.1.0/sportsml/nba/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5442 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nba/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.777678 sportsml-0.1.0/sportsml/nfl/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.777678 sportsml-0.1.0/sportsml/nfl/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/nfl/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.778678 sportsml-0.1.0/sportsml/odds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/odds/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.778678 sportsml-0.1.0/sportsml/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-06-03 16:19:24.000000 sportsml-0.1.0/sportsml/utils/ensemble.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 16:19:31.771678 sportsml-0.1.0/sportsml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-03 16:19:31.000000 sportsml-0.1.0/sportsml.egg-info/top_level.txt
```

### Comparing `sportsml-0.0.9/pyproject.toml` & `sportsml-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sportsml"
-version = "0.0.9"
+version = "0.1.0"
 description = "ML for sports"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT license"}
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 nba_mongo_upload = "sportsml.nba.data.download:mongo_upload"
 nfl_mongo_upload = "sportsml.nfl.data.download:mongo_upload"
-train = "sportsml.cli.train:train"
+odds_upload = "sportsml.odds.utils:mongo_upload"
+train = "sportsml.cli.train.train:train"
+predict = "sportsml.cli.predict.predict:predict"
```

### Comparing `sportsml-0.0.9/sportsml/cbb/data/datamodule.py` & `sportsml-0.1.0/sportsml/cbb/data/datamodule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,124 @@
 import dgl
 import numpy as np
 import pandas as pd
 import torch
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 
 from .features import GRAPH_FEATURES
 
 
 class CBBGraphDataset(object):
-    def __init__(self, df, feature_columns=GRAPH_FEATURES, target_column='PlusMinus'):
+    def __init__(self, df, feature_columns=GRAPH_FEATURES, target_column="PlusMinus"):
         self.df = df
         self.feature_columns = feature_columns
         self.target_column = target_column
-        seasons = df['Season'].unique()
+        seasons = df["Season"].unique()
         self.dates = []
         for season in seasons:
-            s = df[df['Season'] == season]
-            for date in s['DayNum'].unique():
-                if s[s['DayNum'] < date]['TeamID'].unique().size == s['TeamID'].unique().size:
-                    self.dates.extend([
-                        [season, d]
-                        for d in s[s['DayNum'] >= date]['DayNum'].astype(int).unique().tolist()
-                    ])
+            s = df[df["Season"] == season]
+            for date in s["DayNum"].unique():
+                if (
+                    s[s["DayNum"] < date]["TeamID"].unique().size
+                    == s["TeamID"].unique().size
+                ):
+                    self.dates.extend(
+                        [
+                            [season, d]
+                            for d in s[s["DayNum"] >= date]["DayNum"]
+                            .astype(int)
+                            .unique()
+                            .tolist()
+                        ]
+                    )
                     break
         self.graph = self.generate_graph()
 
     def __len__(self):
         return len(self.dates)
 
     def __getitem__(self, idx):
         season, date = self.dates[idx]
         g = self.graph.edge_subgraph(
-            (self.graph.edata['season'] == season) & (self.graph.edata['date'] <= date)
-        , relabel_nodes=False)
-        g.edata['train'] = g.edata['date'] != g.edata['date'].max()
-        g.edata['w'] = 1 / (g.edata['date'].max() - g.edata['date']).clip(1)
+            (self.graph.edata["season"] == season) & (self.graph.edata["date"] <= date),
+            relabel_nodes=False,
+        )
+        g.edata["train"] = g.edata["date"] != g.edata["date"].max()
+        g.edata["w"] = (1 / (g.edata["date"].max() + 1 - g.edata["date"])).reshape(
+            -1, 1
+        )
         return g
 
     def generate_graph(self):
         g = dgl.graph(
-            (torch.from_numpy(self.df['TeamID_OPP'].values), torch.from_numpy(self.df['TeamID'].values)),
-            num_nodes=self.df['TeamID'].max() + 1
+            (
+                torch.from_numpy(self.df["TeamID_OPP"].values),
+                torch.from_numpy(self.df["TeamID"].values),
+            ),
+            num_nodes=self.df["TeamID"].max() + 1,
         )
-        g.edata['f'] = torch.from_numpy(self.df[self.feature_columns].values).float()
-        g.edata['y'] = torch.from_numpy(self.df[[self.target_column]].values).float()
-        g.edata['p'] = torch.from_numpy(self.df[['Loc']].values).float()
-        g.edata['date'] = torch.from_numpy(self.df['DayNum'].values.astype(int))
-        g.edata['season'] = torch.from_numpy(self.df['Season'].values.astype(int))
+        g.edata["f"] = torch.from_numpy(self.df[self.feature_columns].values).float()
+        g.edata["y"] = torch.from_numpy(self.df[[self.target_column]].values).float()
+        g.edata["p"] = torch.from_numpy(self.df[["Loc"]].values).float()
+        g.edata["date"] = torch.from_numpy(self.df["DayNum"].values.astype(int))
+        g.edata["season"] = torch.from_numpy(self.df["Season"].values.astype(int))
         return g
 
 
 class CBBGraphDataModule(pl.LightningDataModule):
     def __init__(
-        self, 
+        self,
         df,
         feature_columns=GRAPH_FEATURES,
-        target_column='PlusMinus',
+        target_column="PlusMinus",
         batch_size=64,
-        split_type='random',
+        split_type="random",
         splits=[0.8, 0.1, 0.1],
-        num_workers=4
+        num_workers=4,
     ):
         super().__init__()
         self.df = df
         self.feature_columns = feature_columns
         self.target_column = target_column
         self.batch_size = batch_size
         self.split_type = split_type
         self.splits = splits
         self.num_workers = num_workers
-    
-    def setup(self, stage='train'):
+
+    def setup(self, stage="train"):
         self.ds = CBBGraphDataset(self.df, self.feature_columns, self.target_column)
-        if self.split_type == 'random':
+        if self.split_type == "random":
             self.train_ds, self.val_ds, self.test_ds = torch.utils.data.random_split(
                 self.ds, self.splits
             )
-        elif self.split_type == 'time':
+        elif self.split_type == "time":
             idx = (len(self.ds) * np.array(self.splits).cumsum()).astype(int)[:2]
             train_idx, val_idx, test_idx = np.array_split(np.arange(len(self.ds)), idx)
             self.train_ds = torch.utils.data.Subset(self.ds, train_idx.tolist())
             self.val_ds = torch.utils.data.Subset(self.ds, val_idx.tolist())
             self.test_ds = torch.utils.data.Subset(self.ds, test_idx.tolist())
         else:
-            raise ValueError(f'split type {self.split_type} not supported')
+            raise ValueError(f"split type {self.split_type} not supported")
 
     def train_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.train_ds, batch_size=self.batch_size, shuffle=True, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.train_ds,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=self.num_workers,
+        )
 
     def val_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.val_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.val_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
 
     def test_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.test_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.test_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
```

### Comparing `sportsml-0.0.9/sportsml/cli/train.py` & `sportsml-0.1.0/sportsml/cli/train/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import hydra
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 from omegaconf import DictConfig, OmegaConf
 
+
 @hydra.main(version_base=None, config_path="conf", config_name="conf")
-def train(cfg : DictConfig) -> None:
+def train(cfg: DictConfig) -> None:
     if cfg.seed is not None:
         pl.seed_everything(cfg.seed)
     trainer = hydra.utils.instantiate(cfg.trainer)
     model = hydra.utils.instantiate(cfg.model)
     dm = hydra.utils.instantiate(cfg.dm)
 
     trainer.fit(model, dm)
 
     if len(dm.test_ds):
-        trainer.test(model, dm, ckpt_path='best')
+        trainer.test(model, dm, ckpt_path="best")
+
 
 if __name__ == "__main__":
     train()
```

### Comparing `sportsml-0.0.9/sportsml/layers/gnn/predictor/nn.py` & `sportsml-0.1.0/sportsml/layers/gnn/predictor/nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import List
 
 import torch
 
 
 class NNPredictor(torch.nn.Module):
-    def __init__(self, in_feats: int, dims: List=[], out_feats: int=1, dropout: float=0.1):
+    def __init__(
+        self, in_feats: int, dims: List = [], out_feats: int = 1, dropout: float = 0.1
+    ):
         super().__init__()
         self.dims = list(dims)
         self.dims.insert(0, in_feats)
         layers = [torch.nn.BatchNorm1d(in_feats)]
         for idx in range(len(self.dims) - 1):
-            layers.append(torch.nn.Linear(self.dims[idx], self.dims[idx+1]))
+            layers.append(torch.nn.Linear(self.dims[idx], self.dims[idx + 1]))
             layers.append(torch.nn.ReLU())
             layers.append(torch.nn.Dropout(dropout))
-            layers.append(torch.nn.BatchNorm1d(self.dims[idx+1]))
+            layers.append(torch.nn.BatchNorm1d(self.dims[idx + 1]))
         layers.append(torch.nn.Linear(self.dims[-1], out_feats))
         self.mlp = torch.nn.Sequential(*layers)
 
     def forward(self, g, h, e):
         g = g.local_var()
         src, dst = g.edges()
         x = torch.cat([h[src], h[dst], e], dim=1)
```

### Comparing `sportsml-0.0.9/sportsml/models/mlp.py` & `sportsml-0.1.0/sportsml/models/mlp.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,62 +6,66 @@
 class MLP(pl.LightningModule):
     def __init__(self, in_feats, dims=[100, 100], out_feats=1, dropout=0.1):
         super().__init__()
         self.dims = list(dims)
         self.dims.insert(0, in_feats)
         layers = [torch.nn.BatchNorm1d(in_feats)]
         for idx in range(len(self.dims) - 1):
-            layers.append(torch.nn.Linear(self.dims[idx], self.dims[idx+1]))
+            layers.append(torch.nn.Linear(self.dims[idx], self.dims[idx + 1]))
             layers.append(torch.nn.ReLU())
             layers.append(torch.nn.Dropout(dropout))
-            layers.append(torch.nn.BatchNorm1d(self.dims[idx+1]))
+            layers.append(torch.nn.BatchNorm1d(self.dims[idx + 1]))
         layers.append(torch.nn.Linear(self.dims[-1], out_feats))
         self.mlp = torch.nn.Sequential(*layers)
 
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
         self.mae = torchmetrics.MeanAbsoluteError()
-        self.accuracy_score = torchmetrics.classification.MulticlassAccuracy(num_classes=2)
-        self.precision_score = torchmetrics.classification.MulticlassPrecision(num_classes=2)
+        self.accuracy_score = torchmetrics.classification.MulticlassAccuracy(
+            num_classes=2
+        )
+        self.precision_score = torchmetrics.classification.MulticlassPrecision(
+            num_classes=2
+        )
         self.recall_score = torchmetrics.classification.MulticlassRecall(num_classes=2)
 
-        self.save_hyperparameters('in_feats', 'dims')
+        self.save_hyperparameters("in_feats", "dims")
 
     def configure_optimizers(self):
         optimizer = torch.optim.Adam(self.parameters(), lr=1e-3)
         return optimizer
-        
+
     def forward(self, x):
         return self.mlp(x)
-    
+
     def training_step(self, batch, batch_idx):
         x, y = batch
         p = self(x)
         loss = torch.nn.functional.mse_loss(p, y)
         return loss
 
     def validation_step(self, batch, batch_idx):
         x, y = batch
         p = self(x)
         self.rmse(p, y)
         self.mae(p, y)
         self.accuracy_score(p > 0, y > 0)
         self.precision_score(p > 0, y > 0)
         self.recall_score(p > 0, y > 0)
-        self.log('val_rmse', self.rmse)
-        self.log('val_mae', self.mae)
-        self.log('val_accuracy', self.accuracy_score)
-        self.log('val_precision', self.precision_score)
-        self.log('val_recall', self.recall_score)
-    
+        self.log("val_rmse", self.rmse)
+        self.log("val_mae", self.mae)
+        self.log("val_accuracy", self.accuracy_score)
+        self.log("val_precision", self.precision_score)
+        self.log("val_recall", self.recall_score)
+
     def test_step(self, batch, batch_idx):
         x, y = batch
         p = self(x)
         self.rmse(p, y)
         self.mae(p, y)
         self.accuracy_score(p > 0, y > 0)
         self.precision_score(p > 0, y > 0)
         self.recall_score(p > 0, y > 0)
-        self.log('test_rmse', self.rmse)
-        self.log('test_mae', self.mae)
-        self.log('test_accuracy', self.accuracy_score)
-        self.log('test_precision', self.precision_score)
-        self.log('test_recall', self.recall_score)
+        self.log("test_rmse", self.rmse)
+        self.log("test_mae", self.mae)
+        self.log("test_accuracy", self.accuracy_score)
+        self.log("test_precision", self.precision_score)
+        self.log("test_recall", self.recall_score)
```

### Comparing `sportsml-0.0.9/sportsml/mongo/averages.py` & `sportsml-0.1.0/sportsml/mongo/averages.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     return list(
         collection.aggregate(
             [
                 {"$match": {season_key: season, date_key: {"$lt": date}}},
                 group_agg,
             ]
         )
-    )
+    )
```

### Comparing `sportsml-0.0.9/sportsml/nba/data/datamodule.py` & `sportsml-0.1.0/sportsml/nba/data/datamodule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,219 @@
+import datetime
 import dgl
 import numpy as np
 import pandas as pd
 import torch
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 
 from .features import GRAPH_FEATURES, FEATURE_COLUMNS
-from .utils import get_regular_season_games, get_training_data
 
 
 class NBAGameDataModule(pl.LightningDataModule):
     def __init__(
         self,
         df=None,
         val_df=None,
         test_df=None,
         feature_columns=FEATURE_COLUMNS,
-        target_column='PLUS_MINUS',
+        target_columns=["PLUS_MINUS"],
         batch_size=64,
         splits=[0.8, 0.1, 0.1],
-        num_workers=4
+        num_workers=4,
     ):
         super().__init__()
-        if df is None:
-            df = get_training_data()
         self.df = df
         self.val_df = val_df
         self.test_df = test_df
         self.feature_columns = feature_columns
-        self.target_column = target_column
+        self.target_columns = target_columns
         self.batch_size = batch_size
         self.splits = splits
         self.num_workers = num_workers
 
     def df_to_dataset(self, df):
         X = df[self.feature_columns].values
-        y = df[[self.target_column]].values
+        y = df[self.target_columns].values
         return torch.utils.data.TensorDataset(
             torch.from_numpy(X).float(), torch.from_numpy(y).float()
         )
-    
-    def setup(self, stage='train'):
+
+    def setup(self, stage="train"):
         if self.val_df is None and self.test_df is None:
             self.ds = self.df_to_dataset(self.df)
             self.train_ds, self.val_ds, self.test_ds = torch.utils.data.random_split(
-                self.ds,
-                self.splits
+                self.ds, self.splits
             )
         else:
             self.train_ds = self.df_to_dataset(self.df)
             self.val_ds = self.df_to_dataset(self.val_df)
             self.test_ds = self.df_to_dataset(self.test_df)
-    
+
     def train_dataloader(self):
-        return torch.utils.data.DataLoader(self.train_ds, batch_size=self.batch_size, shuffle=True, num_workers=self.num_workers)
-    
+        return torch.utils.data.DataLoader(
+            self.train_ds,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=self.num_workers,
+        )
+
     def val_dataloader(self):
-        return torch.utils.data.DataLoader(self.val_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
-    
+        return torch.utils.data.DataLoader(
+            self.val_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
+
     def test_dataloader(self):
-        return torch.utils.data.DataLoader(self.test_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
+        return torch.utils.data.DataLoader(
+            self.test_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
 
 
 class NBAGraphDataset(object):
-    def __init__(self, df, feature_columns=GRAPH_FEATURES, target_column='PLUS_MINUS'):
+    def __init__(
+        self,
+        df,
+        feature_columns=GRAPH_FEATURES,
+        target_columns=["PLUS_MINUS"],
+    ):
         self.df = df
         self.feature_columns = feature_columns
-        self.target_column = target_column
-        seasons = df['SEASON'].unique()
+        self.target_columns = target_columns
+        seasons = df["SEASON"].unique()
         self.dates = []
         for season in seasons:
-            s = df[df['SEASON'] == season]
-            for date in s['GAME_DATE'].unique():
-                if s[s['GAME_DATE'] < date]['TEAM_ABBREVIATION'].unique().size == 30:
-                    self.dates.extend(s[s['GAME_DATE'] >= date]['GAME_DATE'].str.replace('-', '').astype(int).unique().tolist())
+            s = df[df["SEASON"] == season]
+            for date in s["GAME_DATE"].unique():
+                if s[s["GAME_DATE"] < date]["TEAM_ABBREVIATION"].unique().size == 30:
+                    self.dates.extend(
+                        s[s["GAME_DATE"] >= date]["GAME_DATE"]
+                        .str.replace("-", "")
+                        .astype(int)
+                        .unique()
+                        .tolist()
+                    )
                     break
         self.graph = self.generate_graph()
 
     def __len__(self):
         return len(self.dates)
 
     def __getitem__(self, idx):
         date = self.dates[idx]
-        g = self.graph.edge_subgraph(self.graph.edata['date'] < date, relabel_nodes=False)
-        g = g.edge_subgraph(g.edata['season'] == g.edata['season'].max(), relabel_nodes=False)
-        g.edata['train'] = g.edata['date'] != g.edata['date'].max()
-        g.edata['w'] = 1 / (g.edata['date'].max() - g.edata['date']).clip(1)
+        date_str = str(date)
+        date_dt = datetime.date(
+            int(date_str[:4]), int(date_str[4:6]), int(date_str[6:])
+        )
+        g = self.graph.edge_subgraph(
+            (self.graph.edata["date"] < date),
+            relabel_nodes=False,
+        )
+        g = g.edge_subgraph(
+            g.edata["season"] == g.edata["season"].max(), relabel_nodes=False
+        )
+        g.edata["train"] = g.edata["date"] != g.edata["date"].max()
+        g.edata["w"] = (1 / (g.edata["date"].max() + 1 - g.edata["date"])).reshape(
+            -1, 1
+        )
         return g
 
     def generate_graph(self):
         g = dgl.graph(
-            (torch.from_numpy(self.df['src'].values), torch.from_numpy(self.df['target'].values)),
-            num_nodes=30
+            (
+                torch.from_numpy(self.df["src"].values),
+                torch.from_numpy(self.df["target"].values),
+            ),
+            num_nodes=30,
         )
-        g.edata['f'] = torch.from_numpy(self.df[self.feature_columns].values).float()
-        g.edata['y'] = torch.from_numpy(self.df[[self.target_column]].values).float()
-        g.edata['p'] = torch.from_numpy(self.df[['HOME']].values).float()
-        g.edata['rest'] = torch.from_numpy(self.df[['REST']].values).float()
-        g.edata['date'] = torch.from_numpy(self.df['GAME_DATE'].str.replace('-', '').values.astype(int))
-        g.edata['season'] = torch.from_numpy(self.df['SEASON'].values.astype(int))
+        g.edata["f"] = torch.from_numpy(self.df[self.feature_columns].values).float()
+        g.edata["y"] = torch.from_numpy(self.df[self.target_columns].values).float()
+        g.edata["p"] = torch.from_numpy(self.df[["HOME"]].values).float()
+        g.edata["rest"] = torch.from_numpy(self.df[["REST"]].values).float()
+        g.edata["date"] = torch.from_numpy(
+            self.df["GAME_DATE"].str.replace("-", "").values.astype(int)
+        )
+        g.edata["season"] = torch.from_numpy(self.df["SEASON"].values.astype(int))
         return g
 
 
 class NBAGraphDataModule(pl.LightningDataModule):
     def __init__(
-        self, 
+        self,
         df,
+        val_df=None,
+        test_df=None,
         feature_columns=GRAPH_FEATURES,
-        target_column='PLUS_MINUS',
+        target_columns=["PLUS_MINUS"],
         batch_size=64,
-        split_type='random',
+        split_type="random",
         splits=[0.8, 0.1, 0.1],
-        num_workers=4
+        num_workers=4,
     ):
         super().__init__()
         self.df = df
+        self.val_df = val_df
+        self.test_df = test_df
         self.feature_columns = feature_columns
-        self.target_column = target_column
+        self.target_columns = target_columns
         self.batch_size = batch_size
         self.split_type = split_type
         self.splits = splits
         self.num_workers = num_workers
-    
-    def setup(self, stage='train'):
-        self.ds = NBAGraphDataset(self.df, self.feature_columns, self.target_column)
-        if self.split_type == 'random':
+
+    def get_latest_date(self):
+        max_train_date = self.df.iloc[self.train_ds.indices]["GAME_DATE"].max()
+        max_val_date = self.df.iloc[self.val_ds.indices]["GAME_DATE"].max()
+        return max(max_train_date, max_val_date)
+
+    def setup(self, stage="train"):
+        self.ds = NBAGraphDataset(self.df, self.feature_columns, self.target_columns)
+        if self.split_type == "random":
             self.train_ds, self.val_ds, self.test_ds = torch.utils.data.random_split(
                 self.ds, self.splits
             )
-        elif self.split_type == 'time':
+        elif self.split_type == "time":
             idx = (len(self.ds) * np.array(self.splits).cumsum()).astype(int)[:2]
             train_idx, val_idx, test_idx = np.array_split(np.arange(len(self.ds)), idx)
             self.train_ds = torch.utils.data.Subset(self.ds, train_idx.tolist())
             self.val_ds = torch.utils.data.Subset(self.ds, val_idx.tolist())
             self.test_ds = torch.utils.data.Subset(self.ds, test_idx.tolist())
+        elif self.split_type == None:
+            self.train_ds = self.ds
         else:
-            raise ValueError(f'split type {self.split_type} not supported')
+            raise ValueError(f"split type {self.split_type} not supported")
+        if self.val_df is not None:
+            self.val_ds = NBAGraphDataset(
+                self.val_df, self.feature_columns, self.target_columns
+            )
+        if self.test_df is not None:
+            self.test_ds = NBAGraphDataset(
+                self.test_df, self.feature_columns, self.target_columns
+            )
 
     def train_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.train_ds, batch_size=self.batch_size, shuffle=True, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.train_ds,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=self.num_workers,
+        )
 
     def val_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.val_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.val_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
 
     def test_dataloader(self):
-        return dgl.dataloading.GraphDataLoader(self.test_ds, batch_size=self.batch_size, shuffle=False, num_workers=self.num_workers)
+        return dgl.dataloading.GraphDataLoader(
+            self.test_ds,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
```

### Comparing `sportsml-0.0.9/sportsml/nba/data/download.py` & `sportsml-0.1.0/sportsml/nba/data/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 from nba_api.stats.static import teams
 from nba_api.stats.endpoints import leaguegamefinder
 from pymongo import ReplaceOne
 
 from .utils import process_games
 from ...mongo import client
 
+
 def download_games():
     games = []
     for team in tqdm.tqdm(teams.get_teams()):
         gamefinder = leaguegamefinder.LeagueGameFinder(team_id_nullable=team["id"])
         games.append(gamefinder.get_data_frames()[0])
         # try not to overload API service
         time.sleep(0.5)
     return pd.concat(games)
 
 
 def games_from_last_date():
     games = []
     last_date = datetime.date.fromisoformat(
-        client.nba.games.find({}).sort('GAME_DATE', -1).limit(1).next()['GAME_DATE']
-    ).strftime('%m/%d/%Y')
+        client.nba.games.find({}).sort("GAME_DATE", -1).limit(1).next()["GAME_DATE"]
+    ).strftime("%m/%d/%Y")
     for team in tqdm.tqdm(teams.get_teams()):
         gamefinder = leaguegamefinder.LeagueGameFinder(
-            team_id_nullable=team["id"],
-            date_from_nullable=last_date
+            team_id_nullable=team["id"], date_from_nullable=last_date
         )
         games.append(gamefinder.get_data_frames()[0])
         time.sleep(0.5)
     return pd.concat(games)
 
 
 def mongo_upload():
```

### Comparing `sportsml-0.0.9/sportsml/nba/data/utils.py` & `sportsml-0.1.0/sportsml/nba/data/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
+from .datamodule import NBAGraphDataset
 from .features import STATS_COLUMNS, OPP_STATS_COLUMNS, FEATURE_COLUMNS
-from .nodes import team_idx_map
+from .nodes import team_idx_map, team_abr_map
 from ...mongo import client, group_aggregation
 
 
+def get_team_abr_map():
+    return team_abr_map
+
+
 def process_games(games: pd.DataFrame):
     games = games.dropna()
     games = games[games.groupby("GAME_ID")["GAME_ID"].transform("count") == 2]
 
     first_game = games.drop_duplicates(subset=["GAME_ID"], keep="first")
     last_game = games.drop_duplicates(subset=["GAME_ID"], keep="last")
 
     games = pd.concat(
         [
             first_game.merge(
-                last_game[STATS_COLUMNS + ["TEAM_ID", "TEAM_ABBREVIATION", "TEAM_NAME", "GAME_ID"]],
+                last_game[
+                    STATS_COLUMNS
+                    + ["TEAM_ID", "TEAM_ABBREVIATION", "TEAM_NAME", "GAME_ID"]
+                ],
                 on="GAME_ID",
                 how="left",
                 suffixes=("", "_OPP"),
             ).set_index(first_game.index),
             last_game.merge(
-                first_game[STATS_COLUMNS + ["TEAM_ID", "TEAM_ABBREVIATION", "TEAM_NAME", "GAME_ID"]],
+                first_game[
+                    STATS_COLUMNS
+                    + ["TEAM_ID", "TEAM_ABBREVIATION", "TEAM_NAME", "GAME_ID"]
+                ],
                 on="GAME_ID",
                 how="left",
                 suffixes=("", "_OPP"),
             ).set_index(last_game.index),
         ]
     ).reset_index(drop=True)
 
@@ -45,72 +56,110 @@
 
     games["SEASON"] = games["SEASON_ID"].astype(str).str.slice(start=1).astype(int)
 
     return games
 
 
 def process_averages(games):
-    games = games.sort_values('GAME_DATE')
-    avg = games.copy().drop(STATS_COLUMNS+OPP_STATS_COLUMNS, axis=1)
-    avg_stats = games.groupby(['SEASON_ID', 'TEAM_ABBREVIATION'])[STATS_COLUMNS + OPP_STATS_COLUMNS].expanding().mean().groupby(['SEASON_ID', 'TEAM_ABBREVIATION']).shift(1).droplevel([0, 1])
-    rolling_stats = games.groupby(['SEASON_ID', 'TEAM_ABBREVIATION'])[STATS_COLUMNS + OPP_STATS_COLUMNS].rolling(5, 1, closed='left').mean().droplevel([0, 1])
-    rolling_stats.columns = [f'{col}_rolling' for col in rolling_stats.columns]
-    return avg.merge(avg_stats, left_index=True, right_index=True).merge(rolling_stats, left_index=True, right_index=True)
+    games = games.sort_values("GAME_DATE")
+    avg = games.copy().drop(STATS_COLUMNS + OPP_STATS_COLUMNS, axis=1)
+    avg_stats = (
+        games.groupby(["SEASON", "TEAM_ABBREVIATION"])[
+            STATS_COLUMNS + OPP_STATS_COLUMNS
+        ]
+        .expanding()
+        .mean()
+        .groupby(["SEASON", "TEAM_ABBREVIATION"])
+        .shift(1)
+        .droplevel([0, 1])
+    )
+    rolling_stats = (
+        games.groupby(["SEASON", "TEAM_ABBREVIATION"])[
+            STATS_COLUMNS + OPP_STATS_COLUMNS
+        ]
+        .rolling(5, 1, closed="left")
+        .mean()
+        .droplevel([0, 1])
+    )
+    rolling_stats.columns = [f"{col}_rolling" for col in rolling_stats.columns]
+    return avg.merge(avg_stats, left_index=True, right_index=True).merge(
+        rolling_stats, left_index=True, right_index=True
+    )
+
+
+def get_games(query={}):
+    query.update(
+        {
+            "SEASON_ID": {"$regex": "^2|^4"},
+            "GAME_ID": {"$regex": "^0"},
+        }
+    )
+    df = pd.DataFrame(client.nba.games.find(query)).sort_values("GAME_DATE")
+    return df
 
 
 def get_regular_season_games(query={}):
-    query.update({
-        'SEASON_ID': {'$regex': '^2'},
-        'GAME_ID': {'$regex': '^0'},
-    })
-    df = pd.DataFrame(client.nba.games.find(query)).sort_values('GAME_DATE')
+    query.update(
+        {
+            "SEASON_ID": {"$regex": "^2"},
+            "GAME_ID": {"$regex": "^0"},
+        }
+    )
+    df = pd.DataFrame(client.nba.games.find(query)).sort_values("GAME_DATE")
     return df
 
 
+def get_latest_graph():
+    games = get_regular_season_games(
+        {"SEASON": max(client.nba.games.distinct("SEASON"))}
+    )
+    ds = NBAGraphDataset(games)
+    return ds[-1]
 
-def get_regular_season_averages(date):
-    season_id = client.nba.games.find_one({'GAME_DATE': date}).get('SEASON_ID')
+
+def get_season_averages(date, season=None):
+    if season is None:
+        season = client.nba.games.find_one({"GAME_DATE": date}).get("SEASON")
     result = list(
         client.nba.games.aggregate(
             [
                 {
                     "$match": {
-                        'SEASON_ID': season_id,
-                        'GAME_DATE': {"$lt": date},
-                        'GAME_ID': {'$regex': '^0'}
+                        "SEASON": season,
+                        "SEASON_ID": {"$regex": "^2|^4"},
+                        "GAME_DATE": {"$lt": date},
+                        "GAME_ID": {"$regex": "^0"},
                     }
                 },
-                group_aggregation(STATS_COLUMNS + OPP_STATS_COLUMNS, 'TEAM_ABBREVIATION')
+                group_aggregation(
+                    STATS_COLUMNS + OPP_STATS_COLUMNS, "TEAM_ABBREVIATION"
+                ),
             ]
         )
     )
     return {
-        res.pop('_id'): {
-            'stats': {
-                k: v
-                for k,v in res.items()
-                if '_OPP' not in k
-            },
-            'opp_stats': {
-                k: v
-                for k,v in res.items()
-                if '_OPP' in k
-            }
+        res.pop("_id"): {
+            "stats": {k: v for k, v in res.items() if "_OPP" not in k},
+            "opp_stats": {k: v for k, v in res.items() if "_OPP" in k},
         }
         for res in result
     }
 
 
 def featurize_games(avgs):
-    first_avgs = avgs.drop_duplicates('GAME_ID', keep='first').set_index('GAME_ID', drop=True)
-    last_avgs = avgs.drop_duplicates('GAME_ID', keep='last').set_index('GAME_ID', drop=True)
+    first_avgs = avgs.drop_duplicates("GAME_ID", keep="first").set_index(
+        "GAME_ID", drop=True
+    )
+    last_avgs = avgs.drop_duplicates("GAME_ID", keep="last").set_index(
+        "GAME_ID", drop=True
+    )
 
     stats = STATS_COLUMNS + OPP_STATS_COLUMNS
-    stats = stats + [f'{col}_rolling' for col in stats]
-    opp_stats = [f'OPP_{stat}' for stat in stats]
+    stats = stats + [f"{col}_rolling" for col in stats]
+    opp_stats = [f"OPP_{stat}" for stat in stats]
 
     first_avgs[opp_stats] = last_avgs[stats]
 
     return first_avgs
 
 
 def get_training_data(feature_columns=FEATURE_COLUMNS):
@@ -119,17 +168,19 @@
     f = featurize_games(avgs)
     f = f.dropna(subset=feature_columns)
     return f
 
 
 def get_training_data_split(
     feature_columns=FEATURE_COLUMNS,
-    target_column='PLUS_MINUS',
+    target_column="PLUS_MINUS",
     test_size=0.2,
-    random_state=None
+    random_state=None,
 ):
     f = get_training_data()
     f = f.dropna(subset=FEATURE_COLUMNS)
     X = f[feature_columns].values
     y = f[target_column].values
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
+    X_train, X_test, y_train, y_test = train_test_split(
+        X, y, test_size=test_size, random_state=random_state
+    )
     return X_train, X_test, y_train, y_test
```

### Comparing `sportsml-0.0.9/sportsml/nfl/data/download.py` & `sportsml-0.1.0/sportsml/nfl/data/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,19 @@
         r"https://github.com/nflverse/nflverse-data/releases/download/player_stats/player_stats.parquet"
     )
     return data
 
 
 def get_game_totals():
     data = get_play_by_play()
-    game_totals = data.groupby(["recent_team", "season", "week"]).sum(numeric_only=True).reset_index()
+    game_totals = (
+        data.groupby(["recent_team", "season", "week"])
+        .sum(numeric_only=True)
+        .reset_index()
+    )
     return game_totals
 
 
 def get_schedule():
     schedule = pd.pandas.read_csv(
         "https://github.com/nflverse/nfldata/raw/master/data/games.csv"
     )
```

### Comparing `sportsml-0.0.9/sportsml/nfl/data/features.py` & `sportsml-0.1.0/sportsml/nfl/data/features.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 STATS_COLUMNS = [
+    "score",
     "completions",
     "attempts",
     "passing_yards",
     "passing_tds",
     "interceptions",
     "sacks",
     "sack_yards",
@@ -26,8 +27,13 @@
     "special_teams_tds",
     "pacr",
     "racr",
 ]
 
 OPP_STATS_COLUMNS = [f"opp_{col}" for col in STATS_COLUMNS]
 
-FEATURE_COLUMNS = STATS_COLUMNS + OPP_STATS_COLUMNS + [f'{stat}_opp' for stat in STATS_COLUMNS + OPP_STATS_COLUMNS] + ['home', 'rest', 'opp_rest']
+FEATURE_COLUMNS = (
+    STATS_COLUMNS
+    + OPP_STATS_COLUMNS
+    + [f"{stat}_opp" for stat in STATS_COLUMNS + OPP_STATS_COLUMNS]
+    + ["home", "rest", "opp_rest"]
+)
```

### Comparing `sportsml-0.0.9/sportsml/nfl/data/utils.py` & `sportsml-0.1.0/sportsml/nfl/data/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,72 +73,71 @@
                 .rename(columns={"opp_game_id": "game_id"}),
                 on="game_id",
                 how="left",
             ).set_index(last_game.index),
         ]
     )
 
-    games['home'] = games.apply(lambda x: int(x['game_id'].endswith(x['team'])), axis=1)
+    games["home"] = games.apply(lambda x: int(x["game_id"].endswith(x["team"])), axis=1)
+
+    games["plus_minus"] = games["score"] - games["opp_score"]
 
     return games
 
 
 def get_season_averages(season, week):
     result = list(
         client.nfl.games.aggregate(
             [
-                {
-                    "$match": {
-                        'season': season,
-                        'week': {"$lt": week}
-                    }
-                },
-                group_aggregation(STATS_COLUMNS + OPP_STATS_COLUMNS, 'team')
+                {"$match": {"season": season, "week": {"$lt": week}}},
+                group_aggregation(STATS_COLUMNS + OPP_STATS_COLUMNS, "team"),
             ]
         )
     )
     return {
-        res.pop('_id'): {
-            'stats': {
-                k: v
-                for k,v in res.items()
-                if 'opp_' not in k
-            },
-            'opp_stats': {
-                k: v
-                for k,v in res.items()
-                if 'opp_' in k
-            }
+        res.pop("_id"): {
+            "stats": {k: v for k, v in res.items() if "opp_" not in k},
+            "opp_stats": {k: v for k, v in res.items() if "opp_" in k},
         }
         for res in result
     }
 
 
 def process_averages(games):
-    games = games.sort_values(['season', 'week'])
-    avg = games.copy().drop(STATS_COLUMNS+OPP_STATS_COLUMNS, axis=1)
-    avg_stats = games.groupby(['season', 'team'])[STATS_COLUMNS + OPP_STATS_COLUMNS].expanding().mean().groupby(['season', 'team']).shift(1).droplevel([0, 1])
+    games = games.sort_values(["season", "week"])
+    avg = games.copy().drop(STATS_COLUMNS + OPP_STATS_COLUMNS, axis=1)
+    avg_stats = (
+        games.groupby(["season", "team"])[STATS_COLUMNS + OPP_STATS_COLUMNS]
+        .expanding()
+        .mean()
+        .groupby(["season", "team"])
+        .shift(1)
+        .droplevel([0, 1])
+    )
     return avg.merge(avg_stats, left_index=True, right_index=True)
 
+
 def featurize_games(avgs):
     avgs = avgs.copy()
     opp_avgs = avgs.copy()
-    opp_avgs['_id'] = opp_avgs.apply(
-        lambda row: '-'.join([
-            str(row['season']), 
-            str(row['week']), 
-            row['opp_team'], 
-            row['team']
-        ]), 
-        axis=1
+    opp_avgs["_id"] = opp_avgs.apply(
+        lambda row: "-".join(
+            [str(row["season"]), str(row["week"]), row["opp_team"], row["team"]]
+        ),
+        axis=1,
     )
 
     stats = STATS_COLUMNS + OPP_STATS_COLUMNS
 
-    opp_stats = [f'{stat}_opp' for stat in stats]
+    opp_stats = [f"{stat}_opp" for stat in stats]
 
-    avgs = avgs.set_index('_id')
-    opp_avgs = opp_avgs.set_index('_id')
+    avgs = avgs.set_index("_id")
+    opp_avgs = opp_avgs.set_index("_id")
 
     avgs[opp_stats] = opp_avgs[stats]
 
-    return avgs
+    return avgs
+
+
+def get_games(query={}):
+    df = pd.DataFrame(client.nfl.games.find(query)).sort_values(["season", "week"])
+    return df
```

### Comparing `sportsml-0.0.9/sportsml.egg-info/SOURCES.txt` & `sportsml-0.1.0/sportsml.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -11,36 +11,47 @@
 sportsml/cbb/__init__.py
 sportsml/cbb/data/datamodule.py
 sportsml/cbb/data/download.py
 sportsml/cbb/data/features.py
 sportsml/cbb/data/nodes.py
 sportsml/cbb/data/utils.py
 sportsml/cli/__init__.py
-sportsml/cli/train.py
-sportsml/cli/conf/__init__.py
+sportsml/cli/predict/__init__.py
+sportsml/cli/predict/predict.py
+sportsml/cli/predict/conf/__init__.py
+sportsml/cli/train/__init__.py
+sportsml/cli/train/train.py
+sportsml/cli/train/conf/__init__.py
 sportsml/layers/__init__.py
 sportsml/layers/gnn/__init__.py
 sportsml/layers/gnn/encoder/__init__.py
+sportsml/layers/gnn/encoder/gcn.py
 sportsml/layers/gnn/encoder/mean.py
 sportsml/layers/gnn/encoder/nn.py
 sportsml/layers/gnn/predictor/__init__.py
 sportsml/layers/gnn/predictor/nn.py
 sportsml/models/__init__.py
 sportsml/models/gnn.py
 sportsml/models/mlp.py
 sportsml/models/rf.py
 sportsml/mongo/__init__.py
 sportsml/mongo/averages.py
 sportsml/mongo/client.py
+sportsml/mongo/model_store.py
 sportsml/nba/__init__.py
 sportsml/nba/data/__init__.py
 sportsml/nba/data/datamodule.py
 sportsml/nba/data/download.py
 sportsml/nba/data/features.py
 sportsml/nba/data/nodes.py
 sportsml/nba/data/utils.py
 sportsml/nfl/__init__.py
 sportsml/nfl/data/__init__.py
 sportsml/nfl/data/download.py
 sportsml/nfl/data/features.py
 sportsml/nfl/data/names.py
-sportsml/nfl/data/utils.py
+sportsml/nfl/data/utils.py
+sportsml/odds/__init__.py
+sportsml/odds/client.py
+sportsml/odds/utils.py
+sportsml/utils/__init__.py
+sportsml/utils/ensemble.py
```

