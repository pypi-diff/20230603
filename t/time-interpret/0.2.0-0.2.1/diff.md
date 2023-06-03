# Comparing `tmp/time_interpret-0.2.0.tar.gz` & `tmp/time_interpret-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_interpret-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "time_interpret-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time_interpret-0.2.0.tar` & `time_interpret-0.2.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     2354 2023-06-03 09:31:38.184118 time_interpret-0.2.0/README.md
--rw-r--r--   0        0        0     2035 2023-06-03 09:36:55.387260 time_interpret-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.2.0/tint/__init__.py
--rw-r--r--   0        0        0       22 2023-06-03 09:31:38.222143 time_interpret-0.2.0/tint/__version__.py
--rw-r--r--   0        0        0     1231 2023-06-03 09:31:38.222248 time_interpret-0.2.0/tint/attr/__init__.py
--rw-r--r--   0        0        0    13796 2023-06-03 09:31:38.222402 time_interpret-0.2.0/tint/attr/augmented_occlusion.py
--rw-r--r--   0        0        0     4295 2023-06-03 09:31:38.222516 time_interpret-0.2.0/tint/attr/bayes.py
--rw-r--r--   0        0        0    10394 2023-06-03 09:23:02.464050 time_interpret-0.2.0/tint/attr/discretised_ig.py
--rw-r--r--   0        0        0     6497 2023-06-03 09:23:02.464196 time_interpret-0.2.0/tint/attr/dynamic_masks.py
--rw-r--r--   0        0        0     9786 2023-06-03 09:31:38.222641 time_interpret-0.2.0/tint/attr/extremal_mask.py
--rw-r--r--   0        0        0    28774 2023-06-03 09:31:38.222802 time_interpret-0.2.0/tint/attr/feature_ablation.py
--rw-r--r--   0        0        0    13321 2023-06-03 09:23:02.464622 time_interpret-0.2.0/tint/attr/fit.py
--rw-r--r--   0        0        0    31058 2023-06-03 09:31:38.223089 time_interpret-0.2.0/tint/attr/geodesic_ig.py
--rw-r--r--   0        0        0     8439 2023-06-03 09:31:38.223233 time_interpret-0.2.0/tint/attr/lof.py
--rw-r--r--   0        0        0      551 2023-06-03 09:31:38.223361 time_interpret-0.2.0/tint/attr/models/__init__.py
--rw-r--r--   0        0        0     8059 2023-06-03 09:31:38.223488 time_interpret-0.2.0/tint/attr/models/bayes_linear.py
--rw-r--r--   0        0        0     8365 2023-06-03 09:31:38.223599 time_interpret-0.2.0/tint/attr/models/extremal_mask.py
--rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.2.0/tint/attr/models/joint_features_generator.py
--rw-r--r--   0        0        0    15936 2023-06-03 09:31:38.223738 time_interpret-0.2.0/tint/attr/models/mask.py
--rw-r--r--   0        0        0     7693 2023-06-03 09:23:02.465613 time_interpret-0.2.0/tint/attr/models/path_generator.py
--rw-r--r--   0        0        0     7957 2023-06-03 09:23:02.465828 time_interpret-0.2.0/tint/attr/models/retain.py
--rw-r--r--   0        0        0    19107 2023-06-03 09:31:38.223849 time_interpret-0.2.0/tint/attr/occlusion.py
--rw-r--r--   0        0        0        0 2023-06-03 09:31:38.223881 time_interpret-0.2.0/tint/attr/perturbed_ig.py
--rw-r--r--   0        0        0     7881 2023-06-03 09:23:02.466199 time_interpret-0.2.0/tint/attr/retain.py
--rw-r--r--   0        0        0    19391 2023-06-03 09:31:38.224017 time_interpret-0.2.0/tint/attr/seq_ig.py
--rw-r--r--   0        0        0      718 2023-06-03 09:23:02.466282 time_interpret-0.2.0/tint/attr/smooth_grad.py
--rw-r--r--   0        0        0    14038 2023-06-03 09:23:02.466447 time_interpret-0.2.0/tint/attr/temporal_augmented_occlusion.py
--rw-r--r--   0        0        0    23450 2023-06-03 09:31:38.224170 time_interpret-0.2.0/tint/attr/temporal_ig.py
--rw-r--r--   0        0        0    14146 2023-06-03 09:23:02.466742 time_interpret-0.2.0/tint/attr/temporal_occlusion.py
--rw-r--r--   0        0        0    12809 2023-06-03 09:23:02.466921 time_interpret-0.2.0/tint/attr/time_forward_tunnel.py
--rw-r--r--   0        0        0       41 2023-06-03 09:31:38.224431 time_interpret-0.2.0/tint/data/.gitignore
--rw-r--r--   0        0        0      208 2023-06-03 09:31:38.226008 time_interpret-0.2.0/tint/datasets/__init__.py
--rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.2.0/tint/datasets/arma.py
--rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.2.0/tint/datasets/biobank.py
--rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.2.0/tint/datasets/dataset.py
--rw-r--r--   0        0        0    11239 2023-06-03 09:31:38.226150 time_interpret-0.2.0/tint/datasets/hawkes.py
--rw-r--r--   0        0        0     8679 2023-06-03 09:23:02.476396 time_interpret-0.2.0/tint/datasets/hmm.py
--rw-r--r--   0        0        0    33349 2023-06-03 09:31:38.226352 time_interpret-0.2.0/tint/datasets/mimic3.py
--rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.2.0/tint/datasets/utils/__init__.py
--rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.2.0/tint/datasets/utils/fasttext.py
--rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.2.0/tint/datasets/utils/labels.json
--rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.2.0/tint/datasets/utils/labels.py
--rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.2.0/tint/datasets/utils/read_3_2.json
--rw-r--r--   0        0        0      427 2023-06-03 09:31:38.226498 time_interpret-0.2.0/tint/metrics/__init__.py
--rw-r--r--   0        0        0     9162 2023-06-03 09:31:38.226662 time_interpret-0.2.0/tint/metrics/accuracy.py
--rw-r--r--   0        0        0     6147 2023-06-03 09:31:38.226811 time_interpret-0.2.0/tint/metrics/base.py
--rw-r--r--   0        0        0     8751 2023-06-03 09:31:38.227069 time_interpret-0.2.0/tint/metrics/comprehensiveness.py
--rw-r--r--   0        0        0     8915 2023-06-03 09:31:38.227188 time_interpret-0.2.0/tint/metrics/cross_entropy.py
--rw-r--r--   0        0        0    10150 2023-06-03 09:31:38.227340 time_interpret-0.2.0/tint/metrics/lipschitz_max.py
--rw-r--r--   0        0        0     8755 2023-06-03 09:31:38.227464 time_interpret-0.2.0/tint/metrics/log_odds.py
--rw-r--r--   0        0        0     9064 2023-06-03 09:31:38.227565 time_interpret-0.2.0/tint/metrics/mae.py
--rw-r--r--   0        0        0     9048 2023-06-03 09:31:38.227658 time_interpret-0.2.0/tint/metrics/mse.py
--rw-r--r--   0        0        0     8707 2023-06-03 09:31:38.227836 time_interpret-0.2.0/tint/metrics/sufficiency.py
--rw-r--r--   0        0        0      130 2023-06-03 09:31:38.227939 time_interpret-0.2.0/tint/metrics/weights/__init__.py
--rw-r--r--   0        0        0     1674 2023-06-03 09:31:38.228031 time_interpret-0.2.0/tint/metrics/weights/lime_weights.py
--rw-r--r--   0        0        0     1644 2023-06-03 09:31:38.228120 time_interpret-0.2.0/tint/metrics/weights/lof_weights.py
--rw-r--r--   0        0        0      360 2023-06-03 09:31:38.228278 time_interpret-0.2.0/tint/metrics/white_box/__init__.py
--rw-r--r--   0        0        0     2267 2023-06-03 09:31:38.228410 time_interpret-0.2.0/tint/metrics/white_box/aup.py
--rw-r--r--   0        0        0     2157 2023-06-03 09:31:38.228536 time_interpret-0.2.0/tint/metrics/white_box/auprc.py
--rw-r--r--   0        0        0     2261 2023-06-03 09:31:38.228664 time_interpret-0.2.0/tint/metrics/white_box/aur.py
--rw-r--r--   0        0        0     2548 2023-06-03 09:31:38.228771 time_interpret-0.2.0/tint/metrics/white_box/base.py
--rw-r--r--   0        0        0     2448 2023-06-03 09:31:38.228881 time_interpret-0.2.0/tint/metrics/white_box/entropy.py
--rw-r--r--   0        0        0     2285 2023-06-03 09:31:38.228999 time_interpret-0.2.0/tint/metrics/white_box/information.py
--rw-r--r--   0        0        0     2152 2023-06-03 09:31:38.229074 time_interpret-0.2.0/tint/metrics/white_box/mae.py
--rw-r--r--   0        0        0     2148 2023-06-03 09:31:38.229141 time_interpret-0.2.0/tint/metrics/white_box/mse.py
--rw-r--r--   0        0        0     2178 2023-06-03 09:31:38.229223 time_interpret-0.2.0/tint/metrics/white_box/rmse.py
--rw-r--r--   0        0        0     2109 2023-06-03 09:31:38.229337 time_interpret-0.2.0/tint/metrics/white_box/roc_auc.py
--rw-r--r--   0        0        0      346 2023-06-03 09:31:38.229462 time_interpret-0.2.0/tint/models/__init__.py
--rw-r--r--   0        0        0     2304 2023-06-03 09:31:38.229595 time_interpret-0.2.0/tint/models/bert.py
--rw-r--r--   0        0        0     6863 2023-06-03 09:31:38.229855 time_interpret-0.2.0/tint/models/cnn.py
--rw-r--r--   0        0        0     2496 2023-06-03 09:31:38.229929 time_interpret-0.2.0/tint/models/distilbert.py
--rw-r--r--   0        0        0     5058 2023-06-03 09:31:38.230072 time_interpret-0.2.0/tint/models/mlp.py
--rw-r--r--   0        0        0     5581 2023-06-03 09:23:02.479400 time_interpret-0.2.0/tint/models/net.py
--rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.2.0/tint/models/rnn.py
--rw-r--r--   0        0        0     2398 2023-06-03 09:31:38.230138 time_interpret-0.2.0/tint/models/roberta.py
--rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.2.0/tint/models/transformer.py
--rw-r--r--   0        0        0      714 2023-06-03 09:31:38.230248 time_interpret-0.2.0/tint/utils/__init__.py
--rw-r--r--   0        0        0     3429 2023-06-03 09:31:38.230323 time_interpret-0.2.0/tint/utils/a_star_path.py
--rw-r--r--   0        0        0     1809 2023-06-03 09:31:38.230396 time_interpret-0.2.0/tint/utils/baching.py
--rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.2.0/tint/utils/collate.py
--rw-r--r--   0        0        0     9571 2023-06-03 09:31:38.230535 time_interpret-0.2.0/tint/utils/common.py
--rw-r--r--   0        0        0     1540 2023-06-03 09:31:38.230622 time_interpret-0.2.0/tint/utils/perturb_func.py
--rw-r--r--   0        0        0     1000 2023-06-03 09:23:02.479982 time_interpret-0.2.0/tint/utils/tensor_dataset.py
--rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.2.0/tint/utils/tqdm.py
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 time_interpret-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2489 2023-06-03 09:42:15.524925 time_interpret-0.2.1/README.md
+-rw-r--r--   0        0        0     2035 2023-06-03 09:42:42.223361 time_interpret-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-01-17 17:12:35.379363 time_interpret-0.2.1/tint/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-03 09:42:15.598940 time_interpret-0.2.1/tint/__version__.py
+-rw-r--r--   0        0        0     1280 2023-06-03 09:42:15.599056 time_interpret-0.2.1/tint/attr/__init__.py
+-rw-r--r--   0        0        0    14067 2023-06-03 09:42:15.599521 time_interpret-0.2.1/tint/attr/augmented_occlusion.py
+-rw-r--r--   0        0        0     4621 2023-06-03 09:42:15.599623 time_interpret-0.2.1/tint/attr/bayes.py
+-rw-r--r--   0        0        0    10599 2023-06-03 09:42:15.599894 time_interpret-0.2.1/tint/attr/discretised_ig.py
+-rw-r--r--   0        0        0     7152 2023-06-03 09:42:15.600370 time_interpret-0.2.1/tint/attr/dynamic_masks.py
+-rw-r--r--   0        0        0    10206 2023-06-03 09:42:15.600619 time_interpret-0.2.1/tint/attr/extremal_mask.py
+-rw-r--r--   0        0        0    28799 2023-06-03 09:42:15.600970 time_interpret-0.2.1/tint/attr/feature_ablation.py
+-rw-r--r--   0        0        0    13323 2023-06-03 09:42:15.601202 time_interpret-0.2.1/tint/attr/fit.py
+-rw-r--r--   0        0        0    36748 2023-06-03 09:42:15.601584 time_interpret-0.2.1/tint/attr/geodesic_ig.py
+-rw-r--r--   0        0        0     9144 2023-06-03 09:42:15.601704 time_interpret-0.2.1/tint/attr/lof.py
+-rw-r--r--   0        0        0      555 2023-06-03 09:42:15.601821 time_interpret-0.2.1/tint/attr/models/__init__.py
+-rw-r--r--   0        0        0     8059 2023-06-03 09:31:38.223488 time_interpret-0.2.1/tint/attr/models/bayes_linear.py
+-rw-r--r--   0        0        0     8196 2023-06-03 09:42:15.601977 time_interpret-0.2.1/tint/attr/models/extremal_mask.py
+-rw-r--r--   0        0        0     8236 2023-06-03 09:22:02.014070 time_interpret-0.2.1/tint/attr/models/joint_features_generator.py
+-rw-r--r--   0        0        0    15936 2023-06-03 09:31:38.223738 time_interpret-0.2.1/tint/attr/models/mask.py
+-rw-r--r--   0        0        0     8176 2023-06-03 09:42:15.602108 time_interpret-0.2.1/tint/attr/models/path_generator.py
+-rw-r--r--   0        0        0     7585 2023-06-03 09:42:15.602218 time_interpret-0.2.1/tint/attr/models/retain.py
+-rw-r--r--   0        0        0    12726 2023-06-03 09:42:15.602374 time_interpret-0.2.1/tint/attr/non_linearities_tunnel.py
+-rw-r--r--   0        0        0    19109 2023-06-03 09:42:15.602669 time_interpret-0.2.1/tint/attr/occlusion.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:31:38.223881 time_interpret-0.2.1/tint/attr/perturbed_ig.py
+-rw-r--r--   0        0        0     7882 2023-06-03 09:42:15.602969 time_interpret-0.2.1/tint/attr/retain.py
+-rw-r--r--   0        0        0    20151 2023-06-03 09:42:15.603111 time_interpret-0.2.1/tint/attr/seq_ig.py
+-rw-r--r--   0        0        0    14142 2023-06-03 09:42:15.603392 time_interpret-0.2.1/tint/attr/temporal_augmented_occlusion.py
+-rw-r--r--   0        0        0    23920 2023-06-03 09:42:15.603704 time_interpret-0.2.1/tint/attr/temporal_ig.py
+-rw-r--r--   0        0        0    14246 2023-06-03 09:42:15.604180 time_interpret-0.2.1/tint/attr/temporal_occlusion.py
+-rw-r--r--   0        0        0    12703 2023-06-03 09:42:15.604427 time_interpret-0.2.1/tint/attr/time_forward_tunnel.py
+-rw-r--r--   0        0        0       41 2023-06-03 09:31:38.224431 time_interpret-0.2.1/tint/data/.gitignore
+-rw-r--r--   0        0        0      208 2023-06-03 09:31:38.226008 time_interpret-0.2.1/tint/datasets/__init__.py
+-rw-r--r--   0        0        0     5820 2023-06-03 09:22:02.018048 time_interpret-0.2.1/tint/datasets/arma.py
+-rw-r--r--   0        0        0    17094 2023-06-03 09:23:02.476126 time_interpret-0.2.1/tint/datasets/biobank.py
+-rw-r--r--   0        0        0     5028 2023-06-03 09:22:02.018426 time_interpret-0.2.1/tint/datasets/dataset.py
+-rw-r--r--   0        0        0    11239 2023-06-03 09:31:38.226150 time_interpret-0.2.1/tint/datasets/hawkes.py
+-rw-r--r--   0        0        0     8826 2023-06-03 09:42:15.604647 time_interpret-0.2.1/tint/datasets/hmm.py
+-rw-r--r--   0        0        0    33349 2023-06-03 09:31:38.226352 time_interpret-0.2.1/tint/datasets/mimic3.py
+-rw-r--r--   0        0        0      117 2023-06-03 09:22:02.018779 time_interpret-0.2.1/tint/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-03 09:22:02.018844 time_interpret-0.2.1/tint/datasets/utils/fasttext.py
+-rw-r--r--   0        0        0   121020 2023-06-03 09:22:02.019225 time_interpret-0.2.1/tint/datasets/utils/labels.json
+-rw-r--r--   0        0        0     2468 2023-06-03 09:22:02.019304 time_interpret-0.2.1/tint/datasets/utils/labels.py
+-rw-r--r--   0        0        0  6235972 2023-06-03 09:22:02.037402 time_interpret-0.2.1/tint/datasets/utils/read_3_2.json
+-rw-r--r--   0        0        0      427 2023-06-03 09:31:38.226498 time_interpret-0.2.1/tint/metrics/__init__.py
+-rw-r--r--   0        0        0     9162 2023-06-03 09:42:15.604789 time_interpret-0.2.1/tint/metrics/accuracy.py
+-rw-r--r--   0        0        0     6147 2023-06-03 09:31:38.226811 time_interpret-0.2.1/tint/metrics/base.py
+-rw-r--r--   0        0        0     8751 2023-06-03 09:42:15.604936 time_interpret-0.2.1/tint/metrics/comprehensiveness.py
+-rw-r--r--   0        0        0     8915 2023-06-03 09:42:15.605041 time_interpret-0.2.1/tint/metrics/cross_entropy.py
+-rw-r--r--   0        0        0    10150 2023-06-03 09:31:38.227340 time_interpret-0.2.1/tint/metrics/lipschitz_max.py
+-rw-r--r--   0        0        0     8755 2023-06-03 09:42:15.605133 time_interpret-0.2.1/tint/metrics/log_odds.py
+-rw-r--r--   0        0        0     9064 2023-06-03 09:42:15.605323 time_interpret-0.2.1/tint/metrics/mae.py
+-rw-r--r--   0        0        0     9048 2023-06-03 09:42:15.605403 time_interpret-0.2.1/tint/metrics/mse.py
+-rw-r--r--   0        0        0     8707 2023-06-03 09:42:15.605493 time_interpret-0.2.1/tint/metrics/sufficiency.py
+-rw-r--r--   0        0        0      130 2023-06-03 09:31:38.227939 time_interpret-0.2.1/tint/metrics/weights/__init__.py
+-rw-r--r--   0        0        0     2322 2023-06-03 09:42:15.605616 time_interpret-0.2.1/tint/metrics/weights/lime_weights.py
+-rw-r--r--   0        0        0     2299 2023-06-03 09:42:15.605726 time_interpret-0.2.1/tint/metrics/weights/lof_weights.py
+-rw-r--r--   0        0        0      360 2023-06-03 09:31:38.228278 time_interpret-0.2.1/tint/metrics/white_box/__init__.py
+-rw-r--r--   0        0        0     2267 2023-06-03 09:31:38.228410 time_interpret-0.2.1/tint/metrics/white_box/aup.py
+-rw-r--r--   0        0        0     2157 2023-06-03 09:31:38.228536 time_interpret-0.2.1/tint/metrics/white_box/auprc.py
+-rw-r--r--   0        0        0     2261 2023-06-03 09:31:38.228664 time_interpret-0.2.1/tint/metrics/white_box/aur.py
+-rw-r--r--   0        0        0     2551 2023-06-03 09:42:15.605904 time_interpret-0.2.1/tint/metrics/white_box/base.py
+-rw-r--r--   0        0        0     2448 2023-06-03 09:31:38.228881 time_interpret-0.2.1/tint/metrics/white_box/entropy.py
+-rw-r--r--   0        0        0     2285 2023-06-03 09:31:38.228999 time_interpret-0.2.1/tint/metrics/white_box/information.py
+-rw-r--r--   0        0        0     2152 2023-06-03 09:31:38.229074 time_interpret-0.2.1/tint/metrics/white_box/mae.py
+-rw-r--r--   0        0        0     2148 2023-06-03 09:31:38.229141 time_interpret-0.2.1/tint/metrics/white_box/mse.py
+-rw-r--r--   0        0        0     2178 2023-06-03 09:31:38.229223 time_interpret-0.2.1/tint/metrics/white_box/rmse.py
+-rw-r--r--   0        0        0     2109 2023-06-03 09:31:38.229337 time_interpret-0.2.1/tint/metrics/white_box/roc_auc.py
+-rw-r--r--   0        0        0      346 2023-06-03 09:31:38.229462 time_interpret-0.2.1/tint/models/__init__.py
+-rw-r--r--   0        0        0     2308 2023-06-03 09:42:15.606032 time_interpret-0.2.1/tint/models/bert.py
+-rw-r--r--   0        0        0     6869 2023-06-03 09:42:15.606153 time_interpret-0.2.1/tint/models/cnn.py
+-rw-r--r--   0        0        0     2492 2023-06-03 09:42:15.606255 time_interpret-0.2.1/tint/models/distilbert.py
+-rw-r--r--   0        0        0     5064 2023-06-03 09:42:15.606372 time_interpret-0.2.1/tint/models/mlp.py
+-rw-r--r--   0        0        0     5595 2023-06-03 09:42:15.606518 time_interpret-0.2.1/tint/models/net.py
+-rw-r--r--   0        0        0     2361 2023-06-03 09:22:02.042433 time_interpret-0.2.1/tint/models/rnn.py
+-rw-r--r--   0        0        0     2399 2023-06-03 09:42:15.606633 time_interpret-0.2.1/tint/models/roberta.py
+-rw-r--r--   0        0        0     3345 2023-06-03 09:22:02.042728 time_interpret-0.2.1/tint/models/transformer.py
+-rw-r--r--   0        0        0      714 2023-06-03 09:31:38.230248 time_interpret-0.2.1/tint/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2023-06-03 09:31:38.230323 time_interpret-0.2.1/tint/utils/a_star_path.py
+-rw-r--r--   0        0        0     2391 2023-06-03 09:42:15.606765 time_interpret-0.2.1/tint/utils/baching.py
+-rw-r--r--   0        0        0     3563 2023-06-03 09:22:02.043064 time_interpret-0.2.1/tint/utils/collate.py
+-rw-r--r--   0        0        0     9574 2023-06-03 09:42:15.607048 time_interpret-0.2.1/tint/utils/common.py
+-rw-r--r--   0        0        0     1540 2023-06-03 09:31:38.230622 time_interpret-0.2.1/tint/utils/perturb_func.py
+-rw-r--r--   0        0        0      983 2023-06-03 09:42:15.607311 time_interpret-0.2.1/tint/utils/tensor_dataset.py
+-rw-r--r--   0        0        0      854 2023-06-03 09:22:02.043835 time_interpret-0.2.1/tint/utils/tqdm.py
+-rw-r--r--   0        0        0     5492 1970-01-01 00:00:00.000000 time_interpret-0.2.1/PKG-INFO
```

### Comparing `time_interpret-0.2.0/README.md` & `time_interpret-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,25 @@
 
 Time Interpret can be installed with pip:
 
 ```shell script
 pip install time_interpret
 ```
 
-or from source with conda:
+or from source:
+
+with pip:
+
+```shell script
+git clone git@github.com:babylonhealth/time_interpret.git
+cd time_interpret
+pip install -e .
+```
+
+or conda:
 
 ```shell script
 git clone git@github.com:babylonhealth/time_interpret.git
 cd time_interpret
 conda env create
 source activate tint
 pip install --no-deps -e .
@@ -33,29 +43,29 @@
 arma.download()  # This method generates the dataset
 ```
 
 We then load some test data from the dataset and the
 corresponding true saliency:
 
 ```python
-x = arma.preprocess()["x"][0]
-true_saliency = arma.true_saliency(dim=rare_dim)[0]
+inputs = arma.preprocess()["x"][0]
+true_saliency = arma.true_saliency(dim=1)[0]
 ```
 
 We can now load an attribution method and use it to compute the saliency:
 
 ```python
 from tint.attr import TemporalIntegratedGradients
 
 explainer = TemporalIntegratedGradients(arma.get_white_box)
 
-baseline = inputs * 0
+baselines = inputs * 0
 attr = explainer.attribute(
     inputs,
-    baselines=inputs * 0,
+    baselines=baselines,
     additional_forward_args=(true_saliency,),
     temporal_additional_forward_args=(True,),
 ).abs()
 ```
 
 Finally, we evaluate our method using the true saliency and a white box metric:
 
@@ -69,17 +79,17 @@
 
 - [AugmentedOcclusion](https://arxiv.org/abs/2003.02821)
 - [BayesLime](https://arxiv.org/pdf/2008.05030)
 - [BayesShap](https://arxiv.org/pdf/2008.05030)
 - [DynaMask](https://arxiv.org/pdf/2106.05303)
 - [Discretised Integrated Gradients](https://arxiv.org/abs/2108.13654)
 - [Fit](https://arxiv.org/abs/2003.02821)
+- [Non-linearities Tunnel](https://arxiv.org/abs/1906.07983)
 - [Occlusion](https://arxiv.org/abs/1311.2901)
 - [Retain](https://arxiv.org/pdf/1608.05745)
-- [SmoothGrad](https://arxiv.org/abs/1810.03292)
 
 
 ## Acknowledgment
 - [Jonathan Crabbe](https://github.com/JonathanCrabbe/Dynamask) for the DynaMask implementation.
 - [Sana Tonekaboni](https://github.com/sanatonek/time_series_explainability/tree/master/TSX) for the fit implementation.
 - [INK Lab](https://github.com/INK-USC/DIG) for the discretized integrated gradients implementation.
 - [Dylan Slack](https://github.com/dylan-slack/Modeling-Uncertainty-Local-Explainability) for the BayesLime and BayesShap implementations.
```

### Comparing `time_interpret-0.2.0/pyproject.toml` & `time_interpret-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="time_interpret"
-version="0.2.0"
+version="0.2.1"
 authors=[
     {name="Joseph Enguehard", email="joseph@skippr.com"},
 ]
 description="Model interpretability library for PyTorch with a focus on time series."
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

### Comparing `time_interpret-0.2.0/tint/attr/__init__.py` & `time_interpret-0.2.1/tint/attr/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from .discretised_ig import DiscretetizedIntegratedGradients
 from .dynamic_masks import DynaMask
 from .extremal_mask import ExtremalMask
 from .feature_ablation import FeatureAblation
 from .fit import Fit
 from .geodesic_ig import GeodesicIntegratedGradients
 from .lof import LofKernelShap, LofLime
+from .non_linearities_tunnel import NonLinearitiesTunnel
 from .occlusion import Occlusion
 from .retain import Retain
 from .seq_ig import SequentialIntegratedGradients
-from .smooth_grad import SmoothGrad
 from .temporal_augmented_occlusion import TemporalAugmentedOcclusion
 from .temporal_ig import TemporalIntegratedGradients
 from .temporal_occlusion import TemporalOcclusion
 from .time_forward_tunnel import TimeForwardTunnel
 
 __all__ = [
     "AugmentedOcclusion",
@@ -24,14 +24,15 @@
     "DynaMask",
     "ExtremalMask",
     "FeatureAblation",
     "Fit",
     "GeodesicIntegratedGradients",
     "LofKernelShap",
     "LofLime",
+    "NonLinearitiesTunnel",
     "Occlusion",
     "Retain",
     "SequentialIntegratedGradients",
     "SmoothGrad",
     "TemporalAugmentedOcclusion",
     "TemporalIntegratedGradients",
     "TemporalOcclusion",
```

### Comparing `time_interpret-0.2.0/tint/attr/augmented_occlusion.py` & `time_interpret-0.2.1/tint/attr/augmented_occlusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import torch
 
 from captum.log import log_usage
-from captum._utils.common import _format_input
+from captum._utils.common import _format_inputs
 from captum._utils.typing import (
     TargetType,
     TensorOrTupleOfTensorsGeneric,
 )
 
 from torch import Tensor
 from typing import Any, Callable, Tuple, Union
@@ -16,25 +16,31 @@
 
 
 class AugmentedOcclusion(Occlusion):
     """
     Augmented Occlusion by sampling the baseline from a bootstrapped
     distribution.
 
+    Instead of replacing occulted data by zero, this method samples data from
+    a distribution, which replace occulted data. The resulted occulted data
+    should be closer to the actual data as a result, limiting the amount of
+    out of distribution samples.
+
     Args:
         forward_func (callable): The forward function of the model or
             any modification of it.
         data (tuple, Tensor): The data from which the baselines are sampled.
             The shape of the data must be the same as the inputs, except
             on the first dimension.
         n_sampling (int): Number of sampling to run for each occlusion.
-            Default to 1
+            Default: 1
         is_temporal (bool): Whether the data is temporal or not.
             If ``True``, the data will be ablated to the inputs
-            on the temporal dimension (dimension 1). Default to ``False``
+            on the temporal dimension (dimension 1).
+            Default: False
 
     References:
         https://arxiv.org/abs/2003.02821
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import AugmentedOcclusion
@@ -52,15 +58,15 @@
         self,
         forward_func: Callable,
         data: TensorOrTupleOfTensorsGeneric,
         n_sampling: int = 1,
         is_temporal: bool = False,
     ):
         super().__init__(forward_func=forward_func)
-        self.data = _format_input(data)
+        self.data = _format_inputs(data)
         self.n_sampling = n_sampling
         self.is_temporal = is_temporal
 
         assert (
             isinstance(n_sampling, int) and n_sampling >= 1
         ), "N sampling must be an integer and at least 1."
 
@@ -193,15 +199,15 @@
                     If a single tensor is provided as inputs, a single tensor
                     is returned. If a tuple is provided for inputs, a tuple of
                     corresponding sized tensors is returned.
         """
         # Change input to tuple and check that its length is the same as data.
         # Also check that each dimension between inputs and self.data matches
         # except on the first one.
-        formatted_inputs = _format_input(inputs)
+        formatted_inputs = _format_inputs(inputs)
         _validate_input(
             inputs=formatted_inputs,
             data=self.data,
             is_temporal=self.is_temporal,
         )
 
         return super().attribute.__wrapped__(
```

### Comparing `time_interpret-0.2.0/tint/attr/bayes.py` & `time_interpret-0.2.1/tint/attr/bayes.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from .models import BLRRidge
 
 
 class BayesLime(Lime):
     """
     Bayesian version of Lime.
 
+    This method replace the linear regression of the original Lime with a
+    bayesian linear regression, allowing to model uncertainty in
+    explainability.
+
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         interpretable_model (Model): Model object to train interpretable model.
 
             This argument is optional and defaults to SkLearnBayesianRidge(),
             which is a wrapper around the Bayesian Ridge in SkLearn.
@@ -68,14 +72,18 @@
         )
 
 
 class BayesKernelShap(KernelShap):
     """
     Bayesian version of KernelShap.
 
+    This method replace the linear regression of the original KernelShap with
+    a bayesian linear regression, allowing to model uncertainty in
+    explainability.
+
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         interpretable_model (Model): Model object to train interpretable model.
 
             This argument is optional and defaults to SkLearnBayesianRidge(),
             which is a wrapper around the Bayesian Ridge in SkLearn.
```

### Comparing `time_interpret-0.2.0/tint/attr/discretised_ig.py` & `time_interpret-0.2.1/tint/attr/discretised_ig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import torch
 
 from captum.log import log_usage
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
     _format_additional_forward_args,
+    _format_inputs,
     _format_output,
     _is_tuple,
 )
 from captum._utils.typing import (
     TargetType,
     TensorOrTupleOfTensorsGeneric,
 )
 from captum.attr._utils.attribution import GradientAttribution
-from captum.attr._utils.common import _reshape_and_sum, _format_input
+from captum.attr._utils.common import _reshape_and_sum
 
 from torch import Tensor
 from typing import Any, Callable, Tuple, Union
 
 try:
     from transformers import PreTrainedModel
 except ImportError:
     PreTrainedModel = None
 
 
 class DiscretetizedIntegratedGradients(GradientAttribution):
     """
     Discretetized Integrated Gradients.
 
+    This method discretizes the path between an input and a reference
+    baseline. It was developed for text data and language models, to handle
+    the discreteness of the word embedding space.
+
     Args:
         forward_func (callable):  The forward function of the model or any
             modification of it
         multiply_by_inputs (bool, optional): Indicates whether to factor
             model inputs' multiplier in the final attribution scores.
             In the literature this is also known as local vs global
             attribution. If inputs' multiplier isn't factored in,
@@ -162,15 +167,15 @@
                 Delta is calculated per example, meaning that the number of
                 elements in returned delta tensor is equal to the number of
                 of examples in inputs.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(scaled_features)
-        scaled_features_tpl = _format_input(scaled_features)
+        scaled_features_tpl = _format_inputs(scaled_features)
 
         # Set requires_grad = True to inputs
         scaled_features_tpl = tuple(
             x.requires_grad_() for x in scaled_features_tpl
         )
 
         attributions = self.calculate_dig_attributions(
@@ -179,17 +184,17 @@
             additional_forward_args=additional_forward_args,
             n_steps=n_steps,
         )
         if return_convergence_delta:
             assert (
                 len(scaled_features_tpl) == 1
             ), "More than one tuple not supported in this code!"
-            start_point, end_point = _format_input(
+            start_point, end_point = _format_inputs(
                 scaled_features_tpl[0][0].unsqueeze(0)
-            ), _format_input(
+            ), _format_inputs(
                 scaled_features_tpl[0][-1].unsqueeze(0)
             )  # baselines, inputs (only works for one input, len(tuple) == 1)
             # computes approximation error based on the completeness axiom
             delta = self.compute_convergence_delta(
                 attributions,
                 start_point,
                 end_point,
```

### Comparing `time_interpret-0.2.0/tint/attr/dynamic_masks.py` & `time_interpret-0.2.1/tint/attr/dynamic_masks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import torch as th
 
 from captum.attr._utils.attribution import PerturbationAttribution
 from captum.log import log_usage
 from captum._utils.common import (
-    _format_input,
+    _format_inputs,
     _format_output,
     _is_tuple,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 
 from pytorch_lightning import Trainer
 from torch.utils.data import DataLoader
@@ -16,22 +16,34 @@
 
 from tint.utils import TensorDataset, _add_temporal_mask, default_collate
 from .models import MaskNet
 
 
 class DynaMask(PerturbationAttribution):
     """
-    Dynamic masks method.
+    Dynamic masks.
+
+    This method aims to explain time series data, by learning a mask
+    representing features importance. This method was inspired from
+    Fong et al., and can be used in "preservation game" mode: trying to keep
+    the closest predictions, compared with unperturebed data, with the
+    minimal number of features, or in "deletion game" mode, trying to get the
+    furthest predictions by removing the minimal number of features.
+
+    This implementation batchify the original method by leanrning in parallel
+    multiple inputs and multiple ``keep_ratio`` (called ``mask_group`` in the
+    original implementation.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
 
     References:
         https://arxiv.org/pdf/2106.05303
+        https://arxiv.org/pdf/1910.08485
 
     Examples:
         >>> import torch as th
         >>> from tint.attr import DynaMask
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
@@ -80,15 +92,15 @@
 
         Returns:
             (th.Tensor, tuple): Attributions.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         # Init trainer if not provided
         if trainer is None:
             trainer = Trainer(max_epochs=100)
         else:
             trainer = copy.deepcopy(trainer)
```

### Comparing `time_interpret-0.2.0/tint/attr/extremal_mask.py` & `time_interpret-0.2.1/tint/attr/extremal_mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import torch as th
 
 from captum.attr._utils.attribution import PerturbationAttribution
 from captum.log import log_usage
 from captum._utils.common import (
     _format_baseline,
-    _format_input,
+    _format_inputs,
     _format_output,
     _is_tuple,
     _validate_input,
 )
 from captum._utils.typing import (
     BaselineType,
     TargetType,
@@ -22,20 +22,30 @@
 
 from tint.utils import TensorDataset, _add_temporal_mask, default_collate
 from .models import ExtremalMaskNet
 
 
 class ExtremalMask(PerturbationAttribution):
     """
-    Extremal masks method.
+    Extremal masks.
+
+    This method extends the work of Fong et al. and Crabbé et al. by allowing
+    the perturbation function to be learnt. This is in addition to the learnt
+    mask. For instance, this perturbation function can be learnt with a RNN
+    while Crabbé et al. only consider fixed perturbations: Gaussian blur
+    and fade to moving average.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
 
+    References:
+        https://arxiv.org/pdf/2106.05303
+        https://arxiv.org/pdf/1910.08485
+
     Examples:
         >>> import torch as th
         >>> from tint.attr import ExtremalMask
         >>> from tint.models import MLP
         <BLANKLINE>
         >>> inputs = th.rand(8, 7, 5)
         >>> data = th.rand(32, 7, 5)
@@ -167,15 +177,15 @@
                 If a single tensor is provided as inputs, a single tensor is
                 returned. If a tuple is provided for inputs, a tuple of
                 corresponding sized tensors is returned.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         # Format and validate baselines
         baselines = _format_baseline(baselines, inputs)
         _validate_input(inputs, baselines)
 
         # Init trainer if not provided
         if trainer is None:
@@ -221,15 +231,15 @@
         trainer.fit(mask_net, train_dataloaders=dataloader)
 
         # Set model to eval mode and cast it to device
         mask_net.eval()
         mask_net.to(data.device)
 
         # Get attributions as mask representation
-        attributions = mask_net.net.representation(data, baseline)
+        attributions = mask_net.net.representation()
 
         # Reshape representation if temporal attributions
         if return_temporal_attributions:
             attributions = attributions.reshape(
                 (-1, data.shape[1]) + data.shape[1:]
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `time_interpret-0.2.0/tint/attr/feature_ablation.py` & `time_interpret-0.2.1/tint/attr/feature_ablation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Callable, Tuple, Union, cast
 
 import torch
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
     _format_additional_forward_args,
-    _format_input,
+    _format_inputs,
     _format_output,
     _is_tuple,
     _run_forward,
 )
 from captum._utils.progress import progress
 from captum._utils.typing import (
     BaselineType,
@@ -23,14 +23,16 @@
 from captum.attr._utils.common import _format_input_baseline
 from captum.log import log_usage
 from torch import Tensor, dtype
 
 
 class FeatureAblation(PerturbationAttribution):
     r"""
+    Feature ablation.
+
     A perturbation based approach to computing attribution, involving
     replacing each input feature with a given baseline / reference, and
     computing the difference in output. By default, each scalar value within
     each input tensor is taken as a feature and replaced independently. Passing
     a feature mask, allows grouping features to be ablated together. This can
     be used in cases such as images, where an entire segment or region
     can be ablated, measuring the importance of the segment (feature group).
@@ -257,15 +259,15 @@
         is_inputs_tuple = _is_tuple(inputs)
         inputs, baselines = _format_input_baseline(inputs, baselines)
         additional_forward_args = _format_additional_forward_args(
             additional_forward_args
         )
         num_examples = inputs[0].shape[0]
         feature_mask = (
-            _format_input(feature_mask) if feature_mask is not None else None
+            _format_inputs(feature_mask) if feature_mask is not None else None
         )
         assert (
             isinstance(perturbations_per_eval, int)
             and perturbations_per_eval >= 1
         ), "Perturbations per evaluation must be an integer and at least 1."
         with torch.no_grad():
             if show_progress:
```

### Comparing `time_interpret-0.2.0/tint/attr/fit.py` & `time_interpret-0.2.1/tint/attr/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import torch as th
 import torch.nn.functional as F
 
 from captum.attr._utils.attribution import PerturbationAttribution
 from captum.log import log_usage
 from captum._utils.common import (
-    _format_input,
+    _format_inputs,
     _format_output,
     _is_tuple,
     _run_forward,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 
 from pytorch_lightning import LightningDataModule, Trainer
@@ -162,15 +162,15 @@
 
         Returns:
             (th.Tensor, tuple): Attributions.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         # Assert only one input, as the Retain only accepts one
         assert (
             len(inputs) == 1
         ), "Multiple inputs are not accepted for this method"
         data = inputs[0]
```

### Comparing `time_interpret-0.2.0/tint/attr/geodesic_ig.py` & `time_interpret-0.2.1/tint/attr/geodesic_ig.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import torch
 import typing
 import warnings
 
 from captum.attr._utils.approximation_methods import approximation_parameters
 from captum.attr._utils.attribution import GradientAttribution
 from captum.attr._utils.common import (
-    _format_input,
     _format_input_baseline,
     _reshape_and_sum,
     _validate_input,
 )
 from captum.log import log_usage
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
     _format_additional_forward_args,
+    _format_inputs,
     _format_output,
     _is_tuple,
 )
 from captum._utils.typing import (
     BaselineType,
     TargetType,
     TensorOrTupleOfTensorsGeneric,
@@ -30,17 +30,36 @@
 from torch import Tensor
 from typing import Any, Callable, List, Tuple, Union
 
 from tint.utils import astar_path, unsqueeze_like, _geodesic_batch_attribution
 
 
 class GeodesicIntegratedGradients(GradientAttribution):
-    """
+    r"""
     Geodesic Integrated Gradients.
 
+    This method uses K Nearest Neighbors on the input data to approximate the
+    geodesic path between inputs and reference baselines. The input space is
+    seen here as a Riemannian manifold, whose metric is the inner product of
+    the gradient of the model:
+
+    .. math::
+        <\nabla F(x)^T, \nabla F(x)>
+
+    Using this path reduces the risk of creating artifacts compared with
+    the original Integrated Gradients (IG). It also supports
+    ``internal_batch_size`` for faster compute. The number of steps is also
+    set by default to 5, as less steps are required between two neighbors.
+    With this setting, and the number of neighbors set to 10, the number of
+    gradients to compute is 10 * 5 = 50, the same number as the original IG.
+
+    The shortest path is computed using Dijkstra or A* algorithms. This can
+    be computationally expensive for a number of inputs greater than a few
+    thousands.
+
     Args:
         forward_func (callable):  The forward function of the model or any
             modification of it.
         nn (NearestNeighbors, tuple): Nearest neighbors method.
             If not provided, will be created when calling __init__ or
             attribute.
             Default: None
@@ -60,14 +79,28 @@
             method is called global.
             More detailed can be found here:
             https://arxiv.org/abs/1711.06104
 
             In case of integrated gradients, if `multiply_by_inputs`
             is set to True, final sensitivity scores are being multiplied by
             (inputs - baselines).
+
+    Examples:
+        >>> import torch as th
+        >>> from tint.attr import GeodesicIntegratedGradients
+        >>> from tint.models import MLP
+        <BLANKLINE>
+        >>> inputs = th.rand(50, 5)
+        >>> data = th.rand(100, 5)
+        >>> mlp = MLP([5, 3, 1])
+        <BLANKLINE>
+        >>> explainer = GeodesicIntegratedGradients(
+        ...     mlp, data=data, n_neighbors=10,
+        ... )
+        >>> attr = explainer.attribute(inputs)
     """
 
     def __init__(
         self,
         forward_func: Callable,
         nn: Union[NearestNeighbors, Tuple[NearestNeighbors, ...]] = None,
         data: TensorOrTupleOfTensorsGeneric = None,
@@ -87,15 +120,15 @@
             if not isinstance(nn, tuple):
                 nn = (nn,)
             self.nn = nn
             self.n_neighbors = tuple(nn_.n_neighbors for nn_ in self.nn)
 
         # Fit NearestNeighbors if data is provided
         if data is not None:
-            data = _format_input(data)
+            data = _format_inputs(data)
 
             assert n_neighbors is not None, "You must provide n_neighbors"
             if isinstance(n_neighbors, int):
                 n_neighbors = tuple(n_neighbors for _ in data)
 
             self.n_neighbors = n_neighbors
             self.nn = tuple(
@@ -127,14 +160,15 @@
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_neighbors: Union[int, Tuple[int]] = None,
         n_steps: int = 5,
         n_steiner: int = None,
         method: str = "gausslegendre",
         internal_batch_size: Union[None, int] = None,
+        return_curvature: bool = False,
         return_convergence_delta: bool = False,
         distance: str = "geodesic",
         show_progress: bool = False,
         **kwargs,
     ) -> TensorOrTupleOfTensorsGeneric:
         ...
 
@@ -147,14 +181,15 @@
         additional_forward_args: Any = None,
         n_neighbors: Union[int, Tuple[int]] = None,
         n_steps: int = 5,
         n_steiner: int = None,
         method: str = "gausslegendre",
         internal_batch_size: Union[None, int] = None,
         *,
+        return_curvature: bool = False,
         return_convergence_delta: bool,
         distance: str = "geodesic",
         show_progress: bool = False,
         **kwargs,
     ) -> Tuple[TensorOrTupleOfTensorsGeneric, Tensor]:
         ...
 
@@ -166,31 +201,40 @@
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_neighbors: Union[int, Tuple[int]] = None,
         n_steps: int = 5,
         n_steiner: int = None,
         method: str = "gausslegendre",
         internal_batch_size: Union[None, int] = None,
+        return_curvature: bool = False,
         return_convergence_delta: bool = False,
         distance: str = "geodesic",
         show_progress: bool = False,
         **kwargs,
     ) -> Union[
         TensorOrTupleOfTensorsGeneric,
         Tuple[TensorOrTupleOfTensorsGeneric, Tensor],
+        Tuple[TensorOrTupleOfTensorsGeneric, TensorOrTupleOfTensorsGeneric],
+        Tuple[
+            TensorOrTupleOfTensorsGeneric,
+            Tensor,
+            TensorOrTupleOfTensorsGeneric,
+        ],
     ]:
         r"""
         This method attributes the output of the model with given target index
         (in case it is provided, otherwise it assumes that output is a
         scalar) to the inputs of the model using the approach described above.
 
         In addition to that it also returns, if `return_convergence_delta` is
         set to True, integral approximation delta based on the completeness
         property of integrated gradients.
 
+        It also returns the curvature if `return_curvature` is set to True.
+
         Args:
             inputs (tensor or tuple of tensors):  Input for which integrated
                 gradients are computed. If forward_func takes a single
                 tensor as input, a single input tensor should be provided.
                 If forward_func takes multiple tensors as input, a tuple
                 of the input tensors should be provided. It is assumed
                 that for all given input tensors, dimension 0 corresponds
@@ -289,14 +333,19 @@
                 #examples.
                 For DataParallel models, each batch is split among the
                 available devices, so evaluations on each available
                 device contain internal_batch_size / num_devices examples.
                 If internal_batch_size is None, then all evaluations are
                 processed in one batch.
                 Default: None
+            return_curvature (bool, optional): Indicates whether to return
+                the curvature or not. If `return_curvature`
+                is set to True curvature will be returned in a tuple following
+                attributions and optionally convergence delta.
+                Default: False
             return_convergence_delta (bool, optional): Indicates whether to return
                 convergence delta or not. If `return_convergence_delta`
                 is set to True convergence delta will be returned in
                 a tuple following attributions.
                 Default: False
             distance (str, optional): Which distance to use with the A*
                 algorithm:
@@ -309,14 +358,15 @@
 
                 Default: 'geodesic'
             show_progress (bool, optional): Displays the progress of computation.
                 It will try to use tqdm if available for advanced features
                 (e.g. time estimation). Otherwise, it will fallback to
                 a simple output of progress.
                 Default: False
+
         Returns:
             **attributions** or 2-element tuple of **attributions**, **delta**:
             - **attributions** (*tensor* or tuple of *tensors*):
                 Integrated gradients with respect to each input feature.
                 attributions will always be the same size as the provided
                 inputs, with each value providing the attribution of the
                 corresponding input index.
@@ -328,14 +378,27 @@
                 integrated gradients. This is computed using the property
                 that the total sum of forward_func(inputs) -
                 forward_func(baselines) must equal the total sum of the
                 integrated gradient.
                 Delta is calculated per example, meaning that the number of
                 elements in returned delta tensor is equal to the number of
                 examples in inputs.
+            - **curvature** (*tensor*, returned if return_curvature=True):
+                The difference between the distance along the path computed
+                by the A* algorithm and the euclidean distance between
+                inputs and baselines. This value, always positive,
+                returns a measure of the curvature of the input space, with
+                the inner product of the gradient of the model:
+
+                .. math::
+                    <\nabla F(x)^T, \nabla F(x)>
+
+                as a metric. A higher value indicates a higher curvature.
+                This value however depends on the path and is as such only
+                an indication of the true curvature of the input space.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
 
         inputs, baselines = _format_input_baseline(inputs, baselines)
 
@@ -553,25 +616,49 @@
         # Sum over points and paths
         # and stack result
         total_grads = tuple(
             tuple(x.sum(0) for x in grad) for grad in total_grads
         )
         total_grads = tuple(torch.stack(grad) for grad in total_grads)
 
+        # Optionally compute curvature
+        curvature = None
+        if return_curvature:
+            curvature = self.compute_curvature(
+                inputs=inputs,
+                baselines=baselines,
+                data=data,
+                knns=knns,
+                idx=idx,
+                grads_idx=grads_idx,
+                paths_len=paths_len,
+            )
+
         if return_convergence_delta:
             start_point, end_point = baselines, inputs
             # computes approximation error based on the completeness axiom
             delta = self.compute_convergence_delta(
                 total_grads,
                 start_point,
                 end_point,
                 additional_forward_args=additional_forward_args,
                 target=target,
             )
+            if curvature is not None:
+                return (
+                    _format_output(is_inputs_tuple, total_grads),
+                    delta,
+                    _format_output(is_inputs_tuple, curvature),
+                )
             return _format_output(is_inputs_tuple, total_grads), delta
+
+        if curvature is not None:
+            return _format_output(
+                is_inputs_tuple, total_grads
+            ), _format_output(is_inputs_tuple, curvature)
         return _format_output(is_inputs_tuple, total_grads)
 
     def _attribute(
         self,
         inputs: Tuple[Tensor, ...],
         baselines: Tuple[Union[Tensor, int, float], ...],
         target: TargetType = None,
@@ -768,13 +855,74 @@
         knns = tuple(
             torch.cat([k, a], dim=0) if len(a) > 0 else k
             for k, a in zip(knns, add_knns)
         )
 
         return idx, knns, dists
 
+    @staticmethod
+    def compute_curvature(
+        inputs: TensorOrTupleOfTensorsGeneric,
+        baselines: Tuple[Union[Tensor, int, float], ...],
+        data: Tuple[Tensor, ...],
+        knns: Tuple[Tensor, ...],
+        idx: Tuple[Tensor, ...],
+        grads_idx: Tuple[List, ...],
+        paths_len: Tuple[List[int]],
+    ) -> Tuple[Tensor, ...]:
+        """
+        Compute the curvature of the input space, as the difference between
+        the euclidean distance along the path computed by the A* algorithm
+        and the euclidean distance between the inputs and baseline.
+        The curvature is always positive.
+        """
+        # Compute euclidean distances for each neighbors
+        distances_tpl = tuple(
+            torch.linalg.norm(
+                (x[knn] - x[id]).reshape(len(x[knn]), -1),
+                dim=1,
+            )
+            for x, knn, id in zip(data, knns, idx)
+        )
+
+        # Get distance of each path
+        distances_tpl = tuple(
+            dist[grad_idx] for dist, grad_idx in zip(distances_tpl, grads_idx)
+        )
+
+        # Split for each path
+        distances_tpl = tuple(
+            torch.split(grad, split_size_or_sections=path_len, dim=0)
+            for grad, path_len in zip(distances_tpl, paths_len)
+        )
+
+        # Sum over points and paths
+        # and stack result
+        distances_tpl = tuple(
+            tuple(x.sum(0) for x in dist) for dist in distances_tpl
+        )
+        distances_tpl = tuple(torch.stack(dist) for dist in distances_tpl)
+
+        # Compute euclidean distance between inputs and baselines
+        euclidean_tpl = tuple(
+            torch.linalg.norm(
+                (input - baseline).reshape(len(input), -1),
+                dim=1,
+            )
+            for input, baseline in zip(inputs, baselines)
+        )
+
+        # The curvature is the diff between path-based distance and euclidean
+        # distance.
+        curvature = tuple(
+            dist - euclidean
+            for dist, euclidean in zip(distances_tpl, euclidean_tpl)
+        )
+
+        return curvature
+
     def has_convergence_delta(self) -> bool:
         return True
 
     @property
     def multiplies_by_inputs(self):
         return self._multiply_by_inputs
```

### Comparing `time_interpret-0.2.0/tint/attr/lof.py` & `time_interpret-0.2.1/tint/attr/lof.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,24 @@
         ) * max(score.mean().item(), EPS)
 
 
 class LofLime(Lime, LOF):
     r"""
     Local Outlier Factor Lime.
 
+    This method compute a Local Outlier Factor score for every perturbed data.
+    This score is then used to update the weight given by the similarity
+    function:
+
+    .. math::
+        new_weight(x) = similarity(x) * \frac{-1}{lof_score(x)}
+
+    If the perturbed data is considered more out of sample, the weight of
+    this data will be reduced.
+
     Args:
         forward_func (Callable): The forward function of the model or any
             modification of it.
         embeddings (Tensor): Tensor of embeddings to compute the LOF.
         n_neighbors (int): Number of neighbors to use by default.
             Default to 20
         interpretable_model (optional, Model): Model object to train
@@ -190,17 +200,27 @@
 
         # Replace original similarity_func with the custom one
         self._similarity_func = self.similarity_func
         self.similarity_func = self.lof_similarity_func
 
 
 class LofKernelShap(KernelShap, LOF):
-    """
+    r"""
     Local Outlier Factor Kernel Shap.
 
+    This method compute a Local Outlier Factor score for every perturbed data.
+    This score is then used to update the weight given by the similarity
+    function:
+
+    .. math::
+        new_weight(x) = similarity(x) * \frac{-1}{lof_score(x)}
+
+    If the perturbed data is considered more out of sample, the weight of
+    this data will be reduced.
+
     Args:
         forward_func (Callable): The forward function of the model or any
             modification of it.
         embeddings (Tensor): Tensor of embeddings to compute the LOF.
         n_neighbors (int): Number of neighbors to use by default.
             Default to 20
```

### Comparing `time_interpret-0.2.0/tint/attr/models/bayes_linear.py` & `time_interpret-0.2.1/tint/attr/models/bayes_linear.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/attr/models/extremal_mask.py` & `time_interpret-0.2.1/tint/attr/models/extremal_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from captum._utils.common import _run_forward
 
 from typing import Callable, Union
 
 from tint.models import Net
 
 
-class ExtremalMask(nn.Module):
+class ExtremalMaskNN(nn.Module):
     """
-    Extremal Mask model.
+    Extremal Mask NN model.
 
     Args:
         forward_func (callable): The forward function of the model or any
             modification of it.
         model (nnn.Module): A model used to recreate the original
             predictions, in addition to the mask. Default to ``None``
         batch_size (int): Batch size of the model. Default to 32
@@ -56,21 +56,21 @@
         mask = self.mask
 
         # Subset sample to current batch
         mask = mask[
             self.batch_size * batch_idx : self.batch_size * (batch_idx + 1)
         ]
 
-        # We forward model if provided
-        if self.model is not None:
-            mask = mask + self.model(x - baselines)
-
         # We clamp the mask
         mask = mask.clamp(0, 1)
 
+        # If model is provided, we use it as the baselines
+        if self.model is not None:
+            baselines = self.model(x - baselines)
+
         # Mask data according to samples
         # We eventually cut samples up to x time dimension
         # x1 represents inputs with important features masked.
         # x2 represents inputs with unimportant features masked.
         mask = mask[:, : x.shape[1], ...]
         x1 = x * mask + baselines * (1.0 - mask)
         x2 = x * (1.0 - mask) + baselines * mask
@@ -87,23 +87,16 @@
                 forward_func=self.forward_func,
                 inputs=x2,
                 target=target,
                 additional_forward_args=additional_forward_args,
             ),
         )
 
-    def representation(self, data, baselines):
-        if self.model is None:
-            return self.mask.detach().cpu().clamp(0, 1)
-        return (
-            (self.mask + self.model(data - baselines))
-            .detach()
-            .cpu()
-            .clamp(0, 1)
-        )
+    def representation(self):
+        return self.mask.detach().cpu().clamp(0, 1)
 
 
 class ExtremalMaskNet(Net):
     """
     Extremal mask model as a Pytorch Lightning model.
 
     Args:
@@ -148,15 +141,15 @@
         loss: Union[str, Callable] = "mse",
         optim: str = "adam",
         lr: float = 0.001,
         lr_scheduler: Union[dict, str] = None,
         lr_scheduler_args: dict = None,
         l2: float = 0.0,
     ):
-        mask = ExtremalMask(
+        mask = ExtremalMaskNN(
             forward_func=forward_func,
             model=model,
             batch_size=batch_size,
         )
 
         super().__init__(
             layers=mask,
@@ -212,23 +205,23 @@
             target=target,
             additional_forward_args=tuple(additional_forward_args)
             if additional_forward_args is not None
             else None,
         )
 
         # Add L1 loss
-        mask_ = self.net.mask
+        mask_ = self.net.mask.abs()
         if self.net.model is not None:
             mask_ = mask_[
                 self.net.batch_size
                 * batch_idx : self.net.batch_size
                 * (batch_idx + 1)
             ]
-            mask_ = mask_ + self.net.model(x - baselines)
-        reg_loss = mask_.abs().mean()
+            mask_ = mask_ + self.net.model(x - baselines).abs()
+        reg_loss = mask_.mean()
 
         # Compute and return loss
         if self.comp_loss:
             return (
                 self.loss(y_hat1, y_target1)
                 + self.loss(y_hat2, y_target2)
                 + reg_loss
```

### Comparing `time_interpret-0.2.0/tint/attr/models/joint_features_generator.py` & `time_interpret-0.2.1/tint/attr/models/joint_features_generator.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/attr/models/mask.py` & `time_interpret-0.2.1/tint/attr/models/mask.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/attr/models/path_generator.py` & `time_interpret-0.2.1/tint/attr/models/path_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,20 @@
             non_mono_count = 10000 - monotonic(
                 word_features[ref_idx],
                 word_features[wrd_idx],
                 word_features[j],
                 ret="count",
             )
             anchor_map[j] = [non_mono_count]
+        elif strategy == "non_monotonic":
+            # Here we just use the distance between the reference
+            # and the proposed word
+            anchor_map[j] = [
+                distance(word_features[ref_idx], word_features[j])
+            ]
         else:
             raise NotImplementedError
 
     if len(anchor_map) == 0:
         return ref_idx
 
     sorted_dist_map = {
@@ -252,22 +258,27 @@
             ref_input_ids[idx],
             word_idx_map=word_idx_map,
             word_features=word_features,
             adj=adj,
             steps=steps,
             strategy=strategy,
         )
-        monotonic_embs = make_monotonic_path(
-            word_path,
-            ref_input_ids[idx],
-            word_features=word_features,
-            steps=steps,
-            factor=factor,
-        )
-        all_path_embs.append(monotonic_embs)
+        if strategy != "non_monotonic":
+            embs = make_monotonic_path(
+                word_path,
+                ref_input_ids[idx],
+                word_features=word_features,
+                steps=steps,
+                factor=factor,
+            )
+        else:
+            embs = [word_features[idx] for idx in word_path]
+            embs += [word_features[ref_input_ids[idx]]]
+            embs.reverse()  # baseline --> input
+        all_path_embs.append(embs)
     all_path_embs = torch.tensor(
         np.stack(all_path_embs, axis=1),
         dtype=torch.float,
         device=device,
         requires_grad=True,
     )
```

### Comparing `time_interpret-0.2.0/tint/attr/models/retain.py` & `time_interpret-0.2.1/tint/attr/models/retain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch as th
 import torch.nn as nn
 
 from torch.autograd import Variable
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
-from torchmetrics import AUROC
 from typing import Callable, Union
 
 from tint.models import Net
 
 
 def masked_softmax(batch_tensor, mask):
     exp = th.exp(batch_tensor)
@@ -219,28 +218,20 @@
             optim=optim,
             lr=lr,
             lr_scheduler=lr_scheduler,
             lr_scheduler_args=lr_scheduler_args,
             l2=l2,
         )
 
-        if loss == "cross_entropy":
-            for stage in ["train", "val", "test"]:
-                setattr(self, stage + "_auroc", AUROC())
-
     def step(self, batch, batch_idx, stage):
         x, y = batch
 
         lengths = th.randint(low=4, high=x.shape[1], size=(len(x),))
         lengths, _ = th.sort(lengths, descending=True)
         lengths[0] = x.shape[1]
 
         y_hat, _, _ = self.net(x=x.float(), lengths=lengths)
         if self.net.temporal_labels:
             y = y[th.arange(len(x)), lengths - 1, ...]
         loss = self.loss(y_hat, y)
 
-        if isinstance(self._loss, nn.CrossEntropyLoss):
-            getattr(self, stage + "_auroc")(y_hat[:, 1], y.long())
-            self.log(stage + "_auroc", getattr(self, stage + "_auroc"))
-
         return loss
```

### Comparing `time_interpret-0.2.0/tint/attr/occlusion.py` & `time_interpret-0.2.1/tint/attr/occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from typing import Any, Callable, Tuple, Union
 
 import numpy as np
 import torch
-from captum._utils.common import _format_input
+from captum._utils.common import _format_inputs
 from captum._utils.typing import (
     BaselineType,
     TargetType,
     TensorOrTupleOfTensorsGeneric,
 )
 from captum.attr._utils.common import (
     _format_and_verify_sliding_window_shapes,
@@ -233,15 +233,15 @@
             >>> input = torch.randn(2, 4, 4)
             >>> # Defining Occlusion interpreter
             >>> ablator = Occlusion(net)
             >>> # Computes occlusion attribution, ablating each 3x3 patch,
             >>> # shifting in each direction by the default of 1.
             >>> attr = ablator.attribute(input, target=1, sliding_window_shapes=(3,3))
         """
-        formatted_inputs = _format_input(inputs)
+        formatted_inputs = _format_inputs(inputs)
 
         # Formatting strides
         strides = _format_and_verify_strides(strides, formatted_inputs)
 
         # Formatting sliding window shapes
         sliding_window_shapes = _format_and_verify_sliding_window_shapes(
             sliding_window_shapes, formatted_inputs
```

### Comparing `time_interpret-0.2.0/tint/attr/retain.py` & `time_interpret-0.2.1/tint/attr/retain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 
 import torch as th
 
 from captum.attr._utils.attribution import PerturbationAttribution
 from captum.log import log_usage
 from captum._utils.common import (
-    _format_input,
+    _format_inputs,
     _format_output,
     _is_tuple,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric, TargetType
 
 from pytorch_lightning import LightningDataModule, Trainer
 from torch.utils.data import DataLoader, TensorDataset
@@ -62,15 +62,14 @@
         labels: th.Tensor = None,
         trainer: Trainer = None,
         batch_size: int = 32,
     ) -> None:
         # If forward_func is not provided,
         # train retain model
         if forward_func is None:
-
             # Create dataloader if not provided
             dataloader = None
             if datamodule is None:
                 assert (
                     features is not None
                 ), "You must provide either a datamodule or features"
                 assert (
@@ -131,15 +130,15 @@
 
         Returns:
             (th.Tensor, tuple): Attributions.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         # Assert only one input, as the Retain only accepts one
         assert (
             len(inputs) == 1
         ), "Multiple inputs are not accepted for this method"
 
         # Make target a tensor
```

### Comparing `time_interpret-0.2.0/tint/attr/seq_ig.py` & `time_interpret-0.2.1/tint/attr/seq_ig.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,28 @@
 from tint.utils import get_progress_bars
 
 
 class SequentialIntegratedGradients(GradientAttribution):
     r"""
     Sequential Integrated Gradients.
 
+    This method is the regular Integrated Gradients (IG) applied on each
+    component of a sequence. However, the baseline is specific to each
+    component: it keeps fixed the rest of the sequence while only setting the
+    component of interest to a reference baseline.
+
+    For instance, on a setence of m words, the attribution of each word is
+    computed by running IG with a specific baseline: fixing every other word
+    to their current value, and replacing the word of interest with "<pad>",
+    an uninformative baseline.
+
+    This method can be computationally expensive on long sequences, as it
+    needs to compute IG on each component individually. It is therefore
+    suggested to reduce ``n_steps`` when using this method on long sequences.
+
     Args:
         forward_func (callable):  The forward function of the model or any
             modification of it
         multiply_by_inputs (bool, optional): Indicates whether to factor
             model inputs' multiplier in the final attribution scores.
             In the literature this is also known as local vs global
             attribution. If inputs' multiplier isn't factored in,
```

### Comparing `time_interpret-0.2.0/tint/attr/temporal_augmented_occlusion.py` & `time_interpret-0.2.1/tint/attr/temporal_augmented_occlusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import torch
 
 from captum.log import log_usage
-from captum._utils.common import _format_input
+from captum._utils.common import _format_inputs
 from captum._utils.typing import (
     TensorOrTupleOfTensorsGeneric,
     TargetType,
 )
 
 from torch import Tensor
 from typing import Any, Callable, Tuple, Union
 
 from tint.attr import AugmentedOcclusion
 
 
 class TemporalAugmentedOcclusion(AugmentedOcclusion):
     """
-    Temporal Augmented Occlusion
+    Temporal Augmented Occlusion.
 
-    This method modifies the original augmented occlusion by only
-    perturbing the last time, leaving the previous times unchanged.
+    This method modifies the original augmented occlusion by only perturbing
+    the last time, leaving the previous times unchanged. It can be used
+    together with ``time_forward_tunnel`` to compute attributions on time
+    series.
 
     Args:
         forward_func (callable): The forward function of the model or
             any modification of it
         data (tuple, Tensor): The data from which the baselines are sampled.
         n_sampling (int): Number of sampling to run for each occlusion.
             Default to 1
@@ -186,15 +188,15 @@
                             the same size as the provided inputs, with each value
                             providing the attribution of the corresponding input index.
                             If a single tensor is provided as inputs, a single tensor is
                             returned. If a tuple is provided for inputs, a tuple of
                             corresponding sized tensors is returned.
         """
 
-        inputs_tpl = _format_input(inputs)
+        inputs_tpl = _format_inputs(inputs)
 
         assert all(
             x.shape[1] == inputs_tpl[0].shape[1] for x in inputs_tpl
         ), "All inputs must have the same time dimension. (dimension 1)"
 
         # The time sliding must be equal to the time dim as we only
         # perform the perturbation on the last time
```

### Comparing `time_interpret-0.2.0/tint/attr/temporal_ig.py` & `time_interpret-0.2.1/tint/attr/temporal_ig.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 
 from captum.attr import IntegratedGradients
 from captum.log import log_usage
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
-    _format_input,
+    _format_inputs,
     _format_additional_forward_args,
     _format_baseline,
     _is_tuple,
     _format_tensor_into_tuples,
     _format_output,
 )
 from captum._utils.typing import (
@@ -28,14 +28,23 @@
 from typing import Any, Callable, List, Tuple, Union, cast
 
 
 class TemporalIntegratedGradients(IntegratedGradients):
     """
     Temporal Integrated Gradients.
 
+    This method computes gradients iteratively on a time series as such:
+    it crops the sequence up to a time, and only moves this last time from
+    a baseline to its original value.
+
+    The number of steps per time depends on the strategy. If it is
+    ``'fixed'``, then n_steps gradients are computed for each time.
+    If it is ``'interval'``, the number of steps depends on the interval
+    between two times: the larger, the greater number of points.
+
     Args:
         forward_func (callable): The forward function of the model or
             any modification of it.
         multiply_by_inputs (bool, optional): Indicates whether to factor
             model inputs' multiplier in the final attribution scores.
             In the literature this is also known as local vs global
             attribution. If inputs' multiplier isn't factored in,
@@ -104,15 +113,15 @@
         additional_forward_args: Any = None,
         times: Tensor = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
         strategy: str = "fixed",
         internal_batch_size: Union[None, int] = None,
         *,
-        return_convergence_delta: Literal[True],
+        return_convergence_delta: Literal[True] = True,
         temporal_target: bool = False,
         temporal_additional_forward_args: Tuple[bool] = None,
         return_temporal_attributions: bool = False,
         show_progress: bool = False,
     ) -> Tuple[TensorOrTupleOfTensorsGeneric, Tensor]:
         ...
 
@@ -282,15 +291,15 @@
                 elements in returned delta tensor is equal to the number of
                 of examples in inputs.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = isinstance(inputs, tuple)
 
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         # Get baselines
         baselines = _format_baseline(baselines, inputs)
 
         assert all(
             x.shape[1] == inputs[0].shape[1] for x in inputs
         ), "All inputs must have the same time dimension. (dimension 1)"
```

### Comparing `time_interpret-0.2.0/tint/attr/temporal_occlusion.py` & `time_interpret-0.2.1/tint/attr/temporal_occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import torch
 
 from captum.log import log_usage
-from captum._utils.common import _format_input
+from captum._utils.common import _format_inputs
 from captum._utils.typing import (
     TensorOrTupleOfTensorsGeneric,
     BaselineType,
     TargetType,
 )
 
 from torch import Tensor
 from typing import Any, Callable, Tuple, Union
 
 from .occlusion import Occlusion
 
 
 class TemporalOcclusion(Occlusion):
     """
-    Temporal Occlusion
+    Temporal Occlusion.
 
-    This method modifies the original occlusion by only perturbing the
-    last time, leaving the previous times unchanged.
+    This method modifies the original occlusion by only perturbing the last
+    time, leaving the previous times unchanged. It can be used together with
+    ``time_forward_tunnel`` to compute attributions on time series.
 
     Args:
         forward_func (callable): The forward function of the model or
             any modification of it.
 
     Examples:
         >>> import torch as th
@@ -195,15 +196,15 @@
                             the same size as the provided inputs, with each value
                             providing the attribution of the corresponding input index.
                             If a single tensor is provided as inputs, a single tensor is
                             returned. If a tuple is provided for inputs, a tuple of
                             corresponding sized tensors is returned.
         """
 
-        inputs_tpl = _format_input(inputs)
+        inputs_tpl = _format_inputs(inputs)
 
         assert all(
             x.shape[1] == inputs_tpl[0].shape[1] for x in inputs_tpl
         ), "All inputs must have the same time dimension. (dimension 1)"
 
         # The time sliding must be equal to the time dim as we only
         # perform the perturbation on the last time
```

### Comparing `time_interpret-0.2.0/tint/attr/time_forward_tunnel.py` & `time_interpret-0.2.1/tint/attr/time_forward_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import torch
 
 from captum.attr._utils.attribution import Attribution, GradientAttribution
 from captum.log import log_usage
 from captum._utils.common import (
-    _format_input,
+    _format_inputs,
     _is_tuple,
     _format_tensor_into_tuples,
     _format_output,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 
 from torch import Tensor
 from typing import Any, Tuple, Union, cast
 
 from tint.utils import get_progress_bars, _slice_to_time
 
 
 class TimeForwardTunnel(Attribution):
     r"""
+    Time Forward Tunnel.
+
     Performs interpretation method by iteratively retrieving the input data
     up to a time, and computing the predictions using this data and the
     forward_func.
 
-    This method allows to use interpretation methods in a setting which is
-    not retrospective: the true label is not yet known.
-
-    The target will be ignored when using this method, as it will be
-    computed internally.
+    The true target can be passed, otherwise it will be inferred depending on
+    the task.
 
     Args:
         attribution_method (Attribution): An instance of any attribution algorithm
                     of type `Attribution`. E.g. Integrated Gradients,
                     Conductance or Saliency.
 
     References:
@@ -147,15 +146,15 @@
                 return delta value. It is computed only for some
                 algorithms, e.g. integrated gradients.
         """
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = isinstance(inputs, tuple)
 
-        inputs = _format_input(inputs)
+        inputs = _format_inputs(inputs)
 
         assert all(
             x.shape[1] == inputs[0].shape[1] for x in inputs
         ), "All inputs must have the same time dimension. (dimension 1)"
 
         # Check if needs to return convergence delta
         return_convergence_delta = (
```

### Comparing `time_interpret-0.2.0/tint/datasets/arma.py` & `time_interpret-0.2.1/tint/datasets/arma.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/biobank.py` & `time_interpret-0.2.1/tint/datasets/biobank.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/dataset.py` & `time_interpret-0.2.1/tint/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/hawkes.py` & `time_interpret-0.2.1/tint/datasets/hawkes.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/hmm.py` & `time_interpret-0.2.1/tint/datasets/hmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from .dataset import DataModule
 
 
 file_dir = os.path.dirname(__file__)
 
 
 def logit(x):
+    # The real logit should be '1.0 / (1 + np.exp(-x))', but we use -2 as in
+    # https://github.com/JonathanCrabbe/Dynamask for fair comparison.
     return 1.0 / (1 + np.exp(-2 * x))
 
 
 class HMM(DataModule):
     """
     2-state Hidden Markov Model as described in the DynaMask paper.
```

### Comparing `time_interpret-0.2.0/tint/datasets/mimic3.py` & `time_interpret-0.2.1/tint/datasets/mimic3.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/utils/fasttext.py` & `time_interpret-0.2.1/tint/datasets/utils/fasttext.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/utils/labels.json` & `time_interpret-0.2.1/tint/datasets/utils/labels.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/utils/labels.py` & `time_interpret-0.2.1/tint/datasets/utils/labels.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/datasets/utils/read_3_2.json` & `time_interpret-0.2.1/tint/datasets/utils/read_3_2.json`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/accuracy.py` & `time_interpret-0.2.1/tint/metrics/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         mask_largest: Whether to mask the topk attribution or to only keep
```

### Comparing `time_interpret-0.2.0/tint/metrics/base.py` & `time_interpret-0.2.1/tint/metrics/base.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/comprehensiveness.py` & `time_interpret-0.2.1/tint/metrics/comprehensiveness.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         weight_fn (Callable): Function to compute metrics weighting using
```

### Comparing `time_interpret-0.2.0/tint/metrics/cross_entropy.py` & `time_interpret-0.2.1/tint/metrics/cross_entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         mask_largest: Whether to mask the topk attribution or to only keep
```

### Comparing `time_interpret-0.2.0/tint/metrics/lipschitz_max.py` & `time_interpret-0.2.1/tint/metrics/lipschitz_max.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/log_odds.py` & `time_interpret-0.2.1/tint/metrics/log_odds.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         weight_fn (Callable): Function to compute metrics weighting using
```

### Comparing `time_interpret-0.2.0/tint/metrics/mae.py` & `time_interpret-0.2.1/tint/metrics/mae.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         mask_largest: Whether to mask the topk attribution or to only keep
```

### Comparing `time_interpret-0.2.0/tint/metrics/mse.py` & `time_interpret-0.2.1/tint/metrics/mse.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         mask_largest: Whether to mask the topk attribution or to only keep
```

### Comparing `time_interpret-0.2.0/tint/metrics/sufficiency.py` & `time_interpret-0.2.1/tint/metrics/sufficiency.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             of gaussian noise with zero mean that is added to each
             input in the batch. If `stdevs` is a single float value
             then that same value is used for all inputs. If it is
             a tuple, then it must have the same length as the inputs
             tuple. In this case, each stdev value in the stdevs tuple
             corresponds to the input with the same index in the inputs
             tuple.
-            Default: 1.0
+            Default: 0.0
         draw_baseline_from_distrib (bool, optional): Indicates whether to
             randomly draw baseline samples from the `baselines`
             distribution provided as an input tensor.
             Default: False
         topk: Proportion of input to be dropped. Must be between 0 and 1.
             Default: 0.2
         weight_fn (Callable): Function to compute metrics weighting using
```

### Comparing `time_interpret-0.2.0/tint/metrics/weights/lof_weights.py` & `time_interpret-0.2.1/tint/metrics/weights/lof_weights.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,35 @@
         n_neighbors (int, optional): Number of neighbors for the lof.
             Default: 20
         **kwargs: Additional arguments for the lof.
 
     Returns:
         Callable: A function to compute weights given original and
             perturbed inputs.
+
+    Examples:
+        >>> import torch as th
+        >>> from captum.attr import Saliency
+        >>> from tint.metrics import accuracy
+        >>> from tint.metrics.weights import lof_weights
+        >>> from tint.models import MLP
+        <BLANKLINE>
+        >>> inputs = th.rand(8, 7, 5)
+        >>> mlp = MLP([5, 3, 1])
+        <BLANKLINE>
+        >>> explainer = Saliency(mlp)
+        >>> attr = explainer.attribute(inputs, target=0)
+        <BLANKLINE>
+        >>> acc = accuracy(
+        ...     mlp,
+        ...     inputs,
+        ...     attr,
+        ...     target=0,
+        ...     weight_fn=lof_weights(th.rand(20, 7, 5), 5)
+        ... )
     """
     # Format data
     data = _format_tensor_into_tuples(data)
 
     # Def and fit lof
     lof_tpl = tuple(
         LocalOutlierFactor(
```

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/aup.py` & `time_interpret-0.2.1/tint/metrics/white_box/aup.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/auprc.py` & `time_interpret-0.2.1/tint/metrics/white_box/auprc.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/aur.py` & `time_interpret-0.2.1/tint/metrics/white_box/aur.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/base.py` & `time_interpret-0.2.1/tint/metrics/white_box/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from captum.log import log_usage
 from captum._utils.common import (
     _is_tuple,
-    _format_input,
+    _format_inputs,
     _format_output,
     _validate_input,
 )
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
 
 from typing import Callable, Tuple
 
@@ -18,16 +18,16 @@
     attributions: TensorOrTupleOfTensorsGeneric,
     true_attributions: TensorOrTupleOfTensorsGeneric,
     normalize: bool = True,
     hard_labels: bool = True,
 ) -> Tuple[float]:
     # Convert attributions into tuple
     is_inputs_tuple = _is_tuple(attributions)
-    attributions = _format_input(attributions)
-    true_attributions = _format_input(true_attributions)
+    attributions = _format_inputs(attributions)
+    true_attributions = _format_inputs(true_attributions)
 
     # Validate input
     _validate_input(attributions, true_attributions)
 
     # Normalise attributions
     if normalize:
         min_tpl = tuple(
```

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/entropy.py` & `time_interpret-0.2.1/tint/metrics/white_box/entropy.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/information.py` & `time_interpret-0.2.1/tint/metrics/white_box/information.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/mae.py` & `time_interpret-0.2.1/tint/metrics/white_box/mae.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/mse.py` & `time_interpret-0.2.1/tint/metrics/white_box/mse.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/rmse.py` & `time_interpret-0.2.1/tint/metrics/white_box/rmse.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/metrics/white_box/roc_auc.py` & `time_interpret-0.2.1/tint/metrics/white_box/roc_auc.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/models/bert.py` & `time_interpret-0.2.1/tint/models/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,24 +44,24 @@
     Examples:
         >>> from tint.models import Bert
          <BLANKLINE>
          >>> tokenizer, model = Bert("bert-base-uncased")
     """
     assert BertConfig is not None, "transformers is not installed."
 
-    # Load pretrained model if path provided
+    # Return untrained bert model if path not provided
     if pretrained_model_name_or_path is None:
         assert config is not None, "Bert config must be provided."
         assert vocab_file is not None, "vocab file must be provided."
         return (
             BertTokenizer(vocab_file, **kwargs),
             BertForSequenceClassification(config=config),
         )
 
-    # Otherwise return untrained bert model
+    # Otherwise load pretrained model
     return (
         BertTokenizer.from_pretrained(
             pretrained_model_name_or_path,
             cache_dir=cache_dir,
         ),
         BertForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path,
```

### Comparing `time_interpret-0.2.0/tint/models/cnn.py` & `time_interpret-0.2.1/tint/models/cnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "elu": nn.ELU(),
     "leaky_relu": nn.LeakyReLU(),
     "log_softmax": nn.LogSoftmax(dim=-1),
     "relu": nn.ReLU(),
     "relu6": nn.ReLU6(),
     "sigmoid": nn.Sigmoid(),
     "softmax": nn.Softmax(dim=-1),
-    "softplus": nn.Softplus(),
+    "softplus": nn.Softplus(beta=5),
     "softsign": nn.Softsign(),
     "tanh": nn.Tanh(),
     "tanhshrink": nn.Tanhshrink(),
 }
 
 
 POOLS = {
```

### Comparing `time_interpret-0.2.0/tint/models/distilbert.py` & `time_interpret-0.2.1/tint/models/distilbert.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,29 +40,29 @@
             DistilBert model for sentence classification.
 
     References:
         https://huggingface.co/docs/transformers/main/en/model_doc/distilbert
 
     Examples:
         >>> from tint.models import DistilBert
-         <BLANKLINE>
-         >>> tokenizer, model = DistilBert("distilbert-base-uncased")
+        <BLANKLINE>
+        >>> tokenizer, model = DistilBert("distilbert-base-uncased")
     """
     assert DistilBertConfig is not None, "transformers is not installed."
 
-    # Load pretrained model if path provided
+    # Return untrained bert model if path not provided
     if pretrained_model_name_or_path is None:
         assert config is not None, "DistilBert config must be provided."
         assert vocab_file is not None, "vocab file must be provided."
         return (
             DistilBertTokenizer(vocab_file, **kwargs),
             DistilBertForSequenceClassification(config=config),
         )
 
-    # Otherwise return untrained distilbert model
+    # Otherwise load pretrained model
     return (
         DistilBertTokenizer.from_pretrained(
             pretrained_model_name_or_path,
             cache_dir=cache_dir,
         ),
         DistilBertForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path,
```

### Comparing `time_interpret-0.2.0/tint/models/mlp.py` & `time_interpret-0.2.1/tint/models/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "elu": nn.ELU(),
     "leaky_relu": nn.LeakyReLU(),
     "log_softmax": nn.LogSoftmax(dim=-1),
     "relu": nn.ReLU(),
     "relu6": nn.ReLU6(),
     "sigmoid": nn.Sigmoid(),
     "softmax": nn.Softmax(dim=-1),
-    "softplus": nn.Softplus(),
+    "softplus": nn.Softplus(beta=5),
     "softsign": nn.Softsign(),
     "tanh": nn.Tanh(),
     "tanhshrink": nn.Tanhshrink(),
 }
 
 
 class MLP(nn.Module):
```

### Comparing `time_interpret-0.2.0/tint/models/net.py` & `time_interpret-0.2.1/tint/models/net.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     def forward(self, x: th.Tensor) -> th.Tensor:
         return self.net(x)
 
     def loss(self, inputs, target):
         inputs = inputs.reshape(-1, inputs.shape[-1])
         target = target.reshape(-1, target.shape[-1])
 
-        if isinstance(self._loss, nn.CrossEntropyLoss):
+        if isinstance(self._loss, (nn.CrossEntropyLoss, nn.NLLLoss)):
             if self._soft_labels:
                 target = target.softmax(-1)
             else:
                 if inputs.shape == target.shape:
                     target = target.argmax(-1)
                 target = target.reshape(-1).long()
```

### Comparing `time_interpret-0.2.0/tint/models/rnn.py` & `time_interpret-0.2.1/tint/models/rnn.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/models/roberta.py` & `time_interpret-0.2.1/tint/models/roberta.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,24 @@
     Examples:
         >>> from tint.models import Roberta
          <BLANKLINE>
          >>> tokenizer, model = Roberta("roberta-base")
     """
     assert RobertaConfig is not None, "transformers is not installed."
 
-    # Load pretrained model if path provided
+    # Return untrained bert model if path not provided
     if pretrained_model_name_or_path is None:
         assert config is not None, "Roberta config must be provided."
         assert vocab_file is not None, "vocab file must be provided."
         return (
             RobertaTokenizer(vocab_file, **kwargs),
             RobertaForSequenceClassification(config=config),
         )
 
-    # Otherwise return untrained roberta model
+    # Otherwise load pretrained model
     return (
         RobertaTokenizer.from_pretrained(
             pretrained_model_name_or_path,
             cache_dir=cache_dir,
         ),
         RobertaForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path,
```

### Comparing `time_interpret-0.2.0/tint/models/transformer.py` & `time_interpret-0.2.1/tint/models/transformer.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/utils/__init__.py` & `time_interpret-0.2.1/tint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/utils/a_star_path.py` & `time_interpret-0.2.1/tint/utils/a_star_path.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/utils/baching.py` & `time_interpret-0.2.1/tint/utils/baching.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+import copy
 import torch as th
 
+from captum._utils.common import (
+    _expand_and_update_additional_forward_args,
+    _expand_and_update_target,
+)
+
 from torch import Tensor
-from typing import Callable, Tuple
+from typing import Tuple
 
 from .tqdm import get_progress_bars
 
 
 def _geodesic_batch_attribution(
     attr_method,
     inputs: Tuple[Tensor, ...],
@@ -30,23 +36,37 @@
     if show_progress:
         steps = get_progress_bars()(
             steps,
             desc=f"Geodesic Integrated Gradients attribution",
         )
 
     for i in steps:
+        # Get partial inputs and baselines
         partial_knns = tuple(knn[i : i + internal_batch_size] for knn in knns)
         partial_idx = tuple(id[i : i + internal_batch_size] for id in idx)
 
+        # Expand and update additional args
+        n_samples = len(partial_knns[0])
+        kwargs_copy = copy.deepcopy(kwargs)
+        _expand_and_update_additional_forward_args(
+            n_samples=n_samples, kwargs=kwargs_copy
+        )
+        _expand_and_update_target(
+            n_samples=n_samples,
+            kwargs=kwargs_copy,
+        )
+
+        # Compute gradients
         partial_grads_norm, partial_grads = attr_method._attribute(
             inputs=tuple(x[knn] for x, knn in zip(inputs, partial_knns)),
             baselines=tuple(x[id] for x, id in zip(inputs, partial_idx)),
-            **kwargs,
+            **kwargs_copy,
         )
 
+        # Save and stack outputs
         if grads_norm is None:
             grads_norm = partial_grads_norm
             total_grads = partial_grads
         else:
             grads_norm = tuple(
                 th.cat([x, y], dim=0)
                 for x, y in zip(grads_norm, partial_grads_norm)
```

### Comparing `time_interpret-0.2.0/tint/utils/collate.py` & `time_interpret-0.2.1/tint/utils/collate.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/utils/common.py` & `time_interpret-0.2.1/tint/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import numpy as np
 import torch
 
 from captum._utils.common import (
     _expand_additional_forward_args,
     _format_baseline,
-    _format_input,
+    _format_inputs,
     _format_output,
     _format_additional_forward_args,
     _run_forward,
 )
 from captum._utils.typing import (
     BaselineType,
     TensorOrTupleOfTensorsGeneric,
@@ -23,15 +23,15 @@
     inputs: Tensor,
     target: Tensor = None,
     additional_forward_args: Any = None,
     temporal_target: bool = False,
     temporal_additional_forward_args: Tuple[bool] = None,
 ):
     # Format input data
-    inputs = _format_input(inputs)
+    inputs = _format_inputs(inputs)
     additional_forward_args = _format_additional_forward_args(
         additional_forward_args
     )
 
     # Inputs is only of length one
     data = inputs[0]
 
@@ -85,23 +85,23 @@
         "multiclass",
         "regression",
     ], "task is not recognised."
     assert 0 <= threshold <= 1, "threshold must be between 0 and 1"
 
     # Format inputs
     is_inputs_tuple = isinstance(inputs, tuple)
-    inputs = _format_input(inputs)
+    inputs = _format_inputs(inputs)
 
     # Slice inputs
     partial_inputs = tuple(x[:, :time, ...].clone() for x in inputs)
 
     # Format and slice args
     args_copy = copy.deepcopy(args)
     is_args_tuple = tuple(isinstance(arg, tuple) for arg in args_copy)
-    args_copy = tuple(_format_input(arg) for arg in args_copy)
+    args_copy = tuple(_format_inputs(arg) for arg in args_copy)
     args_copy = tuple(
         tuple(x[:, :time, ...] for x in arg) for arg in args_copy
     )
 
     kwargs_copy = copy.deepcopy(kwargs)
 
     # Format and slice baselines
@@ -137,15 +137,14 @@
                 temporal_additional_forward_args,
             )
         )
 
     # If forward_func is provided, compute partial predictions
     # according to task
     if forward_func is not None and task != "none":
-
         # Get additional args
         additional_forward_args = None
         if "additional_forward_args" in kwargs_copy:
             additional_forward_args = kwargs_copy["additional_forward_args"]
 
         with torch.autograd.set_grad_enabled(False):
             # Get model outputs
```

### Comparing `time_interpret-0.2.0/tint/utils/perturb_func.py` & `time_interpret-0.2.1/tint/utils/perturb_func.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/tint/utils/tensor_dataset.py` & `time_interpret-0.2.1/tint/utils/tensor_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch import Tensor
-from torch.utils.data import Dataset, default_collate
+from torch.utils.data import Dataset
 from typing import Tuple
 
 
 class TensorDataset(Dataset[Tuple[Tensor, ...]]):
     r"""
     Dataset wrapping tensors.
```

### Comparing `time_interpret-0.2.0/tint/utils/tqdm.py` & `time_interpret-0.2.1/tint/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `time_interpret-0.2.0/PKG-INFO` & `time_interpret-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_interpret
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model interpretability library for PyTorch with a focus on time series.
 Keywords: deep-learning,pytorch,captum,explainable-ai,time-series
 Author-email: Joseph Enguehard <joseph@skippr.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -79,15 +79,25 @@
 
 Time Interpret can be installed with pip:
 
 ```shell script
 pip install time_interpret
 ```
 
-or from source with conda:
+or from source:
+
+with pip:
+
+```shell script
+git clone git@github.com:babylonhealth/time_interpret.git
+cd time_interpret
+pip install -e .
+```
+
+or conda:
 
 ```shell script
 git clone git@github.com:babylonhealth/time_interpret.git
 cd time_interpret
 conda env create
 source activate tint
 pip install --no-deps -e .
@@ -105,29 +115,29 @@
 arma.download()  # This method generates the dataset
 ```
 
 We then load some test data from the dataset and the
 corresponding true saliency:
 
 ```python
-x = arma.preprocess()["x"][0]
-true_saliency = arma.true_saliency(dim=rare_dim)[0]
+inputs = arma.preprocess()["x"][0]
+true_saliency = arma.true_saliency(dim=1)[0]
 ```
 
 We can now load an attribution method and use it to compute the saliency:
 
 ```python
 from tint.attr import TemporalIntegratedGradients
 
 explainer = TemporalIntegratedGradients(arma.get_white_box)
 
-baseline = inputs * 0
+baselines = inputs * 0
 attr = explainer.attribute(
     inputs,
-    baselines=inputs * 0,
+    baselines=baselines,
     additional_forward_args=(true_saliency,),
     temporal_additional_forward_args=(True,),
 ).abs()
 ```
 
 Finally, we evaluate our method using the true saliency and a white box metric:
 
@@ -141,17 +151,17 @@
 
 - [AugmentedOcclusion](https://arxiv.org/abs/2003.02821)
 - [BayesLime](https://arxiv.org/pdf/2008.05030)
 - [BayesShap](https://arxiv.org/pdf/2008.05030)
 - [DynaMask](https://arxiv.org/pdf/2106.05303)
 - [Discretised Integrated Gradients](https://arxiv.org/abs/2108.13654)
 - [Fit](https://arxiv.org/abs/2003.02821)
+- [Non-linearities Tunnel](https://arxiv.org/abs/1906.07983)
 - [Occlusion](https://arxiv.org/abs/1311.2901)
 - [Retain](https://arxiv.org/pdf/1608.05745)
-- [SmoothGrad](https://arxiv.org/abs/1810.03292)
 
 
 ## Acknowledgment
 - [Jonathan Crabbe](https://github.com/JonathanCrabbe/Dynamask) for the DynaMask implementation.
 - [Sana Tonekaboni](https://github.com/sanatonek/time_series_explainability/tree/master/TSX) for the fit implementation.
 - [INK Lab](https://github.com/INK-USC/DIG) for the discretized integrated gradients implementation.
 - [Dylan Slack](https://github.com/dylan-slack/Modeling-Uncertainty-Local-Explainability) for the BayesLime and BayesShap implementations.
```

