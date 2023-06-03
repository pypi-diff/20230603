# Comparing `tmp/psyke-0.3.5.tar.gz` & `tmp/psyke-0.4.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.3.5.tar", last modified: Wed May 31 00:32:38 2023, max compression
+gzip compressed data, was "psyke-0.4.2.dev2.tar", last modified: Sat Jun  3 17:59:36 2023, max compression
```

## Comparing `psyke-0.3.5.tar` & `psyke-0.4.2.dev2.tar`

### file list

```diff
@@ -1,133 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-31 00:30:48.000000 psyke-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 00:30:48.000000 psyke-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-31 00:32:38.119743 psyke-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-31 00:30:48.000000 psyke-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 00:32:38.000000 psyke-0.3.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/gridrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/extraction/trepan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.107743 psyke-0.3.5/psyke/gui/controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/controller/Controller.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/controller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.099743 psyke-0.3.5/psyke/gui/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.099743 psyke-0.3.5/psyke/gui/libs/garden/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.111743 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50930 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-31 00:32:28.000000 psyke-0.3.5/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.111743 psyke-0.3.5/psyke/gui/model/
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/model/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.111743 psyke-0.3.5/psyke/gui/view/
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/DataPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/ExtractorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/FeaturePanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/PlotPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/PredictorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/TheoryPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/View.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/gui/view/style.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.111743 psyke-0.3.5/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-31 00:30:48.000000 psyke-0.3.5/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.103743 psyke-0.3.5/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-31 00:32:38.000000 psyke-0.3.5/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-31 00:32:38.000000 psyke-0.3.5/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:32:38.000000 psyke-0.3.5/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:32:37.000000 psyke-0.3.5/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-31 00:32:38.000000 psyke-0.3.5/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 00:32:38.000000 psyke-0.3.5/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 00:30:48.000000 psyke-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:32:38.119743 psyke-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-05-31 00:30:48.000000 psyke-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.099743 psyke-0.3.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.115743 psyke-0.3.5/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 00:30:48.000000 psyke-0.3.5/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 00:30:52.000000 psyke-0.3.5/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-31 00:30:52.000000 psyke-0.3.5/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 00:30:53.000000 psyke-0.3.5/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:32:38.119743 psyke-0.3.5/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 00:30:53.000000 psyke-0.3.5/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-03 17:59:29.000000 psyke-0.4.2.dev2/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/extraction/trepan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:59:35.000000 psyke-0.4.2.dev2/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-03 17:59:36.000000 psyke-0.4.2.dev2/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.043313 psyke-0.4.2.dev2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.047313 psyke-0.4.2.dev2/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-03 17:58:20.000000 psyke-0.4.2.dev2/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 17:58:24.000000 psyke-0.4.2.dev2/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 17:58:24.000000 psyke-0.4.2.dev2/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-03 17:58:24.000000 psyke-0.4.2.dev2/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:59:36.051313 psyke-0.4.2.dev2/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-03 17:58:24.000000 psyke-0.4.2.dev2/test/resources/tests/__init__.py
```

### Comparing `psyke-0.3.5/LICENSE` & `psyke-0.4.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/PKG-INFO` & `psyke-0.4.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.5
+Version: 0.4.2.dev2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.5/README.md` & `psyke-0.4.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/__init__.py` & `psyke-0.4.2.dev2/psyke/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 from __future__ import annotations
+
 from abc import ABC
+from enum import Enum
+
 import numpy as np
 import pandas as pd
 from numpy import argmax
 from sklearn.linear_model import LinearRegression
-from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score, f1_score, accuracy_score
+from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score, f1_score, accuracy_score, \
+    adjusted_rand_score, adjusted_mutual_info_score, v_measure_score, fowlkes_mallows_score
+
 from psyke.schema import DiscreteFeature
-from psyke.utils import get_default_random_seed
+from psyke.utils import get_default_random_seed, Target, get_int_precision
 from tuprolog.theory import Theory
 from typing import Iterable
 import logging
 
-
 logging.basicConfig(level=logging.WARN)
 logger = logging.getLogger('psyke')
 
 
-class Extractor(object):
-    """
-    An explanator capable of extracting rules from trained black box.
-
-    Parameters
-    ----------
-    predictor : the underling black box predictor.
-    discretization : A collection of sets of discretised features.
-        Each set corresponds to a set of features derived from a single non-discrete feature.
-    """
+class EvaluableModel(object):
+    class Task(Enum):
+        CLASSIFICATION = 1,
+        REGRESSION = 2,
+        CLUSTERING = 3
+
+    class Score(Enum):
+        pass
+
+    class ClassificationScore(Score):
+        ACCURACY = 1
+        F1 = 2,
+        INVERSE_ACCURACY = 3
+
+    class RegressionScore(Score):
+        MAE = 1
+        MSE = 2
+        R2 = 3
+
+    class ClusteringScore(Score):
+        ARI = 1,
+        AMI = 2,
+        V = 3,
+        FMI = 4
 
-    def __init__(self, predictor, discretization: Iterable[DiscreteFeature] = None, normalization=None):
-        self.predictor = predictor
-        self.discretization = [] if discretization is None else list(discretization)
+    def __init__(self, normalization=None):
         self.normalization = normalization
 
-    def extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
-        """
-        Extracts rules from the underlying predictor.
-
-        :param dataframe: is the set of instances to be used for the extraction.
-        :param mapping: for one-hot encoding.
-        :param sort: alphabetically sort the variables of the head of the rules.
-        :return: the theory created from the extracted rules.
-        """
-        raise NotImplementedError('extract')
-
     def predict(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None) -> Iterable:
         """
         Predicts the output values of every sample in dataset.
 
         :param dataframe: is the set of instances to predict.
         :param mapping: for one-hot encoding.
         :return: a list of predictions.
@@ -60,100 +65,152 @@
     def _predict(self, dataframe: pd.DataFrame) -> Iterable:
         raise NotImplementedError('predict')
 
     def unscale(self, values, name):
         if self.normalization is None or isinstance(values, LinearRegression):
             return values
         if isinstance(values, Iterable):
-            idx = [value is not None for value in values]
-            values[idx] = values[idx] * self.normalization[name][1] + self.normalization[name][0]
+            values = [None if value is None else
+                      value * self.normalization[name][1] + self.normalization[name][0] for value in values]
         else:
             values = values * self.normalization[name][1] + self.normalization[name][0]
         return values
 
-    def regression_score(self, dataframe: pd.DataFrame, predictor=None, scoring_function=mean_absolute_error):
-        predictions = np.array(self.predict(dataframe.iloc[:, :-1]))
-        idx = [prediction is not None for prediction in predictions]
-        true = self.unscale(dataframe.iloc[idx, -1] if predictor is None else
-                            predictor.predict(dataframe.iloc[idx, :-1]).flatten(), dataframe.columns[-1])
-        return scoring_function(true, self.unscale(predictions[idx], dataframe.columns[-1]))
+    def score(self, dataframe: pd.DataFrame, predictor=None, fidelity: bool = False, completeness: bool = True,
+              task: EvaluableModel.Task = Task.CLASSIFICATION,
+              scoring_function: Iterable[EvaluableModel.Score] = [ClassificationScore.ACCURACY]):
+        extracted = np.array(self.predict(dataframe.iloc[:, :-1]))
+        idx = [prediction is not None for prediction in extracted]
+        y_extracted = extracted[idx]
+        true = [dataframe.iloc[idx, -1]]
+
+        if fidelity:
+            if predictor is None:
+                raise ValueError("Predictor must be not None to measure fidelity")
+            true.append(predictor.predict(dataframe.iloc[idx, :-1]).flatten())
+
+        if task == EvaluableModel.Task.REGRESSION:
+            y_extracted = self.unscale(y_extracted, dataframe.columns[-1])
+            true = [self.unscale(t, dataframe.columns[-1]) for t in true]
+
+        res = {
+                  score: EvaluableModel.__evaluate(true, y_extracted, score) for score in scoring_function
+              }, sum(idx) / len(idx)
+        return res if completeness else res[0]
+
+    @staticmethod
+    def __evaluate(y, y_hat, scoring_function):
+        if scoring_function == EvaluableModel.ClassificationScore.ACCURACY:
+            f = accuracy_score
+        elif scoring_function == EvaluableModel.ClassificationScore.F1:
+            def f(true, pred):
+                return f1_score(true, pred, average='weighted')
+        elif scoring_function == EvaluableModel.ClassificationScore.INVERSE_ACCURACY:
+            def f(true, pred):
+                return 1 - accuracy_score(true, pred)
+        elif scoring_function == EvaluableModel.RegressionScore.R2:
+            f = r2_score
+        elif scoring_function == EvaluableModel.RegressionScore.MAE:
+            f = mean_absolute_error
+        elif scoring_function == EvaluableModel.RegressionScore.MSE:
+            f = mean_squared_error
+        elif scoring_function == EvaluableModel.ClusteringScore.ARI:
+            f = adjusted_rand_score
+        elif scoring_function == EvaluableModel.ClusteringScore.AMI:
+            f = adjusted_mutual_info_score
+        elif scoring_function == EvaluableModel.ClusteringScore.V:
+            f = v_measure_score
+        elif scoring_function == EvaluableModel.ClusteringScore.FMI:
+            f = fowlkes_mallows_score
+        else:
+            raise ValueError("Scoring function not supported")
+        return [f(yy, y_hat) for yy in y]
+
+
+class Extractor(EvaluableModel, ABC):
+    """
+    An explanator capable of extracting rules from trained black box.
+
+    Parameters
+    ----------
+    predictor : the underling black box predictor.
+    discretization : A collection of sets of discretised features.
+        Each set corresponds to a set of features derived from a single non-discrete feature.
+    """
+
+    def __init__(self, predictor, discretization: Iterable[DiscreteFeature] = None, normalization=None):
+        super().__init__(normalization)
+        self.predictor = predictor
+        self.discretization = [] if discretization is None else list(discretization)
+
+    def extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
+        """
+        Extracts rules from the underlying predictor.
+
+        :param dataframe: is the set of instances to be used for the extraction.
+        :param mapping: for one-hot encoding.
+        :param sort: alphabetically sort the variables of the head of the rules.
+        :return: the theory created from the extracted rules.
+        """
+        raise NotImplementedError('extract')
 
     def mae(self, dataframe: pd.DataFrame, predictor=None) -> float:
         """
         Calculates the predictions' MAE w.r.t. the instances given as input.
 
         :param dataframe: is the set of instances to be used to calculate the mean absolute error.
         :param predictor: if provided, its predictions on the dataframe are taken instead of the dataframe instances.
         :return: the mean absolute error (MAE) of the predictions.
         """
-        return self.regression_score(dataframe, predictor, mean_absolute_error)
+        return self.score(dataframe, predictor, predictor is not None, False, Extractor.Task.REGRESSION,
+                          [Extractor.RegressionScore.MAE])[Extractor.RegressionScore.MAE][-1]
 
     def mse(self, dataframe: pd.DataFrame, predictor=None) -> float:
         """
         Calculates the predictions' MSE w.r.t. the instances given as input.
 
         :param dataframe: is the set of instances to be used to calculate the mean squared error.
         :param predictor: if provided, its predictions on the dataframe are taken instead of the dataframe instances.
         :return: the mean squared error (MSE) of the predictions.
         """
-        return self.regression_score(dataframe, predictor, mean_squared_error)
+        return self.score(dataframe, predictor, predictor is not None, False, Extractor.Task.REGRESSION,
+                          [Extractor.RegressionScore.MSE])[Extractor.RegressionScore.MSE][-1]
 
     def r2(self, dataframe: pd.DataFrame, predictor=None) -> float:
         """
         Calculates the predictions' R2 score w.r.t. the instances given as input.
 
         :param dataframe: is the set of instances to be used to calculate the R2 score.
         :param predictor: if provided, its predictions on the dataframe are taken instead of the dataframe instances.
         :return: the R2 score of the predictions.
         """
-        return self.regression_score(dataframe, predictor, r2_score)
+        return self.score(dataframe, predictor, predictor is not None, False,
+                          Extractor.Task.REGRESSION, [Extractor.RegressionScore.R2])[Extractor.RegressionScore.R2][-1]
 
     def accuracy(self, dataframe: pd.DataFrame, predictor=None) -> float:
         """
         Calculates the predictions' accuracy classification score w.r.t. the instances given as input.
 
         :param dataframe: is the set of instances to be used to calculate the accuracy classification score.
         :param predictor: if provided, its predictions on the dataframe are taken instead of the dataframe instances.
         :return: the accuracy classification score of the predictions.
         """
-        predictions = np.array(self.predict(dataframe.iloc[:, :-1]))
-        idx = [prediction is not None for prediction in predictions]
-        return accuracy_score(dataframe.iloc[idx, -1] if predictor is None else
-                              predictor.predict(dataframe.iloc[idx, :-1]).flatten(),
-                              predictions[idx])
+        return self.score(dataframe, predictor, predictor is not None, False, Extractor.Task.CLASSIFICATION,
+                          [Extractor.ClassificationScore.ACCURACY])[Extractor.ClassificationScore.ACCURACY][-1]
 
     def f1(self, dataframe: pd.DataFrame, predictor=None) -> float:
         """
         Calculates the predictions' F1 score w.r.t. the instances given as input.
 
         :param dataframe: is the set of instances to be used to calculate the F1 score.
         :param predictor: if provided, its predictions on the dataframe are taken instead of the dataframe instances.
         :return: the F1 score of the predictions.
         """
-        predictions = np.array(self.predict(dataframe.iloc[:, :-1])[:])
-        idx = [prediction is not None for prediction in predictions]
-        return f1_score(dataframe.iloc[idx, -1] if predictor is None else
-                        predictor.predict(dataframe.iloc[idx, :-1]).flatten(),
-                        predictions[idx], average='weighted')
-
-    @staticmethod
-    def exact(depth: int, error_threshold: float, output, gauss_components: int = 2):
-        """
-        Creates a new ExACT instance.
-        """
-        from psyke.clustering.exact import ExACT
-        return ExACT(depth, error_threshold, output, gauss_components)
-
-    @staticmethod
-    def cream(depth: int, error_threshold: float, output, gauss_components: int = 2):
-        """
-        Creates a new CREAM instance.
-        """
-        from psyke.clustering.cream import CREAM
-        return CREAM(depth, error_threshold, output, gauss_components)
+        return self.score(dataframe, predictor, predictor is not None, False, Extractor.Task.CLASSIFICATION,
+                          [Extractor.ClassificationScore.F1])[Extractor.ClassificationScore.F1][-1]
 
     @staticmethod
     def cart(predictor, max_depth: int = 3, max_leaves: int = 3,
              discretization: Iterable[DiscreteFeature] = None, normalization=None, simplify: bool = True) -> Extractor:
         """
         Creates a new Cart extractor.
         """
@@ -219,16 +276,47 @@
         """
         from psyke.extraction.trepan import Trepan, SplitLogic
         if split_logic is None:
             split_logic = SplitLogic.DEFAULT
         return Trepan(predictor, [] if discretization is None else discretization, min_examples, max_depth, split_logic)
 
 
+class Clustering(EvaluableModel, ABC):
+    def __init__(self, normalization=None):
+        super().__init__(normalization)
+
+    def fit(self, dataframe: pd.DataFrame):
+        raise NotImplementedError('extract')
+
+    def explain(self):
+        raise NotImplementedError('extract')
+
+    @staticmethod
+    def exact(depth: int = 2, error_threshold: float = 0.1, output: Target = Target.CONSTANT,
+              gauss_components: int = 2) -> Clustering:
+        """
+        Creates a new ExACT instance.
+        """
+        from psyke.clustering.exact import ExACT
+        return ExACT(depth, error_threshold, output, gauss_components)
+
+    @staticmethod
+    def cream(depth: int, error_threshold: float, output, gauss_components: int = 2) -> Clustering:
+        """
+        Creates a new CREAM instance.
+        """
+        from psyke.clustering.cream import CREAM
+        return CREAM(depth, error_threshold, output, gauss_components)
+
+
 class PedagogicalExtractor(Extractor, ABC):
 
+    def __init__(self, predictor, discretization=None, normalization=None):
+        Extractor.__init__(self, predictor=predictor, discretization=discretization, normalization=normalization)
+
     def extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
         new_y = self.predictor.predict(dataframe.iloc[:, :-1])
         if mapping is not None:
             if hasattr(new_y[0], 'shape'):
                 # One-hot encoding for multi-class tasks
                 if len(new_y[0].shape) > 0 and new_y[0].shape[0] > 1:
                     new_y = [argmax(y, axis=0) for y in new_y]
@@ -237,8 +325,8 @@
                     new_y = [round(y[0]) for y in new_y]
         new_y = pd.DataFrame(new_y).set_index(dataframe.index)
         data = dataframe.iloc[:, :-1].copy().join(new_y)
         data.columns = dataframe.columns
         return self._extract(data, mapping, sort)
 
     def _extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
-        raise NotImplementedError('predict')
+        raise NotImplementedError('extract')
```

### Comparing `psyke-0.3.5/psyke/clustering/cream/__init__.py` & `psyke-0.4.2.dev2/psyke/clustering/cream/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,18 @@
             data = ExACT._remove_string_label(node.dataframe)
             gauss_params = select_gaussian_mixture(data, self.gauss_components)
             gauss_pred = gauss_params[2].predict(data)
             cubes = self.__eligible_cubes(gauss_pred, node, gauss_params[1])
             if len(cubes) < 1:
                 continue
             _, right, left = min(cubes)
+            # find_better_constraints(node.dataframe[right[1]], right[0])
             node.right = Node(node.dataframe[right[1]], right[0])
             node.cube.update(node.dataframe[left[1]], self._predictor)
             node.left = Node(node.dataframe[left[1]], left[0])
 
             if depth < self.depth:
                 to_split += [
                     (error, depth + 1, np.random.uniform(), n) for (n, error) in
                     zip(node.children, [right[0].diversity, left[0].diversity]) if error > self.error_threshold
                 ]
-        return self._node_to_cubes(surrounding)
+        return self._node_to_cubes(surrounding)
```

### Comparing `psyke-0.3.5/psyke/clustering/exact/__init__.py` & `psyke-0.4.2.dev2/psyke/clustering/exact/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from __future__ import annotations
 
+from abc import ABC
 from collections import Counter
-from typing import Iterable
+from typing import Iterable, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import DBSCAN
 from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
 
-from psyke.clustering import InterpretableClustering
+from psyke.clustering import HyperCubeClustering
 from psyke.extraction.hypercubic import Node, ClosedCube, HyperCube
 from psyke.clustering.utils import select_gaussian_mixture, select_dbscan_epsilon
+from psyke.extraction.hypercubic.hypercube import ClosedRegressionCube, ClosedClassificationCube
 from psyke.utils import Target
 
 
-class ExACT(InterpretableClustering):
+class ExACT(HyperCubeClustering, ABC):
     """
     Explanator implementing ExACT algorithm.
     """
 
-    def __init__(self, depth: int, error_threshold: float, output: Target = Target.CONSTANT, gauss_components: int = 5):
-        super().__init__(depth, error_threshold, output, gauss_components)
+    def __init__(self, depth: int = 2, error_threshold: float = 0.1, output: Target = Target.CONSTANT,
+                 gauss_components: int = 2, normalization=None):
+        super().__init__(output, normalization)
+        self.depth = depth
+        self.error_threshold = error_threshold
+        self.gauss_components = gauss_components
         self._predictor = KNeighborsClassifier() if output == Target.CLASSIFICATION else KNeighborsRegressor()
         self._predictor.n_neighbors = 1
 
     def __eligible_cubes(self, gauss_pred: np.ndarray, node: Node, clusters: int):
         cubes = []
         for i in range(len(np.unique(gauss_pred))):
             df = node.dataframe.iloc[np.where(gauss_pred == i)]
@@ -45,21 +51,23 @@
         data = ExACT._remove_string_label(dataframe)
         dbscan_pred = DBSCAN(eps=select_dbscan_epsilon(data, clusters)).fit_predict(data.iloc[:, :-1])
         return HyperCube.create_surrounding_cube(
             dataframe.iloc[np.where(dbscan_pred == Counter(dbscan_pred).most_common(1)[0][0])],
             True, self._output
         )
 
-    def extract(self, dataframe: pd.DataFrame) -> Iterable[HyperCube]:
+    def fit(self, dataframe: pd.DataFrame):
         self._predictor.fit(dataframe.iloc[:, :-1], dataframe.iloc[:, -1])
         self._hypercubes = \
             self._iterate(Node(dataframe, HyperCube.create_surrounding_cube(dataframe, True, self._output)))
+
+    def get_hypercubes(self) -> Iterable[HyperCube]:
         return list(self._hypercubes)
 
-    def print(self):
+    def explain(self):
         for cube in self._hypercubes:
             print(f'Output is {cube.output} if:')
             for feature in cube.dimensions:
                 lower, upper = cube[feature]
                 print(f'    {feature} is in [{lower:.2f}, {upper:.2f}]')
 
     @staticmethod
@@ -94,10 +102,13 @@
 
     def _node_to_cubes(self, root: Node) -> list[ClosedCube]:
         if root.right is None:
             return [root.cube]
         else:
             return self._node_to_cubes(root.right) + self._node_to_cubes(root.left)
 
-    @property
-    def n_rules(self):
-        return len(list(self._hypercubes))
+    def _default_cube(self) -> Union[ClosedCube, ClosedRegressionCube, ClosedClassificationCube]:
+        if self._output == Target.CONSTANT:
+            return ClosedCube()
+        if self._output == Target.REGRESSION:
+            return ClosedRegressionCube()
+        return ClosedClassificationCube()
```

### Comparing `psyke-0.3.5/psyke/clustering/utils.py` & `psyke-0.4.2.dev2/psyke/clustering/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def select_dbscan_epsilon(data: pd.DataFrame, clusters: int) -> float:
     neighbors = NearestNeighbors(n_neighbors=min(len(data.columns) * 2, len(data))).fit(data)
     distances = sorted(np.mean(neighbors.kneighbors(data)[1], axis=1), reverse=True)
     try:
         kn = KneeLocator([d for d in range(len(distances))], distances,
                          curve='convex', direction='decreasing', online=True)
-        if kn.knee_y is None:
+        if kn.knee is None or kn.knee_y is None:
             epsilon = max(distances[-1], 1e-3)
         else:
             epsilon = kn.knee_y
     except (RuntimeWarning, UserWarning, ValueError):
         epsilon = max(distances[-1], 1e-3)
     k = 1.
     dbscan_pred = DBSCAN(eps=epsilon * k).fit_predict(data.iloc[:, :-1])
```

### Comparing `psyke-0.3.5/psyke/extraction/cart/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/cart/predictor.py` & `psyke-0.4.2.dev2/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 from __future__ import annotations
+
 from abc import ABC
 from typing import Iterable
 import numpy as np
 import pandas as pd
-from sklearn.base import ClassifierMixin, RegressorMixin
+from sklearn.base import ClassifierMixin
 from sklearn.feature_selection import SelectKBest, f_regression, f_classif
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct, clause
 from tuprolog.theory import Theory, mutable_theory
-from psyke import Extractor, logger
+from psyke import logger, PedagogicalExtractor
 from psyke.extraction.hypercubic.hypercube import HyperCube, RegressionCube, ClassificationCube, ClosedCube
 from psyke.utils.logic import create_variable_list, create_head, to_var, Simplifier
 from psyke.utils import Target, get_int_precision
 from psyke.extraction.hypercubic.strategy import Strategy, FixedStrategy
 
 
-class HyperCubeExtractor(Extractor, ABC):
-
-    def __init__(self, predictor, normalization):
-        super().__init__(predictor, normalization=normalization)
-        self._hypercubes = []
-        self._output = Target.CONSTANT
+class HyperCubePredictor:
+    def __init__(self, cubes=[], output=Target.CONSTANT, normalization=None):
+        self._hypercubes = cubes
+        self._output = output
+        self.normalization = normalization
 
     def _predict(self, dataframe: pd.DataFrame) -> Iterable:
         return np.array([self._predict_from_cubes(dict(row.to_dict())) for _, row in dataframe.iterrows()])
 
     def _predict_from_cubes(self, data: dict[str, float]) -> float | None:
         data = {k: v for k, v in data.items()}
         for cube in self._hypercubes:
             if cube.__contains__(data):
                 if self._output == Target.CLASSIFICATION:
-                    return HyperCubeExtractor._get_cube_output(cube, data)
+                    return HyperCubePredictor._get_cube_output(cube, data)
                 else:
-                    return round(HyperCubeExtractor._get_cube_output(cube, data), get_int_precision())
+                    return round(HyperCubePredictor._get_cube_output(cube, data), get_int_precision())
         return None
 
+    @property
+    def n_rules(self):
+        return len(list(self._hypercubes))
+
+    @property
+    def volume(self):
+        return sum([cube.volume() for cube in self._hypercubes])
+
+    @staticmethod
+    def _get_cube_output(cube, data: dict[str, float]) -> float:
+        return cube.output.predict(pd.DataFrame([data])).flatten()[0] if \
+            isinstance(cube, RegressionCube) else cube.output
+
+
+class HyperCubeExtractor(HyperCubePredictor, PedagogicalExtractor, ABC):
+    def __init__(self, predictor, output, normalization):
+        PedagogicalExtractor.__init__(self, predictor, normalization=normalization)
+        HyperCubePredictor.__init__(self, output=output, normalization=normalization)
+
     def _default_cube(self) -> HyperCube | RegressionCube | ClassificationCube:
         if self._output == Target.CONSTANT:
             return HyperCube()
         if self._output == Target.REGRESSION:
             return RegressionCube()
         return ClassificationCube()
 
     @staticmethod
-    def _get_cube_output(cube: HyperCube | RegressionCube, data: dict[str, float]) -> float:
-        return cube.output.predict(pd.DataFrame([data])).flatten()[0] if \
-            isinstance(cube, RegressionCube) else cube.output
-
-    @staticmethod
     def _create_head(dataframe: pd.DataFrame, variables: list[Var], output: float | LinearRegression) -> Struct:
         return create_head(dataframe.columns[-1], variables[:-1], output) \
             if not isinstance(output, LinearRegression) else \
             create_head(dataframe.columns[-1], variables[:-1], variables[-1])
 
     def _ignore_dimensions(self) -> Iterable[str]:
         return []
@@ -78,18 +92,14 @@
             structs = body.unfolded if c.body_size > 1 else [body]
             new_structs = []
             for s in structs:
                 new_structs.append(s.accept(visitor))
             new_clauses.append(clause(c.head, new_structs))
         return mutable_theory(new_clauses)
 
-    @property
-    def n_rules(self):
-        return len(self._hypercubes)
-
 
 class FeatureRanker:
     def __init__(self, feat):
         self.scores = None
         self.feat = feat
 
     def fit(self, model, samples):
@@ -140,15 +150,15 @@
     @property
     def children(self) -> list[Node]:
         return [self.right, self.left]
 
     def search(self, point: dict[str, float]) -> ClosedCube:
         if self.right is None:
             return self.cube
-        if self.right.cube.__contains__(point):
+        if point in self.right.cube:
             return self.right.search(point)
         return self.left.search(point)
 
     @property
     def leaves(self):
         if self.right is None:
             return 1
```

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from __future__ import annotations
+
+from abc import ABC
 from collections import Iterable
 import numpy as np
 import pandas as pd
 from sklearn.base import ClassifierMixin
 from tuprolog.core import clause
 from tuprolog.theory import Theory
-from psyke import Extractor, PedagogicalExtractor
+from psyke import Clustering
+from psyke.clustering import HyperCubeClustering
 from psyke.extraction.hypercubic import HyperCubeExtractor
 from psyke.utils import Target
 
 
-class CReEPy(PedagogicalExtractor, HyperCubeExtractor):
+class CReEPy(HyperCubeExtractor, ABC):
     """
     Explanator implementing CReEPy algorithm.
     """
 
     def __init__(self, predictor, depth: int, error_threshold: float, output: Target = Target.CONSTANT,
                  gauss_components: int = 5, ranks: list[(str, float)] = [], ignore_threshold: float = 0.0,
-                 normalization=None, clustering=Extractor.exact):
-        super().__init__(predictor, normalization)
-        self._output = Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else output
+                 normalization=None, clustering=Clustering.exact):
+        super().__init__(predictor, Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else output,
+                         normalization)
         self.clustering = clustering(depth, error_threshold, self._output, gauss_components)
         self.ranks = ranks
         self.ignore_threshold = ignore_threshold
 
     def _extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
-        self._hypercubes = self.clustering.extract(dataframe)
+        if not isinstance(self.clustering, HyperCubeClustering):
+            raise TypeError("clustering must be a HyperCubeClustering")
+
+        self.clustering.fit(dataframe)
+        self._hypercubes = self.clustering.get_hypercubes()
         for cube in self._hypercubes:
             for dimension in self._ignore_dimensions():
                 cube[dimension] = [-np.inf, np.inf]
         theory = self._create_theory(dataframe)
         last_clause = list(theory.clauses)[-1]
         theory.retract(last_clause)
         theory.assertZ(clause(
@@ -37,11 +44,7 @@
         last_cube = self._hypercubes[-1]
         for dimension in last_cube.dimensions.keys():
             last_cube[dimension] = [-np.inf, np.inf]
         return theory
 
     def _ignore_dimensions(self) -> Iterable[str]:
         return [dimension for dimension, relevance in self.ranks if relevance < self.ignore_threshold]
-
-    @property
-    def n_rules(self):
-        return len(list(self._hypercubes))
```

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 import pandas as pd
 from tuprolog.theory import Theory
 from psyke import get_default_random_seed, PedagogicalExtractor
 from psyke.utils import Target
 from psyke.extraction.hypercubic import HyperCubeExtractor, Grid, HyperCube
 
 
-class GridEx(PedagogicalExtractor, HyperCubeExtractor):
+class GridEx(HyperCubeExtractor):
     """
     Explanator implementing GridEx algorithm, doi:10.1007/978-3-030-82017-6_2.
     """
 
-    def __init__(self, predictor, grid: Grid, min_examples: int, threshold: float, normalization,
+    def __init__(self, predictor, grid: Grid, min_examples: int, threshold: float, normalization=None,
                  seed=get_default_random_seed()):
-        super().__init__(predictor, normalization)
+        super().__init__(predictor, Target.CONSTANT, normalization)
         self.grid = grid
         self.min_examples = min_examples
         self.threshold = threshold
         self.__generator = rnd.Random(seed)
 
     def _extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
+        self._hypercubes = []
         if isinstance(np.array(self.predictor.predict(dataframe.iloc[0:1, :-1])).flatten()[0], str):
             self._output = Target.CLASSIFICATION
         surrounding = HyperCube.create_surrounding_cube(dataframe, output=self._output)
-        surrounding.init_std(2 * self.threshold)
+        surrounding.init_diversity(2 * self.threshold)
         self._iterate(surrounding, dataframe)
         return self._create_theory(dataframe, sort)
 
     def _ignore_dimensions(self) -> Iterable[str]:
         cube = self._hypercubes[0]
         return [d for d in cube.dimensions if all(c[d] == cube[d] for c in self._hypercubes)]
```

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/hypercube.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from random import Random
 import numpy as np
 
 
 class FeatureNotFoundException(Exception):
 
     def __init__(self, feature: str):
-        super().__init__('Feature "' + feature + '" not found.')
+        super().__init__(f'Feature {feature} not found.')
 
 
 class HyperCube:
     """
     A N-dimensional cube holding a numeric value.
     """
 
@@ -138,14 +138,16 @@
         return HyperCube(self.dimensions.copy(), self._limits.copy(), self.output)
 
     def count(self, dataset: pd.DataFrame) -> int:
         return self._filter_dataframe(dataset.iloc[:, :-1]).shape[0]
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
         dimensions = dict(self.dimensions)
+        # TODO: there is something strange in the tests here
+        # print('search', [name for name in dimensions.keys()], 'in', (variables.keys()))
         for dimension in ignore:
             del dimensions[dimension]
         return [create_term(variables[name], Between(unscale(values[0], name), unscale(values[1], name)))
                 for name, values in dimensions.items()]
 
     @staticmethod
     def create_surrounding_cube(dataset: pd.DataFrame, closed: bool = False,
@@ -260,15 +262,15 @@
     def update(self, dataset: pd.DataFrame, predictor) -> None:
         filtered = self._filter_dataframe(dataset.iloc[:, :-1])
         predictions = predictor.predict(filtered)
         self._output = np.mean(predictions)
         self._diversity = np.std(predictions)
 
     # TODO: why this is not a property?
-    def init_std(self, std: float) -> None:
+    def init_diversity(self, std: float) -> None:
         self._diversity = std
 
 
 class RegressionCube(HyperCube):
     def __init__(self, dimension: dict[str, tuple] = None):
         super().__init__(dimension=dimension, output=LinearRegression())
```

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from psyke.extraction.hypercubic.hypercube import GenericCube
 from psyke.extraction.hypercubic.utils import MinUpdate, Expansion
 from psyke.utils import get_default_random_seed, Target
 
 DomainProperties = (Iterable[MinUpdate], GenericCube)
 
 
-class ITER(PedagogicalExtractor, HyperCubeExtractor):
+class ITER(HyperCubeExtractor):
     """
     Explanator implementing ITER algorithm, doi:10.1007/11823728_26.
     """
 
     def __init__(self, predictor, min_update, n_points, max_iterations, min_examples, threshold, fill_gaps,
                  normalization, output: Target = Target.CONSTANT, seed=get_default_random_seed()):
-        super().__init__(predictor, normalization)
+        super().__init__(predictor, output, normalization)
         if output is Target.REGRESSION:
             raise NotImplementedError
         self.predictor = predictor
         self.min_update = min_update
         self.n_points = n_points
         self.max_iterations = max_iterations
         self.min_examples = min_examples
```

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/strategy.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/hypercubic/utils.py` & `psyke-0.4.2.dev2/psyke/extraction/hypercubic/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import math
 import warnings
 
 warnings.simplefilter("ignore")
 
 Dimension = tuple[float, float]
 Dimensions = dict[str, Dimension]
@@ -44,7 +45,12 @@
 
 class ZippedDimension:
 
     def __init__(self, name: str, this_dimension: Dimension, other_dimension: Dimension):
         self.name = name
         self.this_dimension = this_dimension
         self.other_dimension = other_dimension
+
+    def __eq__(self, other: ZippedDimension) -> bool:
+        return (self.name == other.name) and (self.this_dimension == other.this_dimension) and \
+               (self.other_dimension == other.other_dimension)
+
```

### Comparing `psyke-0.3.5/psyke/extraction/real/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/real/utils.py` & `psyke-0.4.2.dev2/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/trepan/__init__.py` & `psyke-0.4.2.dev2/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/extraction/trepan/utils.py` & `psyke-0.4.2.dev2/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/schema/__init__.py` & `psyke-0.4.2.dev2/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/tuning/__init__.py` & `psyke-0.4.2.dev2/psyke/tuning/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,45 @@
+from abc import ABC
 from enum import Enum
 import numpy as np
 import pandas as pd
 
 from psyke.utils import Target
 
 
 class Objective(Enum):
     MODEL = 1,
     DATA = 2
 
 
 class Optimizer:
-    def __init__(self, predictor, algorithm, dataframe: pd.DataFrame, max_mae_increase: float = 1.2,
-                 min_rule_decrease: float = 0.9, readability_tradeoff: float = 0.1, max_depth: int = 10,
-                 patience: int = 5, objective: Objective = Objective.MODEL, normalization=None):
-        self.predictor = predictor
-        self.algorithm = algorithm
+    def __init__(self, dataframe: pd.DataFrame, algorithm, output: Target = Target.CONSTANT,
+                 max_mae_increase: float = 1.2, min_rule_decrease: float = 0.9,
+                 readability_tradeoff: float = 0.1, patience: int = 5,
+                 normalization=None, discretization=None):
         self.dataframe = dataframe
+        self.algorithm = algorithm
+        self.output = output
         self.max_mae_increase = max_mae_increase
         self.min_rule_decrease = min_rule_decrease
         self.readability_tradeoff = readability_tradeoff
         self.patience = patience
-        self.max_depth = max_depth
-        self.objective = objective
-        self.model_mae = abs(self.predictor.predict(dataframe.iloc[:, :-1]).flatten() -
-                             self.dataframe.iloc[:, -1].values).mean()
         self.params = None
         self.normalization = normalization
+        self.discretization = discretization
+
+    def search(self):
+        raise NotImplementedError
 
-    def _depth_improvement(self, first, second):
-        if second[0] == first[0]:
-            return (first[1] - second[1]) * 2
+    def _depth_improvement(self, best, other):
+        if other[0] == best[0]:
+            return (best[1] - other[1]) * 2
         return 1 / (
-                (1 - second[0] / first[0]) ** self.readability_tradeoff *
-                np.ceil(second[1] / self.readability_tradeoff) / np.ceil(first[1] / self.readability_tradeoff)
+                (1 - other[0] / best[0]) ** self.readability_tradeoff *
+                np.ceil(other[1] / self.readability_tradeoff) / np.ceil(best[1] / self.readability_tradeoff)
         )
 
     @staticmethod
     def _best(params):
         param_dict = {Optimizer.__score(t): t for t in params}
         min_param = min(param_dict)
         return min_param, param_dict[min_param]
@@ -48,16 +50,28 @@
 
     def _best_param(self, param):
         param_dict = {t[param]: t for t in self.params}
         min_param = min(param_dict)
         return min_param, param_dict[min_param]
 
     def get_best(self):
-        names = [self.algorithm, "  MAE  ", "N rules"]
+        names = [self.algorithm, "Predictive loss", "N rules"]
         params = [Optimizer._best(self.params), self._best_param(0), self._best_param(1)]
         for n, p in zip(names, params):
             self._print_params(n, p[1])
             print()
         return Optimizer._best(self.params)[1], self._best_param(0)[1], self._best_param(1)[1]
 
     def _print_params(self, n, param):
         raise NotImplementedError
+
+
+class GridOptimizer(Optimizer, ABC):
+    def __init__(self, predictor, algorithm, dataframe: pd.DataFrame, max_mae_increase: float = 1.2,
+                 min_rule_decrease: float = 0.9, readability_tradeoff: float = 0.1, max_depth: int = 10,
+                 patience: int = 5, objective: Objective = Objective.MODEL, output: Target = Target.CONSTANT,
+                 normalization=None, discretization=None):
+        super().__init__(dataframe, algorithm, output, max_mae_increase, min_rule_decrease, readability_tradeoff,
+                         patience, normalization, discretization)
+        self.predictor = predictor
+        self.max_depth = max_depth
+        self.objective = objective
```

### Comparing `psyke-0.3.5/psyke/tuning/crash/__init__.py` & `psyke-0.4.2.dev2/psyke/tuning/crash/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 
 import numpy as np
 import pandas as pd
 
-from psyke import Extractor
+from psyke import Extractor, Clustering
 from psyke.tuning import Objective, Optimizer
 from psyke.utils import Target
 
 
 class CRASH(Optimizer):
     class Algorithm(Enum):
         ExACT = 1,
@@ -47,16 +47,17 @@
         step = self.model_mae / 2.0
         threshold = self.model_mae * 0.9
         params = []
         patience = self.patience
         while patience > 0:
             print(f"{self.algorithm}. Depth: {depth}. Threshold = {threshold:.2f}. ", end="")
             extractor = Extractor.creepy(
-                self.predictor, depth, threshold, self.output, 10, normalization=self.normalization,
-                clustering=Extractor.cream if self.algorithm == CRASH.Algorithm.CREAM else Extractor.exact
+                self.predictor, depth=depth, error_threshold=threshold, output=self.output,
+                gauss_components=10, normalization=self.normalization,
+                clustering=Clustering.cream if self.algorithm == CRASH.Algorithm.CREAM else Clustering.exact
             )
             _ = extractor.extract(self.dataframe)
             mae, n = (extractor.mae(self.dataframe, self.predictor) if self.objective == Objective.MODEL else
                       extractor.mae(self.dataframe)), extractor.n_rules
             print(f"MAE = {mae:.2f}, {n} rules")
 
             if len(params) == 0:
```

### Comparing `psyke-0.3.5/psyke/tuning/pedro/__init__.py` & `psyke-0.4.2.dev2/psyke/tuning/pedro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     def __init__(self, predictor, dataframe: pd.DataFrame, max_mae_increase: float = 1.2,
                  min_rule_decrease: float = 0.9, readability_tradeoff: float = 0.1, max_depth: int = 3,
                  patience: int = 3, algorithm: Algorithm = Algorithm.GRIDREX, objective: Objective = Objective.MODEL,
                  normalization=None):
         super().__init__(predictor, algorithm, dataframe, max_mae_increase, min_rule_decrease, readability_tradeoff,
                          max_depth, patience, objective, normalization)
         self.ranked = FeatureRanker(dataframe.columns[:-1]).fit(predictor, dataframe.iloc[:, :-1]).rankings()
+        self.model_mae = abs(self.predictor.predict(dataframe.iloc[:, :-1]).flatten() -
+                             self.dataframe.iloc[:, -1].values).mean()
 
     def __search_threshold(self, grid, critical, max_partitions):
         step = self.model_mae / 2.0
         threshold = self.model_mae * 0.5
         params = []
         patience = self.patience
         while patience > 0:
```

### Comparing `psyke-0.3.5/psyke/utils/__init__.py` & `psyke-0.4.2.dev2/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/utils/dataframe.py` & `psyke-0.4.2.dev2/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/utils/logic.py` & `psyke-0.4.2.dev2/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/utils/metrics.py` & `psyke-0.4.2.dev2/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/utils/plot.py` & `psyke-0.4.2.dev2/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke/utils/sorted.py` & `psyke-0.4.2.dev2/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/psyke.egg-info/PKG-INFO` & `psyke-0.4.2.dev2/psyke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.5
+Version: 0.4.2.dev2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.5/psyke.egg-info/SOURCES.txt` & `psyke-0.4.2.dev2/psyke.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -26,47 +26,27 @@
 psyke/extraction/hypercubic/gridex/__init__.py
 psyke/extraction/hypercubic/gridrex/__init__.py
 psyke/extraction/hypercubic/iter/__init__.py
 psyke/extraction/real/__init__.py
 psyke/extraction/real/utils.py
 psyke/extraction/trepan/__init__.py
 psyke/extraction/trepan/utils.py
-psyke/gui/__init__.py
-psyke/gui/__main__.py
-psyke/gui/controller/Controller.py
-psyke/gui/controller/__init__.py
-psyke/gui/libs/garden/garden.matplotlib/LICENSE
-psyke/gui/libs/garden/garden.matplotlib/README.md
-psyke/gui/libs/garden/garden.matplotlib/__init__.py
-psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
-psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
-psyke/gui/model/Model.py
-psyke/gui/model/__init__.py
-psyke/gui/view/DataPanel.py
-psyke/gui/view/ExtractorPanel.py
-psyke/gui/view/FeaturePanel.py
-psyke/gui/view/PlotPanel.py
-psyke/gui/view/PredictorPanel.py
-psyke/gui/view/TheoryPanel.py
-psyke/gui/view/View.py
-psyke/gui/view/__init__.py
-psyke/gui/view/layout.py
-psyke/gui/view/plot.py
-psyke/gui/view/style.kv
 psyke/schema/__init__.py
 psyke/tuning/__init__.py
 psyke/tuning/crash/__init__.py
+psyke/tuning/orchid/__init__.py
 psyke/tuning/pedro/__init__.py
 psyke/utils/__init__.py
 psyke/utils/dataframe.py
 psyke/utils/logic.py
 psyke/utils/metrics.py
 psyke/utils/plot.py
 psyke/utils/sorted.py
 test/psyke/__init__.py
+test/psyke/clustering/__init__.py
 test/psyke/extraction/__init__.py
 test/psyke/extraction/cart/__init__.py
 test/psyke/extraction/cart/test_cart.py
 test/psyke/extraction/cart/test_simplified_cart.py
 test/psyke/extraction/hypercubic/__init__.py
 test/psyke/extraction/hypercubic/test_hypercube.py
 test/psyke/extraction/hypercubic/gridex/__init__.py
```

### Comparing `psyke-0.3.5/setup.py` & `psyke-0.4.2.dev2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-import platform
-import re
-
 from setuptools import setup, find_packages
 import pathlib
-import sys
-import os
 import subprocess
 import distutils.cmd
 
 here = pathlib.Path(__file__).parent.resolve()
 
 version_file = here / 'VERSION'
 
@@ -20,18 +15,14 @@
 BATCH_SIZE: int = 16
 REQUIREMENTS = [
     'numpy~=1.24.0',
     'pandas~=1.5.0',
     'scikit-learn~=1.2.0',
     '2ppy~=0.4.0',
     'kneed~=0.8.1',
-    'kivy~=2.2.0',
-    'matplotlib~=3.7.0',
-    'kivy-garden~=0.1.5',
-    'screeninfo~=0.8',
     'sympy~=1.11'
 ]  # Optional
 
 
 def format_git_describe_version(version):
     if '-' in version:
         splitted = version.split('-')
@@ -75,42 +66,14 @@
     def finalize_options(self):
         pass
 
     def run(self):
         print(version)
 
 
-class InstallGardenDependency(distutils.cmd.Command):
-    """A custom command to install Garden dependencies"""
-
-    garden_executable = pathlib.Path(sys.executable).parent / 'garden'
-
-    description = 'runs `garden install [--app] PACKAGE`'
-    user_options = [
-        ('package=', None, 'the package to be installed'),
-        ('as-library', None, 'wether to install the dependency as a local library')
-    ]
-
-    def initialize_options(self):
-        self.package = None
-        self.as_library = False
-
-    def finalize_options(self):
-        if self.package is None:
-            raise ValueError("No Garden package provided")
-
-    def run(self):
-        cmd = f"{sys.executable} {InstallGardenDependency.garden_executable} install "
-        if self.as_library:
-            cmd += "--app "
-            os.chdir(here / "psyke" / "gui")
-        cmd += self.package
-        os.system(cmd)
-
-
 class CreateTestPredictors(distutils.cmd.Command):
     description = 'gets the project version from git describe'
     user_options = []
 
     def initialize_options(self):
         pass
 
@@ -249,11 +212,10 @@
         # 'Funding': 'https://donate.pypi.org',
         # 'Say Thanks!': 'http://saythanks.io/to/example',
         'Source': 'https://github.com/psykei/psyke-python',
     },
     cmdclass={
         'get_project_version': GetVersionCommand,
         'create_test_predictors': CreateTestPredictors,
-        'create_theory_plot': CreateTheoryPlot,
-        'garden_install': InstallGardenDependency
+        'create_theory_plot': CreateTheoryPlot
     },
 )
```

### Comparing `psyke-0.3.5/test/psyke/__init__.py` & `psyke-0.4.2.dev2/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/cart/test_cart.py` & `psyke-0.4.2.dev2/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.4.2.dev2/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from psyke import logger
 from parameterized import parameterized_class
-from psyke.utils import get_default_precision
 from test.psyke import initialize
 import unittest
 
 
 @parameterized_class(initialize('gridex'))
 class TestGridEx(unittest.TestCase):
```

### Comparing `psyke-0.3.5/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.4.2.dev2/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,86 @@
 import unittest
 import pandas as pd
+from sklearn.linear_model import LinearRegression
 
-from psyke.extraction.hypercubic.hypercube import FeatureNotFoundException
-from psyke.extraction.hypercubic.utils import MinUpdate, Expansion
+from psyke.extraction.hypercubic.hypercube import FeatureNotFoundException, ClosedRegressionCube, \
+    ClosedClassificationCube, ClosedCube, ClassificationCube, RegressionCube
+from psyke.extraction.hypercubic.utils import MinUpdate, Expansion, ZippedDimension
 from psyke.utils import get_int_precision
 from sklearn.neighbors import KNeighborsRegressor
 from test.psyke import Predictor
 from psyke.extraction.hypercubic import HyperCube
 from test.resources.datasets import get_dataset_path
 
 
 class AbstractTestHypercube(unittest.TestCase):
 
     def setUp(self):
-        self.dimensions = {'X': (0.2, 0.6), 'Y': (0.7, 0.9)}
+        self.x = (0.2, 0.6)
+        self.y = (0.7, 0.9)
+        self.dimensions = {'X': self.x, 'Y': self.y}
         self.mean = 0.5
         self.cube = HyperCube(self.dimensions, set(), self.mean)
         cubes = [({'X': (6.4, 7.9), 'Y': (5.7, 8.9)}, 5.3),
                  ({'X': (0.7, 0.8), 'Y': (0.75, 0.85)}, 6.1),
                  ({'X': (6.6, 7.0), 'Y': (9.1, 10.5)}, 7.5)]
         self.hypercubes = [HyperCube(cube[0], set(), cube[1]) for cube in cubes]
         self.dataset = pd.read_csv(get_dataset_path('arti'))
         self.filtered_dataset = self.dataset[self.dataset.apply(
             lambda row: (0.2 <= row['X'] < 0.6) & (0.7 <= row['Y'] < 0.9), axis=1)]
 
+    def tuple_provider(self, closed=False):
+        return (({'X': (self.x[0] + self.x[1]) / 2, 'Y': (self.y[0] + self.y[1]) / 2}, True),
+                ({'X': self.x[0], 'Y': self.y[0]}, True),
+                ({'X': self.x[0], 'Y': self.y[1]}, closed),
+                ({'X': self.x[1], 'Y': self.y[0]}, closed),
+                ({'X': self.x[1], 'Y': self.y[1]}, closed),
+                ({'X': 1.5, 'Y': 3.6}, False))
+
 
 class TestHypercube(AbstractTestHypercube):
 
-    def test_get_dimension(self):
+    def test_dimension(self):
         self.assertEqual(self.dimensions, self.cube.dimensions)
 
-    def test_get_limit_count(self):
+    def test_limit_count(self):
         self.assertEqual(0, self.cube.limit_count)
         self.cube.add_limit('X', '+')
         self.assertEqual(1, self.cube.limit_count)
         self.cube.add_limit('Y', '-')
         self.assertEqual(2, self.cube.limit_count)
         self.cube.add_limit('X', '+')
         self.assertEqual(2, self.cube.limit_count)
 
-    def test_get_mean(self):
+    def test_output(self):
         self.assertEqual(self.mean, self.cube.output)
 
     def test_get(self):
-        self.assertEqual((0.2, 0.6), self.cube['X'])
-        self.assertEqual((0.7, 0.9), self.cube['Y'])
+        self.assertEqual(self.x, self.cube['X'])
+        self.assertEqual(self.y, self.cube['Y'])
         with self.assertRaises(FeatureNotFoundException):
-            dummy = self.cube['Z']
+            _ = self.cube['Z']
 
     def test_get_first(self):
-        self.assertEqual(0.2, self.cube.get_first('X'))
-        self.assertEqual(0.7, self.cube.get_first('Y'))
+        self.assertEqual(self.x[0], self.cube.get_first('X'))
+        self.assertEqual(self.y[0], self.cube.get_first('Y'))
         with self.assertRaises(FeatureNotFoundException):
-            self.cube.get_first('Z')
+            _ = self.cube.get_first('Z')
 
     def test_get_second(self):
-        self.assertEqual(0.6, self.cube.get_second('X'))
-        self.assertEqual(0.9, self.cube.get_second('Y'))
+        self.assertEqual(self.x[1], self.cube.get_second('X'))
+        self.assertEqual(self.y[1], self.cube.get_second('Y'))
         with self.assertRaises(FeatureNotFoundException):
-            self.cube.get_second('Z')
+            _ = self.cube.get_second('Z')
 
     def test_copy(self):
         copy = self.cube.copy()
         self.assertEqual(self.cube.dimensions, copy.dimensions)
         self.assertEqual(self.cube.output, copy.output)
+        self.assertIsInstance(copy, HyperCube)
 
     def test_expand(self):
         arguments = TestHypercube.expansion_provider()
         for arg in arguments:
             arg[0].expand(arg[1], self.hypercubes)
             self.assertEqual(arg[2], arg[0][arg[1].feature])
 
@@ -97,15 +110,15 @@
         self.assertFalse(no_volume.has_volume())
 
     def test_equal(self):
         self.assertTrue(self.cube == self.cube)
         self.assertFalse(self.cube == self.hypercubes[1])
 
     def test_contains(self):
-        arguments = TestHypercube.tuple_provider()
+        arguments = self.tuple_provider()
         for arg in arguments:
             self.assertEqual(arg[1], arg[0] in self.cube)
 
     def test_count(self):
         self.assertEqual(self.dataset.shape[0], HyperCube.create_surrounding_cube(self.dataset).count(self.dataset))
         self.assertEqual(self.filtered_dataset.shape[0], self.cube.count(self.dataset))
 
@@ -134,19 +147,38 @@
         self.assertEqual('*', self.cube.check_limits('X'))
         self.assertIsNone(self.cube.check_limits('Y'))
         self.cube.add_limit('Y', '+')
         self.assertEqual('+', self.cube.check_limits('Y'))
         self.cube.add_limit('Y', '-')
         self.assertEqual('*', self.cube.check_limits('Y'))
 
-    def test_update_mean(self):
+    def test_filter_indices(self):
+        expected = (self.dataset.X >= self.x[0]) & (self.dataset.X < self.x[1]) & \
+                   (self.dataset.Y >= self.y[0]) & (self.dataset.Y < self.y[1])
+        filtered = self.cube.filter_indices(self.dataset.iloc[:, :-1])
+        self.assertTrue(all(expected == filtered))
+
+    def test_filter_dataframe(self):
+        expected = (self.dataset.X >= self.x[0]) & (self.dataset.X < self.x[1]) & \
+                   (self.dataset.Y >= self.y[0]) & (self.dataset.Y < self.y[1])
+        expected = self.dataset[expected].iloc[:, :-1]
+        filtered = self.cube._filter_dataframe(self.dataset.iloc[:, :-1])
+        self.assertTrue(all(expected == filtered))
+
+    def test_update(self):
         model = KNeighborsRegressor()
         model.fit(self.dataset.iloc[:, :-1], self.dataset.iloc[:, -1])
         predictor = Predictor(model)
         self.cube.update(self.dataset, predictor)
+        predictions = model.predict(self.dataset[
+            (self.dataset.X >= self.x[0]) & (self.dataset.X < self.x[1]) &
+            (self.dataset.Y >= self.y[0]) & (self.dataset.Y < self.y[1])
+        ].iloc[:, :-1])
+        self.assertEqual(self.cube.output, predictions.mean())
+        self.assertEqual(self.cube.diversity, predictions.std())
 
     def test_update_dimension(self):
         new_lower, new_upper = 0.6, 1.4
         updated = {'X': (new_lower, new_upper),
                    'Y': (0.7, 0.9)}
         new_cube1 = self.cube.copy()
         new_cube1.update_dimension('X', new_lower, new_upper)
@@ -170,14 +202,54 @@
 
     def test_check_overlap(self):
         self.assertTrue(HyperCube.check_overlap((self.hypercubes[0], ), (self.hypercubes[0].copy(), )))
         self.assertTrue(HyperCube.check_overlap(self.hypercubes, self.hypercubes + [self.hypercubes[0].copy()]))
         self.assertFalse(HyperCube.check_overlap(self.hypercubes, self.hypercubes))
         self.assertFalse(HyperCube.check_overlap(self.hypercubes[0:1], self.hypercubes[1:]))
 
+    def test_init_diversity(self):
+        d = 2.3
+        self.cube.init_diversity(d)
+        self.assertEqual(self.cube.diversity, d)
+
+    def test_diversity(self):
+        self.assertEqual(self.cube.diversity, 0.0)
+        d = 56.3
+        self.cube.init_diversity(d)
+        self.assertEqual(self.cube.diversity, d)
+
+    def test_volume(self):
+        self.assertEqual(self.cube.volume(), (self.x[1] - self.x[0]) * (self.y[1] - self.y[0]))
+
+    def test_diagonal(self):
+        self.assertEqual(self.cube.diagonal(), ((self.x[1] - self.x[0])**2 + (self.y[1] - self.y[0])**2)**0.5)
+
+    def test_is_adjacent(self):
+        cube_adj = HyperCube({'X': (0.6, 0.9), 'Y': self.y}, set(), self.mean)
+        self.assertTrue(self.cube.is_adjacent(cube_adj))
+        cube_not_adj = HyperCube({'X': self.y, 'Y': self.x}, set(), self.mean)
+        self.assertFalse(self.cube.is_adjacent(cube_not_adj))
+
+    def test_merge_along_dimension(self):
+        cube_adj = HyperCube({'X': (0.6, 0.9), 'Y': self.y}, set(), self.mean)
+        merged = self.cube.merge_along_dimension(cube_adj, 'X')
+        self.assertEqual(merged['X'][0], 0.2)
+        self.assertEqual(merged['X'][1], 0.9)
+
+    def test_zip_dimensions(self):
+        cube = HyperCube({'X': self.y, 'Y': self.x})
+        expected = [ZippedDimension(d, self.cube[d], cube[d]) for d in self.dimensions.keys()]
+        self.assertEqual(self.cube._zip_dimensions(cube), expected)
+
+    def test_fit_dimension(self):
+        new_dimensions = {'X': (5.2, 3.6), 'Y': (9.3, 6.4)}
+        self.assertEqual(self.cube._fit_dimension(new_dimensions), new_dimensions)
+        new_dimensions = {'Z': (5.2, 6.4)}
+        self.assertEqual(self.cube._fit_dimension(new_dimensions), new_dimensions)
+
     @staticmethod
     def expansion_provider():
         cube1 = HyperCube({'X': (2.3, 6.4), 'Y': (8.9, 12.3)}, output=2.3)
         fake1 = cube1.copy()
         fake1.update_dimension('X', 0.5, 2.3)
         fake2 = cube1.copy()
         fake2.update_dimension('X', 6.4, 12.9)
@@ -189,17 +261,66 @@
         fake4.update_dimension('X', 12.3, 15.2)
 
         return [(cube1.copy(), Expansion(fake1, 'X', '-', 0.0), (0.5, 6.4)),
                 (cube1.copy(), Expansion(fake2, 'X', '+', 0.0), (2.3, 6.6)),
                 (cube2.copy(), Expansion(fake3, 'X', '-', 0.0), (7.0, 12.3)),
                 (cube2.copy(), Expansion(fake4, 'X', '+', 0.0), (9.5, 15.2))]
 
-    @staticmethod
-    def tuple_provider():
-        return (({'X': 0.5, 'Y': 0.8}, True),
-                ({'X': 0.1, 'Y': 0.8}, False),
-                ({'X': 0.5, 'Y': 0.95}, False),
-                ({'X': 0.1, 'Y': 0.95}, False))
+
+class TestRegressionCube(AbstractTestHypercube):
+
+    def test_copy(self):
+        cube = RegressionCube(self.dimensions)
+        copy = cube.copy()
+        self.assertEqual(cube.dimensions, copy.dimensions)
+        self.assertIsInstance(copy.output, LinearRegression)
+        self.assertIsInstance(copy, RegressionCube)
+
+
+class TestClassificationCube(AbstractTestHypercube):
+
+    def test_copy(self):
+        cube = ClassificationCube(self.dimensions)
+        copy = cube.copy()
+        self.assertEqual(cube.dimensions, copy.dimensions)
+        self.assertEqual(cube.output, copy.output)
+        self.assertIsInstance(copy, ClassificationCube)
+
+
+class TestClosedCube(AbstractTestHypercube):
+
+    def test_copy(self):
+        cube = ClosedCube(self.dimensions)
+        copy = cube.copy()
+        self.assertEqual(cube.dimensions, copy.dimensions)
+        self.assertEqual(cube.output, copy.output)
+        self.assertIsInstance(copy, ClosedCube)
+
+    def test_contains(self):
+        cube = ClosedCube(self.dimensions)
+        arguments = self.tuple_provider(True)
+        for arg in arguments:
+            self.assertEqual(arg[1], arg[0] in cube)
+
+
+class TestClosedRegressionCube(AbstractTestHypercube):
+
+    def test_copy(self):
+        cube = ClosedRegressionCube(self.dimensions)
+        copy = cube.copy()
+        self.assertEqual(cube.dimensions, copy.dimensions)
+        self.assertIsInstance(copy.output, LinearRegression)
+        self.assertIsInstance(copy, ClosedRegressionCube)
+
+
+class TestClosedClassificationCube(AbstractTestHypercube):
+
+    def test_copy(self):
+        cube = ClosedClassificationCube(self.dimensions)
+        copy = cube.copy()
+        self.assertEqual(cube.dimensions, copy.dimensions)
+        self.assertEqual(cube.output, copy.output)
+        self.assertIsInstance(copy, ClosedClassificationCube)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `psyke-0.3.5/test/psyke/extraction/real/test_real.py` & `psyke-0.4.2.dev2/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/real/test_rule.py` & `psyke-0.4.2.dev2/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/trepan/test_node.py` & `psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/trepan/test_split.py` & `psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.4.2.dev2/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/utils/test_prune.py` & `psyke-0.4.2.dev2/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/utils/test_simplify.py` & `psyke-0.4.2.dev2/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.5/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.4.2.dev2/test/psyke/utils/test_simplify_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from psyke.extraction.hypercubic import Grid
 from test import get_dataset
 
 
 class TestSimplifyFormatter(unittest.TestCase):
 
     def test_simplify_formatter(self):
-        iris_data = get_dataset('house')
-        train, test = train_test_split(iris_data, test_size=0.5, random_state=get_default_random_seed())
+        data = get_dataset('house')
+        train, test = train_test_split(data, test_size=0.5, random_state=get_default_random_seed())
         predictor = DecisionTreeRegressor()
         predictor.fit(train.iloc[:, :-1], train.iloc[:, -1])
         extractor = Extractor.gridrex(predictor, Grid())
         theory = extractor.extract(train)
         # print(pretty_theory(theory))
```

### Comparing `psyke-0.3.5/test/resources/tests/__init__.py` & `psyke-0.4.2.dev2/test/resources/tests/__init__.py`

 * *Files identical despite different names*

