# Comparing `tmp/RelevanceAI-3.2.9.tar.gz` & `tmp/relevanceai-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelevanceAI-3.2.9.tar", last modified: Mon Sep 19 14:03:14 2022, max compression
+gzip compressed data, was "relevanceai-4.0.0.tar", last modified: Sat Jun  3 06:36:38 2023, max compression
```

## Comparing `RelevanceAI-3.2.9.tar` & `relevanceai-4.0.0.tar`

### file list

```diff
@@ -1,533 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11547 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6957 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5042 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/RelevanceAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6957 2022-09-19 14:03:13.000000 RelevanceAI-3.2.9/RelevanceAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18770 2022-09-19 14:03:14.000000 RelevanceAI-3.2.9/RelevanceAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 14:03:13.000000 RelevanceAI-3.2.9/RelevanceAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-09-19 14:03:13.000000 RelevanceAI-3.2.9/RelevanceAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-19 14:03:13.000000 RelevanceAI-3.2.9/RelevanceAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/batch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/batch/chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)    36313 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/batch/insert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/batch/local_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/batch/retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/admin/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/centroids/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/centroids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14312 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/centroids/centroids.py
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    32438 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)    16442 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/documents.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/field_children.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    12890 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/datasets/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/deployables/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/deployables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/deployables/deployables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)    14356 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/recommend.py
--rw-r--r--   0 runner    (1001) docker     (121)    50056 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     7163 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/services/tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/_api/endpoints/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/_api/endpoints/workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.069210 RelevanceAI-3.2.9/relevanceai/apps/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/apps/explorer_app/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/explorer_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6589 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/explorer_app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/explorer_app/auto.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/explorer_app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/apps/report_app/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/advanced_blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/altair.py
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/connected_charts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/markdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/plotly.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/advanced_blocks/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    12414 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/marks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/apps/report_app/sections/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5111 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/sections/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/apps/report_app/sections/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/client/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/client/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    12994 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/client/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/constants/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/config.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3963 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/stopwords.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/constants/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/dataset/apps/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/apps/launch_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/apps/manage_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     9404 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/dataset/io/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.073211 RelevanceAI-3.2.9/relevanceai/dataset/io/export/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/export/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/export/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/export/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/dataset/read/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    29218 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/read.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/dataset/read/statistics/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11280 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/read/statistics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)    18528 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/dataset/write/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39437 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/dataset/write/write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/audio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/auto/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21271 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/auto/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     6693 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/auto/dr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/cluster/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/algorithms/community_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)    17365 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9165 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/centroids.py
--rw-r--r--   0 runner    (1001) docker     (121)    51522 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/groupby.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/cluster/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9845 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/models/community_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/models/summarizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5476 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/partial.py
--rw-r--r--   0 runner    (1001) docker     (121)    20398 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/sub.py
--rw-r--r--   0 runner    (1001) docker     (121)    19244 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/cluster/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/dr/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/dr/models/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/models/ivis.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/models/pca.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/models/tsne.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/models/umap.py
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/dr/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/labels/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34596 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/labels/labels.py
--rw-r--r--   0 runner    (1001) docker     (121)    42032 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/image/base_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/text/base_text_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.077211 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/preprocessing/utils/functools_extend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/text/qa/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/qa/qa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/text/sentiment/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/sentiment/sentiment_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     6011 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text/sentiment/sentiments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/text_finetuning/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text_finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text_finetuning/supervised_finetuning_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     8188 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/text_finetuning/unsupervised_finetuning_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/vector/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14273 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/local_nearest_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (121)    22850 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/search.py
--rw-r--r--   0 runner    (1001) docker     (121)    20094 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/vectorize.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/vector/vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/viz/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10308 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/viz/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/viz/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations/viz/topic2vec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/viz/topic2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15107 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations/viz/topic2vec/plot_text_theme_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5625 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/sklearn/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/models/sklearn/minibatchkmeans.py
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/batch/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/faiss/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/faiss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/faiss/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sentence_transformers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sentence_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sentence_transformers/community_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.081211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sklearn/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/models/sklearn/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    34065 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/sub/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5001 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/sub/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3224 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/sub/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/explainer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9059 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/explainer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8443 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/text/explainer/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cluster/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/cooccurrence_network/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cooccurrence_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cooccurrence_network/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     8700 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/cooccurrence_network/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    43342 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dataset_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/dr/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/ivis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/pca.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/tsne.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/models/umap.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/dr/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/emotion/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/emotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/emotion/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/emotion/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/label/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/label/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     7281 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/label/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/ops_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/ops_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    29959 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/ops_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/clean/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3884 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/clean/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/clean/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/clean/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/count/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/count/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/count/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/count/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/extract_nouns/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/extract_nouns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/extract_nouns/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/extract_nouns/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/html_clean/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/html_clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/html_clean/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/html_clean/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/keywords/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/keywords/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/keywords/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.085211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/ner/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/ner/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/ner/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/sentence_splitting/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/sentence_splitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/sentence_splitting/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/sentence_splitting/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/translate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/translate/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/text/translate/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/processing/transformers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/transformers/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/processing/transformers/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/models/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/models/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/scaling/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/sentiment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/sentiment/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     9772 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/sentiment/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/text_tagging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/text_tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/text_tagging/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/text_tagging/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     5313 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/transform_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/image/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/image/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/audio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/clip/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8505 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/clip/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/tfhub/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/tfhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/image/tfhub/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/sentence_transformers/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/sentence_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/sentence_transformers/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/tfhub/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/tfhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/text/tfhub/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/video/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/models/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/text/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/text/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     5784 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/operations_new/vectorize/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/recipes/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.089211 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/cluster/choosing_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)    19698 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/cluster/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7963 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/recipes/model_observability/cluster/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/base64_decode.py
--rw-r--r--   0 runner    (1001) docker     (121)     8893 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7657 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/config_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/creds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    29277 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/decorators/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/silence.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/thread.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/vectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/decorators/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/distances/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/distances/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/distances/euclidean_distance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/chunk_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11668 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10332 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/read_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/doc_utils/write_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/filter_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/integration_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/list_to_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/utils/migration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/migration/mongo_to_relevance_ai.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/print_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)    17127 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/utils/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/csv_to_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.093211 RelevanceAI-3.2.9/relevanceai/workflow/diagrams/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/diagrams/diagrams.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/relevanceai/workflow/sequential.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4947 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/clusterers/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/clusterers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/clusterers/kmeans_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/clusterers/minibatch_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/clusterers/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/large_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/misc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/nested_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/sample_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/datasets/vector_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/document/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/dataclass_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/datetime_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/error_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/nested_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/numpy_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/pandas_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/simple_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/document/vector_document.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/documents/
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/datetime_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/error_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/misc_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/nested_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/numpy_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/pandas_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/simple_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/documents/vector_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/globals/objects/
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/objects/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/globals/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/unit/test_api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_api/test_insert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/unit/test_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.097211 RelevanceAI-3.2.9/tests/unit/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9925 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_dr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations/test_vectorize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/label/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/label/test_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_batch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_batch/test_batch_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_text/test_explainer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_text/test_explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_cluster/test_text/test_explainer/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/text/clean/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/text/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_operations_new/test_processing/text/clean/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/test_class_based.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/test_read_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_utils/tests_example_datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/tests_example_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/tests_example_datasets/test_example_ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/tests_example_datasets/test_example_get_games.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_utils/tests_example_datasets/test_example_sample_ecommerce.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:14.101211 RelevanceAI-3.2.9/tests/unit/test_workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/unit/test_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-19 14:03:05.000000 RelevanceAI-3.2.9/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-03 06:36:22.000000 relevanceai-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 06:36:38.395334 relevanceai-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-03 06:36:22.000000 relevanceai-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/vector_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-03 06:36:22.000000 relevanceai-4.0.0/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:36:38.395334 relevanceai-4.0.0/relevanceai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 06:36:38.000000 relevanceai-4.0.0/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 06:36:38.395334 relevanceai-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 06:36:22.000000 relevanceai-4.0.0/setup.py
```

### Comparing `RelevanceAI-3.2.9/LICENSE` & `relevanceai-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RelevanceAI-3.2.9/PKG-INFO` & `relevanceai-4.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,14 @@
 Metadata-Version: 2.1
-Name: RelevanceAI
-Version: 3.2.9
-Home-page: https://relevance.ai/
+Name: relevanceai
+Version: 4.0.0
+Home-page: https://relevanceai.com/
 Author: Relevance AI
-Author-email: dev@relevance.ai
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Manufacturing
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Database
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
-Classifier: Topic :: Multimedia :: Video :: Conversion
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.6
+Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
-Provides-Extra: dev-vis
-Provides-Extra: dev-viz
-Provides-Extra: excel
-Provides-Extra: tests
-Provides-Extra: notebook
-Provides-Extra: umap
-Provides-Extra: kmedoids
-Provides-Extra: hdbscan
-Provides-Extra: models
 License-File: LICENSE
 
 ![Github Banner](assets/github_banner.png)
 
 ## Relevance AI - The ML Platform for Unstructured Data Analysis 
 [![Documentation Status](https://readthedocs.org/projects/relevanceai/badge/?version=latest)](https://relevanceai.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
@@ -67,17 +29,17 @@
 - 🔮 ML Dataset Evaluation, for debugging dataset labels, model outputs and surfacing edge cases.
 
 
 ## 🧠 Documentation
 
 | Type      | Link |
 | ------------- | ----------- |
-| Python API | [Documentation](https://sdk.relevance.ai/) |
+| Python API | [Documentation](https://sdk.tryrelevance.com/) |
 | Python Reference | [Documentation](https://relevanceai.readthedocs.io/en/latest/)        |
-| Cloud Dashboard | [Documentation](https://docs.relevance.ai/) |
+| Cloud Dashboard | [Documentation](https://docs.tryrelevance.com/) |
 
 ## 🛠️ Installation
 
 Using pip:
 
 ```{bash}
 pip install -U relevanceai
@@ -130,15 +92,15 @@
     {"vector": [0.2, 0.2, 0.2], "field": "example_vector_"}
 ]
 results = ds.search(
     vector_search_query=query,
     page_size=3,
 )
 ```
-[Learn more about how to flexibly configure your vector search ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your vector search ->](https://sdk.tryrelevance.com/docs/search)
 
 ### Perform clustering
 
 Generate clusters
 ```{python}
 clusterop = ds.cluster(vector_fields=["example_vector_"])
 clusterop.list_closest()
@@ -148,15 +110,15 @@
 ```{python}
 from sklearn.cluster import AgglomerativeClustering
 
 cluster_model = AgglomerativeClustering()
 clusterop = ds.cluster(vector_fields=["example_vector_"], model=cluster_model, alias="agglomerative")
 clusterop.list_closest()
 ```
-[Learn more about how to flexibly configure your clustering ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your clustering ->](https://sdk.tryrelevance.com/docs/search)
 
 ## 🧰 Config
 
 The config object contains the adjustable global settings for the SDK. For a description of all the settings, see [here](https://github.com/RelevanceAI/RelevanceAI/blob/development/relevanceai/constants/config.ini).
 
 To view setting options, run the following:
```

### Comparing `RelevanceAI-3.2.9/README.md` & `relevanceai-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 - 🔮 ML Dataset Evaluation, for debugging dataset labels, model outputs and surfacing edge cases.
 
 
 ## 🧠 Documentation
 
 | Type      | Link |
 | ------------- | ----------- |
-| Python API | [Documentation](https://sdk.relevance.ai/) |
+| Python API | [Documentation](https://sdk.tryrelevance.com/) |
 | Python Reference | [Documentation](https://relevanceai.readthedocs.io/en/latest/)        |
-| Cloud Dashboard | [Documentation](https://docs.relevance.ai/) |
+| Cloud Dashboard | [Documentation](https://docs.tryrelevance.com/) |
 
 ## 🛠️ Installation
 
 Using pip:
 
 ```{bash}
 pip install -U relevanceai
@@ -83,15 +83,15 @@
     {"vector": [0.2, 0.2, 0.2], "field": "example_vector_"}
 ]
 results = ds.search(
     vector_search_query=query,
     page_size=3,
 )
 ```
-[Learn more about how to flexibly configure your vector search ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your vector search ->](https://sdk.tryrelevance.com/docs/search)
 
 ### Perform clustering
 
 Generate clusters
 ```{python}
 clusterop = ds.cluster(vector_fields=["example_vector_"])
 clusterop.list_closest()
@@ -101,15 +101,15 @@
 ```{python}
 from sklearn.cluster import AgglomerativeClustering
 
 cluster_model = AgglomerativeClustering()
 clusterop = ds.cluster(vector_fields=["example_vector_"], model=cluster_model, alias="agglomerative")
 clusterop.list_closest()
 ```
-[Learn more about how to flexibly configure your clustering ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your clustering ->](https://sdk.tryrelevance.com/docs/search)
 
 ## 🧰 Config
 
 The config object contains the adjustable global settings for the SDK. For a description of all the settings, see [here](https://github.com/RelevanceAI/RelevanceAI/blob/development/relevanceai/constants/config.ini).
 
 To view setting options, run the following:
```

### Comparing `RelevanceAI-3.2.9/RelevanceAI.egg-info/PKG-INFO` & `relevanceai-4.0.0/relevanceai.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,14 @@
 Metadata-Version: 2.1
-Name: RelevanceAI
-Version: 3.2.9
-Home-page: https://relevance.ai/
+Name: relevanceai
+Version: 4.0.0
+Home-page: https://relevanceai.com/
 Author: Relevance AI
-Author-email: dev@relevance.ai
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Manufacturing
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Database
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
-Classifier: Topic :: Multimedia :: Video :: Conversion
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.6
+Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
-Provides-Extra: dev-vis
-Provides-Extra: dev-viz
-Provides-Extra: excel
-Provides-Extra: tests
-Provides-Extra: notebook
-Provides-Extra: umap
-Provides-Extra: kmedoids
-Provides-Extra: hdbscan
-Provides-Extra: models
 License-File: LICENSE
 
 ![Github Banner](assets/github_banner.png)
 
 ## Relevance AI - The ML Platform for Unstructured Data Analysis 
 [![Documentation Status](https://readthedocs.org/projects/relevanceai/badge/?version=latest)](https://relevanceai.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
@@ -67,17 +29,17 @@
 - 🔮 ML Dataset Evaluation, for debugging dataset labels, model outputs and surfacing edge cases.
 
 
 ## 🧠 Documentation
 
 | Type      | Link |
 | ------------- | ----------- |
-| Python API | [Documentation](https://sdk.relevance.ai/) |
+| Python API | [Documentation](https://sdk.tryrelevance.com/) |
 | Python Reference | [Documentation](https://relevanceai.readthedocs.io/en/latest/)        |
-| Cloud Dashboard | [Documentation](https://docs.relevance.ai/) |
+| Cloud Dashboard | [Documentation](https://docs.tryrelevance.com/) |
 
 ## 🛠️ Installation
 
 Using pip:
 
 ```{bash}
 pip install -U relevanceai
@@ -130,15 +92,15 @@
     {"vector": [0.2, 0.2, 0.2], "field": "example_vector_"}
 ]
 results = ds.search(
     vector_search_query=query,
     page_size=3,
 )
 ```
-[Learn more about how to flexibly configure your vector search ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your vector search ->](https://sdk.tryrelevance.com/docs/search)
 
 ### Perform clustering
 
 Generate clusters
 ```{python}
 clusterop = ds.cluster(vector_fields=["example_vector_"])
 clusterop.list_closest()
@@ -148,15 +110,15 @@
 ```{python}
 from sklearn.cluster import AgglomerativeClustering
 
 cluster_model = AgglomerativeClustering()
 clusterop = ds.cluster(vector_fields=["example_vector_"], model=cluster_model, alias="agglomerative")
 clusterop.list_closest()
 ```
-[Learn more about how to flexibly configure your clustering ->](https://sdk.relevance.ai/docs/search)
+[Learn more about how to flexibly configure your clustering ->](https://sdk.tryrelevance.com/docs/search)
 
 ## 🧰 Config
 
 The config object contains the adjustable global settings for the SDK. For a description of all the settings, see [here](https://github.com/RelevanceAI/RelevanceAI/blob/development/relevanceai/constants/config.ini).
 
 To view setting options, run the following:
```

### Comparing `RelevanceAI-3.2.9/relevanceai/operations_new/scaling/base.py` & `relevanceai-4.0.0/relevanceai/steps/vector_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,61 @@
-from typing import List, Dict, Any, Optional, Union
+from relevanceai.steps._base import StepBase
 
-from relevanceai.operations_new.run import OperationRun
-from relevanceai.operations_new.scaling.models.base import ScalerModelBase
 
-
-class ScalerBase(OperationRun):
-
-    model: ScalerModelBase
-    fields: List[str]
-    alias: str
+class VectorSimilaritySearch(StepBase):
+    """Vector similarity search on Relevance dataset
+    Search your dataset based on semantic similarity.
+    Args:
+        dataset_id (str): The ID of the dataset to search.
+        query (str): The query to search for.
+        vector_field (str): The name of the field that contains the vector.
+        model (str): The model name to use.
+        content_field ((Optional) str):
+        page_size ((Optional) int): The number of results to return.
+    Returns:
+        results (list): {'type': 'array', 'items': {'type': ['string', 'object']}}
+    """
 
     def __init__(
         self,
-        vector_fields: List[str],
-        model: Union[str, ScalerModelBase],
-        alias: Optional[str] = None,
-        model_kwargs: Optional[dict] = None,
+        dataset_id: str,
+        query: str,
+        vector_field: str,
+        model: str,
+        content_field: str = None,
+        page_size: int = 5,
+        step_name: str = "vector_similarity_search",
+        *args,
         **kwargs,
-    ):
-        self.vector_fields = vector_fields
-
-        # TODO: Add a get ailas method
-        self.alias = alias  # type: ignore
-
-        if model_kwargs is None:
-            model_kwargs = {}
-
-        self.model = self._get_model(
-            model=model,
-            alias=alias,
-            model_kwargs=model_kwargs,
-        )
-        for k, v in kwargs.items():
-            setattr(self, k, v)
+    ) -> None:
+        self.dataset_id = dataset_id
+        self.query = query
+        self.vector_field = vector_field
+        self.model = model
+        self.content_field = content_field
+        self.page_size = page_size
+        self.step_name = step_name
+        self._outputs = ["results"]
+        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
+        super().__init__(*args, **kwargs)
 
     @property
-    def name(self):
-        return "scaing"
-
-    def _get_model(
-        self,
-        model: Union[str, ScalerModelBase],
-        alias: Optional[str] = None,
-        model_kwargs: Optional[dict] = None,
-    ) -> ScalerModelBase:
-
-        from relevanceai.operations_new.scaling.models.sklearn import SKLearnScaler
-
-        mapped_model = SKLearnScaler(
-            model=model,
-            alias=alias,
-            model_kwargs=model_kwargs,
-        )
-
-        return mapped_model
-
-    def transform(
-        self,
-        documents: List[Dict[str, Any]],
-    ) -> List[Dict[str, Any]]:
-
-        scaled_vector_names = []
-
-        for vector_field in self.vector_fields:
-            vectors = self.get_field_across_documents(
-                field=vector_field, docs=documents
-            )
-
-            reduced_vectors = self.model.fit_transform(vectors)
-            scaled_vector_name = self.model.vector_name(vector_field)
-
-            if scaled_vector_name in self.vector_fields:
-                raise ValueError(
-                    "Alias is already being used, Please set a different alias"
-                )
-
-            scaled_vector_names.append(scaled_vector_name)
-
-            self.set_field_across_documents(
-                field=scaled_vector_name,
-                values=reduced_vectors,
-                docs=documents,
-            )
-
-        # removes unnecessary info for updated_where
-        updated_documents = [
+    def steps(self):
+        step_params = {
+            "dataset_id": self.dataset_id,
+            "query": self.query,
+            "vector_field": self.vector_field,
+            "model": self.model,
+        }
+        if self.content_field is not None:
+            step_params["content_field"] = self.content_field
+        if self.page_size is not None:
+            step_params["page_size"] = self.page_size
+        return [
             {
-                key: value
-                for key, value in document.items()
-                if key in ["_id"] + scaled_vector_names
+                "transformation": "search",
+                "name": self.step_name,
+                "foreach": "",
+                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
+                "params": step_params,
             }
-            for document in documents
         ]
-
-        return updated_documents
```

