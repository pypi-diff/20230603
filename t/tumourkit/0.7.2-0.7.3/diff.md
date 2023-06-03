# Comparing `tmp/tumourkit-0.7.2.tar.gz` & `tmp/tumourkit-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.7.2.tar", last modified: Fri Jun  2 09:26:12 2023, max compression
+gzip compressed data, was "tumourkit-0.7.3.tar", last modified: Sat Jun  3 14:18:58 2023, max compression
```

## Comparing `tumourkit-0.7.2.tar` & `tumourkit-0.7.3.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.492331 tumourkit-0.7.2/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.2/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-02 09:26:12.491775 tumourkit-0.7.2/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1580 2023-05-30 20:14:30.000000 tumourkit-0.7.2/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.387445 tumourkit-0.7.2/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.387197 tumourkit-0.7.2/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.402289 tumourkit-0.7.2/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.402977 tumourkit-0.7.2/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.2/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.2/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.2/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-02 09:26:12.492478 tumourkit-0.7.2/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.422828 tumourkit-0.7.2/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.2/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.2/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.2/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.2/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.2/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.2/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.2/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.2/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.2/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.2/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.2/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.2/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.2/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.2/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.2/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.2/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.2/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.2/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.2/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.2/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.429090 tumourkit-0.7.2/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-06-02 09:25:23.000000 tumourkit-0.7.2/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.438178 tumourkit-0.7.2/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.2/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.2/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.2/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.2/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.441079 tumourkit-0.7.2/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.2/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.2/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.2/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.2/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.2/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.2/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.2/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.2/tumourkit/classification/train_xgboost.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.441749 tumourkit-0.7.2/tumourkit/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.2/tumourkit/demo/app.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    11480 2023-06-02 09:23:43.000000 tumourkit-0.7.2/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-31 20:15:09.000000 tumourkit-0.7.2/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.2/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.448458 tumourkit-0.7.2/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.2/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.2/tumourkit/postprocessing/draw_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.2/tumourkit/postprocessing/draw_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-05-30 18:20:42.000000 tumourkit-0.7.2/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-05-30 18:21:29.000000 tumourkit-0.7.2/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.2/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.2/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.458030 tumourkit-0.7.2/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.2/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.2/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.2/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.2/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.2/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.2/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.2/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.2/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.2/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.459493 tumourkit-0.7.2/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.2/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.2/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.2/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.461249 tumourkit-0.7.2/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.2/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-05-30 18:17:43.000000 tumourkit-0.7.2/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.464259 tumourkit-0.7.2/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.466417 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.469031 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.470274 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.473347 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.473935 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.479717 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.481348 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.483987 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.2/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.490841 tumourkit-0.7.2/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.2/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.2/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.2/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.2/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.2/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.2/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.2/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.2/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.2/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.432666 tumourkit-0.7.2/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.989195 tumourkit-0.7.3/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.3/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-03 14:18:58.988704 tumourkit-0.7.3/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1580 2023-05-30 20:14:30.000000 tumourkit-0.7.3/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.856442 tumourkit-0.7.3/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.856222 tumourkit-0.7.3/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.869508 tumourkit-0.7.3/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.870110 tumourkit-0.7.3/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.3/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.3/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.3/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-03 14:18:58.989306 tumourkit-0.7.3/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.888004 tumourkit-0.7.3/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.3/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.3/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.3/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.3/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.3/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.3/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.3/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.3/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.3/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.3/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.3/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.3/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.3/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.3/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.3/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.3/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.3/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.3/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.3/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.3/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.892680 tumourkit-0.7.3/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-06-03 14:17:01.000000 tumourkit-0.7.3/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.902812 tumourkit-0.7.3/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.3/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.3/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.3/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.3/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.907183 tumourkit-0.7.3/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.3/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.3/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.3/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.3/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.3/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.3/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.3/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.3/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.909784 tumourkit-0.7.3/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.3/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14850 2023-06-03 14:07:59.000000 tumourkit-0.7.3/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-31 20:15:09.000000 tumourkit-0.7.3/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.3/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.915939 tumourkit-0.7.3/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.3/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.3/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.3/tumourkit/postprocessing/draw_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-06-03 11:50:00.000000 tumourkit-0.7.3/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-06-03 11:32:58.000000 tumourkit-0.7.3/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.3/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.3/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.925371 tumourkit-0.7.3/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.3/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.3/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.3/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.3/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.3/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.3/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.3/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.3/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.3/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.927018 tumourkit-0.7.3/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.3/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.3/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.3/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.928457 tumourkit-0.7.3/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.3/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-06-03 11:40:22.000000 tumourkit-0.7.3/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.932433 tumourkit-0.7.3/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.936252 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.940284 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.942255 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.946473 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.947607 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.959518 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.964703 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.974884 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.3/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.986264 tumourkit-0.7.3/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.3/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.3/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.3/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.3/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.3/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.3/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.3/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.3/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.3/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.896312 tumourkit-0.7.3/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       42 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.7.2/LICENSE` & `tumourkit-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/PKG-INFO` & `tumourkit-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.2
+Version: 0.7.3
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.2/README.md` & `tumourkit-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2html.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2man.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.7.3/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.7.3/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/docs/source/conf.py` & `tumourkit-0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/pyproject.toml` & `tumourkit-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/requirements.txt` & `tumourkit-0.7.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/centroidspng2csv_test.py` & `tumourkit-0.7.3/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/conf_matrix_sum_test.py` & `tumourkit-0.7.3/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/cpairs_test.py` & `tumourkit-0.7.3/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/example_test.py` & `tumourkit-0.7.3/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/generate_centroids.py` & `tumourkit-0.7.3/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/generate_rswoosh.py` & `tumourkit-0.7.3/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/get_conn_comp_test.py` & `tumourkit-0.7.3/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/graph2centroids_test.py` & `tumourkit-0.7.3/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/graph_idx_test.py` & `tumourkit-0.7.3/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/hov_prob_pipe_test.py` & `tumourkit-0.7.3/tests/hov_prob_pipe_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/hov_prob_test.py` & `tumourkit-0.7.3/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/hovernet_patches_test.py` & `tumourkit-0.7.3/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/metrics_pairs_test.py` & `tumourkit-0.7.3/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/metrics_test.py` & `tumourkit-0.7.3/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/png2graph_test.py` & `tumourkit-0.7.3/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/pngcsv2geojson_test.py` & `tumourkit-0.7.3/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/pngcsv2graph_test.py` & `tumourkit-0.7.3/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/read_nodes_test.py` & `tumourkit-0.7.3/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/remove_idx_test.py` & `tumourkit-0.7.3/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tests/rswoosh_test.py` & `tumourkit-0.7.3/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.7.3/tumourkit/classification/compute_imbalance.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/evaluate.py` & `tumourkit-0.7.3/tumourkit/classification/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/infer.py` & `tumourkit-0.7.3/tumourkit/classification/infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/models/gat.py` & `tumourkit-0.7.3/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/models/gcn.py` & `tumourkit-0.7.3/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/models/hgao.py` & `tumourkit-0.7.3/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/models/norm.py` & `tumourkit-0.7.3/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/read_graph.py` & `tumourkit-0.7.3/tumourkit/classification/read_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/train_graphs.py` & `tumourkit-0.7.3/tumourkit/classification/train_graphs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/classification/train_xgboost.py` & `tumourkit-0.7.3/tumourkit/classification/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/demo/app.py` & `tumourkit-0.7.3/tumourkit/demo/app.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/eval_pipe.py` & `tumourkit-0.7.3/tumourkit/eval_pipe.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import logging
 from logging import Logger
 import numpy as np
 import pandas as pd
 from . import eval_segment
 import os
 import shutil
-from .postprocessing import join_hovprob_graph_main
+from .postprocessing import join_hovprob_graph_main, join_graph_gt_main
 from .preprocessing import hovernet2centroids_main, geojson2pngcsv_main, pngcsv2centroids_main, graph2centroids_main
 from .utils.preprocessing import get_names
 from .utils.pipes import HovernetNotFoundError, check_void
 from .utils.classification import metrics_from_predictions
 from .classification import infer_gnn
 from .infer_pipe import set_best_configuration
 
@@ -47,19 +47,20 @@
     :type logger: Logger
 
     :raises HovernetNotFoundError: If the Hovernet centroids are not found in the training output.
     """
     logger.info('Extracting Hovernet centroids from training output.')
     if not os.path.isdir(os.path.join(args.root_dir, 'data', 'tmp_hov', 'json')):
         raise HovernetNotFoundError('Please, train again or extract hovernet outputs.')
-    newargs = Namespace(
-        json_dir=os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
-        output_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
-    )
-    hovernet2centroids_main(newargs)
+    if check_void(os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov')):
+        newargs = Namespace(
+            json_dir=os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
+            output_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
+        )
+        hovernet2centroids_main(newargs)
     for split in ['train', 'validation', 'test']:
         if check_void(os.path.join(args.root_dir, 'data', split, 'names.txt')):
             logger.info(f'Preprocessing split {split}.')
             split_names = get_names(os.path.join(args.root_dir, 'data', split, 'gson'), '.geojson')
             with open(os.path.join(args.root_dir, 'data', split, 'names.txt'), 'w') as f:
                 for name in split_names:
                     print(name, file=f)
@@ -77,16 +78,17 @@
             newargs = Namespace(
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
             )
             pngcsv2centroids_main(newargs)
 
-    args.best_arch = 'GCN'
-    set_best_configuration(args, logger)
+    if args.best_arch is None:
+        args.best_arch = 'GCN'
+        set_best_configuration(args, logger)
     # Perform inference steps from infer_pipe
     if check_void(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds')):
         logger.info('Starting graph inference.')
         os.makedirs(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds'), exist_ok=True)
         os.makedirs(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'raw'), exist_ok=True)
         os.makedirs(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'), exist_ok=True)
         for split in ['train', 'validation', 'test']: # Move raw morphological features
@@ -105,52 +107,63 @@
         join_hovprob_graph_main(newargs, logger)
         for file in os.listdir(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds')):
             df = pd.read_csv(os.path.join(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'), file))
             assert (df['class'].to_numpy() == ((df['prob1'].to_numpy() > 0.5) * 1 + 1)).all(), f"Probs and prediction of Hovernet don't coincide. {file}"
             df.drop('class', axis=1).to_csv(os.path.join(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'), file), index=False)
         model_name = 'best_' + args.best_arch + '_' + args.best_num_layers + '_' \
             + args.best_dropout + '_' + args.best_norm_type
+        if args.gnn_dir is None:
+            args.gnn_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn')
         newargs = Namespace(
             node_dir=os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'),
             output_dir=os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds'),
-            weights=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
-            conf=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'confs', model_name + '.json'),
-            normalizers=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'normalizers', model_name + '.pkl'),
+            weights=os.path.join(args.gnn_dir, 'weights', model_name + '.pth'),
+            conf=os.path.join(args.gnn_dir, 'confs', model_name + '.json'),
+            normalizers=os.path.join(args.gnn_dir, 'normalizers', model_name + '.pkl'),
             num_classes=args.num_classes,
-            disable_prior=False,
-            disable_morph_feats=False,
+            disable_prior=args.disable_prior,
+            disable_morph_feats=args.disable_morph,
         )
         infer_gnn(newargs)
     # Postproc to obtain centroids
     if check_void(os.path.join(args.root_dir, 'tmp_graphs', 'centroids')):
         logger.info('Parsing gnn output.')
         logger.info('   Converting .nodes.csv to .centroids.csv.')
         newargs = Namespace(
             graph_dir=os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds'),
             centroids_dir=os.path.join(args.root_dir, 'tmp_graphs', 'centroids'),
             num_classes=args.num_classes,
         )
         graph2centroids_main(newargs)
+
+    logger.info('Creating folders.')
+    os.makedirs(os.path.join(args.save_dir, 'conf-matrices', 'gnn_individual'), exist_ok=True)
+    os.makedirs(os.path.join(args.save_dir, 'conf-matrices', 'hov_individual'), exist_ok=True)
+    for split in ['train', 'validation', 'test']:
+        os.makedirs(os.path.join(args.save_dir, split), exist_ok=True)
     return
 
 
-def compute_ece(args: Namespace, split: str) -> None:
+def compute_ece(args: Namespace, split: str, is_hov: bool) -> None:
     """
     Computes Expected Calibration Error (ECE) and other metrics for the given split.
 
     :param args: The arguments for computing ECE and metrics.
     :type args: Namespace
 
-    :param logger: The logger object used for logging messages.
-    :type logger: Logger
-
     :param split: The name of the split (e.g., 'train', 'validation', 'test').
     :type split: str
+
+    :param is_hov: Whether we are computing for hovernet or gnns. The directories have different structure, so we need to know.
+    :type is_hov: bool
     """
-    folder = os.path.join(args.root_dir, 'data', split, 'graphs', 'preds')
+    if is_hov:
+        folder = os.path.join(args.root_dir, 'data', split, 'graphs', 'preds')
+    else:
+        folder = os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds_gt', split)
     trues, probs = None, None
     for file in os.listdir(folder):
         df = pd.read_csv(os.path.join(folder, file))
         _trues = df['class'].to_numpy() - 1
         if trues is None:
             trues = _trues.reshape((-1, 1))
         else:
@@ -161,28 +174,30 @@
         else:
             cols = ['prob' + str(k) for k in range(1, args.num_classes + 1)]
             _probs = df[cols].to_numpy()
         if probs is None:
             probs = _probs
         else:
             probs = np.vstack((probs, _probs))
+        if pd.isna(trues).any():
+            print(file)
     preds = np.argmax(probs, axis=1).reshape((-1, 1))
     metrics = metrics_from_predictions(trues, preds, probs[:, 1], args.num_classes)
     if args.num_classes == 2:
         acc, f1, auc, perc_error, ece = metrics
         dic_metrics = {
             'F1': [f1], 'Accuracy': [acc], 'ROC_AUC': [auc], 'Perc_err': [perc_error], 'ECE': [ece]
         }
     else:
         micro, macro, weighted, ece = metrics
         dic_metrics = {
             'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro], 'ECE': [ece]
         }
     metrics_df = pd.DataFrame(dic_metrics)
-    metrics_df.to_csv(args.save_name + '_' + split + '_ece.csv', index=False)
+    metrics_df.to_csv(os.path.join(args.save_dir, split, ('hov' if is_hov else 'gnn') + '_ece.csv'), index=False)
 
 
 def run_evaluation(args: Namespace, logger: Logger) -> None:
     """
     Runs the evaluation of Hovernet output for different splits.
 
     :param args: The arguments for the evaluation.
@@ -194,42 +209,71 @@
     logger.info('Starting evaluation of Hovernet output.')
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
             pred_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
-            save_name=args.save_name + '_' + split,
-            debug_path=args.save_name + '_debug_hov' if args.debug else None,
+            save_name=os.path.join(args.save_dir, split, 'hov'),
+            debug_path=os.path.join(args.save_dir, 'conf-matrices', 'hov_individual', 'debug_hov') if args.debug else None,
             num_classes=args.num_classes
         )
         eval_segment(newargs, logger)
-        compute_ece(args, split)
+        compute_ece(args, split, is_hov=True)
+        if args.debug:
+            shutil.move(
+                os.path.join(args.save_dir, 'conf-matrices', 'hov_individual', 'debug_hov_global.csv'),
+                os.path.join(args.save_dir, 'conf-matrices', 'debug_hov_global_' + split + '.csv'))
     # Evaluate graph output same as hov output
     logger.info('Starting evaluation of Hovernet output.')
     for split in ['train', 'validation', 'test']:
-        logger.info(f'    Evaluating {split} split')
+        logger.info(f'    Evaluating {split} split (with background)')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
             pred_path=os.path.join(args.root_dir, 'tmp_graphs', 'centroids'),
-            save_name=args.save_name + '_' + split + '_gnn',
-            debug_path=args.save_name + '_debug_gnn' if args.debug else None,
+            save_name=os.path.join(args.save_dir, split, 'gnn'),
+            debug_path=os.path.join(args.save_dir, 'conf-matrices', 'gnn_individual', 'debug_gnn') if args.debug else None,
             num_classes=args.num_classes
         )
         eval_segment(newargs, logger)
+        if args.debug:
+            shutil.move(
+                os.path.join(args.save_dir, 'conf-matrices', 'gnn_individual', 'debug_gnn_global.csv'),
+                os.path.join(args.save_dir, 'conf-matrices', 'debug_gnn_global_' + split + '.csv'))
+    for split in ['train', 'validation', 'test']:
+        os.makedirs(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds_gt', split), exist_ok=True)
+        for file in get_names(os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'), '.nodes.csv'):
+            df_gt = pd.read_csv(os.path.join(args.root_dir, 'data', split, 'graphs', 'preds', file + '.nodes.csv'))
+            df = pd.read_csv(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds', file + '.nodes.csv'))
+            # import pdb;pdb.set_trace()
+            df = df[df.id.isin(df_gt.id)]
+            df = df.set_index(df.id)
+            df_gt = df_gt.set_index(df_gt.id)
+            df['class'] = df_gt['class']
+            assert not df['class'].isna().any()
+            df.to_csv(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds_gt', split, file + '.nodes.csv'), index=False)
+        compute_ece(args, split, is_hov=False)
+    shutil.rmtree(os.path.join(args.root_dir, 'tmp_graphs'))
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--root-dir', type=str, default='./.internals/', help='Root folder to save data and models.')
-    parser.add_argument('--save-name', type=str, required=True, help='Name to save the result, without file type.')
+    parser.add_argument('--save-dir', type=str, required=True, help='Folder to save the results, without file type.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
-    parser.add_argument('--debug', actions='store_true', help='Whether to save confusion matrices.')
+    parser.add_argument('--best-num-layers', type=str, help='Optimal number of layers when training GNNs.')
+    parser.add_argument('--best-dropout', type=str, help='Optimal dropout rate when training GNNs')
+    parser.add_argument('--best-norm-type', type=str, help='Optimal type of normalization layers when training GNNs')
+    parser.add_argument('--best-arch', type=str, help='Best architecture (convolutional, attention, ...) when training GNNs', choices=['GCN', 'ATT'])
+    parser.add_argument('--debug', action='store_true', help='Whether to save confusion matrices.')
+    parser.add_argument('--gnn-dir', type=str, help='Path where the gnn is saved, otherwise the default in root-dir will be used. It must have three folder inside: confs, weights and normalizers.')
+    parser.add_argument('--disable-prior', action='store_true', help='Whether to disable the use of Hovernet probabilities.')
+    parser.add_argument('--disable-morph', action='store_true', help='Whether to disable the use of morphological properties.')
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.7.2/tumourkit/infer_pipe.py` & `tumourkit-0.7.3/tumourkit/infer_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/make_dirs.py` & `tumourkit-0.7.3/tumourkit/make_dirs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/draw_cells.py` & `tumourkit-0.7.3/tumourkit/postprocessing/draw_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/draw_graph.py` & `tumourkit-0.7.3/tumourkit/postprocessing/draw_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.7.3/tumourkit/postprocessing/join_graph_gt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.7.3/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.7.3/tumourkit/postprocessing/merge_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.7.3/tumourkit/postprocessing/rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/__init__.py` & `tumourkit-0.7.3/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.7.3/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.7.3/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.7.3/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.7.3/tumourkit/preprocessing/graph2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.7.3/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.7.3/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.7.3/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/preprocessing/remove_uncertain.py` & `tumourkit-0.7.3/tumourkit/preprocessing/remove_uncertain.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.7.3/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.7.3/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/research_pipe.py` & `tumourkit-0.7.3/tumourkit/research_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/evaluate.py` & `tumourkit-0.7.3/tumourkit/segmentation/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.7.3/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/train_pipe.py` & `tumourkit-0.7.3/tumourkit/train_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/calibration_error.py` & `tumourkit-0.7.3/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/classification.py` & `tumourkit-0.7.3/tumourkit/utils/classification.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/folder2txt.py` & `tumourkit-0.7.3/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/nearest.py` & `tumourkit-0.7.3/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/pipes.py` & `tumourkit-0.7.3/tumourkit/utils/pipes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/postprocessing.py` & `tumourkit-0.7.3/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/preprocessing.py` & `tumourkit-0.7.3/tumourkit/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit/utils/read_nodes.py` & `tumourkit-0.7.3/tumourkit/utils/read_nodes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.7.3/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.2
+Version: 0.7.3
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.2/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.7.3/tumourkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.7.3/tumourkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.2/tumourkit.egg-info/requires.txt` & `tumourkit-0.7.3/tumourkit.egg-info/requires.txt`

 * *Files identical despite different names*

