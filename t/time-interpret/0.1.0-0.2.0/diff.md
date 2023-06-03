# Comparing `tmp/time_interpret-0.1.0.tar.gz` & `tmp/time_interpret-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_interpret-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "time_interpret-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time_interpret-0.1.0.tar` & `time_interpret-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,85 @@
--rw-r--r--   0        0        0     2215 2023-06-03 09:23:02.422959 time_interpret-0.1.0/README.md
--rw-r--r--   0        0        0     1999 2023-06-03 09:26:47.240403 time_interpret-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.1.0/tint/__init__.py
--rw-r--r--   0        0        0       22 2023-06-03 09:23:02.462862 time_interpret-0.1.0/tint/__version__.py
--rw-r--r--   0        0        0      966 2023-06-03 09:23:02.462995 time_interpret-0.1.0/tint/attr/__init__.py
--rw-r--r--   0        0        0    13788 2023-06-03 09:23:02.463319 time_interpret-0.1.0/tint/attr/augmented_occlusion.py
--rw-r--r--   0        0        0       84 2023-06-03 09:23:02.463444 time_interpret-0.1.0/tint/attr/base/__init__.py
--rw-r--r--   0        0        0    28773 2023-06-03 09:23:02.463603 time_interpret-0.1.0/tint/attr/base/feature_ablation.py
--rw-r--r--   0        0        0     4337 2023-06-03 09:23:02.463734 time_interpret-0.1.0/tint/attr/bayes.py
--rw-r--r--   0        0        0     5583 2023-06-03 09:23:02.463834 time_interpret-0.1.0/tint/attr/bayes_mask.py
--rw-r--r--   0        0        0    10394 2023-06-03 09:23:02.464050 time_interpret-0.1.0/tint/attr/discretised_ig.py
--rw-r--r--   0        0        0     6497 2023-06-03 09:23:02.464196 time_interpret-0.1.0/tint/attr/dynamic_masks.py
--rw-r--r--   0        0        0    13321 2023-06-03 09:23:02.464622 time_interpret-0.1.0/tint/attr/fit.py
--rw-r--r--   0        0        0      420 2023-06-03 09:23:02.464739 time_interpret-0.1.0/tint/attr/geodesic_ig.py
--rw-r--r--   0        0        0     8144 2023-06-03 09:23:02.464897 time_interpret-0.1.0/tint/attr/lof.py
--rw-r--r--   0        0        0      887 2023-06-03 09:23:02.465026 time_interpret-0.1.0/tint/attr/models/__init__.py
--rw-r--r--   0        0        0    11264 2023-06-03 09:23:02.465191 time_interpret-0.1.0/tint/attr/models/bayes_linear.py
--rw-r--r--   0        0        0    11749 2023-06-03 09:23:02.465316 time_interpret-0.1.0/tint/attr/models/bayes_mask.py
--rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.1.0/tint/attr/models/joint_features_generator.py
--rw-r--r--   0        0        0    15814 2023-06-03 09:23:02.465493 time_interpret-0.1.0/tint/attr/models/mask.py
--rw-r--r--   0        0        0     7693 2023-06-03 09:23:02.465613 time_interpret-0.1.0/tint/attr/models/path_generator.py
--rw-r--r--   0        0        0     7957 2023-06-03 09:23:02.465828 time_interpret-0.1.0/tint/attr/models/retain.py
--rw-r--r--   0        0        0    19095 2023-06-03 09:23:02.466012 time_interpret-0.1.0/tint/attr/occlusion.py
--rw-r--r--   0        0        0     7881 2023-06-03 09:23:02.466199 time_interpret-0.1.0/tint/attr/retain.py
--rw-r--r--   0        0        0      718 2023-06-03 09:23:02.466282 time_interpret-0.1.0/tint/attr/smooth_grad.py
--rw-r--r--   0        0        0    14038 2023-06-03 09:23:02.466447 time_interpret-0.1.0/tint/attr/temporal_augmented_occlusion.py
--rw-r--r--   0        0        0    21753 2023-06-03 09:23:02.466608 time_interpret-0.1.0/tint/attr/temporal_ig.py
--rw-r--r--   0        0        0    14146 2023-06-03 09:23:02.466742 time_interpret-0.1.0/tint/attr/temporal_occlusion.py
--rw-r--r--   0        0        0    12809 2023-06-03 09:23:02.466921 time_interpret-0.1.0/tint/attr/time_forward_tunnel.py
--rw-r--r--   0        0        0       23 2023-06-03 09:23:02.467044 time_interpret-0.1.0/tint/data/.gitignore
--rw-r--r--   0        0        0      261 2023-06-03 09:23:02.475939 time_interpret-0.1.0/tint/datasets/__init__.py
--rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.1.0/tint/datasets/arma.py
--rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.1.0/tint/datasets/biobank.py
--rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.1.0/tint/datasets/dataset.py
--rw-r--r--   0        0        0    11253 2023-06-03 09:23:02.476261 time_interpret-0.1.0/tint/datasets/hawkes.py
--rw-r--r--   0        0        0     8679 2023-06-03 09:23:02.476396 time_interpret-0.1.0/tint/datasets/hmm.py
--rw-r--r--   0        0        0    32885 2023-06-03 09:23:02.476586 time_interpret-0.1.0/tint/datasets/mimic3.py
--rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.1.0/tint/datasets/utils/__init__.py
--rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.1.0/tint/datasets/utils/fasttext.py
--rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.1.0/tint/datasets/utils/labels.json
--rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.1.0/tint/datasets/utils/labels.py
--rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.1.0/tint/datasets/utils/read_3_2.json
--rw-r--r--   0        0        0      363 2023-06-03 09:23:02.476845 time_interpret-0.1.0/tint/metrics/__init__.py
--rw-r--r--   0        0        0     6894 2023-06-03 09:23:02.476999 time_interpret-0.1.0/tint/metrics/accuracy.py
--rw-r--r--   0        0        0     3276 2023-06-03 09:23:02.477132 time_interpret-0.1.0/tint/metrics/base.py
--rw-r--r--   0        0        0     6677 2023-06-03 09:23:02.477251 time_interpret-0.1.0/tint/metrics/comprehensiveness.py
--rw-r--r--   0        0        0     6651 2023-06-03 09:23:02.477365 time_interpret-0.1.0/tint/metrics/cross_entropy.py
--rw-r--r--   0        0        0    11449 2023-06-03 09:23:02.477516 time_interpret-0.1.0/tint/metrics/lipschitz_max.py
--rw-r--r--   0        0        0     6681 2023-06-03 09:23:02.477630 time_interpret-0.1.0/tint/metrics/log_odds.py
--rw-r--r--   0        0        0     6698 2023-06-03 09:23:02.477739 time_interpret-0.1.0/tint/metrics/sufficiency.py
--rw-r--r--   0        0        0      261 2023-06-03 09:23:02.477875 time_interpret-0.1.0/tint/metrics/white_box/__init__.py
--rw-r--r--   0        0        0     2241 2023-06-03 09:23:02.477994 time_interpret-0.1.0/tint/metrics/white_box/aup.py
--rw-r--r--   0        0        0     2131 2023-06-03 09:23:02.478101 time_interpret-0.1.0/tint/metrics/white_box/auprc.py
--rw-r--r--   0        0        0     2235 2023-06-03 09:23:02.478221 time_interpret-0.1.0/tint/metrics/white_box/aur.py
--rw-r--r--   0        0        0     2411 2023-06-03 09:23:02.478321 time_interpret-0.1.0/tint/metrics/white_box/base.py
--rw-r--r--   0        0        0     2422 2023-06-03 09:23:02.478433 time_interpret-0.1.0/tint/metrics/white_box/entropy.py
--rw-r--r--   0        0        0     2259 2023-06-03 09:23:02.478553 time_interpret-0.1.0/tint/metrics/white_box/information.py
--rw-r--r--   0        0        0     2083 2023-06-03 09:23:02.478675 time_interpret-0.1.0/tint/metrics/white_box/roc_auc.py
--rw-r--r--   0        0        0      249 2023-06-03 09:23:02.478816 time_interpret-0.1.0/tint/models/__init__.py
--rw-r--r--   0        0        0     2022 2023-06-03 09:23:02.478991 time_interpret-0.1.0/tint/models/bert.py
--rw-r--r--   0        0        0     6531 2023-06-03 09:23:02.479129 time_interpret-0.1.0/tint/models/cnn.py
--rw-r--r--   0        0        0     4932 2023-06-03 09:23:02.479251 time_interpret-0.1.0/tint/models/mlp.py
--rw-r--r--   0        0        0     5581 2023-06-03 09:23:02.479400 time_interpret-0.1.0/tint/models/net.py
--rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.1.0/tint/models/rnn.py
--rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.1.0/tint/models/transformer.py
--rw-r--r--   0        0        0      342 2023-06-03 09:23:02.479544 time_interpret-0.1.0/tint/utils/__init__.py
--rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.1.0/tint/utils/collate.py
--rw-r--r--   0        0        0     6628 2023-06-03 09:23:02.479682 time_interpret-0.1.0/tint/utils/common.py
--rw-r--r--   0        0        0     1000 2023-06-03 09:23:02.479982 time_interpret-0.1.0/tint/utils/tensor_dataset.py
--rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.1.0/tint/utils/tqdm.py
--rw-r--r--   0        0        0     5182 1970-01-01 00:00:00.000000 time_interpret-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2354 2023-06-03 09:31:38.184118 time_interpret-0.2.0/README.md
+-rw-r--r--   0        0        0     2035 2023-06-03 09:36:55.387260 time_interpret-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.2.0/tint/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-03 09:31:38.222143 time_interpret-0.2.0/tint/__version__.py
+-rw-r--r--   0        0        0     1231 2023-06-03 09:31:38.222248 time_interpret-0.2.0/tint/attr/__init__.py
+-rw-r--r--   0        0        0    13796 2023-06-03 09:31:38.222402 time_interpret-0.2.0/tint/attr/augmented_occlusion.py
+-rw-r--r--   0        0        0     4295 2023-06-03 09:31:38.222516 time_interpret-0.2.0/tint/attr/bayes.py
+-rw-r--r--   0        0        0    10394 2023-06-03 09:23:02.464050 time_interpret-0.2.0/tint/attr/discretised_ig.py
+-rw-r--r--   0        0        0     6497 2023-06-03 09:23:02.464196 time_interpret-0.2.0/tint/attr/dynamic_masks.py
+-rw-r--r--   0        0        0     9786 2023-06-03 09:31:38.222641 time_interpret-0.2.0/tint/attr/extremal_mask.py
+-rw-r--r--   0        0        0    28774 2023-06-03 09:31:38.222802 time_interpret-0.2.0/tint/attr/feature_ablation.py
+-rw-r--r--   0        0        0    13321 2023-06-03 09:23:02.464622 time_interpret-0.2.0/tint/attr/fit.py
+-rw-r--r--   0        0        0    31058 2023-06-03 09:31:38.223089 time_interpret-0.2.0/tint/attr/geodesic_ig.py
+-rw-r--r--   0        0        0     8439 2023-06-03 09:31:38.223233 time_interpret-0.2.0/tint/attr/lof.py
+-rw-r--r--   0        0        0      551 2023-06-03 09:31:38.223361 time_interpret-0.2.0/tint/attr/models/__init__.py
+-rw-r--r--   0        0        0     8059 2023-06-03 09:31:38.223488 time_interpret-0.2.0/tint/attr/models/bayes_linear.py
+-rw-r--r--   0        0        0     8365 2023-06-03 09:31:38.223599 time_interpret-0.2.0/tint/attr/models/extremal_mask.py
+-rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.2.0/tint/attr/models/joint_features_generator.py
+-rw-r--r--   0        0        0    15936 2023-06-03 09:31:38.223738 time_interpret-0.2.0/tint/attr/models/mask.py
+-rw-r--r--   0        0        0     7693 2023-06-03 09:23:02.465613 time_interpret-0.2.0/tint/attr/models/path_generator.py
+-rw-r--r--   0        0        0     7957 2023-06-03 09:23:02.465828 time_interpret-0.2.0/tint/attr/models/retain.py
+-rw-r--r--   0        0        0    19107 2023-06-03 09:31:38.223849 time_interpret-0.2.0/tint/attr/occlusion.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:31:38.223881 time_interpret-0.2.0/tint/attr/perturbed_ig.py
+-rw-r--r--   0        0        0     7881 2023-06-03 09:23:02.466199 time_interpret-0.2.0/tint/attr/retain.py
+-rw-r--r--   0        0        0    19391 2023-06-03 09:31:38.224017 time_interpret-0.2.0/tint/attr/seq_ig.py
+-rw-r--r--   0        0        0      718 2023-06-03 09:23:02.466282 time_interpret-0.2.0/tint/attr/smooth_grad.py
+-rw-r--r--   0        0        0    14038 2023-06-03 09:23:02.466447 time_interpret-0.2.0/tint/attr/temporal_augmented_occlusion.py
+-rw-r--r--   0        0        0    23450 2023-06-03 09:31:38.224170 time_interpret-0.2.0/tint/attr/temporal_ig.py
+-rw-r--r--   0        0        0    14146 2023-06-03 09:23:02.466742 time_interpret-0.2.0/tint/attr/temporal_occlusion.py
+-rw-r--r--   0        0        0    12809 2023-06-03 09:23:02.466921 time_interpret-0.2.0/tint/attr/time_forward_tunnel.py
+-rw-r--r--   0        0        0       41 2023-06-03 09:31:38.224431 time_interpret-0.2.0/tint/data/.gitignore
+-rw-r--r--   0        0        0      208 2023-06-03 09:31:38.226008 time_interpret-0.2.0/tint/datasets/__init__.py
+-rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.2.0/tint/datasets/arma.py
+-rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.2.0/tint/datasets/biobank.py
+-rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.2.0/tint/datasets/dataset.py
+-rw-r--r--   0        0        0    11239 2023-06-03 09:31:38.226150 time_interpret-0.2.0/tint/datasets/hawkes.py
+-rw-r--r--   0        0        0     8679 2023-06-03 09:23:02.476396 time_interpret-0.2.0/tint/datasets/hmm.py
+-rw-r--r--   0        0        0    33349 2023-06-03 09:31:38.226352 time_interpret-0.2.0/tint/datasets/mimic3.py
+-rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.2.0/tint/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.2.0/tint/datasets/utils/fasttext.py
+-rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.2.0/tint/datasets/utils/labels.json
+-rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.2.0/tint/datasets/utils/labels.py
+-rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.2.0/tint/datasets/utils/read_3_2.json
+-rw-r--r--   0        0        0      427 2023-06-03 09:31:38.226498 time_interpret-0.2.0/tint/metrics/__init__.py
+-rw-r--r--   0        0        0     9162 2023-06-03 09:31:38.226662 time_interpret-0.2.0/tint/metrics/accuracy.py
+-rw-r--r--   0        0        0     6147 2023-06-03 09:31:38.226811 time_interpret-0.2.0/tint/metrics/base.py
+-rw-r--r--   0        0        0     8751 2023-06-03 09:31:38.227069 time_interpret-0.2.0/tint/metrics/comprehensiveness.py
+-rw-r--r--   0        0        0     8915 2023-06-03 09:31:38.227188 time_interpret-0.2.0/tint/metrics/cross_entropy.py
+-rw-r--r--   0        0        0    10150 2023-06-03 09:31:38.227340 time_interpret-0.2.0/tint/metrics/lipschitz_max.py
+-rw-r--r--   0        0        0     8755 2023-06-03 09:31:38.227464 time_interpret-0.2.0/tint/metrics/log_odds.py
+-rw-r--r--   0        0        0     9064 2023-06-03 09:31:38.227565 time_interpret-0.2.0/tint/metrics/mae.py
+-rw-r--r--   0        0        0     9048 2023-06-03 09:31:38.227658 time_interpret-0.2.0/tint/metrics/mse.py
+-rw-r--r--   0        0        0     8707 2023-06-03 09:31:38.227836 time_interpret-0.2.0/tint/metrics/sufficiency.py
+-rw-r--r--   0        0        0      130 2023-06-03 09:31:38.227939 time_interpret-0.2.0/tint/metrics/weights/__init__.py
+-rw-r--r--   0        0        0     1674 2023-06-03 09:31:38.228031 time_interpret-0.2.0/tint/metrics/weights/lime_weights.py
+-rw-r--r--   0        0        0     1644 2023-06-03 09:31:38.228120 time_interpret-0.2.0/tint/metrics/weights/lof_weights.py
+-rw-r--r--   0        0        0      360 2023-06-03 09:31:38.228278 time_interpret-0.2.0/tint/metrics/white_box/__init__.py
+-rw-r--r--   0        0        0     2267 2023-06-03 09:31:38.228410 time_interpret-0.2.0/tint/metrics/white_box/aup.py
+-rw-r--r--   0        0        0     2157 2023-06-03 09:31:38.228536 time_interpret-0.2.0/tint/metrics/white_box/auprc.py
+-rw-r--r--   0        0        0     2261 2023-06-03 09:31:38.228664 time_interpret-0.2.0/tint/metrics/white_box/aur.py
+-rw-r--r--   0        0        0     2548 2023-06-03 09:31:38.228771 time_interpret-0.2.0/tint/metrics/white_box/base.py
+-rw-r--r--   0        0        0     2448 2023-06-03 09:31:38.228881 time_interpret-0.2.0/tint/metrics/white_box/entropy.py
+-rw-r--r--   0        0        0     2285 2023-06-03 09:31:38.228999 time_interpret-0.2.0/tint/metrics/white_box/information.py
+-rw-r--r--   0        0        0     2152 2023-06-03 09:31:38.229074 time_interpret-0.2.0/tint/metrics/white_box/mae.py
+-rw-r--r--   0        0        0     2148 2023-06-03 09:31:38.229141 time_interpret-0.2.0/tint/metrics/white_box/mse.py
+-rw-r--r--   0        0        0     2178 2023-06-03 09:31:38.229223 time_interpret-0.2.0/tint/metrics/white_box/rmse.py
+-rw-r--r--   0        0        0     2109 2023-06-03 09:31:38.229337 time_interpret-0.2.0/tint/metrics/white_box/roc_auc.py
+-rw-r--r--   0        0        0      346 2023-06-03 09:31:38.229462 time_interpret-0.2.0/tint/models/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-03 09:31:38.229595 time_interpret-0.2.0/tint/models/bert.py
+-rw-r--r--   0        0        0     6863 2023-06-03 09:31:38.229855 time_interpret-0.2.0/tint/models/cnn.py
+-rw-r--r--   0        0        0     2496 2023-06-03 09:31:38.229929 time_interpret-0.2.0/tint/models/distilbert.py
+-rw-r--r--   0        0        0     5058 2023-06-03 09:31:38.230072 time_interpret-0.2.0/tint/models/mlp.py
+-rw-r--r--   0        0        0     5581 2023-06-03 09:23:02.479400 time_interpret-0.2.0/tint/models/net.py
+-rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.2.0/tint/models/rnn.py
+-rw-r--r--   0        0        0     2398 2023-06-03 09:31:38.230138 time_interpret-0.2.0/tint/models/roberta.py
+-rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.2.0/tint/models/transformer.py
+-rw-r--r--   0        0        0      714 2023-06-03 09:31:38.230248 time_interpret-0.2.0/tint/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2023-06-03 09:31:38.230323 time_interpret-0.2.0/tint/utils/a_star_path.py
+-rw-r--r--   0        0        0     1809 2023-06-03 09:31:38.230396 time_interpret-0.2.0/tint/utils/baching.py
+-rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.2.0/tint/utils/collate.py
+-rw-r--r--   0        0        0     9571 2023-06-03 09:31:38.230535 time_interpret-0.2.0/tint/utils/common.py
+-rw-r--r--   0        0        0     1540 2023-06-03 09:31:38.230622 time_interpret-0.2.0/tint/utils/perturb_func.py
+-rw-r--r--   0        0        0     1000 2023-06-03 09:23:02.479982 time_interpret-0.2.0/tint/utils/tensor_dataset.py
+-rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.2.0/tint/utils/tqdm.py
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 time_interpret-0.2.0/PKG-INFO
```

### Comparing `time_interpret-0.1.0/README.md` & `time_interpret-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,8 +77,9 @@
 - [Retain](https://arxiv.org/pdf/1608.05745)
 - [SmoothGrad](https://arxiv.org/abs/1810.03292)
 
 
 ## Acknowledgment
 - [Jonathan Crabbe](https://github.com/JonathanCrabbe/Dynamask) for the DynaMask implementation.
 - [Sana Tonekaboni](https://github.com/sanatonek/time_series_explainability/tree/master/TSX) for the fit implementation.
-- [INK Lab](https://github.com/INK-USC/DIG) for the discretized integrated gradients implementation.
+- [INK Lab](https://github.com/INK-USC/DIG) for the discretized integrated gradients implementation.
+- [Dylan Slack](https://github.com/dylan-slack/Modeling-Uncertainty-Local-Explainability) for the BayesLime and BayesShap implementations.
```

### Comparing `time_interpret-0.1.0/pyproject.toml` & `time_interpret-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="time_interpret"
-version="0.1.0"
+version="0.2.0"
 authors=[
     {name="Joseph Enguehard", email="joseph@skippr.com"},
 ]
-description="Time interpret library for PyTorch."
+description="Model interpretability library for PyTorch with a focus on time series."
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
     "deep-learning",
     "pytorch",
     "captum",
     "explainable-ai",
```

### Comparing `time_interpret-0.1.0/tint/attr/augmented_occlusion.py` & `time_interpret-0.2.0/tint/attr/augmented_occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
             baselines=tuple(range(len(inputs))),
             target=target,
             additional_forward_args=additional_forward_args,
             # We multiply perturbations_per_eval by the number of
             # sampling to expand tensors along the first dim
             perturbations_per_eval=perturbations_per_eval * self.n_sampling,
             attributions_fn=attributions_fn,
-            show_progress=False,
+            show_progress=show_progress,
         )
 
     def _construct_ablated_input(
         self,
         expanded_input: Tensor,
         input_mask: Union[None, Tensor],
         baseline: Union[Tensor, int, float],
```

### Comparing `time_interpret-0.1.0/tint/attr/base/feature_ablation.py` & `time_interpret-0.2.0/tint/attr/feature_ablation.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                             or the first dimension is one and the remaining
                             dimensions match with the corresponding
                             input tensor.
 
                           - or a scalar, corresponding to a tensor in the
                             inputs' tuple. This scalar value is broadcasted
                             for corresponding input tensor.
+
                         In the cases when `baselines` is not provided, we internally
                         use zero scalar corresponding to each input tensor.
                         Default: None
             target (int, tuple, tensor or list, optional):  Output indices for
                         which gradients are computed (for classification cases,
                         this is usually the target class).
                         If the network returns a scalar value per example,
```

### Comparing `time_interpret-0.1.0/tint/attr/bayes.py` & `time_interpret-0.2.0/tint/attr/bayes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from captum.attr import Lime, KernelShap
 from captum._utils.models import Model
 from typing import Callable
 
-from .models import SkLearnBayesianRidge
+from .models import BLRRidge
 
 
 class BayesLime(Lime):
     """
     Bayesian version of Lime.
 
     Args:
@@ -58,21 +58,21 @@
     def __init__(
         self,
         forward_func: Callable,
         interpretable_model: Model = None,
     ) -> None:
         super().__init__(
             forward_func=forward_func,
-            interpretable_model=interpretable_model or SkLearnBayesianRidge(),
+            interpretable_model=interpretable_model or BLRRidge(),
             similarity_func=None,
             perturb_func=None,
         )
 
 
-class BayesShap(KernelShap):
+class BayesKernelShap(KernelShap):
     """
     Bayesian version of KernelShap.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         interpretable_model (Model): Model object to train interpretable model.
@@ -104,27 +104,25 @@
             Default: None
 
     References:
         https://arxiv.org/pdf/2008.05030
 
     Examples:
         >>> import torch as th
-        >>> from tint.attr import BayesShap
+        >>> from tint.attr import BayesKernelShap
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 5)
         >>> mlp = MLP([5, 3, 1])
         <BLANKLINE>
-        >>> explainer = BayesShap(mlp)
+        >>> explainer = BayesKernelShap(mlp)
         >>> attr = explainer.attribute(inputs)
     """
 
     def __init__(
         self,
         forward_func: Callable,
         interpretable_model: Model = None,
     ) -> None:
         super().__init__(forward_func=forward_func)
 
-        self.interpretable_model = (
-            interpretable_model or SkLearnBayesianRidge()
-        )
+        self.interpretable_model = interpretable_model or BLRRidge()
```

### Comparing `time_interpret-0.1.0/tint/attr/discretised_ig.py` & `time_interpret-0.2.0/tint/attr/discretised_ig.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/dynamic_masks.py` & `time_interpret-0.2.0/tint/attr/dynamic_masks.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/fit.py` & `time_interpret-0.2.0/tint/attr/fit.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/lof.py` & `time_interpret-0.2.0/tint/attr/lof.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from captum.attr import KernelShap, Lime
 from captum._utils.models.model import Model
+from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 
 from sklearn.neighbors import LocalOutlierFactor
 from torch import Tensor
 from typing import Callable, Optional
 
 EPS = 1e-5
 
@@ -25,32 +26,36 @@
         **kwargs,
     ):
         self.lof = LocalOutlierFactor(
             n_neighbors=n_neighbors,
             novelty=True,
             **kwargs,
         )
-        self.lof.fit(
-            X=embeddings.reshape(-1, embeddings.shape[-1]).cpu().numpy()
-        )
+        self.lof.fit(X=embeddings.reshape(len(embeddings), -1).cpu().numpy())
 
         self._similarity_func = None
 
     def lof_similarity_func(
         self,
-        original_inp: Tensor,
-        perturbed_inp: Tensor,
-        interpretable_sample: Tensor,
+        original_inp: TensorOrTupleOfTensorsGeneric,
+        perturbed_inp: TensorOrTupleOfTensorsGeneric,
+        interpretable_sample: TensorOrTupleOfTensorsGeneric,
         **kwargs,
     ):
-        assert isinstance(
-            original_inp, Tensor
-        ), "Only one input is accepted with this method."
+        # Only use the first input if tuple
+        # Lof only accepts one input
+        pert_inp = perturbed_inp
+        if isinstance(perturbed_inp, tuple):
+            assert (
+                len(perturbed_inp) == 1
+            ), "Only one input is accepted with this method."
+            pert_inp = perturbed_inp[0]
+
         score = -self.lof.score_samples(
-            perturbed_inp.reshape(-1, perturbed_inp.shape[-1]).cpu().numpy()
+            pert_inp.reshape(len(pert_inp), -1).cpu().numpy()
         )
         score = 1 / score.clip(min=1)
         return self._similarity_func(
             original_inp,
             perturbed_inp,
             interpretable_sample,
             **kwargs,
```

### Comparing `time_interpret-0.1.0/tint/attr/models/joint_features_generator.py` & `time_interpret-0.2.0/tint/attr/models/joint_features_generator.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/models/mask.py` & `time_interpret-0.2.0/tint/attr/models/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,25 +217,27 @@
     def regularisation(self, loss: th.Tensor) -> th.Tensor:
         # Get size regularisation
         mask_sorted = self.mask.reshape(len(self.mask), -1).sort().values
         size_reg = (
             (self.reg_ref.to(self.mask.device) - mask_sorted) ** 2
         ).mean()
 
-        # Get time regularisation
-        mask = self.mask.reshape(
-            (len(self.mask) // len(self.keep_ratio), len(self.keep_ratio))
-            + self.mask.shape[1:]
-        )
-        time_reg = (
-            th.abs(
-                mask[:, :, 1 : self.mask.shape[TIME_DIM] - 1, ...]
-                - mask[:, :, : self.mask.shape[TIME_DIM] - 2, ...]
+        # Get time regularisation if factor is positive
+        time_reg = 0.0
+        if self.time_reg_factor > 0:
+            mask = self.mask.reshape(
+                (len(self.mask) // len(self.keep_ratio), len(self.keep_ratio))
+                + self.mask.shape[1:]
             )
-        ).mean()
+            time_reg = (
+                th.abs(
+                    mask[:, :, 1 : self.mask.shape[TIME_DIM] - 1, ...]
+                    - mask[:, :, : self.mask.shape[TIME_DIM] - 2, ...]
+                )
+            ).mean()
 
         # Return loss plus regularisation
         return (
             (1.0 - 2 * self.deletion_mode) * loss
             + self.size_reg_factor * size_reg
             + self.time_reg_factor * time_reg
         )
```

### Comparing `time_interpret-0.1.0/tint/attr/models/path_generator.py` & `time_interpret-0.2.0/tint/attr/models/path_generator.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/models/retain.py` & `time_interpret-0.2.0/tint/attr/models/retain.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/occlusion.py` & `time_interpret-0.2.0/tint/attr/occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from captum.attr._utils.common import (
     _format_and_verify_sliding_window_shapes,
     _format_and_verify_strides,
 )
 from captum.log import log_usage
 from torch import Tensor
 
-from .base import FeatureAblation
+from .feature_ablation import FeatureAblation
 
 
 class Occlusion(FeatureAblation):
     r"""
     A perturbation based approach to compute attribution, involving
     replacing each contiguous rectangular region with a given baseline /
     reference, and computing the difference in output. For features located
```

### Comparing `time_interpret-0.1.0/tint/attr/retain.py` & `time_interpret-0.2.0/tint/attr/retain.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/smooth_grad.py` & `time_interpret-0.2.0/tint/attr/smooth_grad.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/temporal_augmented_occlusion.py` & `time_interpret-0.2.0/tint/attr/temporal_augmented_occlusion.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/temporal_ig.py` & `time_interpret-0.2.0/tint/attr/temporal_ig.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,25 @@
             method is called global.
             More detailed can be found here:
             https://arxiv.org/abs/1711.06104
 
             In case of integrated gradients, if `multiply_by_inputs`
             is set to True, final sensitivity scores are being multiplied by
             (inputs - baselines).
+
+    Examples:
+        >>> import torch as th
+        >>> from tint.attr import TemporalIntegratedGradients
+        >>> from tint.models import MLP
+        <BLANKLINE>
+        >>> inputs = th.rand(8, 7, 5)
+        >>> mlp = MLP([5, 3, 1])
+        <BLANKLINE>
+        >>> explainer = TemporalIntegratedGradients(mlp)
+        >>> attr = explainer.attribute(inputs, target=0)
     """
 
     def __init__(
         self,
         forward_func: Callable,
         multiply_by_inputs: bool = True,
     ) -> None:
@@ -67,16 +78,18 @@
     @typing.overload
     def attribute(
         self,
         inputs: TensorOrTupleOfTensorsGeneric,
         baselines: BaselineType = None,
         target: TargetType = None,
         additional_forward_args: Any = None,
+        times: Tensor = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
+        strategy: str = "fixed",
         internal_batch_size: Union[None, int] = None,
         return_convergence_delta: Literal[False] = False,
         temporal_target: bool = False,
         temporal_additional_forward_args: Tuple[bool] = None,
         return_temporal_attributions: bool = False,
         show_progress: bool = False,
     ) -> TensorOrTupleOfTensorsGeneric:
@@ -85,16 +98,18 @@
     @typing.overload
     def attribute(
         self,
         inputs: TensorOrTupleOfTensorsGeneric,
         baselines: BaselineType = None,
         target: TargetType = None,
         additional_forward_args: Any = None,
+        times: Tensor = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
+        strategy: str = "fixed",
         internal_batch_size: Union[None, int] = None,
         *,
         return_convergence_delta: Literal[True],
         temporal_target: bool = False,
         temporal_additional_forward_args: Tuple[bool] = None,
         return_temporal_attributions: bool = False,
         show_progress: bool = False,
@@ -104,16 +119,18 @@
     @log_usage()
     def attribute(  # type: ignore
         self,
         inputs: TensorOrTupleOfTensorsGeneric,
         baselines: BaselineType = None,
         target: TargetType = None,
         additional_forward_args: Any = None,
+        times: Tensor = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
+        strategy: str = "fixed",
         internal_batch_size: Union[None, int] = None,
         return_convergence_delta: bool = False,
         temporal_target: bool = False,
         temporal_additional_forward_args: Tuple[bool] = None,
         return_temporal_attributions: bool = False,
         show_progress: bool = False,
     ) -> Union[
@@ -199,20 +216,26 @@
                 correspond to the number of examples. It will be
                 repeated for each of `n_steps` along the integrated
                 path. For all other types, the given argument is used
                 for all forward evaluations.
                 Note that attributions are not computed with respect
                 to these arguments.
                 Default: None
+            times (Tensor, optional): Tensor of times. If not provided, it is
+                assumed that the points are temporally equally spaced.
+                Default: None
             n_steps (int, optional): The number of steps used by the approximation
                 method. Default: 50.
             method (string, optional): Method for approximating the integral,
                 one of `riemann_right`, `riemann_left`, `riemann_middle`,
                 `riemann_trapezoid` or `gausslegendre`.
                 Default: `gausslegendre` if no method is provided.
+            strategy (str, optinal): Strategy to distribute gradients
+                evaluations over time. Either ``'fixed'`` or ``'interval'``
+                Default: 'fixed'
             internal_batch_size (int, optional): Divides total #steps * #examples
                 data points into chunks of size at most internal_batch_size,
                 which are computed (forward / backward passes)
                 sequentially. internal_batch_size must be at least equal to
                 #examples.
                 For DataParallel models, each batch is split among the
                 available devices, so evaluations on each available
@@ -268,14 +291,30 @@
         # Get baselines
         baselines = _format_baseline(baselines, inputs)
 
         assert all(
             x.shape[1] == inputs[0].shape[1] for x in inputs
         ), "All inputs must have the same time dimension. (dimension 1)"
 
+        # Get n_steps depending on strategy
+        n_steps = [n_steps] * inputs[0].shape[1]
+        assert strategy in [
+            "fixed",
+            "interval",
+        ], f"strategy must be either fixed or interval, got {strategy}."
+        if strategy == "interval" and times is not None:
+            max_interval = (times[1:] - times[:-1]).max().item()
+            n_steps = [
+                torch.div(t, max_interval / n_steps[0], rounding_mode="floor")
+                .long()
+                .item()
+                + 1
+                for t in times[1:] - times[:-1]
+            ]
+
         attributions_partial_list = list()
         delta_partial_list = list()
         is_attrib_tuple = True
 
         times = range(1, inputs[0].shape[1] + 1)
         if show_progress:
             times = get_progress_bars()(
@@ -311,15 +350,15 @@
                 delta_partial,
             ) = self.compute_partial_attribution(
                 partial_inputs=partial_inputs,
                 is_inputs_tuple=is_inputs_tuple,
                 baselines=partial_baselines,
                 target=partial_target,
                 additional_forward_args=partial_additional_forward_args,
-                n_steps=n_steps,
+                n_steps=n_steps[time - 1],
                 method=method,
                 internal_batch_size=internal_batch_size,
                 return_convergence_delta=return_convergence_delta,
             )
             attributions_partial_list.append(attributions_partial)
             delta_partial_list.append(delta_partial)
 
@@ -441,37 +480,42 @@
 
     @staticmethod
     def scale_features(
         inputs: Tuple[Tensor, ...],
         baselines: Tuple[Union[Tensor, int, float], ...],
         alphas: List[float],
     ) -> Tuple[Tensor]:
+        # Get last time of baseline if Tensor
+        baselines = tuple(
+            baseline[:, -1, ...] if isinstance(baseline, Tensor) else baseline
+            for baseline in baselines
+        )
+
         # Only rescale the last time of the inputs
         scaled_features_tpl = tuple(
             torch.cat(
                 [
                     torch.cat(
                         [
                             input[:, :-1, ...],
                             (
-                                baseline[:, -1, ...]
-                                + alpha
-                                * (input[:, -1, ...] - baseline[:, -1, ...])
+                                baseline
+                                + alpha * (input[:, -1, ...] - baseline)
                             ).unsqueeze(1),
                         ],
                         dim=1,
                     )
                     for alpha in alphas
                 ],
                 dim=0,
             ).requires_grad_()
             for input, baseline in zip(inputs, baselines)
         )
 
-        return scaled_features_tpl
+        return cast(Tuple[Tensor, ...], scaled_features_tpl)
 
     def compute_partial_attribution(
         self,
         partial_inputs: Tuple[Tensor, ...],
         is_inputs_tuple: bool,
         baselines: BaselineType = None,
         target: TargetType = None,
```

### Comparing `time_interpret-0.1.0/tint/attr/temporal_occlusion.py` & `time_interpret-0.2.0/tint/attr/temporal_occlusion.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/attr/time_forward_tunnel.py` & `time_interpret-0.2.0/tint/attr/time_forward_tunnel.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/arma.py` & `time_interpret-0.2.0/tint/datasets/arma.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/biobank.py` & `time_interpret-0.2.0/tint/datasets/biobank.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/dataset.py` & `time_interpret-0.2.0/tint/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/hawkes.py` & `time_interpret-0.2.0/tint/datasets/hawkes.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
             n_folds=n_folds,
             fold=fold,
             num_workers=num_workers,
             seed=seed,
         )
 
         self.mu = mu or [0.05, 0.05]
-        self.alpha = alpha or [[0.05, 0.2], [0.3, 0.1]]
-        self.decay = decay or [[1.0, 1.0], [2.0, 1.0]]
-        self.window = window or 1000
+        self.alpha = alpha or [[0.5, 0.05], [0.02, 0.3]]
+        self.decay = decay or [[1.0, 0.0], [0.0, 1.0]]
+        self.window = window or 100
 
     def download(
         self,
         train_size: int = 1000,
         test_size: int = 100,
         split: str = "train",
     ):
@@ -165,15 +165,15 @@
         )
         for i in range(len(mu)):
             for j in range(len(mu)):
                 hawkes.set_kernel(
                     i=i,
                     j=j,
                     kernel=HawkesKernelExp(
-                        intensity=alpha[i][j] / decay[i][j], decay=decay[i][j]
+                        intensity=alpha[i][j], decay=decay[i][j]
                     ),
                 )
             hawkes.set_baseline(i, mu[i])
 
         hawkes.track_intensity(dt)
         hawkes.simulate()
         return hawkes.timestamps
```

### Comparing `time_interpret-0.1.0/tint/datasets/hmm.py` & `time_interpret-0.2.0/tint/datasets/hmm.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/mimic3.py` & `time_interpret-0.2.0/tint/datasets/mimic3.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
     .. warning::
         Using this dataset requires to have the MIMIC III data running on a
         local server. Please see https://mimic.mit.edu/docs/gettingstarted/local/install-mimic-locally-ubuntu/
         for more information.
 
     Args:
+        task (str): Name of the task to perform. Either ``'mortality'`` or
+            ``'blood_pressure'``. Default to ``'mortality'``
         data_dir (str): Where to download files.
         batch_size (int): Batch size. Default to 32
         n_folds (int): Number of folds for cross validation. If ``None``,
             the dataset is only split once between train and val using
             ``prop_val``. Default to ``None``
         fold (int): Index of the fold to use with cross-validation.
             Ignored if n_folds is None. Default to ``None``
@@ -95,14 +97,15 @@
         >>> mimci3.download(sqluser="your_username", split="train")
         >>> x_train = mimci3.preprocess(split="train")["x"]
         >>> y_train = mimci3.preprocess(split="train")["y"]
     """
 
     def __init__(
         self,
+        task: str = "mortality",
         data_dir: str = os.path.join(
             os.path.split(file_dir)[0],
             "data",
             "mimic3",
         ),
         batch_size: int = 32,
         prop_val: float = 0.2,
@@ -117,14 +120,20 @@
             prop_val=prop_val,
             n_folds=n_folds,
             fold=fold,
             num_workers=num_workers,
             seed=seed,
         )
 
+        assert task in [
+            "mortality",
+            "blood_pressure",
+        ], f"task must be either mortality or blood_pressure, got {task}."
+        self.task = task
+
         # Init mean and std
         self._mean = None
         self._std = None
 
     def download(
         self,
         sqluser: str = "mimicuser",
@@ -718,35 +727,38 @@
     def preprocess(self, split: str = "train") -> dict:
         # Load data
         file = os.path.join(self.data_dir, f"{split}_")
         with open(file + "patient_vital_preprocessed.pkl", "rb") as fp:
             data = pkl.load(fp)
 
         features = th.Tensor([x for (x, y, z) in data]).transpose(1, 2)
-        labels = th.Tensor([y for (x, y, z) in data])
+
+        if self.task == "mortality":
+            labels = th.Tensor([y for (x, y, z) in data])
+        else:
+            labels = features[..., 22]
+            features = th.cat([features[..., :20], features[..., 23:]], dim=-1)
 
         # Compute mean and std
         if split == "train":
-            self._mean = features.reshape(-1, features.shape[-1]).mean(0)
-            self._std = features.reshape(-1, features.shape[-1]).mean(0)
+            self._mean = features.mean(dim=(0, 1), keepdim=True)
+            self._std = features.std(dim=(0, 1), keepdim=True)
         else:
             assert split == "test", "split must be train or test"
 
         assert (
             self._mean is not None
         ), "You must call preprocess('train') first"
 
         # Normalise
-        mean = self._mean.unsqueeze(0).unsqueeze(0)
-        std = self._std.unsqueeze(0).unsqueeze(0)
-        features = (features - mean) / (std + EPS)
+        features = (features - self._mean) / (self._std + EPS)
 
         return {
             "x": features.float(),
-            "y": labels.long(),
+            "y": labels.long() if self.task == "mortality" else labels.float(),
         }
 
 
 def quantize_signal(
     signal, start, step_size, n_steps, value_column, charttime_column
 ):
     quantized_signal = []
```

### Comparing `time_interpret-0.1.0/tint/datasets/utils/fasttext.py` & `time_interpret-0.2.0/tint/datasets/utils/fasttext.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/utils/labels.json` & `time_interpret-0.2.0/tint/datasets/utils/labels.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/utils/labels.py` & `time_interpret-0.2.0/tint/datasets/utils/labels.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/datasets/utils/read_3_2.json` & `time_interpret-0.2.0/tint/datasets/utils/read_3_2.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/metrics/accuracy.py` & `time_interpret-0.2.0/tint/metrics/accuracy.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from captum._utils.typing import (
     BaselineType,
     TargetType,
     TensorOrTupleOfTensorsGeneric,
 )
 
 from torch import Tensor
-from typing import Any, Callable
+from typing import Any, Callable, Tuple, Union
 
 from .base import _base_metric
 
 
 def _accuracy(
     prob_original: Tensor,
     prob_pert: Tensor,
@@ -26,22 +26,31 @@
 def accuracy(
     forward_func: Callable,
     inputs: TensorOrTupleOfTensorsGeneric,
     attributions: TensorOrTupleOfTensorsGeneric,
     baselines: BaselineType = None,
     additional_forward_args: Any = None,
     target: TargetType = None,
+    n_samples: int = 1,
+    n_samples_batch_size: int = None,
+    stdevs: Union[float, Tuple[float, ...]] = 0.0,
+    draw_baseline_from_distrib: bool = False,
     topk: float = 0.2,
+    mask_largest: bool = True,
+    weight_fn: Callable[
+        [Tuple[Tensor, ...], Tuple[Tensor, ...]], Tensor
+    ] = None,
     threshold: float = 0.5,
-) -> Tensor:
+) -> float:
     """
     Accuracy metric.
 
     This metric measures by how much the accuracy of a model drops when
-    removing the topk most important features. Lower is better.
+    removing or only keeping the topk most important features.
+    Lower is better.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         inputs (tensor or tuple of tensors):  Input for which occlusion
             attributions are computed. If forward_func takes a single
             tensor as input, a single input tensor should be provided.
@@ -126,22 +135,52 @@
 
             - A list of tuples with length equal to the number of
               examples in inputs (dim 0), and each tuple containing
               #output_dims - 1 elements. Each tuple is applied as the
               target for the corresponding example.
 
             Default: None
+        n_samples (int, optional): The number of randomly generated examples
+            per sample in the input batch. Random examples are
+            generated by adding gaussian random noise to each sample.
+            Default: 1
+        n_samples_batch_size (int, optional):  The number of the `n_samples`
+            that will be processed together. With the help
+            of this parameter we can avoid out of memory situation and
+            reduce the number of randomly generated examples per sample
+            in each batch.
+            Default: None if `n_samples_batch_size` is not provided. In
+            this case all `n_samples` will be processed together.
+        stdevs (float, or a tuple of floats optional): The standard deviation
+            of gaussian noise with zero mean that is added to each
+            input in the batch. If `stdevs` is a single float value
+            then that same value is used for all inputs. If it is
+            a tuple, then it must have the same length as the inputs
+            tuple. In this case, each stdev value in the stdevs tuple
+            corresponds to the input with the same index in the inputs
+            tuple.
+            Default: 1.0
+        draw_baseline_from_distrib (bool, optional): Indicates whether to
+            randomly draw baseline samples from the `baselines`
+            distribution provided as an input tensor.
+            Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
+        mask_largest: Whether to mask the topk attribution or to only keep
+            the topk attribution.
+            Default: True
+        weight_fn (Callable): Function to compute metrics weighting using
+            original inputs and pertubed inputs. None if note provided.
+            Default: None
         threshold: Threshold for the accuracy. Data higher than the threshold
             is considered as positive, and lower (strictly) negative.
             Default: 0.5
 
     Returns:
-        (float or tuple of floats): The accuracy metric.
+        (float): The accuracy metric.
 
     References:
         https://arxiv.org/pdf/2106.05303
 
     Examples:
         >>> import torch as th
         >>> from captum.attr import Saliency
@@ -160,11 +199,17 @@
         metric=_accuracy,
         forward_func=forward_func,
         inputs=inputs,
         attributions=attributions,
         baselines=baselines,
         additional_forward_args=additional_forward_args,
         target=target,
+        n_samples=n_samples,
+        n_samples_batch_size=n_samples_batch_size,
+        stdevs=stdevs,
+        draw_baseline_from_distrib=draw_baseline_from_distrib,
         topk=topk,
-        largest=True,
+        largest=mask_largest,
+        weight_fn=weight_fn,
+        classification=True,
         threshold=threshold,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/comprehensiveness.py` & `time_interpret-0.2.0/tint/attr/extremal_mask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,240 @@
+import copy
+import torch as th
+
+from captum.attr._utils.attribution import PerturbationAttribution
 from captum.log import log_usage
-from captum._utils.common import _select_targets
+from captum._utils.common import (
+    _format_baseline,
+    _format_input,
+    _format_output,
+    _is_tuple,
+    _validate_input,
+)
 from captum._utils.typing import (
     BaselineType,
     TargetType,
     TensorOrTupleOfTensorsGeneric,
 )
 
-from torch import Tensor
-from typing import Any, Callable
+from pytorch_lightning import Trainer
+from torch.utils.data import DataLoader
+from typing import Any, Callable, Tuple
 
-from .base import _base_metric
+from tint.utils import TensorDataset, _add_temporal_mask, default_collate
+from .models import ExtremalMaskNet
 
 
-def _comprehensiveness(
-    prob_original: Tensor, prob_pert: Tensor, target: Tensor
-) -> Tensor:
-    return _select_targets(prob_original, target) - _select_targets(
-        prob_pert, target
-    )
-
-
-@log_usage()
-def comprehensiveness(
-    forward_func: Callable,
-    inputs: TensorOrTupleOfTensorsGeneric,
-    attributions: TensorOrTupleOfTensorsGeneric,
-    baselines: BaselineType = None,
-    additional_forward_args: Any = None,
-    target: TargetType = None,
-    topk: float = 0.2,
-) -> Tensor:
+class ExtremalMask(PerturbationAttribution):
     """
-    Comprehensiveness metric.
-
-    This comprehensiveness measures by how much the predicted class
-    probability changes when removing the topk most important features.
-    Higher is better.
+    Extremal masks method.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
-        inputs (tensor or tuple of tensors):  Input for which occlusion
-            attributions are computed. If forward_func takes a single
-            tensor as input, a single input tensor should be provided.
-            If forward_func takes multiple tensors as input, a tuple
-            of the input tensors should be provided. It is assumed
-            that for all given input tensors, dimension 0 corresponds
-            to the number of examples (aka batch size), and if
-            multiple input tensors are provided, the examples must
-            be aligned appropriately.
-        attributions (tensor or tuple of tensors):
-            The attributions with respect to each input feature.
-            Attributions will always be
-            the same size as the provided inputs, with each value
-            providing the attribution of the corresponding input index.
-            If a single tensor is provided as inputs, a single tensor
-            is returned. If a tuple is provided for inputs, a tuple of
-            corresponding sized tensors is returned.
-        baselines (scalar, tensor, tuple of scalars or tensors, optional):
-            Baselines define the starting point from which integral
-            is computed and can be provided as:
-
-            - a single tensor, if inputs is a single tensor, with
-              exactly the same dimensions as inputs or the first
-              dimension is one and the remaining dimensions match
-              with inputs.
-
-            - a single scalar, if inputs is a single tensor, which will
-              be broadcasted for each input value in input tensor.
-
-            - a tuple of tensors or scalars, the baseline corresponding
-              to each tensor in the inputs' tuple can be:
-
-              - either a tensor with matching dimensions to
-                corresponding tensor in the inputs' tuple
-                or the first dimension is one and the remaining
-                dimensions match with the corresponding
-                input tensor.
-
-              - or a scalar, corresponding to a tensor in the
-                inputs' tuple. This scalar value is broadcasted
-                for corresponding input tensor.
-
-            In the cases when `baselines` is not provided, we internally
-            use zero scalar corresponding to each input tensor.
-
-            Default: None
-        additional_forward_args (any, optional): If the forward function
-            requires additional arguments other than the inputs for
-            which attributions should not be computed, this argument
-            can be provided. It must be either a single additional
-            argument of a Tensor or arbitrary (non-tuple) type or a
-            tuple containing multiple additional arguments including
-            tensors or any arbitrary python types. These arguments
-            are provided to forward_func in order following the
-            arguments in inputs.
-            For a tensor, the first dimension of the tensor must
-            correspond to the number of examples. It will be
-            repeated for each of `n_steps` along the integrated
-            path. For all other types, the given argument is used
-            for all forward evaluations.
-            Note that attributions are not computed with respect
-            to these arguments.
-            Default: None
-        target (int, tuple, tensor or list, optional):  Output indices for
-            which gradients are computed (for classification cases,
-            this is usually the target class).
-            If the network returns a scalar value per example,
-            no target index is necessary.
-            For general 2D outputs, targets can be either:
-
-            - a single integer or a tensor containing a single
-              integer, which is applied to all input examples
-
-            - a list of integers or a 1D tensor, with length matching
-              the number of examples in inputs (dim 0). Each integer
-              is applied as the target for the corresponding example.
-
-            For outputs with > 2 dimensions, targets can be either:
-
-            - A single tuple, which contains #output_dims - 1
-              elements. This target index is applied to all examples.
-
-            - A list of tuples with length equal to the number of
-              examples in inputs (dim 0), and each tuple containing
-              #output_dims - 1 elements. Each tuple is applied as the
-              target for the corresponding example.
-
-            Default: None
-        topk: Proportion of input to be dropped. Must be between 0 and 1.
-            Default: 0.2
-
-    Returns:
-        (float or tuple of floats): The comprehensiveness metric.
-
-    References:
-        https://arxiv.org/abs/1911.03429
 
     Examples:
         >>> import torch as th
-        >>> from captum.attr import Saliency
-        >>> from tint.metrics import comprehensiveness
+        >>> from tint.attr import ExtremalMask
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
+        >>> data = th.rand(32, 7, 5)
         >>> mlp = MLP([5, 3, 1])
         <BLANKLINE>
-        >>> explainer = Saliency(mlp)
-        >>> attr = explainer.attribute(inputs, target=0)
-        <BLANKLINE>
-        >>> comp = comprehensiveness(mlp, inputs, attr, target=0)
+        >>> explainer = ExtremalMask(mlp)
+        >>> attr = explainer.attribute(inputs)
     """
-    return _base_metric(
-        metric=_comprehensiveness,
-        forward_func=forward_func,
-        inputs=inputs,
-        attributions=attributions,
-        baselines=baselines,
-        additional_forward_args=additional_forward_args,
-        target=target,
-        topk=topk,
-        largest=True,
-    )
+
+    def __init__(self, forward_func: Callable) -> None:
+        super().__init__(forward_func=forward_func)
+
+    @log_usage()
+    def attribute(
+        self,
+        inputs: TensorOrTupleOfTensorsGeneric,
+        baselines: BaselineType = None,
+        target: TargetType = None,
+        additional_forward_args: Any = None,
+        trainer: Trainer = None,
+        mask_net: ExtremalMaskNet = None,
+        batch_size: int = 32,
+        temporal_additional_forward_args: Tuple[bool] = None,
+        return_temporal_attributions: bool = False,
+    ) -> TensorOrTupleOfTensorsGeneric:
+        """
+        Attribute method.
+
+        Args:
+            inputs (tensor or tuple of tensors):  Input for which occlusion
+                attributions are computed. If forward_func takes a single
+                tensor as input, a single input tensor should be provided.
+                If forward_func takes multiple tensors as input, a tuple
+                of the input tensors should be provided. It is assumed
+                that for all given input tensors, dimension 0 corresponds
+                to the number of examples (aka batch size), and if
+                multiple input tensors are provided, the examples must
+                be aligned appropriately.
+            baselines (scalar, tensor, tuple of scalars or tensors, optional):
+                Baselines define reference value which replaces each
+                feature when occluded.
+                Baselines can be provided as:
+
+                - a single tensor, if inputs is a single tensor, with
+                  exactly the same dimensions as inputs or
+                  broadcastable to match the dimensions of inputs
+
+                - a single scalar, if inputs is a single tensor, which will
+                  be broadcasted for each input value in input tensor.
+
+                - a tuple of tensors or scalars, the baseline corresponding
+                  to each tensor in the inputs' tuple can be:
+
+                  - either a tensor with matching dimensions to
+                    corresponding tensor in the inputs' tuple
+                    or the first dimension is one and the remaining
+                    dimensions match with the corresponding
+                    input tensor.
+
+                  - or a scalar, corresponding to a tensor in the
+                    inputs' tuple. This scalar value is broadcasted
+                    for corresponding input tensor.
+
+                In the cases when `baselines` is not provided, we internally
+                use zero scalar corresponding to each input tensor.
+                Default: None
+            target (int, tuple, tensor or list, optional):  Output indices for
+                which difference is computed (for classification cases,
+                this is usually the target class).
+                If the network returns a scalar value per example,
+                no target index is necessary.
+                For general 2D outputs, targets can be either:
+
+                - a single integer or a tensor containing a single
+                  integer, which is applied to all input examples
+
+                - a list of integers or a 1D tensor, with length matching
+                  the number of examples in inputs (dim 0). Each integer
+                  is applied as the target for the corresponding example.
+
+                For outputs with > 2 dimensions, targets can be either:
+
+                - A single tuple, which contains #output_dims - 1
+                  elements. This target index is applied to all examples.
+
+                - A list of tuples with length equal to the number of
+                  examples in inputs (dim 0), and each tuple containing
+                  #output_dims - 1 elements. Each tuple is applied as the
+                  target for the corresponding example.
+
+                Default: None
+            additional_forward_args (any, optional): If the forward function
+                requires additional arguments other than the inputs for
+                which attributions should not be computed, this argument
+                can be provided. It must be either a single additional
+                argument of a Tensor or arbitrary (non-tuple) type or a
+                tuple containing multiple additional arguments including
+                tensors or any arbitrary python types. These arguments
+                are provided to forward_func in order following the
+                arguments in inputs.
+                For a tensor, the first dimension of the tensor must
+                correspond to the number of examples. For all other types,
+                the given argument is used for all forward evaluations.
+                Note that attributions are not computed with respect
+                to these arguments.
+                Default: None
+            trainer (Trainer): Pytorch Lightning trainer. If ``None``, a
+                default trainer will be provided.
+                Default: None
+            mask_net (BayesMaskNet): A Mask model. If ``None``, a default model
+                will be provided.
+                Default: None
+            batch_size (int): Batch size for Mask training.
+                Default: 32
+            temporal_additional_forward_args (tuple): Set each
+                additional forward arg which is temporal.
+                Only used with return_temporal_attributions.
+                Default: None
+            return_temporal_attributions (bool): Whether to return
+                attributions for all times or not.
+                Default: False
+
+        Returns:
+            - **attributions** (*tensor* or tuple of *tensors*):
+                The attributions with respect to each input feature.
+                Attributions will always be
+                the same size as the provided inputs, with each value
+                providing the attribution of the corresponding input index.
+                If a single tensor is provided as inputs, a single tensor is
+                returned. If a tuple is provided for inputs, a tuple of
+                corresponding sized tensors is returned.
+        """
+        # Keeps track whether original input is a tuple or not before
+        # converting it into a tuple.
+        is_inputs_tuple = _is_tuple(inputs)
+        inputs = _format_input(inputs)
+
+        # Format and validate baselines
+        baselines = _format_baseline(baselines, inputs)
+        _validate_input(inputs, baselines)
+
+        # Init trainer if not provided
+        if trainer is None:
+            trainer = Trainer(max_epochs=100)
+        else:
+            trainer = copy.deepcopy(trainer)
+
+        # Assert only one input, as the Retain only accepts one
+        assert (
+            len(inputs) == 1
+        ), "Multiple inputs are not accepted for this method"
+        data = inputs[0]
+        baseline = baselines[0]
+
+        # If return temporal attr, we expand the input data
+        # and multiply it with a lower triangular mask
+        if return_temporal_attributions:
+            data, additional_forward_args, _ = _add_temporal_mask(
+                inputs=data,
+                additional_forward_args=additional_forward_args,
+                temporal_additional_forward_args=temporal_additional_forward_args,
+            )
+
+        # Init MaskNet if not provided
+        if mask_net is None:
+            mask_net = ExtremalMaskNet(forward_func=self.forward_func)
+
+        # Init model
+        mask_net.net.init(input_size=data.shape, batch_size=batch_size)
+
+        # Prepare data
+        dataloader = DataLoader(
+            TensorDataset(
+                *(data, data, baseline, target, *additional_forward_args)
+                if additional_forward_args is not None
+                else (data, data, baseline, target, None)
+            ),
+            batch_size=batch_size,
+            collate_fn=default_collate,
+        )
+
+        # Fit model
+        trainer.fit(mask_net, train_dataloaders=dataloader)
+
+        # Set model to eval mode and cast it to device
+        mask_net.eval()
+        mask_net.to(data.device)
+
+        # Get attributions as mask representation
+        attributions = mask_net.net.representation(data, baseline)
+
+        # Reshape representation if temporal attributions
+        if return_temporal_attributions:
+            attributions = attributions.reshape(
+                (-1, data.shape[1]) + data.shape[1:]
+            )
+
+        # Reshape as a tuple
+        attributions = (attributions,)
+
+        # Format attributions and return
+        return _format_output(is_inputs_tuple, attributions)
```

### Comparing `time_interpret-0.1.0/tint/metrics/lipschitz_max.py` & `time_interpret-0.2.0/tint/metrics/lipschitz_max.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,51 +11,15 @@
     _format_tensor_into_tuples,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 from captum.log import log_usage
 from captum.metrics._utils.batching import _divide_and_aggregate_metrics
 from torch import Tensor
 
-
-def default_perturb_func(
-    inputs: TensorOrTupleOfTensorsGeneric, perturb_radius: float = 0.02
-) -> Tuple[Tensor, ...]:
-    r"""A default function for generating perturbations of `inputs`
-    within perturbation radius of `perturb_radius`.
-    This function samples uniformly random from the L_Infinity ball
-    with `perturb_radius` radius.
-    The users can override this function if they prefer to use a
-    different perturbation function.
-
-    Args:
-
-        inputs (tensor or a tuple of tensors): The input tensors that we'd
-                like to perturb by adding a random noise sampled unifromly
-                random from an L_infinity ball with a radius `perturb_radius`.
-
-        radius (float): A radius used for sampling from
-                an L_infinity ball.
-
-    Returns:
-
-        perturbed_input (tuple(tensor)): A list of perturbed inputs that
-                are createed by adding noise sampled uniformly random
-                from L_infiniy ball with a radius `perturb_radius` to the
-                original inputs.
-
-    """
-    inputs = _format_tensor_into_tuples(inputs)
-    perturbed_input = tuple(
-        input
-        + torch.FloatTensor(input.size())  # type: ignore
-        .uniform_(-perturb_radius, perturb_radius)
-        .to(input.device)
-        for input in inputs
-    )
-    return perturbed_input
+from tint.utils import default_perturb_func
 
 
 @log_usage()
 def lipschitz_max(
     explanation_func: Callable,
     inputs: TensorOrTupleOfTensorsGeneric,
     perturb_func: Callable = default_perturb_func,
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/aup.py` & `time_interpret-0.2.0/tint/metrics/white_box/aur.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 
 from sklearn.metrics import precision_recall_curve, auc
 from typing import Tuple
 
 from .base import _base_white_box_metric
 
 
-def _aup(
+def _aur(
     attributions: Tuple[np.ndarray],
     true_attributions: Tuple[np.ndarray],
     attributions_subset: Tuple[np.ndarray],
 ) -> Tuple[float]:
     pre_rec_tpl = tuple(
         precision_recall_curve(true_attr, attr)
         for true_attr, attr in zip(true_attributions, attributions)
     )
     return tuple(
-        auc(pre_rec[2], pre_rec[0][:-1]) if len(pre_rec[2]) > 1 else 0.0
+        auc(pre_rec[2], pre_rec[1][:-1]) if len(pre_rec[2]) > 1 else 0.0
         for pre_rec in pre_rec_tpl
     )
 
 
 @log_usage()
-def aup(
+def aur(
     attributions: TensorOrTupleOfTensorsGeneric,
     true_attributions: TensorOrTupleOfTensorsGeneric,
     normalize: bool = True,
 ) -> Tuple[float]:
     """
-    Area under precision.
+    Area under recall.
 
-    This is the standard area under the precision curve. Higher is better.
+    This is the standard area under the recall curve. Higher is better.
 
     Args:
         attributions (tensor or tuple of tensors):
             The attributions with respect to each input feature.
             Attributions will always be
             the same size as the provided inputs, with each value
             providing the attribution of the corresponding input index.
@@ -47,24 +47,25 @@
         true_attributions (tensor or tuple of tensors):
             True attributions to be used as a benchmark. Should be of
             the same format as the attributions.
         normalize (bool): Whether to normalize the attributions before
             computing the metric or not. Default: True
 
     Returns:
-        (float or tuple or floats): The aup metric.
+        (float or tuple or floats): The aur metric.
 
     Examples:
         >>> import torch as th
-        >>> from tint.metrics.white_box import aup
+        >>> from tint.metrics.white_box import aur
         <BLANKLINE>
         >>> attr = th.rand(8, 7, 5)
         >>> true_attr = th.randint(2, (8, 7, 5))
         <BLANKLINE>
-        >>> aup_ = aup(attr, true_attr)
+        >>> aur_ = aur(attr, true_attr)
     """
     return _base_white_box_metric(
-        metric=_aup,
+        metric=_aur,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/auprc.py` & `time_interpret-0.2.0/tint/metrics/white_box/auprc.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,9 @@
         >>> auprc_ = auprc(attr, true_attr)
     """
     return _base_white_box_metric(
         metric=_auprc,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/aur.py` & `time_interpret-0.2.0/tint/metrics/white_box/aup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 
 from sklearn.metrics import precision_recall_curve, auc
 from typing import Tuple
 
 from .base import _base_white_box_metric
 
 
-def _aur(
+def _aup(
     attributions: Tuple[np.ndarray],
     true_attributions: Tuple[np.ndarray],
     attributions_subset: Tuple[np.ndarray],
 ) -> Tuple[float]:
     pre_rec_tpl = tuple(
         precision_recall_curve(true_attr, attr)
         for true_attr, attr in zip(true_attributions, attributions)
     )
     return tuple(
-        auc(pre_rec[2], pre_rec[1][:-1]) if len(pre_rec[2]) > 1 else 0.0
+        auc(pre_rec[2], pre_rec[0][:-1]) if len(pre_rec[2]) > 1 else 0.0
         for pre_rec in pre_rec_tpl
     )
 
 
 @log_usage()
-def aur(
+def aup(
     attributions: TensorOrTupleOfTensorsGeneric,
     true_attributions: TensorOrTupleOfTensorsGeneric,
     normalize: bool = True,
 ) -> Tuple[float]:
     """
-    Area under recall.
+    Area under precision.
 
-    This is the standard area under the recall curve. Higher is better.
+    This is the standard area under the precision curve. Higher is better.
 
     Args:
         attributions (tensor or tuple of tensors):
             The attributions with respect to each input feature.
             Attributions will always be
             the same size as the provided inputs, with each value
             providing the attribution of the corresponding input index.
@@ -47,24 +47,25 @@
         true_attributions (tensor or tuple of tensors):
             True attributions to be used as a benchmark. Should be of
             the same format as the attributions.
         normalize (bool): Whether to normalize the attributions before
             computing the metric or not. Default: True
 
     Returns:
-        (float or tuple or floats): The aur metric.
+        (float or tuple or floats): The aup metric.
 
     Examples:
         >>> import torch as th
-        >>> from tint.metrics.white_box import aur
+        >>> from tint.metrics.white_box import aup
         <BLANKLINE>
         >>> attr = th.rand(8, 7, 5)
         >>> true_attr = th.randint(2, (8, 7, 5))
         <BLANKLINE>
-        >>> aur_ = aur(attr, true_attr)
+        >>> aup_ = aup(attr, true_attr)
     """
     return _base_white_box_metric(
-        metric=_aur,
+        metric=_aup,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/base.py` & `time_interpret-0.2.0/tint/metrics/white_box/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import torch
-
 from captum.log import log_usage
 from captum._utils.common import (
     _is_tuple,
     _format_input,
     _format_output,
     _validate_input,
 )
@@ -16,14 +14,15 @@
 
 @log_usage()
 def _base_white_box_metric(
     metric: Callable,
     attributions: TensorOrTupleOfTensorsGeneric,
     true_attributions: TensorOrTupleOfTensorsGeneric,
     normalize: bool = True,
+    hard_labels: bool = True,
 ) -> Tuple[float]:
     # Convert attributions into tuple
     is_inputs_tuple = _is_tuple(attributions)
     attributions = _format_input(attributions)
     true_attributions = _format_input(true_attributions)
 
     # Validate input
@@ -48,19 +47,23 @@
             for max_, attr in zip(max_tpl, attributions)
         )
         attributions = tuple(
             (attr - min_) / (max_ - min_ + EPS)
             for attr, min_, max_ in zip(attributions, min_tpl, max_tpl)
         )
 
-    # Reshape attributions and get a subset corresponding to the true ones
+    # Reshape attributions
     attributions = tuple(attr.reshape(-1) for attr in attributions)
-    true_attributions = tuple(
-        attr.reshape(-1).int() for attr in true_attributions
-    )
+    true_attributions = tuple(attr.reshape(-1) for attr in true_attributions)
+
+    # Get int value if necessary
+    if hard_labels:
+        true_attributions = tuple(attr.int() for attr in true_attributions)
+
+    # Get a subset corresponding to the true attributions
     attributions_subset = tuple(
         attr[true_attr != 0]
         for attr, true_attr in zip(attributions, true_attributions)
     )
 
     # Convert to numpy
     attributions = tuple(attr.detach().cpu().numpy() for attr in attributions)
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/entropy.py` & `time_interpret-0.2.0/tint/metrics/white_box/entropy.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,8 +71,9 @@
         >>> entropy_ = entropy(attr, true_attr)
     """
     return _base_white_box_metric(
         metric=_entropy,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/information.py` & `time_interpret-0.2.0/tint/metrics/white_box/information.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,8 +65,9 @@
         >>> information_ = information(attr, true_attr)
     """
     return _base_white_box_metric(
         metric=_information,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/metrics/white_box/roc_auc.py` & `time_interpret-0.2.0/tint/metrics/white_box/roc_auc.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,8 +59,9 @@
         >>> roc_auc_ = roc_auc(attr, true_attr)
     """
     return _base_white_box_metric(
         metric=_roc_auc,
         attributions=attributions,
         true_attributions=true_attributions,
         normalize=normalize,
+        hard_labels=True,
     )
```

### Comparing `time_interpret-0.1.0/tint/models/bert.py` & `time_interpret-0.2.0/tint/models/bert.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,45 @@
     from transformers.models.bert import (
         BertConfig,
         BertTokenizer,
         BertForSequenceClassification,
     )
 except ImportError:
     BertConfig = None
+    BertTokenizer = None
     BertForSequenceClassification = None
 
 
 def Bert(
     pretrained_model_name_or_path: str = None,
     config=None,
     vocab_file=None,
+    cache_dir=None,
     **kwargs
 ):
     r"""
     Get Bert model for sentence classification, either as a pre-trained model
-    or from scratch. Any transformers model could theoretically be used, this
-    method is provided as an example.
+    or from scratch.
 
     Args:
         pretrained_model_name_or_path: Path of the pre-trained model.
             If ``None``, return an untrained Bert model. Default to ``None``
         config: Config of the Bert. Required when not loading a pre-trained
             model, otherwise unused. Default to ``None``
         vocab_file: Path to a vocab file for the tokenizer.
             Default to ``None``
+        cache_dir: Where to save pretrained model. Default to ``None``
         kwargs: Additional arguments for the tokenizer if not pretrained.
 
     Returns:
-        BertForSequenceClassification: Bert model for sentence classification.
+        2-element tuple of **Bert Tokenizer**, **Bert Model**:
+        - **Bert Tokenizer** (*BertTokenizer*):
+            Bert Tokenizer.
+        - **Bert Model** (*BertForSequenceClassification*):
+            Bert model for sentence classification.
 
     References:
         https://huggingface.co/docs/transformers/main/en/model_doc/bert
 
     Examples:
         >>> from tint.models import Bert
          <BLANKLINE>
@@ -49,13 +55,17 @@
         return (
             BertTokenizer(vocab_file, **kwargs),
             BertForSequenceClassification(config=config),
         )
 
     # Otherwise return untrained bert model
     return (
-        BertTokenizer.from_pretrained(pretrained_model_name_or_path),
+        BertTokenizer.from_pretrained(
+            pretrained_model_name_or_path,
+            cache_dir=cache_dir,
+        ),
         BertForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path,
+            cache_dir=cache_dir,
             return_dict=False,
         ),
     )
```

### Comparing `time_interpret-0.1.0/tint/models/cnn.py` & `time_interpret-0.2.0/tint/models/cnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import torch as th
 import torch.nn as nn
 
 from typing import Union
 
 
 NORMS = {
@@ -65,15 +66,17 @@
             Default to ``None``
         dropout (list, float): Dropout rates. Default to 0.0
         norm (list, str): Normalisation layers. Either a list or a string.
             Default to ``None``
         activations (list, str): Activation functions. Either a list or a
             string. Default to ``'relu'``
         pooling (list, str): Pooling module. Either a list or a string.
-            Default t0 ``None``
+            Default to ``None``
+        flatten (bool): Whether to flatten the output of the model or not.
+            Default to ``True``
 
     References:
         https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html#torch.nn.Conv2d
 
     Examples:
         >>> import torch.nn as nn
         >>> from tint.models import CNN
@@ -93,14 +96,15 @@
         groups: Union[list, int] = 1,
         bias: Union[list, bool] = True,
         padding_mode: Union[list, str] = "zeros",
         dropout: Union[list, float] = 0.0,
         norm: Union[list, str] = None,
         activations: Union[list, str] = "relu",
         pooling: Union[list, str] = None,
+        flatten: bool = True,
     ):
         super().__init__()
 
         assert len(units) > 1, "At least two units must be provided."
         length = len(units) - 1
 
         if isinstance(dropout, list):
@@ -120,15 +124,15 @@
             )
         if isinstance(pooling, list):
             assert len(pooling) == length - 1, (
                 f"Inconsistent number of pooling: found "
                 f"{len(pooling)} but should be {length - 1}."
             )
 
-        layers = [nn.Conv2d] * length
+        layers = [nn.Conv2d for _ in range(length)]
         if isinstance(kernel_size, int):
             kernel_size = [kernel_size] * length
         if isinstance(stride, int):
             stride = [stride] * length
         if isinstance(padding, int):
             padding = [padding] * length
         if isinstance(dilation, int):
@@ -138,19 +142,24 @@
         if isinstance(bias, bool):
             bias = [bias] * length
         if isinstance(padding_mode, str):
             padding_mode = [padding_mode] * length
         if isinstance(dropout, float):
             dropout = [dropout] * (length - 1)
         if isinstance(norm, str):
-            norm = [NORMS[norm]] * (length - 1)
+            norm = [copy.deepcopy(NORMS[norm]) for _ in range(length - 1)]
         if isinstance(activations, str):
-            activations = [ACTIVATIONS[activations]] * (length - 1)
+            activations = [
+                copy.deepcopy(ACTIVATIONS[activations])
+                for _ in range(length - 1)
+            ]
         if isinstance(pooling, str):
-            pooling = [POOLS[pooling]] * (length - 1)
+            pooling = [
+                copy.deepcopy(POOLS[pooling]) for _ in range(length - 1)
+            ]
 
         model = dict()
         for i in range(length):
             final_layer = i == length - 1
             name = layers[i].__name__
             model[f"{name}_{i}"] = layers[i](
                 units[i],
@@ -183,15 +192,15 @@
                 not final_layer
                 and pooling is not None
                 and pooling[i] is not None
             ):
                 name = pooling[i].__class__.__name__
                 model[f"{name}_{i}"] = pooling[i]
 
-            if final_layer:
+            if final_layer and flatten:
                 name = nn.Flatten.__name__
                 model[f"{name}_{i}"] = nn.Flatten(1)
 
         self.cnn = nn.Sequential()
         for k, v in model.items():
             self.cnn.add_module(k, v)
```

### Comparing `time_interpret-0.1.0/tint/models/mlp.py` & `time_interpret-0.2.0/tint/models/mlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import torch as th
 import torch.nn as nn
 
 from typing import Union
 
 
 NORMS = {
@@ -102,25 +103,28 @@
             )
         if isinstance(activations, list):
             assert len(activations) == length - 1, (
                 f"Inconsistent number of activations: found "
                 f"{len(activations)} but should be {length - 1}."
             )
 
-        layers = [nn.Linear] * length
+        layers = [nn.Linear for _ in range(length)]
         if isinstance(bias, bool):
             bias = [bias] * length
         if isinstance(dropout, float):
             dropout = [dropout] * (length - 1)
         if isinstance(norm, str):
-            norm = [NORMS[norm]] * (length - 1)
+            norm = [NORMS[norm] for _ in range(length - 1)]
         if isinstance(activations, str):
-            activations = [ACTIVATIONS[activations]] * (length - 1)
+            activations = [
+                copy.deepcopy(ACTIVATIONS[activations])
+                for _ in range(length - 1)
+            ]
         if isinstance(activation_final, str):
-            activation_final = ACTIVATIONS[activation_final]
+            activation_final = copy.deepcopy(ACTIVATIONS[activation_final])
 
         model = dict()
         for i in range(length):
             final_layer = i == length - 1
             name = layers[i].__name__
             model[f"{name}_{i}"] = layers[i](units[i], units[i + 1], bias=bias)
```

### Comparing `time_interpret-0.1.0/tint/models/net.py` & `time_interpret-0.2.0/tint/models/net.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/models/rnn.py` & `time_interpret-0.2.0/tint/models/rnn.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/models/transformer.py` & `time_interpret-0.2.0/tint/models/transformer.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/utils/collate.py` & `time_interpret-0.2.0/tint/utils/collate.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/utils/tensor_dataset.py` & `time_interpret-0.2.0/tint/utils/tensor_dataset.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/tint/utils/tqdm.py` & `time_interpret-0.2.0/tint/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.1.0/PKG-INFO` & `time_interpret-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: time_interpret
-Version: 0.1.0
-Summary: Time interpret library for PyTorch.
+Version: 0.2.0
+Summary: Model interpretability library for PyTorch with a focus on time series.
 Keywords: deep-learning,pytorch,captum,explainable-ai,time-series
 Author-email: Joseph Enguehard <joseph@skippr.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -150,7 +150,8 @@
 - [SmoothGrad](https://arxiv.org/abs/1810.03292)
 
 
 ## Acknowledgment
 - [Jonathan Crabbe](https://github.com/JonathanCrabbe/Dynamask) for the DynaMask implementation.
 - [Sana Tonekaboni](https://github.com/sanatonek/time_series_explainability/tree/master/TSX) for the fit implementation.
 - [INK Lab](https://github.com/INK-USC/DIG) for the discretized integrated gradients implementation.
+- [Dylan Slack](https://github.com/dylan-slack/Modeling-Uncertainty-Local-Explainability) for the BayesLime and BayesShap implementations.
```

