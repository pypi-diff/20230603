# Comparing `tmp/DAJIN2-0.1.8.tar.gz` & `tmp/DAJIN2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.1.8.tar", last modified: Tue Oct 25 01:29:54 2022, max compression
+gzip compressed data, was "DAJIN2-0.1.9.tar", last modified: Tue Oct 25 02:24:53 2022, max compression
```

## Comparing `DAJIN2-0.1.8.tar` & `DAJIN2-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.780000 DAJIN2-0.1.8/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1090 2021-11-02 03:02:14.000000 DAJIN2-0.1.8/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       51 2022-10-21 03:50:00.000000 DAJIN2-0.1.8/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 01:29:56.000000 DAJIN2-0.1.8/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      882 2022-10-22 00:26:32.000000 DAJIN2-0.1.8/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2022-10-25 01:29:56.000000 DAJIN2-0.1.8/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1078 2022-10-25 00:39:16.000000 DAJIN2-0.1.8/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.810000 DAJIN2-0.1.8/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.830000 DAJIN2-0.1.8/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4305 2022-10-20 03:39:06.000000 DAJIN2-0.1.8/src/DAJIN2/DAJIN2.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-06-01 03:40:28.000000 DAJIN2-0.1.8/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2440 2022-10-20 04:06:14.000000 DAJIN2-0.1.8/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.880000 DAJIN2-0.1.8/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-18 23:05:02.000000 DAJIN2-0.1.8/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.910000 DAJIN2-0.1.8/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       72 2022-10-14 23:47:26.000000 DAJIN2-0.1.8/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1291 2022-10-14 08:26:46.000000 DAJIN2-0.1.8/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2022-10-14 23:47:16.000000 DAJIN2-0.1.8/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.940000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       70 2022-10-15 20:47:06.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3282 2022-10-15 05:37:02.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/clustering_main.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3390 2022-10-09 04:32:38.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/make_scores.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1242 2022-10-25 01:23:36.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/mask_control.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1533 2022-10-09 03:39:40.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/return_labels.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5500 2022-10-15 05:37:42.000000 DAJIN2-0.1.8/src/DAJIN2/core/clustering/screen_diffloci.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.960000 DAJIN2-0.1.8/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       33 2022-10-15 01:49:44.000000 DAJIN2-0.1.8/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6882 2022-10-15 21:01:44.000000 DAJIN2-0.1.8/src/DAJIN2/core/consensus/consensus_main.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6870 2022-10-24 08:13:24.000000 DAJIN2-0.1.8/src/DAJIN2/core/core.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.990000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      106 2022-10-15 20:45:00.000000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      432 2022-10-07 03:32:56.000000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/calc_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4546 2022-10-24 08:12:10.000000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/check_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4141 2022-10-20 03:27:22.000000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3435 2022-10-25 00:21:36.000000 DAJIN2-0.1.8/src/DAJIN2/core/preprocess/mappy_align.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:54.020000 DAJIN2-0.1.8/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       52 2022-10-05 02:14:58.000000 DAJIN2-0.1.8/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11038 2022-10-21 06:50:06.000000 DAJIN2-0.1.8/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1154 2022-10-05 02:03:22.000000 DAJIN2-0.1.8/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2427 2022-10-21 04:05:16.000000 DAJIN2-0.1.8/src/DAJIN2/gui.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:54.040000 DAJIN2-0.1.8/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-20 07:45:58.000000 DAJIN2-0.1.8/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2254 2022-10-20 03:51:18.000000 DAJIN2-0.1.8/src/DAJIN2/postprocess/report.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      208 2022-10-20 04:06:30.000000 DAJIN2-0.1.8/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:54.070000 DAJIN2-0.1.8/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:54.100000 DAJIN2-0.1.8/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-07 04:06:40.000000 DAJIN2-0.1.8/src/DAJIN2/static/css/style.css
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:54.120000 DAJIN2-0.1.8/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1692 2022-10-07 07:26:20.000000 DAJIN2-0.1.8/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2582 2022-10-18 20:42:58.000000 DAJIN2-0.1.8/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 01:29:53.860000 DAJIN2-0.1.8/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1342 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      217 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2022-10-25 01:29:54.000000 DAJIN2-0.1.8/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.530000 DAJIN2-0.1.9/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1090 2021-11-02 03:02:14.000000 DAJIN2-0.1.9/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       51 2022-10-21 03:50:00.000000 DAJIN2-0.1.9/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      882 2022-10-22 00:26:32.000000 DAJIN2-0.1.9/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1078 2022-10-25 02:24:42.000000 DAJIN2-0.1.9/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.560000 DAJIN2-0.1.9/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.590000 DAJIN2-0.1.9/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4305 2022-10-20 03:39:06.000000 DAJIN2-0.1.9/src/DAJIN2/DAJIN2.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-06-01 03:40:28.000000 DAJIN2-0.1.9/src/DAJIN2/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2440 2022-10-20 04:06:14.000000 DAJIN2-0.1.9/src/DAJIN2/batch.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.640000 DAJIN2-0.1.9/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-18 23:05:02.000000 DAJIN2-0.1.9/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.670000 DAJIN2-0.1.9/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       72 2022-10-14 23:47:26.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1291 2022-10-14 08:26:46.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2022-10-14 23:47:16.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.700000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       70 2022-10-15 20:47:06.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3282 2022-10-25 02:14:38.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/clustering_main.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3390 2022-10-09 04:32:38.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/make_scores.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1242 2022-10-25 01:23:36.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/mask_control.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1533 2022-10-09 03:39:40.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/return_labels.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6564 2022-10-25 02:24:14.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/screen_diffloci.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.730000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       33 2022-10-15 01:49:44.000000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6882 2022-10-15 21:01:44.000000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/consensus_main.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6870 2022-10-24 08:13:24.000000 DAJIN2-0.1.9/src/DAJIN2/core/core.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.760000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      106 2022-10-15 20:45:00.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      432 2022-10-07 03:32:56.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/calc_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4546 2022-10-24 08:12:10.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/check_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4141 2022-10-20 03:27:22.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3435 2022-10-25 00:21:36.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/mappy_align.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.790000 DAJIN2-0.1.9/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       52 2022-10-05 02:14:58.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11038 2022-10-21 06:50:06.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1154 2022-10-05 02:03:22.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2427 2022-10-21 04:05:16.000000 DAJIN2-0.1.9/src/DAJIN2/gui.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.820000 DAJIN2-0.1.9/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-20 07:45:58.000000 DAJIN2-0.1.9/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2254 2022-10-20 03:51:18.000000 DAJIN2-0.1.9/src/DAJIN2/postprocess/report.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      208 2022-10-20 04:06:30.000000 DAJIN2-0.1.9/src/DAJIN2/single.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.850000 DAJIN2-0.1.9/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.870000 DAJIN2-0.1.9/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-07 04:06:40.000000 DAJIN2-0.1.9/src/DAJIN2/static/css/style.css
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.930000 DAJIN2-0.1.9/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1692 2022-10-07 07:26:20.000000 DAJIN2-0.1.9/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2582 2022-10-18 20:42:58.000000 DAJIN2-0.1.9/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.610000 DAJIN2-0.1.9/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1342 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      217 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.1.8/LICENSE` & `DAJIN2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/PKG-INFO` & `DAJIN2-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.1.8
+Version: 0.1.9
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.1.8/README.md` & `DAJIN2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/setup.py` & `DAJIN2-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.1.8",
+    version="0.1.9",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="One-step genotyping tools for Nanopore amplicon sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
```

### Comparing `DAJIN2-0.1.8/src/DAJIN2/DAJIN2.py` & `DAJIN2-0.1.9/src/DAJIN2/DAJIN2.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/batch.py` & `DAJIN2-0.1.9/src/DAJIN2/batch.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/classification/classify.py` & `DAJIN2-0.1.9/src/DAJIN2/core/classification/classify.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/clustering/clustering_main.py` & `DAJIN2-0.1.9/src/DAJIN2/core/clustering/clustering_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     dict_cssplit_control = defaultdict(list[dict])
     for allele in DICT_ALLELE.keys():
         path_control = Path(TEMPDIR, "midsv", f"{CONTROL_NAME}_{allele}.jsonl")
         cssplit_control = [cs["CSSPLIT"] for cs in midsv.read_jsonl(path_control)]
         dict_cssplit_control[allele] = cssplit_control
     classif_sample.sort(key=lambda x: (x["ALLELE"], x["SV"]))
     diffloci_by_alleles = defaultdict(list[dict])
-    for (ALLELE, SV), group in groupby(classif_sample, key=lambda x: (x["ALLELE"], x["SV"])):
+    for (allele, sv), group in groupby(classif_sample, key=lambda x: (x["ALLELE"], x["SV"])):
         cssplit_sample = [record["CSSPLIT"] for record in group]
-        cssplit_control = dict_cssplit_control[ALLELE]
-        sequence = DICT_ALLELE[ALLELE]
-        masks_control = MASKS_CONTROL[ALLELE]
+        cssplit_control = dict_cssplit_control[allele]
+        sequence = DICT_ALLELE[allele]
+        masks_control = MASKS_CONTROL[allele]
         diffloci = screen_different_loci(
             cssplit_sample, cssplit_control, sequence, masks_control, alpha=0.01, threshold=0.05
         )
-        diffloci_by_alleles[f"{ALLELE}-{SV}"] = diffloci
+        diffloci_by_alleles[f"{allele}-{sv}"] = diffloci
     return diffloci_by_alleles
 
 
 def add_labels(classif_sample, diffloci_by_alleles):
     labels = []
     label_start = 1
     classif_sample.sort(key=lambda x: (x["ALLELE"], x["SV"]))
-    for (ALLELE, SV), group in groupby(classif_sample, key=lambda x: (x["ALLELE"], x["SV"])):
-        key = f"{ALLELE}-{SV}"
+    for (allele, sv), group in groupby(classif_sample, key=lambda x: (x["ALLELE"], x["SV"])):
+        key = f"{allele}-{sv}"
         cssplit_sample = [g["CSSPLIT"] for g in group]
         diffloci = diffloci_by_alleles[key]
         scores = []
         if diffloci is not None:
             scores = make_scores(cssplit_sample, diffloci)
         if any(scores):
             labels += [label + label_start for label in return_labels(scores).tolist()]
```

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/clustering/make_scores.py` & `DAJIN2-0.1.9/src/DAJIN2/core/clustering/make_scores.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/clustering/mask_control.py` & `DAJIN2-0.1.9/src/DAJIN2/core/clustering/mask_control.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/clustering/return_labels.py` & `DAJIN2-0.1.9/src/DAJIN2/core/clustering/return_labels.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/clustering/screen_diffloci.py` & `DAJIN2-0.1.9/src/DAJIN2/core/clustering/screen_diffloci.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import re
+import numpy as np
 import scipy.stats as st
 
 
 def replaceNtoMatch(sample_cs: list[str]) -> list[str]:
     # Replace N to @ at the left ends
     for i, cs in enumerate(sample_cs):
         if cs != "N":
@@ -62,14 +63,20 @@
 def chistatistic(s_table, c_table, threshold=0.05) -> float:
     chisq_value, _, ddof, _ = st.chi2_contingency([s_table, c_table])
     delta = sum(s_table + c_table) * threshold ** 2
     pval = 1 - st.ncx2.cdf(chisq_value, ddof, delta)
     return pval
 
 
+def pearson_corr(x, y):
+    x_diff = x - np.mean(x)
+    y_diff = y - np.mean(y)
+    return np.dot(x_diff, y_diff) / (np.sqrt(sum(x_diff ** 2)) * np.sqrt(sum(y_diff ** 2)))
+
+
 def screen_different_loci(
     cssplit_sample: list[str],
     cssplit_control: list[str],
     sequence: str,
     masks_control: list[bool],
     alpha: float = 0.01,
     threshold: float = 0.05,
@@ -85,60 +92,74 @@
         list[dict]: Scores at significantly different base loci
     """
     different_loci = []
     coverage = min(len(cssplit_sample), len(cssplit_control))
     table_sample, table_control = make_table(cssplit_sample, cssplit_control)
     table_control = mask_table_control(table_control, masks_control)
     repeat_regrex = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
-    repeat_span = (x.span() for x in re.finditer(repeat_regrex, sequence))
-    try:
-        repeat_start, repeat_end = next(repeat_span)
-        repeat_end -= 1
-    except StopIteration:
+    repeat_span = list(x.span() for x in re.finditer(repeat_regrex, sequence))
+    repeat_idx = 0
+    if len(repeat_span) == 0:
         # Compare each nucleotide locus when sequence does not have a repeat
         for i, (s, c) in enumerate(zip(table_sample, table_control)):
             pval = chistatistic([coverage, sum(s)], [coverage, sum(c)], threshold)
             if pval < alpha:
                 different_loci.append(i)
         return different_loci
+    repeat_start, repeat_end = repeat_span[repeat_idx]
+    repeat_end -= 1
+    repeat_idx += 1
     # Sum of deletion and other mismatchs
-    repeat_del = [1, 1]
-    repeat_other = [1, 1]
+    repeat_sample_del = []
+    repeat_control_del = []
+    repeat_sample_others = []
+    repeat_control_others = []
     for i, (s, c) in enumerate(zip(table_sample, table_control)):
         if repeat_start <= i < repeat_end:
-            repeat_del[0] += s[0]
-            repeat_del[1] += c[0]
-            repeat_other[0] += s[1]
-            repeat_other[1] += c[1]
+            repeat_sample_del.append(s[0])
+            repeat_control_del.append(c[0])
+            repeat_sample_others.append(s[1])
+            repeat_control_others.append(c[1])
         elif i == repeat_end:
-            repeat_del[0] += s[0]
-            repeat_del[1] += c[0]
-            repeat_other[0] += s[1]
-            repeat_other[1] += c[1]
+            repeat_sample_del.append(s[0])
+            repeat_control_del.append(c[0])
+            repeat_sample_others.append(s[1])
+            repeat_control_others.append(c[1])
             # statistics to deletion
-            pval = chistatistic([coverage, repeat_del[0]], [coverage, repeat_del[1]], threshold)
-            if pval < pow(alpha, 3):
-                for j in range(repeat_start, repeat_end + 1):
-                    s, c = table_sample[j], table_control[j]
-                    pval = chistatistic([coverage, s[0]], [coverage, c[0]], threshold)
-                    if pval < pow(alpha, 3):
-                        different_loci.append(j)
+            corr_deletion = pearson_corr(repeat_sample_del, repeat_control_del)
+            """
+            Nanopore reads tend to have a deletion in repetitive sequences.
+            Since the deletion pattern between sample and control is similar,
+            highly-correlated deletion patterns in repetitive sequences are ignored.
+            """
+            if corr_deletion < 0.9:
+                pval = chistatistic([coverage, sum(repeat_sample_del)], [coverage, sum(repeat_control_del)], threshold)
+                if pval < pow(alpha, 3):
+                    for j in range(repeat_start, repeat_end + 1):
+                        sample_del, control_del = table_sample[j][0], table_control[j][0]
+                        pval = chistatistic([coverage, sample_del], [coverage, control_del], threshold)
+                        if pval < pow(alpha, 3):
+                            different_loci.append(j)
             # statistics to others
-            pval = chistatistic([coverage, repeat_other[0]], [coverage, repeat_other[1]], threshold)
+            pval = chistatistic(
+                [coverage, sum(repeat_sample_others)], [coverage, sum(repeat_control_others)], threshold
+            )
             if pval < alpha:
                 for j in range(repeat_start, repeat_end + 1):
-                    s, c = table_sample[j], table_control[j]
-                    pval = chistatistic([coverage, s[1]], [coverage, c[1]], threshold)
+                    sample_others, control_others = table_sample[j][1], table_control[j][1]
+                    pval = chistatistic([coverage, sample_others], [coverage, control_others], threshold)
                     if pval < alpha and j not in different_loci:
                         different_loci.append(j)
-            repeat_del = [1, 1]
-            repeat_other = [1, 1]
-            try:
-                repeat_start, repeat_end = next(repeat_span)
+            # reflesh
+            repeat_sample_del = []
+            repeat_control_del = []
+            repeat_sample_others = []
+            repeat_control_others = []
+            if repeat_idx < len(repeat_span):
+                repeat_start, repeat_end = repeat_span[repeat_idx]
                 repeat_end -= 1
-            except StopIteration:
-                pass
+                repeat_idx += 1
         else:
             pval = chistatistic([coverage, sum(s)], [coverage, sum(c)], threshold)
             if pval < alpha:
                 different_loci.append(i)
     return different_loci
```

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/consensus/consensus_main.py` & `DAJIN2-0.1.9/src/DAJIN2/core/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/core.py` & `DAJIN2-0.1.9/src/DAJIN2/core/core.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/preprocess/check_inputs.py` & `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/check_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/report/report_bam.py` & `DAJIN2-0.1.9/src/DAJIN2/core/report/report_bam.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.1.9/src/DAJIN2/core/report/report_files.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/gui.py` & `DAJIN2-0.1.9/src/DAJIN2/gui.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.1.9/src/DAJIN2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/templates/index.html` & `DAJIN2-0.1.9/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2/view.py` & `DAJIN2-0.1.9/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.1.8/src/DAJIN2.egg-info/PKG-INFO` & `DAJIN2-0.1.9/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.1.8
+Version: 0.1.9
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.1.8/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.1.9/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

