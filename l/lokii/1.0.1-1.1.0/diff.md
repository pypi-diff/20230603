# Comparing `tmp/lokii-1.0.1.tar.gz` & `tmp/lokii-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-1.0.1.tar", last modified: Wed May 31 14:39:28 2023, max compression
+gzip compressed data, was "lokii-1.1.0.tar", last modified: Fri Jun  2 08:01:57 2023, max compression
```

## Comparing `lokii-1.0.1.tar` & `lokii-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.0.1/LICENSE
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5407 2023-05-31 14:39:28.861541 lokii-1.0.1/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4297 2023-05-31 14:39:03.000000 lokii-1.0.1/README.md
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-05-31 14:39:03.000000 lokii-1.0.1/VERSION
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/__main__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3309 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/cli.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2287 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/config.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/exec/node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/logger/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/logger/color.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/context.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      664 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/logger/formatter.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/progress.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4466 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/main.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/model/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/model/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      730 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/model/group_module.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/model/node_module.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/base_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2776 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2783 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4529 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/storage/data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      835 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/storage/temp_storage.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/util/graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/util/module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/util/perf_timer_context.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5407 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1307 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/entry_points.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.0.1/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-05-31 14:39:28.861541 lokii-1.0.1/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1788 2023-05-31 14:39:03.000000 lokii-1.0.1/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2451 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/conftest.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/exec/test_node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1635 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/parse/test_group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/parse/test_node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/tests/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4091 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/storage/test_data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/storage/test_temp_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4211 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/test_cli.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/tests/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/util/test_graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/test_module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/test_perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.0/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-02 08:01:57.975506 lokii-1.1.0/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.0/README.md
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-06-02 08:01:36.000000 lokii-1.1.0/VERSION
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2287 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/exec/node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      664 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6956 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/model/group_module.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/model/node_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/parse/base_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2977 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/parse/group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2799 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/storage/batch_iterator.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4915 2023-06-02 08:01:36.000000 lokii-1.1.0/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      835 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/util/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.0/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.0/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.971506 lokii-1.1.0/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1339 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.0/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-02 08:01:57.000000 lokii-1.1.0/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-06-02 08:01:57.975506 lokii-1.1.0/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1801 2023-06-02 08:01:36.000000 lokii-1.1.0/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.0/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.0/tests/exec/test_node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.0/tests/parse/test_group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.0/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4431 2023-06-02 08:01:36.000000 lokii-1.1.0/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3271 2023-06-02 08:01:36.000000 lokii-1.1.0/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-02 08:01:57.975506 lokii-1.1.0/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.0/tests/util/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.0/tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.0.1/LICENSE` & `lokii-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/PKG-INFO` & `lokii-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: lokii
-Version: 1.0.1
-Summary: Generate, Load, Develop and Test with consistent relational datasets!
-Home-page: https://github.com/dorukerenaktas/lokii
-Author: Doruk Eren Aktaş
-Author-email: dorukerenaktas@gmail.com
-License: MIT License
-Keywords: data generation,relational datasets,development environment,testing,database
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![lokii-logo](https://github.com/dorukerenaktas/lokii/assets/20422563/fe774eba-ddd0-4bad-a093-553bb980f54c)
 
 ![PyPI](https://img.shields.io/pypi/v/lokii)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/lokii)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dorukerenaktas/lokii/python-app.yml)
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/dorukerenaktas/lokii)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -75,15 +48,15 @@
 from faker import Faker
 
 # use your favorite tools to generate data
 # you can even use database connection, filesystem or AI
 fake = Faker()
 
 # if you want you can override the node name if not provided filename will be used
-# node name can be used in source queries if you want to retrieve rows that depends on another node
+# can be used in source queries if you want to retrieve rows that depends on another node
 # name = "business.offices"
 
 # define a query that returns one or more rows
 source = "SELECT * FROM range(10)"
 
 
 # item function will be called for each row in `source` query result
@@ -104,25 +77,60 @@
 
 ## Group Definition
 
 Group file defines how each node data will be exported. There are special functions in group definition files.
 - `before`: Called once before export operation
 - `export`: Called for every node in the group
 - `after`: Called once after export operation
-- 
+
 ```python
-# database.group.py
+# filesystem.group.py
+import os
+import shutil
+from csv import DictWriter
+
+out_path = "out_data"
+
 
 def before(args):
-    pass
+    """
+    Executed before export function.
+    :param args: contains node names that belongs to this group
+    :type args: {"nodes": list[str]} 
+    """
+    if os.path.exists(out_path):
+        # always clear your storage before starting a new export
+        shutil.rmtree(out_path)
+    os.makedirs(out_path)
+
 
 def export(args):
-    pass
+    """
+    Executed for all nodes that belongs to this group
+    :param args: contains node name, node columns and a batch iterator
+    :type args: {"name": str, "cols": list[str], "batches": list[dict]} 
+    """
+    node_name = args["name"]
+    node_cols = args["cols"]
+    batches = args["batches"]
+    # out_data/offices.csv
+    out_file_path = os.path.join(out_path, node_name + ".csv")
+    with open(out_file_path, 'w+', newline='', encoding='utf-8') as outfile:
+        writer = DictWriter(outfile, fieldnames=node_cols)
+        writer.writeheader()
+        for batch in batches:
+            writer.writerows(batch)
+
 
 def after(args):
+    """
+    Executed after export function.
+    :param args: contains node names that belongs to this group
+    :type args: {"nodes": list[str]} 
+    """
     pass
 ```
 
 
 ## Upload to PyPI
 
 You can create the source distribution of the package by running the command given below:
```

### Comparing `lokii-1.0.1/lokii/cli.py` & `lokii-1.1.0/lokii/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,21 +68,18 @@
             metavar="PATH",
             default=".",
             type=str,
             help="generate the specified number of outputs",
         )
 
         parser.add_argument(
-            "-o",
-            "--out-folder",
-            action="store",
-            metavar="PATH",
-            default="./data",
-            type=str,
-            help="redirect output to a file",
+            "-e",
+            "--export",
+            action="store_true",
+            help="execute group export modules",
         )
 
         parser.add_argument(
             "-p",
             "--purge",
             action="store_true",
             help="purge cache database after generation",
@@ -95,17 +92,16 @@
             verbose = logging.DEBUG
         if arguments.quiet:
             verbose = logging.ERROR
 
         with LoggingContext(level=verbose, filename=arguments.log_file):
             try:
                 print(LOKII_ASCII)
-                lokii_gen = Lokii(arguments.source_folder, arguments.out_folder)
-                lokii_gen.generate(arguments.purge)
+                _lokii = Lokii(arguments.source_folder)
+                _lokii.generate(arguments.export, arguments.purge)
             except Exception as err:
                 logging.critical(str(err), exc_info=True)
 
 
 def exec_cmd(argv=None) -> None:
-    """A simple method that runs a Command."""
     command = Command(argv)
     command.execute()
```

### Comparing `lokii-1.0.1/lokii/config.py` & `lokii-1.1.0/lokii/config.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/exec/node_executor.py` & `lokii-1.1.0/lokii/exec/node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/logger/color.py` & `lokii-1.1.0/lokii/logger/color.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/logger/context.py` & `lokii-1.1.0/lokii/logger/context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/logger/formatter.py` & `lokii-1.1.0/lokii/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/logger/progress.py` & `lokii-1.1.0/lokii/logger/progress.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/model/node_module.py` & `lokii-1.1.0/lokii/model/node_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/parse/base_parser.py` & `lokii-1.1.0/lokii/parse/base_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/parse/group_parser.py` & `lokii-1.1.0/lokii/parse/node_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 import logging
 from os import path
 from glob import glob
 
 from lokii.config import CONFIG
-from lokii.model.group_module import GroupModule
+from lokii.model.node_module import GenNodeModule
 from lokii.util.module_file_loader import ModuleFileLoader
 from lokii.util.perf_timer_context import PerfTimerContext
 from lokii.parse.base_parser import BaseParser
 
-GROUP_RESOLVER = "**/*%s" % CONFIG.gen.group_ext
+NODE_RESOLVER = "**/*%s" % CONFIG.gen.node_ext
 
 
-class GroupParser(BaseParser):
+class NodeParser(BaseParser):
     """
-    Reads and validates group export configurations from filesystem structure.
+    Reads and validates node configurations from filesystem structure.
 
-    :var groups: parsed group modules
-    :type groups: dict[str, GroupModule]
+    :var nodes: parsed generation nodes
+    :type nodes: dict[str, GenNodeModule]
     """
 
     def __init__(self, source_folder):
         """
         Initializes parser.
         :param source_folder: root path of the project
         :type source_folder: str
         """
         self.root = source_folder
-        self.groups = {}
+        self.nodes = {}
 
     def parse(self):
         """
         :return: parsed and validated node run flat map
-        :rtype: dict[str, GroupModule]
+        :rtype: dict[str, GenNodeModule]
         """
         with PerfTimerContext() as t:
-            groups = list(self.__parse_groups())
-            self.groups = {n.name: n for n in groups}
+            nodes = list(self.__parse_nodes())
+            self.nodes = {n.name: n for n in nodes}
 
-        group_count = len(groups)
-        if group_count == 0:
-            logging.warning("No group conf file found at %s" % self.root)
+        node_count = len(nodes)
+        if node_count == 0:
+            logging.warning("No generation node file found at %s" % self.root)
         else:
-            logging.info("%d group definitions parsed in %s" % (group_count, t))
-        return self.groups
+            logging.info("%d generation node parsed in %s" % (node_count, t))
+        return self.nodes
 
-    def __parse_groups(self):
+    def __parse_nodes(self):
         """
-        Finds all the groups matching the group file pattern. Loads group modules and ensures
-        group module configuration is valid.
+        Finds all the nodes matching the node file pattern. Loads node modules and ensures
+        node module configuration is valid.
 
-        :return: parsed and validated group modules
-        :rtype: list[GroupModule]
+        :return: parsed and validated node modules
+        :rtype: list[GenNodeModule]
         """
-        glob_path = path.join(self.root, GROUP_RESOLVER)
-        file_paths = [f for f in glob(glob_path)]
+        glob_path = path.join(self.root, NODE_RESOLVER)
+        file_paths = [f for f in glob(glob_path, recursive=True)]
 
         for fp in file_paths:
             loader = ModuleFileLoader(fp)
             loader.load()
             mod = loader.module
 
-            m_name = path.dirname(fp).split(path.sep)[-1]
-            parsed = GroupModule(m_name)
+            # extract node name from filename
+            m_name = path.basename(fp).replace(CONFIG.gen.node_ext, "")
+            # extract groups from file path
+            m_groups = path.relpath(fp, self.root).split(path.sep)[:-1]
+            m_version = loader.version
+
+            # ensure provided module is valid
+            self.attr(mod, "source", "`source` not found at %s" % fp)
+            self.inst(mod.source, str, "`source` must be str at %s" % fp)
+            self.attr(mod, "item", "`item` not found at %s" % fp)
+            self.func(mod.item, "`item` must be function at %s" % fp)
+            self.sig(mod.item, 1, "`item` accepts only one param at %s" % fp)
+            if self.attr(mod, "name"):
+                self.inst(mod.name, str, "`name` must be str at %s" % fp)
+                m_name = mod.name
 
-            # ensure group configuration is valid
-            if self.attr(mod, "before"):
-                self.func(mod.before, "`before` must be function at %s" % fp)
-                self.sig(mod.before, 1, "`before` accepts only one param at %s" % fp)
-                parsed.before = mod.before
-            if self.attr(mod, "export"):
-                self.func(mod.export, "`export` must be function at %s" % fp)
-                self.sig(mod.export, 1, "`export` accepts only one param at %s" % fp)
-                parsed.export = mod.export
-            if self.attr(mod, "after"):
-                self.func(mod.after, "`after` must be function at %s" % fp)
-                self.sig(mod.after, 1, "`after` accepts only one param at %s" % fp)
-                parsed.export = mod.after
+            parsed = GenNodeModule(mod.source, mod.item, m_name, m_version, m_groups)
             yield parsed
```

### Comparing `lokii-1.0.1/lokii/storage/data_storage.py` & `lokii-1.1.0/lokii/storage/data_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,26 @@
         """
         with self.connect() as conn:
             keys = ",".join(["'%s'" % n for n in names])
             q = "SELECT name, version, gen_id FROM __meta WHERE name IN (%s);"
             data = conn.execute(q % keys).fetch_df()
             return data.to_dict("records")
 
+    def cols(self, name) -> list[str]:
+        """
+        Fetches generated column name list for given node.
+        :param name: name of the node
+        :type name: str
+        :return: list of no columns
+        """
+        with self.connect() as conn:
+            q = "DESCRIBE %s;"
+            data = conn.execute(q % name).fetchall()
+            return [col[0] for col in data]
+
     def insert(self, name: str, files: list[str]) -> None:
         """
         Creates a table for given node name in local relational database. If there is a table
         with the same node name it will drop all data and create a fresh one. Given files will
         be concatenated and inserted in the fresh table.
 
         :param name: node name of the module
```

### Comparing `lokii-1.0.1/lokii/storage/temp_storage.py` & `lokii-1.1.0/lokii/storage/temp_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/util/graph_analyzer.py` & `lokii-1.1.0/lokii/util/graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/util/module_file_loader.py` & `lokii-1.1.0/lokii/util/module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii/util/perf_timer_context.py` & `lokii-1.1.0/lokii/util/perf_timer_context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/lokii.egg-info/PKG-INFO` & `lokii-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.0.1
+Version: 1.1.0
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -75,15 +75,15 @@
 from faker import Faker
 
 # use your favorite tools to generate data
 # you can even use database connection, filesystem or AI
 fake = Faker()
 
 # if you want you can override the node name if not provided filename will be used
-# node name can be used in source queries if you want to retrieve rows that depends on another node
+# can be used in source queries if you want to retrieve rows that depends on another node
 # name = "business.offices"
 
 # define a query that returns one or more rows
 source = "SELECT * FROM range(10)"
 
 
 # item function will be called for each row in `source` query result
@@ -104,25 +104,60 @@
 
 ## Group Definition
 
 Group file defines how each node data will be exported. There are special functions in group definition files.
 - `before`: Called once before export operation
 - `export`: Called for every node in the group
 - `after`: Called once after export operation
-- 
+
 ```python
-# database.group.py
+# filesystem.group.py
+import os
+import shutil
+from csv import DictWriter
+
+out_path = "out_data"
+
 
 def before(args):
-    pass
+    """
+    Executed before export function.
+    :param args: contains node names that belongs to this group
+    :type args: {"nodes": list[str]} 
+    """
+    if os.path.exists(out_path):
+        # always clear your storage before starting a new export
+        shutil.rmtree(out_path)
+    os.makedirs(out_path)
+
 
 def export(args):
-    pass
+    """
+    Executed for all nodes that belongs to this group
+    :param args: contains node name, node columns and a batch iterator
+    :type args: {"name": str, "cols": list[str], "batches": list[dict]} 
+    """
+    node_name = args["name"]
+    node_cols = args["cols"]
+    batches = args["batches"]
+    # out_data/offices.csv
+    out_file_path = os.path.join(out_path, node_name + ".csv")
+    with open(out_file_path, 'w+', newline='', encoding='utf-8') as outfile:
+        writer = DictWriter(outfile, fieldnames=node_cols)
+        writer.writeheader()
+        for batch in batches:
+            writer.writerows(batch)
+
 
 def after(args):
+    """
+    Executed after export function.
+    :param args: contains node names that belongs to this group
+    :type args: {"nodes": list[str]} 
+    """
     pass
 ```
 
 
 ## Upload to PyPI
 
 You can create the source distribution of the package by running the command given below:
```

### Comparing `lokii-1.0.1/lokii.egg-info/SOURCES.txt` & `lokii-1.1.0/lokii.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 lokii/model/group_module.py
 lokii/model/node_module.py
 lokii/parse/__init__.py
 lokii/parse/base_parser.py
 lokii/parse/group_parser.py
 lokii/parse/node_parser.py
 lokii/storage/__init__.py
+lokii/storage/batch_iterator.py
 lokii/storage/data_storage.py
 lokii/storage/temp_storage.py
 lokii/util/__init__.py
 lokii/util/graph_analyzer.py
 lokii/util/module_file_loader.py
 lokii/util/perf_timer_context.py
 tests/__init__.py
```

### Comparing `lokii-1.0.1/setup.py` & `lokii-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     version=VERSION,
     packages=find_packages(where="."),
     description="Generate, Load, Develop and Test with consistent relational datasets!",
     long_description=README,
     long_description_content_type="text/markdown",
     keywords="data generation, relational datasets, development environment, testing, database",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
```

### Comparing `lokii-1.0.1/tests/conftest.py` & `lokii-1.1.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import shutil
 
 import pytest
-from lokii.config import CONFIG
 from pytest import FixtureRequest
 from pytest_mock import MockerFixture
 
+
+from lokii.config import CONFIG
 from lokii import Lokii
 
 
 @pytest.fixture
 def glob_files(mocker, request):
     """
     :param mocker: Fixture that provides the same interface to functions in the mock module,
@@ -17,14 +18,15 @@
     :type mocker: MockerFixture
     :param request: A request for a fixture from a test or fixture function.
     :type request: FixtureRequest
     :return: list of found files
     :rtype: list[str]
     """
     files = request.param if hasattr(request, "param") else []
+    files = [os.path.normpath(f) for f in files]
     mocker.patch(
         "lokii.parse.group_parser.glob",
         return_value=[f for f in files if CONFIG.gen.group_ext in f],
     )
     mocker.patch(
         "lokii.parse.node_parser.glob",
         return_value=[f for f in files if CONFIG.gen.node_ext in f],
```

### Comparing `lokii-1.0.1/tests/exec/test_node_executor.py` & `lokii-1.1.0/tests/exec/test_node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/tests/parse/test_group_parser.py` & `lokii-1.1.0/tests/parse/test_group_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,33 @@
     glob_files, load_modules, expect
 ):
     parsed = GroupParser("/test/proj").parse()
     assert expect in parsed
     assert expect == parsed[expect].name
 
 
+@pytest.mark.parametrize(
+    "glob_files, load_modules, expect",
+    [
+        (
+            ["/test/path/g1/t1.group.py", "/test/path/g1/g2/t2.group.py"],
+            [{"name": "g1"}, {"name": "g2"}],
+            [[], ["g1"]],
+        )
+    ],
+    indirect=["glob_files", "load_modules"],
+)
+def test_parse_should_use_file_path_to_extract_groups(glob_files, load_modules, expect):
+    parser = GroupParser("/test/path")
+    parser.parse()
+    for i, module_path in enumerate(glob_files):
+        node_name = load_modules[i]["name"]
+        assert expect[i] == parser.groups[node_name].groups
+
+
 @pytest.mark.parametrize("glob_files", [["/test/path/g1/g1.group.py"]], indirect=True)
 @pytest.mark.parametrize(
     "load_modules, expect",
     [
         ([{"before": ""}], "`before` must be function"),
         ([{"before": lambda x, y: x}], "`before` accepts only one param"),
         ([{"export": ""}], "`export` must be function"),
```

### Comparing `lokii-1.0.1/tests/parse/test_node_parser.py` & `lokii-1.1.0/tests/parse/test_node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/tests/storage/test_data_storage.py` & `lokii-1.1.0/tests/storage/test_data_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 @pytest.mark.parametrize(
     "query, expect",
     [
         ("SELECT * from customers", ["customers"]),
         ("SELECT 100", []),
         (
             """
-                SELECT i.range, t, o.officeCode
-                    FROM offices o
-                    CROSS JOIN VALUES('manager', 'employee') as data(t)
-                    CROSS JOIN range(3) as i
-                """,
+                    SELECT i.range, t, o.officeCode
+                        FROM offices o
+                        CROSS JOIN VALUES('manager', 'employee') as data(t)
+                        CROSS JOIN range(3) as i
+                    """,
             ["offices"],
         ),
     ],
 )
 def test_deps_should_return_dependencies_from_query(query, expect):
     storage = DataStorage()
     deps = storage.deps(query)
@@ -78,14 +78,23 @@
     storage.save("test_gen2", "test_node3", "test_v4")
     deps = storage.meta(["test_node2", "test_node3"])
     assert len(deps) == 2
     assert len([d for d in deps if d["name"] == "test_node2"]) == 1
     assert len([d for d in deps if d["name"] == "test_node3"]) == 1
 
 
+def test_cols_should_return_column_names_for_given_node():
+    storage = DataStorage()
+    with storage.connect() as conn:
+        _temp = TempStorage("_")
+        _temp.dump([{"col1": i, "col2": i} for i in range(10)])
+        storage.insert("n1", _temp.batches)
+        assert ["col1", "col2"] == storage.cols("n1")
+
+
 @pytest.mark.parametrize("node, expect", [("s1.n2", "s1"), ("s2.n2", "s2")])
 def test_insert_should_create_schema_if_node_name_contain_dot(node, expect):
     storage = DataStorage()
     with storage.connect() as conn:
         _temp = TempStorage("_")
         _temp.dump([{"data": i} for i in range(10)])
         storage.insert(node, _temp.batches)
```

### Comparing `lokii-1.0.1/tests/test_cli.py` & `lokii-1.1.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,91 +42,68 @@
     assert "CRITICAL" in caplog.text
 
 
 @pytest.mark.parametrize("glob_files, load_modules", [([], [])], indirect=True)
 def test_exec_cmd_should_clear_db_if_purge(glob_files, load_modules):
     exec_cmd("lokii -p")
     assert not os.path.exists(CONFIG.temp.db_path)
-    assert os.path.exists("data")
-    shutil.rmtree("data")
 
 
 @pytest.mark.parametrize(
-    "glob_files, load_modules, out_path",
-    [(["t1.node.py"], [{"source": "SELECT 1", "item": lambda x: x}], "test_out_1")],
-    indirect=["glob_files", "load_modules"],
-)
-def test_exec_cmd_should_execute_generation(glob_files, load_modules, out_path):
-    exec_cmd("lokii -p -o %s -f ." % out_path)
-    assert os.path.exists(out_path)
-    shutil.rmtree(out_path)
-
-
-@pytest.mark.parametrize(
-    "glob_files, load_modules, out_path",
-    [(["t1.node.py"], [{"source": "SELECT 1", "item": lambda x: x}], "test_out_1")],
-    indirect=["glob_files", "load_modules"],
+    "glob_files, load_modules",
+    [(["t1.node.py"], [{"source": "SELECT 1", "item": lambda x: x}])],
+    indirect=True,
 )
-def test_exec_cmd_should_cache_consequent_runs(
-    glob_files, load_modules, out_path, caplog
-):
-    exec_cmd("lokii -o %s -f ." % out_path)
+def test_exec_cmd_should_cache_consequent_runs(glob_files, load_modules, caplog):
+    exec_cmd("lokii -f .")
     assert os.path.exists(CONFIG.temp.db_path)
     caplog.clear()
 
-    exec_cmd("lokii -p -o %s -f ." % out_path)
+    exec_cmd("lokii -p -f .")
     assert "not changed. Using existing dataset." in caplog.text
-    assert os.path.exists(out_path)
-    shutil.rmtree(out_path)
 
 
 gen_mod = {"source": "SELECT 1", "item": lambda x: x, "version": "v1"}
 
 
 @pytest.mark.usefixtures("glob_files", "load_modules")
-@pytest.mark.parametrize("out_path", ["test_out_1"])
 @pytest.mark.parametrize(
     "glob_files, load_modules", [(["t1.node.py"], [gen_mod])], indirect=True
 )
-def test_exec_cmd_should_regenerate_on_code_change(caplog, out_path):
+def test_exec_cmd_should_regenerate_on_code_change(caplog):
     # start generation for code version v1
     gen_mod["version"] = "v1"
-    exec_cmd("lokii -o %s -f ." % out_path)
+    exec_cmd("lokii -f .")
     assert os.path.exists(CONFIG.temp.db_path)
     caplog.clear()
 
     # start generation for code version v2
     gen_mod["version"] = "v2"
-    exec_cmd("lokii -p -o %s -f ." % out_path)
+    exec_cmd("lokii -p -f .")
     # should regenerate and not use cache
     assert "not changed. Using existing dataset." not in caplog.text
-    assert os.path.exists(out_path)
-    shutil.rmtree(out_path)
 
 
 gen_mod1, gen_mod2 = (
     {"source": "SELECT * from n2", "item": lambda x: x, "name": "n1"},
     {"source": "SELECT 1", "item": lambda x: x, "name": "n2", "version": "v1"},
 )
 
 
 @pytest.mark.usefixtures("glob_files", "load_modules")
-@pytest.mark.parametrize("out_path", ["test_out_1"])
 @pytest.mark.parametrize(
     "glob_files, load_modules",
     [(["t1.node.py", "t2.node.py"], [gen_mod1, gen_mod2])],
     indirect=True,
 )
-def test_exec_cmd_should_regenerate_on_dependency_change(caplog, out_path):
+def test_exec_cmd_should_regenerate_on_dependency_change(caplog):
     # start generation for dependency code version v1
     gen_mod2["version"] = "v1"
-    exec_cmd("lokii -o %s -f ." % out_path)
+    exec_cmd("lokii -f .")
     assert os.path.exists(CONFIG.temp.db_path)
     caplog.clear()
 
     # start generation for dependency code version v2
     gen_mod2["version"] = "v2"
-    exec_cmd("lokii -p -o %s -f ." % out_path)
+    exec_cmd("lokii -p -f .")
     # should regenerate and not use cache because of dependency change
     assert "not changed. Using existing dataset." not in caplog.text
-    assert os.path.exists(out_path)
-    shutil.rmtree(out_path)
```

### Comparing `lokii-1.0.1/tests/util/test_graph_analyzer.py` & `lokii-1.1.0/tests/util/test_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/tests/util/test_module_file_loader.py` & `lokii-1.1.0/tests/util/test_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.1/tests/util/test_perf_timer_context.py` & `lokii-1.1.0/tests/util/test_perf_timer_context.py`

 * *Files identical despite different names*

