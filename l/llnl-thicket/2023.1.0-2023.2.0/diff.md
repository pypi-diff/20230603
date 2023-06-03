# Comparing `tmp/llnl-thicket-2023.1.0.tar.gz` & `tmp/llnl-thicket-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/g/g19/brink2/git_root_pub/thicket/dist/.tmp-2u2a5lth/llnl-thicket-2023.1.0.tar", last modified: Thu Jan 26 06:32:08 2023, max compression
+gzip compressed data, was "llnl-thicket-2023.2.0.tar", last modified: Sat Jun  3 21:48:06 2023, max compression
```

## Comparing `llnl-thicket-2023.1.0.tar` & `llnl-thicket-2023.2.0.tar`

### file list

```diff
@@ -1,63 +1,69 @@
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/
--rw-------   0 brink2   (42788) brink2   (42788)     1087 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/LICENSE
--rw-------   0 brink2   (42788) brink2   (42788)      223 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/MANIFEST.in
--rw-------   0 brink2   (42788) brink2   (42788)     1167 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/NOTICE
--rw-------   0 brink2   (42788) brink2   (42788)     2987 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/PKG-INFO
--rw-------   0 brink2   (42788) brink2   (42788)     2589 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/README.md
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/
--rw-------   0 brink2   (42788) brink2   (42788)     2987 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/PKG-INFO
--rw-------   0 brink2   (42788) brink2   (42788)     1481 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/SOURCES.txt
--rw-------   0 brink2   (42788) brink2   (42788)        1 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/dependency_links.txt
--rw-------   0 brink2   (42788) brink2   (42788)       79 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/requires.txt
--rw-------   0 brink2   (42788) brink2   (42788)        8 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/llnl_thicket.egg-info/top_level.txt
--rw-------   0 brink2   (42788) brink2   (42788)      456 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/pyproject.toml
--rw-------   0 brink2   (42788) brink2   (42788)       38 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/setup.cfg
--rw-------   0 brink2   (42788) brink2   (42788)     1447 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/setup.py
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/
--rw-------   0 brink2   (42788) brink2   (42788)      744 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/__init__.py
--rw-------   0 brink2   (42788) brink2   (42788)     1905 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/helpers.py
--rw-------   0 brink2   (42788) brink2   (42788)    13988 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/model_extrap.py
--rw-------   0 brink2   (42788) brink2   (42788)     3674 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/ncu.py
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/stats/
--rw-------   0 brink2   (42788) brink2   (42788)      176 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/__init__.py
--rw-------   0 brink2   (42788) brink2   (42788)     1088 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/calc_average.py
--rw-------   0 brink2   (42788) brink2   (42788)     1907 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/calc_corr_nodewise.py
--rw-------   0 brink2   (42788) brink2   (42788)     1252 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/calc_deviation.py
--rw-------   0 brink2   (42788) brink2   (42788)     1161 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/calc_extremum.py
--rw-------   0 brink2   (42788) brink2   (42788)     1375 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/calc_percentiles.py
--rw-------   0 brink2   (42788) brink2   (42788)     1314 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/check_normality.py
--rw-------   0 brink2   (42788) brink2   (42788)      672 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/display_heatmap.py
--rw-------   0 brink2   (42788) brink2   (42788)      842 2023-01-23 21:52:38.000000 llnl-thicket-2023.1.0/thicket/stats/display_histogram.py
--rw-------   0 brink2   (42788) brink2   (42788)    46374 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/thicket.py
--rw-------   0 brink2   (42788) brink2   (42788)     1891 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/utils.py
--rw-------   0 brink2   (42788) brink2   (42788)      256 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/version.py
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/
--rw-------   0 brink2   (42788) brink2   (42788)     1378 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/__init__.py
--rw-------   0 brink2   (42788) brink2   (42788)      814 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/package.json
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/
--rw-------   0 brink2   (42788) brink2   (42788)      368 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/globals.js
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/
--rw-------   0 brink2   (42788) brink2   (42788)     2653 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/datautil.js
--rw-------   0 brink2   (42788) brink2   (42788)      368 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/globals.js
--rw-------   0 brink2   (42788) brink2   (42788)    19679 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/pcp.js
--rw-------   0 brink2   (42788) brink2   (42788)    11479 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/scatter.js
--rw-------   0 brink2   (42788) brink2   (42788)     5266 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/stackedarea.js
--rw-------   0 brink2   (42788) brink2   (42788)     1638 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/store.js
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/topdown/
--rw-------   0 brink2   (42788) brink2   (42788)    12742 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/topdown/stackedbars.js
--rw-------   0 brink2   (42788) brink2   (42788)      428 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/topdown/topdown.js
--rw-------   0 brink2   (42788) brink2   (42788)     6015 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/scripts/treetable.js
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/static/
--rw-------   0 brink2   (42788) brink2   (42788)      938 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static/pcp_bundle.html
--rw-------   0 brink2   (42788) brink2   (42788)   338991 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static/pcp_bundle.js
--rw-------   0 brink2   (42788) brink2   (42788)      139 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static/topdown_bundle.html
--rw-------   0 brink2   (42788) brink2   (42788)   188237 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/static/topdown_bundle.js
--rw-------   0 brink2   (42788) brink2   (42788)      397 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static/treetable_bundle.html
--rw-------   0 brink2   (42788) brink2   (42788)   282630 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static/treetable_bundle.js
--rw-------   0 brink2   (42788) brink2   (42788)      728 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/static_fixer.py
-drwx------   0 brink2   (42788) brink2   (42788)        0 2023-01-26 06:32:08.000000 llnl-thicket-2023.1.0/thicket/vis/templates/
--rw-------   0 brink2   (42788) brink2   (42788)      984 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/templates/pcp.html
--rw-------   0 brink2   (42788) brink2   (42788)       26 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/templates/topdown.html
--rw-------   0 brink2   (42788) brink2   (42788)      393 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/templates/treetable.html
--rw-------   0 brink2   (42788) brink2   (42788)     1576 2023-01-26 06:31:42.000000 llnl-thicket-2023.1.0/thicket/vis/visualizations.py
--rw-------   0 brink2   (42788) brink2   (42788)     1388 2023-01-23 21:52:39.000000 llnl-thicket-2023.1.0/thicket/vis/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3088 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.761327 llnl-thicket-2023.2.0/llnl_thicket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-06-03 21:48:06.000000 llnl-thicket-2023.2.0/llnl_thicket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-06-03 21:48:06.000000 llnl-thicket-2023.2.0/llnl_thicket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 21:48:06.000000 llnl-thicket-2023.2.0/llnl_thicket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-03 21:48:06.000000 llnl-thicket-2023.2.0/llnl_thicket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-03 21:48:06.000000 llnl-thicket-2023.2.0/llnl_thicket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.761327 llnl-thicket-2023.2.0/thicket/
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14230 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/model_extrap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4639 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/ncu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.761327 llnl-thicket-2023.2.0/thicket/stats/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6073 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/calc_boxplot_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/check_normality.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4592 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/correlation_nodewise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/display_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/display_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/display_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/mean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/median.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/std.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/stats/variance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9450 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/statspreference.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50088 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/thicket.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.761327 llnl-thicket-2023.2.0/thicket/vis/
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.761327 llnl-thicket-2023.2.0/thicket/vis/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/globals.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/datautil.js
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/globals.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19679 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/pcp.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11479 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/scatter.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5266 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/stackedarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/store.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/thicket/vis/scripts/topdown/
+-rw-r--r--   0 runner    (1001) docker     (122)    12742 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/topdown/stackedbars.js
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/topdown/topdown.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/scripts/treetable.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/thicket/vis/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/pcp_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (122)   338991 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/pcp_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/topdown_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (122)   188237 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/topdown_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/treetable_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (122)   282630 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static/treetable_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/static_fixer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 21:48:06.765328 llnl-thicket-2023.2.0/thicket/vis/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/templates/pcp.html
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/templates/topdown.html
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/templates/treetable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1577 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1388 2023-06-03 21:47:58.000000 llnl-thicket-2023.2.0/thicket/vis/webpack.config.js
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `llnl-thicket-2023.1.0/LICENSE` & `llnl-thicket-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/NOTICE` & `llnl-thicket-2023.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/PKG-INFO` & `llnl-thicket-2023.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-Metadata-Version: 2.1
-Name: llnl-thicket
-Version: 2023.1.0
-Summary: Toolkit for exploratory data analysis of ensemble performance data
-License: MIT
-Project-URL: Source Code, https://github.com/LLNL/thicket
-Project-URL: Documentation, https://thicket.readthedocs.io/
-Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown
-Provides-Extra: extrap
-License-File: LICENSE
-License-File: NOTICE
+# <img src="https://raw.githubusercontent.com/llnl/thicket/develop/logo-notext.png" width="64" valign="middle" alt="thicket"/> Thicket
+
+[![Build Status](https://github.com/llnl/thicket/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/llnl/thicket/actions)
+[![Read the Docs](http://readthedocs.org/projects/thicket/badge/?version=latest)](http://thicket.readthedocs.io)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Thicket
 
 A Python-based toolkit for analyzing ensemble performance data.
 
 ### Installation
```

### Comparing `llnl-thicket-2023.1.0/README.md` & `llnl-thicket-2023.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: llnl-thicket
+Version: 2023.2.0
+Summary: Toolkit for exploratory data analysis of ensemble performance data
+License: MIT
+Project-URL: Source Code, https://github.com/LLNL/thicket
+Project-URL: Documentation, https://thicket.readthedocs.io/
+Requires-Python: >=3.6.1
+Description-Content-Type: text/markdown
+Provides-Extra: extrap
+License-File: LICENSE
+License-File: NOTICE
+
+# <img src="https://raw.githubusercontent.com/llnl/thicket/develop/logo-notext.png" width="64" valign="middle" alt="thicket"/> Thicket
+
+[![Build Status](https://github.com/llnl/thicket/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/llnl/thicket/actions)
+[![Read the Docs](http://readthedocs.org/projects/thicket/badge/?version=latest)](http://thicket.readthedocs.io)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # Thicket
 
 A Python-based toolkit for analyzing ensemble performance data.
 
 ### Installation
 
 To use thicket, install it with pip:
```

### Comparing `llnl-thicket-2023.1.0/llnl_thicket.egg-info/PKG-INFO` & `llnl-thicket-2023.2.0/llnl_thicket.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: llnl-thicket
-Version: 2023.1.0
+Version: 2023.2.0
 Summary: Toolkit for exploratory data analysis of ensemble performance data
 License: MIT
 Project-URL: Source Code, https://github.com/LLNL/thicket
 Project-URL: Documentation, https://thicket.readthedocs.io/
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Provides-Extra: extrap
 License-File: LICENSE
 License-File: NOTICE
 
+# <img src="https://raw.githubusercontent.com/llnl/thicket/develop/logo-notext.png" width="64" valign="middle" alt="thicket"/> Thicket
+
+[![Build Status](https://github.com/llnl/thicket/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/llnl/thicket/actions)
+[![Read the Docs](http://readthedocs.org/projects/thicket/badge/?version=latest)](http://thicket.readthedocs.io)
+[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # Thicket
 
 A Python-based toolkit for analyzing ensemble performance data.
 
 ### Installation
 
 To use thicket, install it with pip:
```

### Comparing `llnl-thicket-2023.1.0/llnl_thicket.egg-info/SOURCES.txt` & `llnl-thicket-2023.2.0/llnl_thicket.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,32 @@
 llnl_thicket.egg-info/dependency_links.txt
 llnl_thicket.egg-info/requires.txt
 llnl_thicket.egg-info/top_level.txt
 thicket/__init__.py
 thicket/helpers.py
 thicket/model_extrap.py
 thicket/ncu.py
+thicket/statspreference.py
 thicket/thicket.py
 thicket/utils.py
 thicket/version.py
 thicket/stats/__init__.py
-thicket/stats/calc_average.py
-thicket/stats/calc_corr_nodewise.py
-thicket/stats/calc_deviation.py
-thicket/stats/calc_extremum.py
-thicket/stats/calc_percentiles.py
+thicket/stats/calc_boxplot_statistics.py
 thicket/stats/check_normality.py
+thicket/stats/correlation_nodewise.py
+thicket/stats/display_boxplot.py
 thicket/stats/display_heatmap.py
 thicket/stats/display_histogram.py
+thicket/stats/maximum.py
+thicket/stats/mean.py
+thicket/stats/median.py
+thicket/stats/minimum.py
+thicket/stats/percentiles.py
+thicket/stats/std.py
+thicket/stats/variance.py
 thicket/vis/__init__.py
 thicket/vis/package.json
 thicket/vis/static_fixer.py
 thicket/vis/visualizations.py
 thicket/vis/webpack.config.js
 thicket/vis/scripts/globals.js
 thicket/vis/scripts/treetable.js
```

### Comparing `llnl-thicket-2023.1.0/setup.py` & `llnl-thicket-2023.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/model_extrap.py` & `llnl-thicket-2023.2.0/thicket/model_extrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import base64
+from io import BytesIO
+from statistics import mean
 
 import extrap.entities as xent
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
-# For some reason it errors if "Experiment" is not explicitly imported
-from extrap.entities.experiment import Experiment
+from extrap.entities.experiment import (
+    Experiment,
+)  # For some reason it errors if "Experiment" is not explicitly imported
 from extrap.fileio import io_helper
 from extrap.modelers.model_generator import ModelGenerator
-from io import BytesIO
-from statistics import mean
 
 
 MODEL_TAG = "_extrap-model"
 
 
 class ModelWrapper:
     """Wrapper for an Extra-P model.
 
-    Provides more convenient functions for evaluating the model at given data
-    points, for writing out a string representation of the model, and for
-    displaying (plotting) the model.
+    Provides more convenient functions for evaluating the model at given data points,
+    for writing out a string representation of the model, and for displaying (plotting)
+    the model.
     """
 
     def __init__(self, mdl, param_name):
         self.mdl = mdl
         self.param_name = param_name  # Needed for plotting / displaying the model
 
     def __str__(self):
@@ -88,32 +88,33 @@
 
 class Modeling:
     """Produce models for all the metrics across the given graphframes."""
 
     def __init__(self, tht, param_name, params=None, chosen_metrics=None):
         """Create a new model object.
 
-        Adds a model column for each metric for each common frame across all
-        the graph frames.
+        Adds a model column for each metric for each common frame across all the
+        graphframes.
 
-        The given list of params contains the parameters to build the models.
-        For example, MPI ranks, input sizes, and so on.
+        The given list of params contains the parameters to build the models.  For
+        example, MPI ranks, input sizes, and so on.
 
         Arguments:
             tht (Thicket): thicket object
-            param_name (str): arbitrary if 'params' is being provided, otherwise
-                name of the metadata column from which 'params' will be extracted
+            param_name (str): arbitrary if 'params' is being provided, otherwise name of
+                the metadata column from which 'params' will be extracted
             params (list): parameters list, domain for the model
-            chosen_metrics (list): metrics to be evaluated in the model, range for the model
+            chosen_metrics (list): metrics to be evaluated in the model, range for the
+                model
         """
         self.tht = tht
         self.param_name = param_name
 
         # Assign param
-        # Get params from metadata DataFrames
+        # Get params from metadata table
         if not params:
             self.params = self.tht.metadata[param_name].tolist()
         # params must be provided by the user
         else:
             if not isinstance(params, dict):
                 raise TypeError("'params' must be provided as a dict")
             elif len(params) != len(self.tht.profile):
@@ -145,21 +146,22 @@
             figdata_jpg = base64.b64encode(figfile.getvalue()).decode()
             imgstr = '<img src="data:image/jpg;base64,{}" />'.format(figdata_jpg)
             plt.close(fig)
             return imgstr
 
         frm_dict = {met + MODEL_TAG: model_to_img_html for met in self.chosen_metrics}
 
-        # Subset of the statsframes with only the Extra-P columns selected
+        # Subset of the aggregated statistics table with only the Extra-P columns selected
         return self.tht.statsframe.dataframe[
             [met + MODEL_TAG for met in self.chosen_metrics]
         ].to_html(escape=False, formatters=frm_dict)
 
     def _add_extrap_statistics(self, node, metric):
-        """Insert the Extra-P hypothesis function statistics into the statsframe. Has to be called after "produce_models".
+        """Insert the Extra-P hypothesis function statistics into the aggregated
+            statistics table. Has to be called after "produce_models".
 
         Arguments:
             node (hatchet.Node): The node for which statistics should be calculated
             metric (str): The metric for which statistics should be calculated
         """
         hypothesis_fn = self.tht.statsframe.dataframe.at[
             node, metric + MODEL_TAG
@@ -178,35 +180,37 @@
             node, metric + "_AR2" + MODEL_TAG
         ] = hypothesis_fn.AR2
         self.tht.statsframe.dataframe.at[
             node, metric + "_RE" + MODEL_TAG
         ] = hypothesis_fn.RE
 
     def produce_models(self, agg_func=mean, add_stats=True):
-        """Produces an Extra-P model. Models are generated by calling Extra-P's ModelGenerator.
+        """Produces an Extra-P model. Models are generated by calling Extra-P's
+            ModelGenerator.
 
         Arguments:
-            agg_func (function): aggregation function to apply to
-                multi-dimensional measurement values. Extra-P v4.0.4 applies
-                mean by default so that is set here for clarity.
-            add_stats (bool): Option to add hypothesis function statistics to the statsframe
+            agg_func (function): aggregation function to apply to multi-dimensional
+                measurement values. Extra-P v4.0.4 applies mean by default so that is
+                set here for clarity.
+            add_stats (bool): Option to add hypothesis function statistics to the
+                aggregated statistics table
         """
         # Setup domain values one time. Have to match ordering with range
-        # values (i.e. ensembleframe profile ordering)
+        # values (i.e. performance data table profile ordering)
         param_coords = []  # default coordinates for all profiles
 
         # Mapping from metadata profiles to the parameter
         meta_param_mapping = self.tht.metadata[self.param_name].to_dict()
 
         # Flipped version of mapping dictionary
         meta_param_mapping_flipped = dict(
             [(value, key) for key, value in meta_param_mapping.items()]
         )
 
-        # Ordering of profiles in the ensembleframe
+        # Ordering of profiles in the performance data table
         ensemble_profile_ordering = list(self.tht.dataframe.index.unique(level=1))
 
         # Append coordinates in order
         for profile in ensemble_profile_ordering:
             param_coords.append(
                 xent.coordinate.Coordinate(float(meta_param_mapping[profile]))
             )
@@ -270,15 +274,15 @@
                 # Generate model
                 model_gen = ModelGenerator(exp)
                 model_gen.model_all()
                 mkey = (cpath, metric_obj)
                 self.tht.statsframe.dataframe.at[node, met + MODEL_TAG] = ModelWrapper(
                     model_gen.models[mkey], self.param_name
                 )
-                # Add statistics to statsframe
+                # Add statistics to aggregated statistics table
                 if add_stats:
                     self._add_extrap_statistics(node, met)
 
     def _componentize_function(model_object):
         """Componentize one Extra-P modeling object into a dictionary of its parts
 
         Arguments:
@@ -300,32 +304,35 @@
             variable_column = " * ".join(t.to_string() for t in term.simple_terms)
 
             term_dict[variable_column] = term.coefficient
 
         return term_dict
 
     def componentize_statsframe(self, columns=None):
-        """Componentize multiple Extra-P modeling objects in the statsframe
+        """Componentize multiple Extra-P modeling objects in the aggregated statistics
+        table
 
         Arguments:
-            column (list): list of column names in the statsframe to componentize.
-                Values must be of type 'thicket.model_extrap.ModelWrapper'.
+            column (list): list of column names in the aggregated statistics table to
+                componentize. Values must be of type 'thicket.model_extrap.ModelWrapper'.
         """
         # Use all Extra-P columns
         if columns is None:
             columns = [
                 col
                 for col in self.tht.statsframe.dataframe
                 if isinstance(self.tht.statsframe.dataframe[col][0], ModelWrapper)
             ]
 
         # Error checking
         for c in columns:
             if c not in self.tht.statsframe.dataframe.columns:
-                raise ValueError("column " + c + " is not in the statsframe.")
+                raise ValueError(
+                    "column " + c + " is not in the aggregated statistics table."
+                )
             elif not isinstance(self.tht.statsframe.dataframe[c][0], ModelWrapper):
                 raise TypeError(
                     "column "
                     + c
                     + " is not the right type (thicket.model_extrap.ModelWrapper)."
                 )
```

### Comparing `llnl-thicket-2023.1.0/thicket/ncu.py` & `llnl-thicket-2023.2.0/thicket/ncu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,124 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
-import ncu_report
 import re
+from collections import defaultdict
 
 import pandas as pd
-
-from collections import defaultdict
+import ncu_report
 
 
-def add_ncu_metrics(thicket, ncu_report_file, chosen_metrics=None):
-    """Add metrics from one ncu report file to one thicket"""
+def add_ncu_metrics(th, ncu_report_mapping, chosen_metrics=None):
+    """Add metrics from one ncu report file to one thicket
 
-    # Load kernels
-    report = ncu_report.load_report(ncu_report_file)
-    kernels = report[0]
-
-    # Mapping from node names to kernels
-    nodes = thicket.dataframe.index.get_level_values("node").tolist()
-    names = thicket.dataframe["name"]
-    cpu_side_kernels = {}
-    for i in range(len(nodes)):
-        if nodes[i].frame["type"] == "kernel":
-            cpu_side_kernels[names[i]] = nodes[i]
-
-    # Pre-processing
-    # Remove warmup kernels
-    warmup_end_idx = 0
-    i = 0
-    first_warmup_kernel = kernels[0]
-    same_kernel = True
-    for i in range(1, len(kernels)):
-        if kernels[i].name(kernels[i].NameBase_DEMANGLED) != first_warmup_kernel.name(
-            first_warmup_kernel.NameBase_DEMANGLED
-        ):
-            same_kernel = False
-        if not same_kernel and kernels[i].name(
-            kernels[i].NameBase_DEMANGLED
-        ) == first_warmup_kernel.name(first_warmup_kernel.NameBase_DEMANGLED):
-            warmup_end_idx = i
-            break
-    remove_warmup_kernels = kernels[warmup_end_idx:]
-    # Remove duplicate kernels
-    remove_dupe_kernels = []
-    for kernel in remove_warmup_kernels:
-        dupe = False
-        for other_kernel in remove_dupe_kernels:
-            if other_kernel.name(kernel.NameBase_DEMANGLED) == kernel.name(
-                kernel.NameBase_DEMANGLED
-            ):
-                dupe = True
-        if not dupe:
-            remove_dupe_kernels.append(kernel)
-
-    # Dictionary for metric values
-    data_dict = defaultdict(list)
-    # Matches everything between "<>"
-    regex_str = r".*?\<(.*)\>.*"
-    # For assertion
-    first_kernel_metric_count = len(remove_dupe_kernels[0].metric_names())
-    # Match kernels and add data
-    for kernel in remove_dupe_kernels:
-        kernel_name = kernel.name(kernel.NameBase_DEMANGLED)
-        kernel_match = re.search(regex_str, kernel_name).group(1)
-        ncu_side_kernel = kernel_name.replace(kernel_match, "").replace(" ", "")
-        matches = []
-        for other_kernel in cpu_side_kernels:
-            k_match = re.search(regex_str, other_kernel).group(1)
-            cpu_side_kernel = other_kernel.replace(k_match, "").replace(" ", "")
-            if ncu_side_kernel == cpu_side_kernel:
-                matches.append(cpu_side_kernels[other_kernel])
-                # Remove entry since it should not be re-useable
-                cpu_side_kernels.pop(other_kernel)
+    Arguments:
+        th (Thicket): Thicket object
+        ncu_report_mapping (dict): dictionary mapping from "NCU report file":"Thicket
+            profile"
+        chosen_metrics (str): If known, which NCU metrics to add
+    """
+    # Keep list of NCU dfs for concat
+    ncu_df_list = []
+
+    # Loop through dict
+    for ncu_report_file in ncu_report_mapping:
+        # Hash value that should exist in th
+        ncu_hash = hash(ncu_report_mapping[ncu_report_file])
+
+        # Load kernels
+        report = ncu_report.load_report(ncu_report_file)
+        kernels = report[0]
+
+        # Mapping from node names to kernels
+        nodes = th.dataframe.index.get_level_values("node").tolist()
+        names = th.dataframe["name"]
+        cpu_side_kernels = {}
+        for i in range(len(nodes)):
+            if nodes[i].frame["type"] == "kernel":
+                cpu_side_kernels[names[i]] = nodes[i]
+
+        # Pre-processing
+        # Remove warmup kernels
+        warmup_end_idx = 0
+        i = 0
+        first_warmup_kernel = kernels[0]
+        same_kernel = True
+        for i in range(1, len(kernels)):
+            if kernels[i].name(
+                kernels[i].NameBase_DEMANGLED
+            ) != first_warmup_kernel.name(first_warmup_kernel.NameBase_DEMANGLED):
+                same_kernel = False
+            if not same_kernel and kernels[i].name(
+                kernels[i].NameBase_DEMANGLED
+            ) == first_warmup_kernel.name(first_warmup_kernel.NameBase_DEMANGLED):
+                warmup_end_idx = i
                 break
-        if len(matches) == 0:
-            print("Could not match", kernel_name)
-            continue
-        # Add metrics from NCU side
-        data_dict["node"].append(matches[0])
-        metrics = [kernel[name] for name in kernel.metric_names()]
-        # Undefined behavior if this isn't true. We assume all kernels have same amount of metrics in the same order.
-        assert len(metrics) == first_kernel_metric_count
-        for metric in metrics:
-            data_dict[metric.name()].append(metric.value())
+        remove_warmup_kernels = kernels[warmup_end_idx:]
+        # Remove duplicate kernels
+        remove_dupe_kernels = []
+        for kernel in remove_warmup_kernels:
+            dupe = False
+            for other_kernel in remove_dupe_kernels:
+                if other_kernel.name(kernel.NameBase_DEMANGLED) == kernel.name(
+                    kernel.NameBase_DEMANGLED
+                ):
+                    dupe = True
+            if not dupe:
+                remove_dupe_kernels.append(kernel)
+
+        # Dictionary for metric values
+        data_dict = defaultdict(list)
+        # Matches everything between "<>"
+        regex_str = r".*?\<(.*)\>.*"
+        # For assertion
+        first_kernel_metric_count = len(remove_dupe_kernels[0].metric_names())
+        # Match kernels and add data
+        for kernel in remove_dupe_kernels:
+            kernel_name = kernel.name(kernel.NameBase_DEMANGLED)
+            kernel_match = re.search(regex_str, kernel_name).group(1)
+            ncu_side_kernel = kernel_name.replace(kernel_match, "").replace(" ", "")
+            matches = []
+            for other_kernel in cpu_side_kernels:
+                k_match = re.search(regex_str, other_kernel).group(1)
+                cpu_side_kernel = other_kernel.replace(k_match, "").replace(" ", "")
+                if ncu_side_kernel == cpu_side_kernel:
+                    matches.append(cpu_side_kernels[other_kernel])
+                    # Remove entry since it should not be re-usable
+                    cpu_side_kernels.pop(other_kernel)
+                    break
+            if len(matches) == 0:
+                print(f"Could not match {kernel_name}")
+                continue
+            # Add metrics from NCU side
+            data_dict["node"].append(matches[0])
+            metrics = [kernel[name] for name in kernel.metric_names()]
+            # Undefined behavior if this isn't true. We assume all kernels have same amount of metrics in the same order.
+            assert len(metrics) == first_kernel_metric_count
+            for metric in metrics:
+                data_dict[metric.name()].append(metric.value())
+
+        # Create NCU df
+        ncu_df = pd.DataFrame.from_dict(data_dict)
+        ncu_df["profile"] = ncu_hash
+        ncu_df.set_index(["node", "profile"], inplace=True)
+
+        # Get subset of metrics
+        if chosen_metrics:
+            ncu_df = ncu_df[chosen_metrics]
 
-    ncu_df = pd.DataFrame.from_dict(data_dict)
-    ncu_df.set_index("node", inplace=True)
+        # Append df to list
+        ncu_df_list.append(ncu_df)
 
-    if chosen_metrics:
-        ncu_df = ncu_df[chosen_metrics]
+    # First join NCU dfs
+    ncu_df = pd.concat(ncu_df_list)
 
-    # Join thicket and NCU dfs
-    thicket.dataframe = thicket.dataframe.join(
+    # Join Thicket and NCU dfs
+    th.dataframe = th.dataframe.join(
         ncu_df,
         how="outer",
         sort=True,
         lsuffix="_left",
         rsuffix="_right",
     )
```

### Comparing `llnl-thicket-2023.1.0/thicket/stats/calc_deviation.py` & `llnl-thicket-2023.2.0/thicket/stats/std.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,31 +2,50 @@
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 import pandas as pd
 
+from ..utils import verify_thicket_structures
 
-def calc_deviation(thicket=None, columns=None):
-    """Calculate standard deviation and variance per node.
 
-    Designed to take in a Thicket, and will append a column to the statsframe
-    for the standard deviation and variance calculations per node.
+def std(thicket, columns=None):
+    """Calculate the standard deviation for each node in the performance data table.
 
-    Variance will allow you to see the spread within a dataset and standard
-    deviation will tell you how dispersed the data is in relation to the mean.
+    Designed to take in a thicket, and append one or more columns to the aggregated
+    statistics table for the standard deviation calculation for each node.
+
+    Standard deviation describes how dispersed the data is in relation to the mean.
 
     Arguments:
         thicket (thicket): Thicket object
-        columns (list): list of hardware/timing metrics to perform deviation calculations on
+        columns (list): List of hardware/timing metrics to perform standard deviation
+            calculation on. Note, if using a columnar_joined thicket a list of tuples
+            must be passed in with the format (column index, column name).
     """
-    for column in columns:
-        var = []
-        std = []
-        for node in pd.unique(thicket.dataframe.reset_index()["node"].tolist()):
-            var_value = np.var(thicket.dataframe.loc[node][column])
-            std_value = np.std(thicket.dataframe.loc[node][column])
-            var.append(var_value)
-            std.append(std_value)
-        thicket.statsframe.dataframe[column + "_var"] = var
-        thicket.statsframe.dataframe[column + "_std"] = std
+    if columns is None:
+        raise ValueError(
+            "To see a list of valid columns, please run Thicket.get_perf_columns()."
+        )
+
+    verify_thicket_structures(
+        thicket.dataframe, index=["node", "profile"], columns=columns
+    )
+
+    # thicket object without columnar index
+    if thicket.dataframe.columns.nlevels == 1:
+        for column in columns:
+            std = []
+            for node in pd.unique(thicket.dataframe.reset_index()["node"].tolist()):
+                std.append(np.std(thicket.dataframe.loc[node][column]))
+            thicket.statsframe.dataframe[column + "_std"] = std
+    # columnar joined thicket object
+    else:
+        for idx, column in columns:
+            std = []
+            for node in pd.unique(thicket.dataframe.reset_index()["node"].tolist()):
+                std.append(np.std(thicket.dataframe.loc[node][(idx, column)]))
+            thicket.statsframe.dataframe[(idx, column + "_std")] = std
+
+        # sort columns in index
+        thicket.statsframe.dataframe = thicket.statsframe.dataframe.sort_index(axis=1)
```

### Comparing `llnl-thicket-2023.1.0/thicket/stats/calc_extremum.py` & `llnl-thicket-2023.2.0/thicket/stats/display_heatmap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,57 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
-import pandas as pd
+import seaborn as sns
 
+from ..utils import verify_thicket_structures
 
-def calc_extremum(thicket=None, columns=None):
-    """Calculate min and max per node.
 
-    Designed to take in a Thicket, and will append a column to the statsframe
-    for the min and max calculations per node.
-
-    The minimum is the lowest observation and the maxiumum is the highest
-    observation in the dataset.
+def display_heatmap(thicket, columns=None, **kwargs):
+    """Display a heatmap which contains a full list of nodes and user passed columns.
+    Columns must be from the aggregated statistics table.
 
     Arguments:
         thicket (thicket): Thicket object
-        columns (list): list of hardware/timing metrics to perform extremnum calculations on
+        columns (list): List of hardware/timing metrics from aggregated statistics table
+            to display. Note, if using a columnar joined thicket a list of tuples must
+            be passed in with the format (column index, column name).
+
+    Returns:
+        (matplotlib Axes): Object for managing heatmap plot.
     """
-    for column in columns:
-        minimum = []
-        maximum = []
-        for node in pd.unique(thicket.dataframe.reset_index()["node"].tolist()):
-            min_value = min(thicket.dataframe.loc[node][column])
-            max_value = max(thicket.dataframe.loc[node][column])
-            minimum.append(min_value)
-            maximum.append(max_value)
-        thicket.statsframe.dataframe[column + "_min"] = minimum
-        thicket.statsframe.dataframe[column + "_max"] = maximum
+    if columns is None:
+        raise ValueError(
+            "To see a list of valid columns, run Thicket.get_perf_columns()."
+        )
+
+    verify_thicket_structures(
+        thicket.statsframe.dataframe, index=["node"], columns=columns
+    )
+
+    # thicket object without columnar index
+    if thicket.dataframe.columns.nlevels == 1:
+        thicket.statsframe.dataframe.index = thicket.statsframe.dataframe.index.map(str)
+        ax = sns.heatmap(thicket.statsframe.dataframe[columns], **kwargs)
+
+        return ax
+    # columnar joined thicket object
+    else:
+        thicket.statsframe.dataframe.index = thicket.statsframe.dataframe.index.map(str)
+
+        initial_idx = columns[0][0]
+        cols = [columns[0][1]]
+        for i in range(1, len(columns)):
+            if initial_idx != columns[i][0]:
+                raise ValueError(
+                    "Columns specified as tuples must have the same column index (first element)."
+                )
+            else:
+                cols.append(columns[i][1])
+
+        ax = sns.heatmap(
+            thicket.statsframe.dataframe[initial_idx][cols], **kwargs
+        ).set_title(initial_idx)
+
+        return ax
```

### Comparing `llnl-thicket-2023.1.0/thicket/thicket.py` & `llnl-thicket-2023.2.0/thicket/thicket.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,95 +3,122 @@
 #
 # SPDX-License-Identifier: MIT
 
 import copy
 import os
 import json
 import warnings
+from collections import OrderedDict
 
 import pandas as pd
 import numpy as np
-
-from collections import OrderedDict
 from hatchet import GraphFrame
 from hatchet.query import AbstractQuery
-from .helpers import print_graph
+
+import thicket.helpers as helpers
+from .utils import verify_sorted_profile
 from .utils import verify_thicket_structures
 
 
 class Thicket(GraphFrame):
-    """Ensemble of profiles, includes a graph and three dataframes, ensemble
-    data, metadata, and statistics."""
+    """Ensemble of profiles, includes a graph and three dataframes, performance data,
+    metadata, and aggregated statistics.
+    """
 
     def __init__(
         self,
         graph,
         dataframe,
         exc_metrics=None,
         inc_metrics=None,
         default_metric="time",
         metadata={},
+        performance_cols=None,
         profile=None,
         profile_mapping=None,
         statsframe=None,
     ):
         """Create a new thicket from a graph and a dataframe.
 
         Arguments:
             graph (Graph): graph of nodes in this thicket
-            dataframe (DataFrame): pandas DataFrame indexed by Nodes from the
-                graph, and potentially other indexes
+            dataframe (DataFrame): pandas DataFrame indexed by Nodes from the graph, and
+                potentially other indexes
             exc_metrics (list): list of names of exclusive metrics in the dataframe
             inc_metrics (list): list of names of inclusive metrics in the dataframe
             default_metric (str): primary metric
-            metadata (DataFrame): pandas DataFrame indexed by profile hashes,
-                contains profile metadata
+            metadata (DataFrame): pandas DataFrame indexed by profile hashes, contains
+                profile metadata
+            performance_cols (list): list of numeric columns within the performance
+                dataframe
             profile (list): list of hashed profile strings
             profile_mapping (dict): mapping of hashed profile strings to original strings
-            statsframe (DataFrame): pandas DataFrame indexed by Nodes from the
-                graph
+            statsframe (DataFrame): pandas DataFrame indexed by Nodes from the graph
         """
         super().__init__(
             graph, dataframe, exc_metrics, inc_metrics, default_metric, metadata
         )
         self.profile = profile
         self.profile_mapping = profile_mapping
         if statsframe is None:
-            # Drop duplicates based on nid
-            subset_df = dataframe["name"].reset_index().drop_duplicates(subset=["node"])
             self.statsframe = GraphFrame(
                 graph=self.graph,
-                dataframe=pd.DataFrame(
-                    index=subset_df["node"],
-                    data={"name": subset_df["name"].values},
-                ),
+                dataframe=helpers._new_statsframe_df(dataframe),
             )
         else:
             self.statsframe = statsframe
 
+        self.performance_cols = helpers._get_perf_columns(self.dataframe)
+
+    def __eq__(self, other):
+        """Compare two thicket objects.
+
+        Arguments:
+            other (Thicket): Thicket object to compare to
+
+        Returns:
+            (bool): True if equal, False otherwise
+        """
+        assert isinstance(other, Thicket)
+        return (
+            self.graph == other.graph
+            and self.dataframe.equals(other.dataframe)
+            and self.exc_metrics == other.exc_metrics
+            and self.inc_metrics == other.inc_metrics
+            and self.default_metric == other.default_metric
+            and self.metadata.equals(other.metadata)
+            and self.performance_cols == other.performance_cols
+            and self.profile == other.profile
+            and self.profile_mapping == other.profile_mapping
+            and self.statsframe.graph == other.statsframe.graph
+            and self.statsframe.dataframe.equals(other.statsframe.dataframe)
+        )
+
     def __str__(self):
         s = (
             "graph: "
-            + print_graph(self.graph)
+            + helpers._print_graph(self.graph)
             + "\ndataframe:\n"
             + self.dataframe
             + "\nexc_metrics: "
             + self.exc_metrics
             + "\ninc_metrics: "
             + self.inc_metrics
             + "\ndefault_metric: "
             + self.default_metric
             + "\nmetadata:\n"
             + self.metadata
+            + "\nperformance_cols:\n"
+            + self.performance_cols
             + "\nprofile: "
             + self.profile
             + "\nprofile_mapping: "
             + self.profile_mapping
             + "\nstatsframe:\n"
-            + print_graph(self.statsframe.graph)
+            + helpers._print_graph(self.statsframe.graph)
             + "\n"
             + self.statsframe.dataframe
         )
 
         return s
 
     @staticmethod
@@ -132,27 +159,27 @@
         return th
 
     @staticmethod
     def from_caliper(filename_or_stream, query=None, intersection=False):
         """Read in a Caliper .cali or .json file.
 
         Arguments:
-            filename_or_stream (str or file-like): name of a Caliper output
-                file in `.cali` or JSON-split format, or an open file object
-                to read one
+            filename_or_stream (str or file-like): name of a Caliper output file in
+                `.cali` or JSON-split format, or an open file object to read one
             query (str): cali-query in CalQL format
             intersection (bool): whether to perform intersection or union (default)
         """
         return Thicket.reader_dispatch(
             GraphFrame.from_caliper, intersection, filename_or_stream, query
         )
 
     @staticmethod
     def from_hpctoolkit(dirname, intersection=False):
-        """Create a GraphFrame using hatchet's HPCToolkit reader and use its attributes to make a new thicket.
+        """Create a GraphFrame using hatchet's HPCToolkit reader and use its attributes
+        to make a new thicket.
 
         Arguments:
             dirname (str): parent directory of an HPCToolkit experiment.xml file
             intersection (bool): whether to perform intersection or union (default)
 
         Returns:
             (thicket): new thicket containing HPCToolkit profile data
@@ -162,16 +189,16 @@
         )
 
     @staticmethod
     def from_caliperreader(filename_or_caliperreader, intersection=False):
         """Helper function to read one caliper file.
 
         Arguments:
-            filename_or_caliperreader (str or CaliperReader): name of a Caliper
-                output file in `.cali` format, or a CaliperReader object
+            filename_or_caliperreader (str or CaliperReader): name of a Caliper output
+                file in `.cali` format, or a CaliperReader object
             intersection (bool): whether to perform intersection or union (default)
         """
         return Thicket.reader_dispatch(
             GraphFrame.from_caliperreader, intersection, filename_or_caliperreader
         )
 
     @staticmethod
@@ -249,131 +276,301 @@
             }
             th.statsframe = GraphFrame.from_json(json.dumps(sf_spec))
             th.statsframe.graph = th.graph
 
         # make and return thicket?
         return th
 
-    def add_column_from_metadata_to_ensemble(self, column_name, overwrite=False):
-        """Add a column from the MetadataFrame to the EnsembleFrame.
+    @staticmethod
+    def columnar_join(
+        thicket_list,
+        header_list=None,
+        column_name=None,
+    ):
+        """Join Thickets column-wise. New column multi-index will be created with
+        columns under separate indexer headers.
+
+        Arguments:
+            thicket_list (list): List of Thickets to join
+            header_list (list): List of headers to use for the new columnar multi-index
+            column_name (str): Name of the column from the metadata table to join on. If
+                no argument is provided, it is assumed that there is no profile-wise
+                relationship between self and other.
+
+        Returns:
+            (Thicket): New Thicket object with joined columns
+        """
+
+        def _create_multiindex_columns(df, upper_idx_name):
+            """Helper function to create multi-index column names from a dataframe's
+            current columns.
+
+            Arguments:
+            df (DataFrame): source dataframe
+            upper_idx_name (String): name of the newly added index in the multi-index.
+                Prepended before each column as a tuple.
+
+            Returns:
+                (list): list of new indicies generated from the source dataframe
+            """
+            new_idx = []
+            for column in df.columns:
+                new_tuple = (upper_idx_name, column)
+                new_idx.append(new_tuple)
+            return new_idx
+
+        ###
+        # Step 0A: Pre-check of data structures
+        ###
+        # Required/expected format of the data
+        for th in thicket_list:
+            verify_thicket_structures(th.dataframe, index=["node", "profile"])
+            verify_thicket_structures(th.statsframe.dataframe, index=["node"])
+            verify_thicket_structures(th.metadata, index=["profile"])
+        # Check for column_name in metadata
+        if column_name:
+            for th in thicket_list:
+                verify_thicket_structures(th.metadata, columns=[column_name])
+        # Check length of profiles match
+        for i in range(len(thicket_list) - 1):
+            if len(thicket_list[i].profile) != len(thicket_list[i + 1].profile):
+                raise ValueError(
+                    "Length of all thicket profiles must match. {} != {}".format(
+                        len(thicket_list[i].profile), len(thicket_list[i + 1].profile)
+                    )
+                )
+        # Ensure all thickets profiles are sorted. Must be true when column_name=None to
+        # guarantee performance data table and metadata table match up.
+        if column_name is None:
+            for th in thicket_list:
+                verify_sorted_profile(th.dataframe)
+                verify_sorted_profile(th.metadata)
+
+        ###
+        # Step 0B: Variable Initialization
+        ###
+        # Initialize combined thicket
+        combined_th = thicket_list[0].deepcopy()
+        # Use copies to be non-destructive
+        thicket_list_cp = [th.deepcopy() for th in thicket_list]
+
+        ###
+        # Step 1: Unify the thickets
+        ###
+        # Unify graphs if "self" and "other" do not have the same graph
+        union_graph = thicket_list_cp[0].graph
+        for i in range(len(thicket_list_cp) - 1):
+            if thicket_list_cp[i].graph != thicket_list_cp[i + 1].graph:
+                union_graph = union_graph.union(thicket_list_cp[i + 1].graph)
+        combined_th.graph = union_graph
+        for i in range(len(thicket_list_cp)):
+            # Set all graphs to the union graph
+            thicket_list_cp[i].graph = union_graph
+            # Necessary to change dataframe hatchet id's to match the nodes in the graph
+            helpers._sync_nodes_frame(union_graph, thicket_list_cp[i].dataframe)
+            # For tree diff. dataframes need to be sorted.
+            thicket_list_cp[i].dataframe.sort_index(inplace=True)
+
+        ###
+        # Step 2: Join "self" & "other" performance data table
+        ###
+        # Create header list if not provided
+        if header_list is None:
+            header_list = [i for i in range(len(thicket_list))]
+
+        # Update index to reflect performance data table index
+        new_mappings = {}  # Dictionary mapping old profiles to new profiles
+        if column_name is None:  # Create index from scratch
+            new_profiles = [i for i in range(len(thicket_list_cp[0].profile))]
+            for i in range(len(thicket_list_cp)):
+                thicket_list_cp[i].metadata["new_profiles"] = new_profiles
+                thicket_list_cp[i].add_column_from_metadata_to_ensemble(
+                    "new_profiles", drop=True
+                )
+                thicket_list_cp[i].dataframe.reset_index(level="profile", inplace=True)
+                new_mappings.update(
+                    pd.Series(
+                        thicket_list_cp[i]
+                        .dataframe["new_profiles"]
+                        .map(lambda x: (x, header_list[i]))
+                        .values,
+                        index=thicket_list_cp[i].dataframe["profile"],
+                    ).to_dict()
+                )
+                thicket_list_cp[i].dataframe.drop("profile", axis=1, inplace=True)
+                thicket_list_cp[i].dataframe.set_index(
+                    "new_profiles", append=True, inplace=True
+                )
+                thicket_list_cp[i].dataframe.index.rename(
+                    "profile", level="new_profiles", inplace=True
+                )
+        else:  # Change second-level index to be from metadata's "column_name" column
+            for i in range(len(thicket_list_cp)):
+                thicket_list_cp[i].add_column_from_metadata_to_ensemble(column_name)
+                thicket_list_cp[i].dataframe.reset_index(level="profile", inplace=True)
+                new_mappings.update(
+                    pd.Series(
+                        thicket_list_cp[i]
+                        .dataframe[column_name]
+                        .map(lambda x: (x, header_list[i]))
+                        .values,
+                        index=thicket_list_cp[i].dataframe["profile"],
+                    ).to_dict()
+                )
+                thicket_list_cp[i].dataframe.drop("profile", axis=1, inplace=True)
+                thicket_list_cp[i].dataframe.set_index(
+                    column_name, append=True, inplace=True
+                )
+                thicket_list_cp[i].dataframe.sort_index(inplace=True)
+
+        # Create tuple columns
+        new_columns = [
+            _create_multiindex_columns(th.dataframe, header_list[i])
+            for i, th in enumerate(thicket_list_cp)
+        ]
+        # Clear old metrics (non-tuple)
+        combined_th.exc_metrics.clear()
+        combined_th.inc_metrics.clear()
+        # Update inc/exc metrics
+        for i in range(len(new_columns)):
+            for col_tuple in new_columns[i]:
+                if col_tuple[1] in thicket_list_cp[i].exc_metrics:
+                    combined_th.exc_metrics.append(col_tuple)
+                if col_tuple[1] in thicket_list_cp[i].inc_metrics:
+                    combined_th.inc_metrics.append(col_tuple)
+        # Update columns
+        for i in range(len(thicket_list_cp)):
+            thicket_list_cp[i].dataframe.columns = pd.MultiIndex.from_tuples(
+                new_columns[i]
+            )
+
+        # Concat performance data table together
+        combined_th.dataframe = pd.concat(
+            [thicket_list_cp[i].dataframe for i in range(len(thicket_list_cp))],
+            axis="columns",
+            join="outer",
+        )
+
+        # Extract "name" columns to upper level
+        nodes = list(set(combined_th.dataframe.reset_index()["node"]))
+        for node in nodes:
+            combined_th.dataframe.loc[node, "name"] = node.frame["name"]
+        combined_th.dataframe.drop(
+            columns=[(header_list[i], "name") for i in range(len(header_list))],
+            inplace=True,
+        )
+
+        ###
+        # Step 3: Join "self" & "other" metadata table
+        ###
+        # Update index to reflect performance data table index
+        for i in range(len(thicket_list_cp)):
+            thicket_list_cp[i].metadata.reset_index(drop=True, inplace=True)
+        if column_name is None:
+            for i in range(len(thicket_list_cp)):
+                thicket_list_cp[i].metadata.index.set_names("profile", inplace=True)
+        else:
+            for i in range(len(thicket_list_cp)):
+                thicket_list_cp[i].metadata.set_index(column_name, inplace=True)
+                thicket_list_cp[i].metadata.sort_index(inplace=True)
+
+        # Create multi-index columns
+        for i in range(len(thicket_list_cp)):
+            thicket_list_cp[i].metadata.columns = pd.MultiIndex.from_tuples(
+                _create_multiindex_columns(thicket_list_cp[i].metadata, header_list[i])
+            )
+
+        # Concat metadata together
+        combined_th.metadata = pd.concat(
+            [thicket_list_cp[i].metadata for i in range(len(thicket_list_cp))],
+            axis="columns",
+            join="outer",
+        )
+
+        ###
+        # Step 4: Update other Thicket objects.
+        ###
+        for i in range(1, len(thicket_list_cp)):
+            combined_th.profile += thicket_list_cp[i].profile  # Update "profile" object
+            combined_th.profile_mapping.update(
+                thicket_list_cp[i].profile_mapping
+            )  # Update "profile_mapping" object
+        combined_th.profile = [new_mappings[prf] for prf in combined_th.profile]
+        profile_mapping_cp = combined_th.profile_mapping.copy()
+        for k, v in profile_mapping_cp.items():
+            combined_th.profile_mapping[
+                new_mappings[k]
+            ] = combined_th.profile_mapping.pop(k)
+
+        # Clear aggregated statistics table
+        combined_th.statsframe = GraphFrame(
+            graph=combined_th.graph,
+            dataframe=helpers._new_statsframe_df(
+                combined_th.dataframe, multiindex=True
+            ),
+        )
+        combined_th.performance_cols = helpers._get_perf_columns(combined_th.dataframe)
+
+        return combined_th
+
+    def add_column_from_metadata_to_ensemble(
+        self, column_name, overwrite=False, drop=False
+    ):
+        """Add a column from the metadata table to the performance data table.
 
         Arguments:
-            column_name (str): jame of the column from the metadataframe
-            overwrite (bool): determines overriding behavior in ensembleframe
+            column_name (str): Name of the column from the metadata table
+            overwrite (bool): Determines overriding behavior in performance data table
+            drop (bool): Whether to drop the column from the metadata table afterwards
         """
-        # Add warning if column already exists in EnsembleFrame
+        # Add warning if column already exists in performance data table
         if column_name in self.dataframe.columns:
             # Drop column to overwrite, otherwise warn and return
             if overwrite:
                 self.dataframe.drop(column_name, axis=1, inplace=True)
             else:
                 warnings.warn(
                     "Column "
                     + column_name
                     + " already exists. Set 'overwrite=True' to force update the column."
                 )
                 return
 
-        # Add the column to the EnsembleFrame
+        # Add the column to the performance data table
         self.dataframe = self.dataframe.join(
             self.metadata[column_name], on=self.dataframe.index.names[1]
         )
 
-    @staticmethod
-    def _sync_nodes_frame(gh, df):
-        """Set the node objects to be equal in both the graph and the dataframe.
-
-        id(graph_node) == id(df_node) after this function for nodes with equivalent hatchet nid's.
-
-        TODO: This function may be superior to _sync_nodes and may be able to replace it. Need to investigate.
-        """
-        index_names = df.index.names
-        df.reset_index(inplace=True)
-        for graph_node in gh.traverse():
-            df["node"] = df["node"].apply(
-                lambda df_node: graph_node
-                if (graph_node.frame == df_node.frame)
-                else df_node
-            )
-        df.set_index(index_names, inplace=True)
-
-    @staticmethod
-    def _missing_nodes_to_list(a_df, b_df):
-        """Get a list of node differences between two dataframes. Mainly used for "tree" function.
-
-        Arguments:
-            a_df (Dataframe): First pandas Dataframe
-            b_df (Dataframe): Second pandas Dataframe
-
-        Returns:
-            (list): List of numbers in range (0, 1, 2). "0" means node is in both, "1" is only in "a", "2" is only in "b"
-        """
-        missing_nodes = []
-        a_list = list(map(hash, list(a_df.index.get_level_values("node"))))
-        b_list = list(map(hash, list(b_df.index.get_level_values("node"))))
-        # Basic cases
-        while a_list and b_list:
-            a = a_list.pop(0)
-            b = b_list.pop(0)
-            while a > b and b_list:
-                missing_nodes.append(2)
-                b = b_list.pop(0)
-            while b > a and a_list:
-                missing_nodes.append(1)
-                a = a_list.pop(0)
-            if a == b:
-                missing_nodes.append(0)
-                continue
-            elif (
-                a > b
-            ):  # Case where last two nodes and "a" is missing "b" then opposite
-                missing_nodes.append(2)
-                missing_nodes.append(1)
-            elif (
-                b > a
-            ):  # Case where last two nodes and "b" is missing "a" then opposite
-                missing_nodes.append(1)
-                missing_nodes.append(2)
-        while a_list:  # In case "a" has a lot more nodes than "b"
-            missing_nodes.append(1)
-            a = a_list.pop(0)
-        while b_list:  # In case "b" has a lot more nodes than "a"
-            missing_nodes.append(2)
-            b = b_list.pop(0)
-        return missing_nodes
-
-    def squash(self, preserve_stats_dataframe=False):
-        """Rewrite the Graph to include only nodes present in the performance DataFrame's rows.
+        # Drop column
+        if drop:
+            self.metadata.drop(column_name, axis=1, inplace=True)
+
+    def squash(self, update_inc_cols=True):
+        """Rewrite the Graph to include only nodes present in the performance
+        data table's rows.
 
-        This can be used to simplify the Graph, or to normalize Graph indexes
-        between two Thickets.
+        This can be used to simplify the Graph, or to normalize Graph indexes between
+        two Thickets.
 
         Arguments:
-            preserve_stats_dataframe (bool): if true, use the existing DataFrame in the statsframe. Otherwise,
-                                             create a new, empty statsframe for the squashed Thicket object.
+            update_inc_cols (boolean, optional): if True, update inclusive columns.
 
         Returns:
             (Thicket): a newly squashed Thicket object
         """
-        squashed_gf = GraphFrame.squash(self)
+        squashed_gf = GraphFrame.squash(self, update_inc_cols=update_inc_cols)
         new_graph = squashed_gf.graph
-        # The following code updates the performance data and the statsframe with the remaining (re-indexed) nodes.
-        # The dataframe is internally updated in squash(), so we can easily just save it to our thicket perfdata.
-        # For the statsframe, we'll have to come up with a better way eventually, but for now, we'll just create
-        #    a new statsframe the same way we do when we create a new thicket.
+        # The following code updates the performance data and the aggregated statistics
+        # table with the remaining (re-indexed) nodes. The dataframe is internally
+        # updated in squash(), so we can easily just save it to our thicket performance
+        # data. For the aggregated statistics table, we'll have to come up with a better
+        # way eventually, but for now, we'll just create a new aggregated statistics
+        # table the same way we do when we create a new thicket.
         new_dataframe = squashed_gf.dataframe
-        stats_df = self.statsframe.dataframe
-        if not preserve_stats_dataframe:
-            subset_df = (
-                new_dataframe["name"].reset_index().drop_duplicates(subset=["node"])
-            )
-            stats_df = pd.DataFrame(
-                index=subset_df["node"],
-                data={"name": subset_df["name"].values},
-            )
+        stats_df = helpers._new_statsframe_df(new_dataframe)
         sframe = GraphFrame(
             graph=new_graph,
             dataframe=stats_df,
         )
         return Thicket(
             new_graph,
             new_dataframe,
@@ -382,142 +579,14 @@
             default_metric=self.default_metric,
             metadata=self.metadata,
             profile=self.profile,
             profile_mapping=self.profile_mapping,
             statsframe=sframe,
         )
 
-    def columnar_join(self, other, column_name, self_new_name, other_new_name):
-        """Join two Thickets column-wise. New column multi-index will be created with self and other's columns under separate indexers.
-
-        Arguments:
-            self (Thicket): left-side thicket
-            other (Thicket): right-side thicket
-            column_name (str): Name of the column from the metadataframe to join on
-            self_new_name (str): The name for self's new upper-level columnar multi-index
-            other_new_name (str): The name for other's new upper-level columnar multi-index
-
-        Returns:
-            (Thicket): New thicket with joined DataFrame
-        """
-        # Pre-check of data structures
-        # Required for deepcopy operation
-        verify_thicket_structures(self.dataframe, index=["node", "profile"])
-        verify_thicket_structures(self.statsframe.dataframe, index=["node"])
-        verify_thicket_structures(self.metadata, index=["profile"])
-        # For joining with "self"
-        verify_thicket_structures(other.dataframe, index=["node", "profile"])
-        verify_thicket_structures(other.statsframe.dataframe, index=["node"])
-        verify_thicket_structures(other.metadata, index=["profile"])
-
-        # For tree diff
-        missing_nodes = None
-        # Initialize combined thicket
-        combined_th = self.deepcopy()
-        # Use copies to be non-destructive
-        self_cp = self.deepcopy()
-        other_cp = other.deepcopy()
-
-        # Create profile index mapping from metadata
-        self_map_flipped = {
-            v: k for k, v in self_cp.metadata[column_name].to_dict().items()
-        }
-        other_map = other.metadata[column_name].to_dict()
-        other_self_map = {
-            k: self_map_flipped[other_map[k]] for k, v in other_map.items()
-        }
-        # Apply index mapping to other dataframe
-        other_cp.dataframe = other.dataframe.rename(
-            index=other_self_map, level="profile"
-        )
-        Thicket._sync_nodes_frame(
-            other_cp.graph, other_cp.dataframe
-        )  # Sync nodes between graph and dataframe
-
-        # Unify graphs if "self" and "other" do not have the same graph
-        if self_cp.graph != other_cp.graph:
-            union_graph = self_cp.graph.union(other_cp.graph)
-            combined_th.graph = union_graph
-            self_cp.graph = union_graph
-            other_cp.graph = union_graph
-
-            # Necessary to change dataframe hatchet id's to match the nodes in the graph
-            Thicket._sync_nodes_frame(self_cp.graph, self_cp.dataframe)
-            Thicket._sync_nodes_frame(other_cp.graph, other_cp.dataframe)
-
-            # For tree diff. DataFrames need to be sorted.
-            self_cp.dataframe.sort_index(inplace=True)
-            other_cp.dataframe.sort_index(inplace=True)
-            missing_nodes = Thicket._missing_nodes_to_list(
-                self_cp.dataframe, other_cp.dataframe
-            )
-
-        # Concatenate combined dataframe column-wise. Assumes row-wise alignment in respect to nodes
-        combined_th.dataframe = self_cp.dataframe.join(
-            other_cp.dataframe,
-            how="outer",
-            sort=True,
-            lsuffix="_left",
-            rsuffix="_right",
-        )
-
-        # Fix renaming of duplicate columns since pandas requires it in "join" function. #TODO: Figure out how to join without renaming. This would remove this step.
-        rename_dict = {}
-        for column in combined_th.dataframe.columns:
-            if "_left" in column:
-                rename_dict[column] = column.replace("_left", "")
-            elif "_right" in column:
-                rename_dict[column] = column.replace("_right", "")
-        combined_th.dataframe.rename(columns=rename_dict, inplace=True)
-
-        # Change second-level index to be from metadata's "column_name" column
-        combined_th.add_column_from_metadata_to_ensemble(column_name)
-        combined_th.dataframe.reset_index(level="profile", drop=True, inplace=True)
-        combined_th.dataframe.set_index(column_name, append=True, inplace=True)
-        combined_th.dataframe.sort_index(inplace=True)
-        # Create new columnar multi-index for "self" and "other"
-        new_idx = []
-        for column in self_cp.dataframe.columns:
-            new_idx.append((self_new_name, column))
-        for column in other_cp.dataframe.columns:
-            new_idx.append((other_new_name, column))
-        combined_th.dataframe.columns = pd.MultiIndex.from_tuples(new_idx)
-
-        # Join "self" & "other" metadata frames
-        combined_th.metadata = pd.concat([self_cp.metadata, other_cp.metadata])
-        # Update "profile" object
-        combined_th.profile += other_cp.profile
-        # Update "profile_mapping" object
-        combined_th.profile_mapping.update(other_cp.profile_mapping)
-
-        # Clear statsframe
-        subset_df = (
-            combined_th.dataframe[(self_new_name, "name")]
-            .combine_first(combined_th.dataframe[(other_new_name, "name")])
-            .rename("name")
-            .reset_index()
-            .drop_duplicates(subset=["node"])
-        )
-        combined_th.statsframe = GraphFrame(
-            graph=combined_th.graph,
-            dataframe=pd.DataFrame(
-                index=subset_df["node"],
-                data={"name": subset_df["name"].values},
-            ),
-        )
-
-        # For tree diff
-        if missing_nodes:
-            try:
-                combined_th.dataframe["_missing_node"] = missing_nodes
-            except Exception:
-                warnings.warn("Unable to add '_missing_node' column.")
-
-        return combined_th
-
     def copy(self):
         """Return a partially shallow copy of the Thicket.
 
         See GraphFrame.copy() for more details
 
         Arguments:
             self (Thicket): object to make a copy of
@@ -572,46 +641,28 @@
             profile=copy.deepcopy(self.profile),
             profile_mapping=copy.deepcopy(self.profile_mapping),
             statsframe=self.statsframe.deepcopy(),
         )
 
     def tree(self):
         """hatchet tree() function for a thicket"""
-        try:
-            if isinstance(self.dataframe.columns, pd.MultiIndex):
-                t_set = set(self.dataframe.columns.get_level_values(0))
-                t_set.remove("_missing_node")
-                name_1, name_2 = t_set
-                temp_df = (
-                    self.dataframe[(name_1, "name")]
-                    .combine_first(self.dataframe[(name_2, "name")])
-                    .rename("name")
-                    .reset_index()
-                    .drop_duplicates(subset=["node"])
-                )
-                temp_df["_missing_node"] = self.dataframe["_missing_node"].to_list()[
-                    :: len(self.profile)
-                ]
-                temp_df.set_index("node", inplace=True)
-            else:
-                temp_df = self.dataframe.drop_duplicates(subset="name").reset_index(
-                    level="profile"
-                )
-            temp_df["thicket_tree"] = -1
-            return GraphFrame.tree(
-                self=Thicket(graph=self.graph, dataframe=temp_df),
-                metric_column="thicket_tree",
-            )
-        except KeyError:
-            raise NotImplementedError(
-                "Printing this collection of profiles is not supported."
-            )
+        temp_df = self.statsframe.dataframe.copy()
+        # Adjustments specific for multi-index.
+        if isinstance(temp_df.columns, pd.MultiIndex):
+            temp_df.columns = temp_df.columns.to_flat_index()
+            temp_df.rename(columns={("", "name"): "name"}, inplace=True)
+        # Placeholder value. TODO: Enable selection from performance data table.
+        temp_df["thicket_tree"] = -1
+        return GraphFrame.tree(
+            self=Thicket(graph=self.graph, dataframe=temp_df),
+            metric_column="thicket_tree",
+        )
 
     def unify_pair(self, other):
-        """Unify two Thicket's graphs and DataFrames"""
+        """Unify two Thicket's graphs and dataframes"""
         # Check for the same object. Cheap operation since no graph walkthrough.
         if self.graph is other.graph:
             print("same graph (object)")
             return self.graph
 
         # Check for the same graph structure. Need to walk through graphs *but should
         # still be less expensive then performing the rest of this function.*
@@ -639,43 +690,62 @@
         other.dataframe.set_index(other_index_names, inplace=True)
 
         self.graph = union_graph
         other.graph = union_graph
 
         return union_graph
 
-    def unify_pairwise(th_list):
+    @staticmethod
+    def unify_pairwise(th_list, debug=False):
         """Unifies two thickets graphs and dataframes.
 
-        Ensure self and other have the same graph and same node IDs. This may
-        change the node IDs in the dataframe.
+        Ensure self and other have the same graph and same node IDs. This may change the
+        node IDs in the dataframe.
 
         Update the graphs in the graphframe if they differ.
+
+        Arguments:
+            th_list (list): list of Thicket objects
+            debug (bool): print debug statements
+
+        Returns:
+            union_graph (Graph): unified graph
         """
         union_graph = th_list[0].graph
         for i in range(len(th_list)):
             for j in range(i + 1, len(th_list)):
-                print("Unifying (" + str(i) + ", " + str(j) + "...")
+                if debug:
+                    print("Unifying (" + str(i) + ", " + str(j) + "...")
                 union_graph = th_list[i].unify_pair(th_list[j])
         return union_graph
 
     @staticmethod
-    def unify_listwise(th_list):
-        """Unify a list of Thicket's graphs and DataFrames"""
+    def unify_listwise(th_list, debug=False):
+        """Unify a list of Thicket's graphs and dataframes
+
+        Arguments:
+            th_list (list): list of Thicket objects
+            debug (bool): print debug statements
+
+        Returns:
+            union_graph (Graph): unified graph
+        """
         # variable to keep track of case where all graphs are the same
         same_graphs = True
 
         # GRAPH UNIFICATION
         union_graph = th_list[0].graph
         for i in range(1, len(th_list)):  # n-1 unions
-            # Check to skip unecessary computation. apply short circuiting with 'or'.
+            # Check to skip unnecessary computation. apply short circuiting with 'or'.
             if union_graph is th_list[i].graph or union_graph == th_list[i].graph:
-                print("Union Graph == thicket[" + str(i) + "].graph")
+                if debug:
+                    print("Union Graph == thicket[" + str(i) + "].graph")
             else:
-                print("Unifying (Union Graph, " + str(i) + ")")
+                if debug:
+                    print("Unifying (Union Graph, " + str(i) + ")")
                 same_graphs = False
                 # Unify graph with current thickets graph
                 union_graph = union_graph.union(th_list[i].graph)
 
         # If the graphs were all the same in the first place then there is no need to
         # apply any node mappings.
         if same_graphs:
@@ -699,73 +769,33 @@
         # After this point the graph and dataframe in each thicket is out of sync.
         # We could update the graph element in thicket to be the union graph but if the
         # user prints out the graph how do we annotate nodes only contained in one
         # thicket.
         return union_graph
 
     @staticmethod
-    def _resolve_missing_indicies(th_list):
-        """Resolve indices if at least 1 profile has an indexx that another doesn't
-
-        If at least one profile has an index that another doesn't, then issues will
-        arise when unifying. Need to add this index to other thickets.
-
-        Note that the value to use for the new index is set to '0' for ease-of-use, but
-        something like 'NaN' may arguably provide more clarity.
-        """
-        # Create a set of all index possibilities
-        idx_set = set({})
-        for th in th_list:
-            idx_set.update(th.dataframe.index.names)
-
-        # Apply missing indicies to thickets
-        for th in th_list:
-            for idx in idx_set:
-                if idx not in th.dataframe.index.names:
-                    print(
-                        "Resolving '" + str(idx) + "' in thicket: (" + str(id(th)) + ")"
-                    )
-                    th.dataframe[idx] = 0
-                    th.dataframe.set_index(idx, append=True, inplace=True)
-
-    @staticmethod
-    def _sync_nodes(gh, df):
-        """Set the node objects to be equal in both the graph and the dataframe.
-
-        id(graph_node) == id(df_node) after this function for nodes with equivalent hatchet nid's.
-        """
-        index_names = df.index.names
-        df.reset_index(inplace=True)
-        for graph_node in gh.traverse():
-            df["node"] = df["node"].apply(
-                lambda df_node: graph_node
-                if (hash(graph_node) == hash(df_node))
-                else df_node
-            )
-        df.set_index(index_names, inplace=True)
-
-    @staticmethod
     def unify_ensemble(th_list, pairwise=False, superthicket=False):
         """Unify a list of thickets into a single thicket
 
         Arguments:
             th_list (list): list of thickets
-            pairwise (bool): use the pairwise implementation of unify (use if having issues)
+            pairwise (bool): use the pairwise implementation of unify (use if having
+                issues)
             superthicket (bool): whether the result is a superthicket
 
         Returns:
             (thicket): unified thicket
         """
         unify_graph = None
         if pairwise:
             unify_graph = Thicket.unify_pairwise(th_list)
         else:
             unify_graph = Thicket.unify_listwise(th_list)
 
-        Thicket._resolve_missing_indicies(th_list)
+        helpers._resolve_missing_indicies(th_list)
 
         # Unify dataframe
         unify_df = pd.DataFrame()
         unify_inc_metrics = []
         unify_exc_metrics = []
         unify_metadata = pd.DataFrame()
         unify_profile = []
@@ -785,39 +815,39 @@
             unify_df = pd.concat([th.dataframe, unify_df])
 
         # Operations specific to a superthicket
         if superthicket:
             unify_metadata.index.rename("thicket", inplace=True)
 
             # Process to aggregate rows of thickets with the same name.
-            def agg_function(obj):
+            def _agg_function(obj):
                 """Aggregate values in 'obj' into a set to remove duplicates."""
                 if len(obj) <= 1:
                     return obj
                 else:
                     _set = set(obj)
                     if len(_set) == 1:
                         return _set.pop()
                     else:
                         return _set
 
-            unify_metadata = unify_metadata.groupby("thicket").agg(agg_function)
+            unify_metadata = unify_metadata.groupby("thicket").agg(_agg_function)
 
-        # Have metadata index match ensembleframe index
+        # Have metadata index match performance data table index
         unify_metadata.sort_index(inplace=True)
 
         # Sort by hatchet node id
         unify_df.sort_index(inplace=True)
 
         unify_inc_metrics = list(set(unify_inc_metrics))
         unify_exc_metrics = list(set(unify_exc_metrics))
 
         # Workaround for graph/df node id mismatch.
         # (n tree nodes) X (m df nodes) X (m)
-        Thicket._sync_nodes(unify_graph, unify_df)
+        helpers._sync_nodes(unify_graph, unify_df)
 
         # Mutate into OrderedDict to sort profile hashes
         unify_profile_mapping = OrderedDict(sorted(unify_profile_mapping.items()))
 
         unify_th = Thicket(
             graph=unify_graph,
             dataframe=unify_df,
@@ -829,81 +859,82 @@
         )
         return unify_th
 
     @staticmethod
     def make_superthicket(th_list, profiles_from_meta=None):
         """Convert a list of thickets into a 'superthicket'.
 
-        Their individual statsframes are ensembled and become the superthicket's
-        ensembleframe.
+        Their individual aggregated statistics table are ensembled and become the
+        superthicket's performance data table.
 
         Arguments:
             th_list (list): list of thickets
-            profiles_from_meta (str, optional): name of the metadata column to use as the new second-level index
+            profiles_from_meta (str, optional): name of the metadata column to use as
+                the new second-level index. Uses the first value so this only makes
+                sense if provided column is all equal values and each thicket's columns
+                differ in value.
 
         Returns:
             (thicket): superthicket
         """
         # Pre-check of data structures
         for th in th_list:
             verify_thicket_structures(
                 th.dataframe, index=["node", "profile"]
             )  # Required for deepcopy operation
             verify_thicket_structures(
                 th.statsframe.dataframe, index=["node"]
             )  # Required for deepcopy operation
 
         # Setup names list
-        if profiles_from_meta is None:
-            profiles_from_meta = []
-            for th in range(len(th_list)):
-                profiles_from_meta.append(th)
-
-        # Build names list
         th_names = []
-        for th in th_list:
-            # Get name from metadataframe
-            name_list = th.metadata[profiles_from_meta].tolist()
-
-            if len(name_list) > 1:
-                warnings.warn(
-                    "Multiple values for name "
-                    + name_list
-                    + "at thicket.metadata["
-                    + profiles_from_meta
-                    + "]. Only the first will be used."
-                )
-            th_names.append(name_list[0])
+        if profiles_from_meta is None:
+            for i in range(len(th_list)):
+                th_names.append(i)
+        else:  # profiles_from_meta was provided.
+            for th in th_list:
+                # Get name from metadata table
+                name_list = th.metadata[profiles_from_meta].tolist()
+
+                if len(name_list) > 1:
+                    warnings.warn(
+                        f"Multiple values for name {name_list} at thicket.metadata[{profiles_from_meta}]. Only the first will be used."
+                    )
+                th_names.append(name_list[0])
 
+        th_copy_list = []
         for i in range(len(th_list)):
-            th_list[i] = th_list[i].deepcopy()
+            th_copy = th_list[i].deepcopy()
 
             th_id = th_names[i]
 
             # Modify graph
             # Necessary so node ids match up
-            th_list[i].graph = th_list[i].statsframe.graph
+            th_copy.graph = th_copy.statsframe.graph
 
-            # Modify the ensembleframe
-            df = th_list[i].statsframe.dataframe
+            # Modify the performance data table
+            df = th_copy.statsframe.dataframe
             df["thicket"] = th_id
             df.set_index("thicket", inplace=True, append=True)
-            th_list[i].dataframe = df
+            th_copy.dataframe = df
 
             # Adjust profile and profile_mapping
-            th_list[i].profile = [th_id]
-            profile_paths = list(th_list[i].profile_mapping.values())
-            th_list[i].profile_mapping = OrderedDict({th_id: profile_paths})
+            th_copy.profile = [th_id]
+            profile_paths = list(th_copy.profile_mapping.values())
+            th_copy.profile_mapping = OrderedDict({th_id: profile_paths})
 
             # Modify metadata dataframe
             idx_name = "new_idx"
-            th_list[i].metadata[idx_name] = th_id
-            th_list[i].metadata.set_index(idx_name, inplace=True)
+            th_copy.metadata[idx_name] = th_id
+            th_copy.metadata.set_index(idx_name, inplace=True)
+
+            # Append copy to list
+            th_copy_list.append(th_copy)
 
-        return Thicket.unify_ensemble(th_list, superthicket=True)
+        return Thicket.unify_ensemble(th_copy_list, superthicket=True)
 
     def to_json(self, ensemble=True, metadata=True, stats=True):
         jsonified_thicket = {}
 
         # jsonify graph
         """
         Nodes: {hatchet_nid: {node data, children:[by-id]}}
@@ -949,29 +980,29 @@
 
         Nodes not contained in all profiles are removed.
 
         Returns:
             remaining_node_list (list): list of nodes that were not removed
             removed_node_list (list): list of removed nodes
         """
-        # Filter the ensembleframe
+        # Filter the performance data table
         total_profiles = len(self.profile)
         remaining_node_list = []  # Needed for graph
         removed_node_list = []
 
         # For each node
         for node, new_df in self.dataframe.groupby(level=0):
             # Use profile count to make decision
             if len(new_df) < total_profiles:
                 removed_node_list.append(node)
             else:
                 remaining_node_list.append(node)
         self.dataframe.drop(removed_node_list, inplace=True)
 
-        # Propagate change to statsframe
+        # Propagate change to aggregated statistics table
         self.statsframe.dataframe.drop(removed_node_list, inplace=True)
 
         # Filter the graph
 
         # Remove roots
         self.graph.roots = list(set(self.graph.roots).intersection(remaining_node_list))
         for node in self.graph.traverse():
@@ -991,55 +1022,59 @@
         self.graph.enumerate_traverse()
 
         return remaining_node_list, removed_node_list
 
     def filter_metadata(self, select_function):
         """Filter thicket object based on a metadata key.
 
-        Changes are propogated to the entire thicket object.
+        Changes are propagated to the entire thicket object.
 
         Arguments:
-            select_function (lambda function): filter to apply to the MetadataFrame
+            select_function (lambda function): filter to apply to the metadata table
 
         Returns:
             (thicket): new thicket object with selected value
         """
         if callable(select_function):
             if not self.metadata.empty:
-                # check profile is an index level in metadata
-                verify_thicket_structures(self.metadata, index=["profile"])
+                # check only 1 index in metadata
+                assert self.metadata.index.nlevels == 1
+
+                # Add warning if filtering on multi-index columns
+                if isinstance(self.metadata.columns, pd.MultiIndex):
+                    warnings.warn(
+                        "Filtering on MultiIndex columns will impact the entire row, not just the subsection of the provided MultiIndex."
+                    )
+
+                # Get index name
+                index_name = self.metadata.index.name
 
                 # create a copy of the thicket object
                 new_thicket = self.copy()
 
-                # filter MetadataFrame
+                # filter metadata table
                 filtered_rows = new_thicket.metadata.apply(select_function, axis=1)
                 new_thicket.metadata = new_thicket.metadata[filtered_rows]
 
-                # note profile keys to filter EnsembleFrame
-                profile_id = new_thicket.metadata.index.values.tolist()
-                # filter EnsembleFrame based on the MetadataFrame
+                # note index keys to filter performance data table
+                index_id = new_thicket.metadata.index.values.tolist()
+                # filter performance data table based on the metadata table
                 new_thicket.dataframe = new_thicket.dataframe[
-                    new_thicket.dataframe.index.get_level_values("profile").isin(
-                        profile_id
+                    new_thicket.dataframe.index.get_level_values(index_name).isin(
+                        index_id
                     )
                 ]
 
-                # create an empty StatsFrame with the name column
-                subset_df = (
-                    new_thicket.dataframe["name"]
-                    .reset_index()
-                    .drop_duplicates(subset=["node"])
-                )
-                new_thicket.statsframe.dataframe = pd.DataFrame(
-                    index=subset_df["node"], data={"name": subset_df["name"].values}
+                # create an empty aggregated statistics table with the name column
+                new_thicket.statsframe.dataframe = helpers._new_statsframe_df(
+                    new_thicket.dataframe
                 )
             else:
-                raise EmptyMetadataFrame(
-                    "The provided Thicket object has an empty MetadataFrame."
+                raise EmptyMetadataTable(
+                    "The provided Thicket object has an empty MetadataTable."
                 )
 
         else:
             raise InvalidFilter("The argument passed to filter must be a callable.")
 
         return new_thicket
 
@@ -1048,20 +1083,24 @@
 
         Provides a helper message for using the thicket filter functions.
         """
         raise RuntimeError(
             "Invalid function: thicket.filter(), please use thicket.filter_metadata() or thicket.filter_stats()"
         )
 
-    def query(self, query_obj, squash=True):
+    def query(self, query_obj, squash=True, update_inc_cols=True):
         """Apply a Hatchet query to the Thicket object.
 
         Arguments:
-            query_obj (AbstractQuery): the query, represented as by a subclass of Hatchet's AbstractQuery
-            squash (bool): if true, run Thicket.squash before returning the result of the query
+            query_obj (AbstractQuery): the query, represented as by a subclass of
+                Hatchet's AbstractQuery
+            squash (bool): if true, run Thicket.squash before returning the result of
+                the query
+            update_inc_cols (boolean, optional): if True, update inclusive columns when
+                performing squash.
 
         Returns:
             (Thicket): a new Thicket object containing the data that matches the query
         """
         if isinstance(query_obj, (list, str)):
             raise UnsupportedQuery(
                 "Object and String queries from Hatchet are not yet supported in Thicket"
@@ -1088,115 +1127,161 @@
             default_metric=self.default_metric,
             metadata=self.metadata,
             profile=self.profile,
             profile_mapping=self.profile_mapping,
             statsframe=self.statsframe,
         )
         if squash:
-            return filtered_th.squash()
+            return filtered_th.squash(update_inc_cols=update_inc_cols)
         return filtered_th
 
     def groupby(self, groupby_function):
         """Create sub-thickets based on unique values in metadata column(s).
 
         Arguments:
             groupby_function (groupby_function): groupby function on dataframe
 
         Returns:
             (list): list of (sub)thickets
         """
         if not self.metadata.empty:
-            # group MetadataFrame by unique values in a column
+            # group metadata table by unique values in a column
             sub_metadataframes = self.metadata.groupby(groupby_function, dropna=False)
 
             list_sub_thickets = []
             unique_vals = []
 
-            # for all unique groups of MetadataFrame
+            # for all unique groups of metadata table
             for key, df in sub_metadataframes:
                 unique_vals.append(key)
 
                 # create a thicket copy
                 sub_thicket = self.copy()
 
-                # return unique group as the MetadataFrame
+                # return unique group as the metadata table
                 sub_thicket.metadata = df
 
-                # find profiles in current unique group and filter EnsembleFrame
+                # find profiles in current unique group and filter performance data
+                # table
                 profile_id = df.index.values.tolist()
                 sub_thicket.dataframe = sub_thicket.dataframe[
                     sub_thicket.dataframe.index.get_level_values("profile").isin(
                         profile_id
                     )
                 ]
 
-                # clear the StatsFrame for current unique group
-                subset_df = (
-                    sub_thicket.dataframe["name"]
-                    .reset_index()
-                    .drop_duplicates(subset=["node"])
-                )
-                sub_thicket.statsframe.dataframe = pd.DataFrame(
-                    index=subset_df["node"], data={"name": subset_df["name"].values}
+                # Updates the profiles to only contain the remaining ones
+                profile_mapping_tmp = sub_thicket.profile_mapping.copy()
+                for profile_mapping_key in profile_mapping_tmp:
+                    if profile_mapping_key not in profile_id:
+                        sub_thicket.profile_mapping.pop(profile_mapping_key)
+
+                sub_thicket.profile = [
+                    profile for profile in sub_thicket.profile if profile in profile_id
+                ]
+
+                # clear the aggregated statistics table for current unique group
+                sub_thicket.statsframe.dataframe = helpers._new_statsframe_df(
+                    sub_thicket.dataframe
                 )
                 list_sub_thickets.append(sub_thicket)
         else:
-            raise EmptyMetadataFrame(
-                "The provided Thicket object has an empty MetadataFrame."
+            raise EmptyMetadataTable(
+                "The provided Thicket object has an empty metadata table."
             )
 
-        print(len(list_sub_thickets), " Sub-Thickets created...")
+        print(len(list_sub_thickets), " thickets created...")
         print(unique_vals)
 
         return list_sub_thickets
 
     def filter_stats(self, filter_function):
         """Filter thicket object based on a stats column.
 
         Propagate changes to the entire thicket object.
 
         Arguments:
-            select_function (lambda function): filter to apply to the StatsFrame
+            select_function (lambda function): filter to apply to the aggregated
+                statistics table
 
         Returns:
             (thicket): new thicket object with applied filter function
         """
         # copy thicket
         new_thicket = self.copy()
 
-        # filter stats rows based on greater than restriction
+        # filter aggregated statistics table based on greater than restriction
         filtered_rows = new_thicket.statsframe.dataframe.apply(filter_function, axis=1)
         new_thicket.statsframe.dataframe = new_thicket.statsframe.dataframe[
             filtered_rows
         ]
 
-        # filter ensembleframe based on filtered nodes
+        # filter performance data table based on filtered nodes
         filtered_nodes = new_thicket.statsframe.dataframe.index.values.tolist()
         new_thicket.dataframe = new_thicket.dataframe[
             new_thicket.dataframe.index.get_level_values("node").isin(filtered_nodes)
         ]
 
-        # filter nodes in the graph frame based on the DataFrame nodes
+        # filter nodes in the graphframe based on the dataframe nodes
         # TODO see if the new Thicket.squash function will work here
         filtered_graphframe = GraphFrame.squash(new_thicket)
         new_thicket.graph = filtered_graphframe.graph
         new_thicket.statsframe.graph = filtered_graphframe.graph
 
         return new_thicket
 
+    def get_unique_metadata(self):
+        """Get unique values per column in metadata.
+
+        Returns:
+            (dict): alphabetical ordered dictionary with key's being the column names
+                and the values being unique values for a metadata column.
+        """
+        unique_meta = {}
+
+        # thicket object without columnar index
+        if self.dataframe.columns.nlevels == 1:
+            for col in self.metadata.columns:
+                # skip columns where the values are a list
+                if isinstance(self.metadata[col].iloc[0], list):
+                    continue
+                else:
+                    unique_entries = self.metadata[col].unique().tolist()
+                    unique_meta[col] = unique_entries
+
+            sorted_meta = dict(sorted(unique_meta.items(), key=lambda x: x[0].lower()))
+        # columnar joined thicket object
+        else:
+            sorted_meta = []
+            for idx in list(self.metadata.columns.levels[0]):
+                for col in self.metadata[idx].columns:
+                    if isinstance(self.metadata[idx][col].iloc[0], list):
+                        continue
+                    else:
+                        unique_entries = self.metadata[idx][col].unique().tolist()
+                        unique_meta[col] = unique_entries
+
+                sorted_meta.append(
+                    (idx, dict(sorted(unique_meta.items(), key=lambda x: x[0].lower())))
+                )
+
+        return sorted_meta
+
 
 class InvalidFilter(Exception):
     """Raised when an invalid argument is passed to the filter function."""
 
 
-class EmptyMetadataFrame(Exception):
-    """Raised when a Thicket object argument is passed with an empty MetadataFrame to the filter function."""
+class EmptyMetadataTable(Exception):
+    """Raised when a Thicket object argument is passed with an empty MetadataTable to
+    the filter function.
+    """
 
 
 class UnsupportedQuery(Exception):
-    """Raised when an object query or string query are provided
-    to the 'query' function because those types of queries are
-    not yet supported in Thicket."""
+    """Raised when an object query or string query are provided to the 'query' function
+    because those types of queries are not yet supported in Thicket.
+    """
 
 
 class EmptyQuery(Exception):
     """Raised when a query would result in an empty Thicket object."""
```

### Comparing `llnl-thicket-2023.1.0/thicket/utils.py` & `llnl-thicket-2023.2.0/thicket/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
+from collections import OrderedDict
+
+
+def verify_sorted_profile(thicket_component):
+    """Assertion to check if profiles are sorted in a thicket dataframe
+
+    Arguments:
+        thicket_component (DataFrame): component of thicket to check
+    """
+    profile_index_values = list(
+        OrderedDict.fromkeys(thicket_component.index.get_level_values("profile"))
+    )
+    if profile_index_values != sorted(profile_index_values):
+        raise ValueError(
+            "The profiles in this dataframe must be sorted. Try 'pandas.DataFrame.sort_index'."
+        )
+
 
 def verify_thicket_structures(thicket_component, columns=[], index=[]):
     """Assertion for missing input requirements to execute thicket functions.
 
     Arguments:
         thicket_components (DataFrame): component of thicket to check
         columns (list): list of columns to check for in the component
         index (list): list of index levels to check for in the component
 
     Returns:
-        Raises an error if any columns or index levels are not in component,
-        continues program if all columns and index levels are in component
+        Raises an error if any columns or index levels are not in component, continues
+            program if all columns and index levels are in component
     """
+    if not isinstance(columns, list):
+        raise RuntimeError("columns= must be specified as a list")
+    if not isinstance(index, list):
+        raise RuntimeError("index= must be specified as a list")
+
     # collect component columns and index
     component_columns = thicket_component.columns.tolist()
     component_index = thicket_component.index.names
 
     # check existence of columns and index
     column_result = all(elem in component_columns for elem in columns)
     index_result = all(elem in component_index for elem in index)
 
-    # store missing collumns or index if they exist
+    # store missing columns or index if they exist
     missing_columns = list(set(columns).difference(component_columns))
     missing_index = list(set(index).difference(component_index))
 
     if not column_result and not index_result:
         raise RuntimeError(
-            "\n Missing column(s): "
-            + missing_columns
-            + " required for the function. \n Missing index level(s): "
-            + missing_index
+            "Specified column(s) not found: "
+            + str(missing_columns)
+            + "\nMissing index level(s): "
+            + str(missing_index)
             + " required for the function"
         )
     elif not column_result and index_result:
-        raise RuntimeError(
-            "\n Missing column(s): " + missing_columns + " required for the function"
-        )
+        raise RuntimeError("Specified column(s) not found: " + str(missing_columns))
     elif column_result and not index_result:
         raise RuntimeError(
-            "\n Missing index level(s): " + missing_index + " required for the function"
+            "Missing index level(s): "
+            + str(missing_index)
+            + " required for the function"
         )
```

### Comparing `llnl-thicket-2023.1.0/thicket/vis/__init__.py` & `llnl-thicket-2023.2.0/thicket/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/package.json` & `llnl-thicket-2023.2.0/thicket/vis/package.json`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/datautil.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/datautil.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/pcp.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/pcp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -51,15 +51,15 @@
 
             if (c_domain.length > 0 && isNaN(c_domain[0]) && !invalid) {
                 this.xs[dim] = d3.scalePoint()
                     .domain(c_domain)
                     .range([this.checkbox_margin, width]);
                 this.valid_dims.push(dim);
                 this.c_dims.push(dim);
-            } else if (c_domain.length > 1 && !(isNaN(c_domain[0])) && !invalid) {
+            } else if (c_domain.length > 0 && !(isNaN(c_domain[0])) && !invalid) {
                 let n_domain = getNumericalDomain(data.metadata, dim);
                 this.xs[dim] = d3.scaleLinear()
                     .domain(n_domain)
                     .range([this.checkbox_margin, width]);
                 this.valid_dims.push(dim);
                 this.n_dims.push(dim);
             }
```

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/scatter.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/scatter.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/stackedarea.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/stackedarea.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/pcp/store.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/pcp/store.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/topdown/stackedbars.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/topdown/stackedbars.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/scripts/treetable.js` & `llnl-thicket-2023.2.0/thicket/vis/scripts/treetable.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/static/pcp_bundle.html` & `llnl-thicket-2023.2.0/thicket/vis/static/pcp_bundle.html`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/static/pcp_bundle.js` & `llnl-thicket-2023.2.0/thicket/vis/static/pcp_bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11707,15 +11707,15 @@
                     return n != null;
                 });
 
                 if (c_domain.length > 0 && isNaN(c_domain[0]) && !invalid) {
                     this.xs[dim] = point().domain(c_domain).range([this.checkbox_margin, width]);
                     this.valid_dims.push(dim);
                     this.c_dims.push(dim);
-                } else if (c_domain.length > 1 && !isNaN(c_domain[0]) && !invalid) {
+                } else if (c_domain.length > 0 && !isNaN(c_domain[0]) && !invalid) {
                     var n_domain = getNumericalDomain(data.metadata, dim);
                     this.xs[dim] = linear_linear().domain(n_domain).range([this.checkbox_margin, width]);
                     this.valid_dims.push(dim);
                     this.n_dims.push(dim);
                 }
             }
```

### Comparing `llnl-thicket-2023.1.0/thicket/vis/static/topdown_bundle.js` & `llnl-thicket-2023.2.0/thicket/vis/static/topdown_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/static/treetable_bundle.js` & `llnl-thicket-2023.2.0/thicket/vis/static/treetable_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/static_fixer.py` & `llnl-thicket-2023.2.0/thicket/vis/static_fixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
-from bs4 import BeautifulSoup
 from os import walk, path
 
+from bs4 import BeautifulSoup
+
 static_filepath = path.abspath("static/")
 
 for (pt, dirs, files) in walk(static_filepath):
     for file in files:
         if ".html" in file:
             with open(path.join(static_filepath, file), "r") as f:
                 html = f.read()
```

### Comparing `llnl-thicket-2023.1.0/thicket/vis/templates/pcp.html` & `llnl-thicket-2023.2.0/thicket/vis/templates/pcp.html`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.1.0/thicket/vis/visualizations.py` & `llnl-thicket-2023.2.0/thicket/vis/visualizations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from hatchet.external import Roundtrip as RT
-from IPython.core.magic import Magics, magics_class, line_magic
 from os import path
 from os.path import dirname
 
+from IPython.core.magic import Magics, magics_class, line_magic
+from hatchet.external import Roundtrip as RT
+
 
 def _thicket_to_json(data):
     return data.to_json()
 
 
 def _df_to_json(data):
     return data.to_json(orient="records")
```

### Comparing `llnl-thicket-2023.1.0/thicket/vis/webpack.config.js` & `llnl-thicket-2023.2.0/thicket/vis/webpack.config.js`

 * *Files identical despite different names*

