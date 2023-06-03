# Comparing `tmp/time_interpret-0.0.1.tar.gz` & `tmp/time_interpret-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_interpret-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "time_interpret-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time_interpret-0.0.1.tar` & `time_interpret-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,71 @@
--rw-r--r--   0        0        0      510 2023-06-03 08:35:44.239756 time_interpret-0.0.1/README.md
--rw-r--r--   0        0        0     1999 2023-06-03 09:12:27.039109 time_interpret-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.0.1/tint/__init__.py
--rw-r--r--   0        0        0       22 2023-06-03 08:35:44.247594 time_interpret-0.0.1/tint/__version__.py
--rw-r--r--   0        0        0     3477 1970-01-01 00:00:00.000000 time_interpret-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2215 2023-06-03 09:23:02.422959 time_interpret-0.1.0/README.md
+-rw-r--r--   0        0        0     1999 2023-06-03 09:26:47.240403 time_interpret-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.1.0/tint/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-03 09:23:02.462862 time_interpret-0.1.0/tint/__version__.py
+-rw-r--r--   0        0        0      966 2023-06-03 09:23:02.462995 time_interpret-0.1.0/tint/attr/__init__.py
+-rw-r--r--   0        0        0    13788 2023-06-03 09:23:02.463319 time_interpret-0.1.0/tint/attr/augmented_occlusion.py
+-rw-r--r--   0        0        0       84 2023-06-03 09:23:02.463444 time_interpret-0.1.0/tint/attr/base/__init__.py
+-rw-r--r--   0        0        0    28773 2023-06-03 09:23:02.463603 time_interpret-0.1.0/tint/attr/base/feature_ablation.py
+-rw-r--r--   0        0        0     4337 2023-06-03 09:23:02.463734 time_interpret-0.1.0/tint/attr/bayes.py
+-rw-r--r--   0        0        0     5583 2023-06-03 09:23:02.463834 time_interpret-0.1.0/tint/attr/bayes_mask.py
+-rw-r--r--   0        0        0    10394 2023-06-03 09:23:02.464050 time_interpret-0.1.0/tint/attr/discretised_ig.py
+-rw-r--r--   0        0        0     6497 2023-06-03 09:23:02.464196 time_interpret-0.1.0/tint/attr/dynamic_masks.py
+-rw-r--r--   0        0        0    13321 2023-06-03 09:23:02.464622 time_interpret-0.1.0/tint/attr/fit.py
+-rw-r--r--   0        0        0      420 2023-06-03 09:23:02.464739 time_interpret-0.1.0/tint/attr/geodesic_ig.py
+-rw-r--r--   0        0        0     8144 2023-06-03 09:23:02.464897 time_interpret-0.1.0/tint/attr/lof.py
+-rw-r--r--   0        0        0      887 2023-06-03 09:23:02.465026 time_interpret-0.1.0/tint/attr/models/__init__.py
+-rw-r--r--   0        0        0    11264 2023-06-03 09:23:02.465191 time_interpret-0.1.0/tint/attr/models/bayes_linear.py
+-rw-r--r--   0        0        0    11749 2023-06-03 09:23:02.465316 time_interpret-0.1.0/tint/attr/models/bayes_mask.py
+-rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.1.0/tint/attr/models/joint_features_generator.py
+-rw-r--r--   0        0        0    15814 2023-06-03 09:23:02.465493 time_interpret-0.1.0/tint/attr/models/mask.py
+-rw-r--r--   0        0        0     7693 2023-06-03 09:23:02.465613 time_interpret-0.1.0/tint/attr/models/path_generator.py
+-rw-r--r--   0        0        0     7957 2023-06-03 09:23:02.465828 time_interpret-0.1.0/tint/attr/models/retain.py
+-rw-r--r--   0        0        0    19095 2023-06-03 09:23:02.466012 time_interpret-0.1.0/tint/attr/occlusion.py
+-rw-r--r--   0        0        0     7881 2023-06-03 09:23:02.466199 time_interpret-0.1.0/tint/attr/retain.py
+-rw-r--r--   0        0        0      718 2023-06-03 09:23:02.466282 time_interpret-0.1.0/tint/attr/smooth_grad.py
+-rw-r--r--   0        0        0    14038 2023-06-03 09:23:02.466447 time_interpret-0.1.0/tint/attr/temporal_augmented_occlusion.py
+-rw-r--r--   0        0        0    21753 2023-06-03 09:23:02.466608 time_interpret-0.1.0/tint/attr/temporal_ig.py
+-rw-r--r--   0        0        0    14146 2023-06-03 09:23:02.466742 time_interpret-0.1.0/tint/attr/temporal_occlusion.py
+-rw-r--r--   0        0        0    12809 2023-06-03 09:23:02.466921 time_interpret-0.1.0/tint/attr/time_forward_tunnel.py
+-rw-r--r--   0        0        0       23 2023-06-03 09:23:02.467044 time_interpret-0.1.0/tint/data/.gitignore
+-rw-r--r--   0        0        0      261 2023-06-03 09:23:02.475939 time_interpret-0.1.0/tint/datasets/__init__.py
+-rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.1.0/tint/datasets/arma.py
+-rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.1.0/tint/datasets/biobank.py
+-rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.1.0/tint/datasets/dataset.py
+-rw-r--r--   0        0        0    11253 2023-06-03 09:23:02.476261 time_interpret-0.1.0/tint/datasets/hawkes.py
+-rw-r--r--   0        0        0     8679 2023-06-03 09:23:02.476396 time_interpret-0.1.0/tint/datasets/hmm.py
+-rw-r--r--   0        0        0    32885 2023-06-03 09:23:02.476586 time_interpret-0.1.0/tint/datasets/mimic3.py
+-rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.1.0/tint/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.1.0/tint/datasets/utils/fasttext.py
+-rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.1.0/tint/datasets/utils/labels.json
+-rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.1.0/tint/datasets/utils/labels.py
+-rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.1.0/tint/datasets/utils/read_3_2.json
+-rw-r--r--   0        0        0      363 2023-06-03 09:23:02.476845 time_interpret-0.1.0/tint/metrics/__init__.py
+-rw-r--r--   0        0        0     6894 2023-06-03 09:23:02.476999 time_interpret-0.1.0/tint/metrics/accuracy.py
+-rw-r--r--   0        0        0     3276 2023-06-03 09:23:02.477132 time_interpret-0.1.0/tint/metrics/base.py
+-rw-r--r--   0        0        0     6677 2023-06-03 09:23:02.477251 time_interpret-0.1.0/tint/metrics/comprehensiveness.py
+-rw-r--r--   0        0        0     6651 2023-06-03 09:23:02.477365 time_interpret-0.1.0/tint/metrics/cross_entropy.py
+-rw-r--r--   0        0        0    11449 2023-06-03 09:23:02.477516 time_interpret-0.1.0/tint/metrics/lipschitz_max.py
+-rw-r--r--   0        0        0     6681 2023-06-03 09:23:02.477630 time_interpret-0.1.0/tint/metrics/log_odds.py
+-rw-r--r--   0        0        0     6698 2023-06-03 09:23:02.477739 time_interpret-0.1.0/tint/metrics/sufficiency.py
+-rw-r--r--   0        0        0      261 2023-06-03 09:23:02.477875 time_interpret-0.1.0/tint/metrics/white_box/__init__.py
+-rw-r--r--   0        0        0     2241 2023-06-03 09:23:02.477994 time_interpret-0.1.0/tint/metrics/white_box/aup.py
+-rw-r--r--   0        0        0     2131 2023-06-03 09:23:02.478101 time_interpret-0.1.0/tint/metrics/white_box/auprc.py
+-rw-r--r--   0        0        0     2235 2023-06-03 09:23:02.478221 time_interpret-0.1.0/tint/metrics/white_box/aur.py
+-rw-r--r--   0        0        0     2411 2023-06-03 09:23:02.478321 time_interpret-0.1.0/tint/metrics/white_box/base.py
+-rw-r--r--   0        0        0     2422 2023-06-03 09:23:02.478433 time_interpret-0.1.0/tint/metrics/white_box/entropy.py
+-rw-r--r--   0        0        0     2259 2023-06-03 09:23:02.478553 time_interpret-0.1.0/tint/metrics/white_box/information.py
+-rw-r--r--   0        0        0     2083 2023-06-03 09:23:02.478675 time_interpret-0.1.0/tint/metrics/white_box/roc_auc.py
+-rw-r--r--   0        0        0      249 2023-06-03 09:23:02.478816 time_interpret-0.1.0/tint/models/__init__.py
+-rw-r--r--   0        0        0     2022 2023-06-03 09:23:02.478991 time_interpret-0.1.0/tint/models/bert.py
+-rw-r--r--   0        0        0     6531 2023-06-03 09:23:02.479129 time_interpret-0.1.0/tint/models/cnn.py
+-rw-r--r--   0        0        0     4932 2023-06-03 09:23:02.479251 time_interpret-0.1.0/tint/models/mlp.py
+-rw-r--r--   0        0        0     5581 2023-06-03 09:23:02.479400 time_interpret-0.1.0/tint/models/net.py
+-rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.1.0/tint/models/rnn.py
+-rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.1.0/tint/models/transformer.py
+-rw-r--r--   0        0        0      342 2023-06-03 09:23:02.479544 time_interpret-0.1.0/tint/utils/__init__.py
+-rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.1.0/tint/utils/collate.py
+-rw-r--r--   0        0        0     6628 2023-06-03 09:23:02.479682 time_interpret-0.1.0/tint/utils/common.py
+-rw-r--r--   0        0        0     1000 2023-06-03 09:23:02.479982 time_interpret-0.1.0/tint/utils/tensor_dataset.py
+-rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.1.0/tint/utils/tqdm.py
+-rw-r--r--   0        0        0     5182 1970-01-01 00:00:00.000000 time_interpret-0.1.0/PKG-INFO
```

### Comparing `time_interpret-0.0.1/pyproject.toml` & `time_interpret-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="time_interpret"
-version="0.0.1"
+version="0.1.0"
 authors=[
     {name="Joseph Enguehard", email="joseph@skippr.com"},
 ]
 description="Time interpret library for PyTorch."
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

