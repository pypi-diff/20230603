# Comparing `tmp/HTMACat-1.0.4.tar.gz` & `tmp/HTMACat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTMACat-1.0.4.tar", last modified: Wed Apr 26 08:13:04 2023, max compression
+gzip compressed data, was "HTMACat-1.0.5.tar", last modified: Fri Jun  2 23:59:03 2023, max compression
```

## Comparing `HTMACat-1.0.4.tar` & `HTMACat-1.0.5.tar`

### file list

```diff
@@ -1,68 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.672052 HTMACat-1.0.4/HTMACat/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/Base_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    60385 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/Extract_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/IO.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.672052 HTMACat-1.0.4/HTMACat/NEB/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/Construct_neb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/Construct_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/Dismove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/Post_struc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/post_neb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/NEB/vaspneb6.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.672052 HTMACat-1.0.4/HTMACat/catkit/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.672052 HTMACat-1.0.4/HTMACat/catkit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/HTMACat/catkit/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/adsorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/HTMACat/catkit/gen/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gen/utils/vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/catkit/gratoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/HTMACat/descriptor/
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_NEB.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_coad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_surface_single.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/descriptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/HTMACat/model/
--rw-r--r--   0 runner    (1001) docker     (123)    16569 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/model/Ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/model/Construct_adsorption_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/model/Structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/model/Substrate.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.676052 HTMACat-1.0.4/HTMACat/post/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/Extract_adener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/Extract_adener_alloy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/Extract_adener_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/Extract_cal_fre.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-26 08:13:01.000000 HTMACat-1.0.4/HTMACat/post/cal_adsE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:13:04.672052 HTMACat-1.0.4/HTMACat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:13:04.000000 HTMACat-1.0.4/HTMACat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-04-26 08:13:01.000000 HTMACat-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 08:13:04.676052 HTMACat-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-26 08:13:01.000000 HTMACat-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-26 08:13:01.000000 HTMACat-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:13:04.676052 HTMACat-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 08:13:01.000000 HTMACat-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.202231 HTMACat-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.190231 HTMACat-1.0.5/HTMACat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/Base_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61587 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/Extract_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/IO.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.194231 HTMACat-1.0.5/HTMACat/NEB/
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/Construct_neb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/Construct_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/Dismove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/Post_struc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/post_neb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/NEB/vaspneb6.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.194231 HTMACat-1.0.5/HTMACat/catkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.194231 HTMACat-1.0.5/HTMACat/catkit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.198231 HTMACat-1.0.5/HTMACat/catkit/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32321 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/adsorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24582 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.198231 HTMACat-1.0.5/HTMACat/catkit/gen/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/utils_mdnm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gen/utils/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/catkit/gratoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.202231 HTMACat-1.0.5/HTMACat/descriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_NEB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_coad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_surface_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/descriptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.202231 HTMACat-1.0.5/HTMACat/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/Ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/Construct_adsorption_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/Species.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/Structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/Substrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.202231 HTMACat-1.0.5/HTMACat/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/Extract_adener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/Extract_adener_alloy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/Extract_adener_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/Extract_cal_fre.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-02 23:58:59.000000 HTMACat-1.0.5/HTMACat/post/cal_adsE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.194231 HTMACat-1.0.5/HTMACat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-02 23:59:02.000000 HTMACat-1.0.5/HTMACat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-02 23:59:03.000000 HTMACat-1.0.5/HTMACat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 23:59:02.000000 HTMACat-1.0.5/HTMACat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 23:59:02.000000 HTMACat-1.0.5/HTMACat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 23:59:02.000000 HTMACat-1.0.5/HTMACat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 23:59:02.000000 HTMACat-1.0.5/HTMACat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-02 23:58:59.000000 HTMACat-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-02 23:59:03.202231 HTMACat-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-02 23:58:59.000000 HTMACat-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 23:59:00.000000 HTMACat-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 23:59:03.202231 HTMACat-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-02 23:59:00.000000 HTMACat-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:59:03.202231 HTMACat-1.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_adsorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_coadsorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_slab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-02 23:59:00.000000 HTMACat-1.0.5/test/test_species.py
```

### Comparing `HTMACat-1.0.4/HTMACat/Extract_info.py` & `HTMACat-1.0.5/HTMACat/Extract_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,134 @@
-# -*- coding: UTF-8 -*-
 from ase.io import read
 from HTMACat.catkit.gen.utils import to_gratoms
- 
+
 import os
-#from catkit.build import molecule
+
+# from catkit.build import molecule
 from ase.build import molecule
 from itertools import chain
 from collections import Counter
 
 
-
-### 1.Substract the reaction species
+# 1.Substract the reaction species
 def Extract_reaction(Efile):
-    """
-    Extract the adsorbate and gas species from a given reaction file.
+    """Extract the adsorbate and gas species from a given reaction file.
 
     Parameters
     ----------
     Efile : str
         Path of the reaction file.The reaction formula can be NH3(a)+O(a)=N(a)+NO(a)
 
     Returns
     -------
     tuple
         A tuple of two lists containing adsorbate and gas species, respectively.
-
     """
 
     ReaInfo = open(f"{Efile}", "r+")
     ad_species = []
     gas_species = []
     specie_f_mol = []
     specie_f_typ = []
     specie_b_mol = []
     specie_b_typ = []
 
     for index, line in enumerate(ReaInfo):
-        specie_f = line.split('=')[0].strip()
-        specie_b = line.split('=')[1].strip()
+        specie_f = line.split("=")[0].strip()
+        specie_b = line.split("=")[1].strip()
 
-        ### Operation on reactant
+        # Operation on reactant
         ##Extract the product molecule and type (a g s)
         specie_f_list = []
-        for i in range(len(specie_f.split('+'))):
-            specie_f_list += [specie_f.split('+')[i].strip()]
+        for i in range(len(specie_f.split("+"))):
+            specie_f_list += [specie_f.split("+")[i].strip()]
         for j, specie in enumerate(specie_f_list):
-            mol = specie.split('(', 1)[0].strip()
-            typ = specie.split('(', 1)[1].split(')')[0].strip()
-            if typ == 'a':
+            mol = specie.split("(", 1)[0].strip()
+            typ = specie.split("(", 1)[1].split(")")[0].strip()
+            if typ == "a":
                 if mol not in ad_species:
                     ad_species += [mol]
-            elif typ == 'g':
+            elif typ == "g":
                 if mol not in gas_species:
                     gas_species += [mol]
             specie_f_mol += [mol]
             specie_f_typ += [typ]
-        #print(ad_species)
-        #print(gas_species)
+        # print(ad_species)
+        # print(gas_species)
 
-        ### Operation on product
+        # Operation on product
         ##Exstract the product molecule and type (a g s)
         specie_b_list = []
-        for i in range(len(specie_b.split('+'))):
-            specie_b_list += [specie_b.split('+')[i].strip()]
+        for i in range(len(specie_b.split("+"))):
+            specie_b_list += [specie_b.split("+")[i].strip()]
         for j, specie in enumerate(specie_b_list):
-            mol = specie.split('(', 1)[0].strip()
-            typ = specie.split('(', 1)[1].split(')')[0].strip()
-            if typ == 'a':
+            mol = specie.split("(", 1)[0].strip()
+            typ = specie.split("(", 1)[1].split(")")[0].strip()
+            if typ == "a":
                 if mol not in ad_species:
                     ad_species += [mol]
-            elif typ == 'g':
+            elif typ == "g":
                 if mol not in gas_species:
                     gas_species += [mol]
             specie_b_mol += [mol]
             specie_b_typ += [typ]
-        #print(ad_species)
-        #print(gas_species)
+        # print(ad_species)
+        # print(gas_species)
 
     ReaInfo.close()
     return ad_species, gas_species
 
 
-#print(Extract_reaction())
+# print(Extract_reaction())
 
 
-### 2.Substract energy of adsoprtion configuration
+# 2.Substract energy of adsoprtion configuration
 def Extract_energy(Efile, struc):
-    """
-        Batch extraction of calculated energy for specific species structure
+    """Batch extraction of calculated energy for specific species structure.
+
+    Parameters
+    ----------
+    Efile : str
+        Energy information file
+    struc : list of str
+        Specific species that want to extract energy
+
+    Returns
+    -------
+    tuple
+        A tuple containing two lists:
 
-        Parameters
-        ----------
-        Efile : str
-            Energy information file
-        struc : list of str
-            Specific species that want to extract energy
-
-        Returns
-        -------
-        tuple
-            A tuple containing two lists:
-
-            - Ener : list of float
-                The list of extracted energies.
-            - order : list of str
-                The sequential list of the extracted energies.
+        - Ener : list of float
+            The list of extracted energies.
+        - order : list of str
+            The sequential list of the extracted energies.
     """
     EnerInfo = open(Efile, "r+")
     order = []
     Ener = []
     for i, ads_ener in enumerate(EnerInfo):
-        ads = ads_ener.split(',', 1)[0]
-        ener = ads_ener.split(',', 1)[1].strip()
-        ads1 = sorted(ads.split('_', 3)[1:-1])
-        num = ads.split('_', 3)[-1]
+        ads = ads_ener.split(",", 1)[0]
+        ener = ads_ener.split(",", 1)[1].strip()
+        ads1 = sorted(ads.split("_", 3)[1:-1])
+        num = ads.split("_", 3)[-1]
         if ads1 == sorted(struc):
             order += [num]
             Ener += [round(float(ener), 3)]
     EnerInfo.close()
     return Ener, order
 
 
-#Dir = "../Info/energy_list_coad.csv"
-#Ener,order=Extract_energy(Efile=Dir,struc=["NH3","OH"])
-#print(Ener,order)
+# Dir = "../Info/energy_list_coad.csv"
+# Ener,order=Extract_energy(Efile=Dir,struc=["NH3","OH"])
+# print(Ener,order)
 
 
-### 3.Extract energy of radical & slab
+# 3.Extract energy of radical & slab
 def Extract_energy_single(Efile, struc):
-    """
-    Extract energy of radical & slab.
+    """Extract energy of radical & slab.
 
     Parameters
     ----------
     Efile : str
         Energy information file.
     struc : str
         Structure that want to extract energy.
@@ -143,39 +138,37 @@
     tuple
         A tuple containing the energy and the structure:
 
         - Ener : float
             The extracted energy.
         - struc : str
             The extracted structure.
-
     """
     EnerInfo = open(Efile, "r+")
-    #Ener=[]
+    # Ener=[]
     for i, ads_ener in enumerate(EnerInfo):
-        ads = ads_ener.split(',', 1)[0]
-        ener = ads_ener.split(',', 1)[1].strip()
-        #conf=ads.s[lit('_')[0:-2]
+        ads = ads_ener.split(",", 1)[0]
+        ener = ads_ener.split(",", 1)[1].strip()
+        # conf=ads.s[lit('_')[0:-2]
         if ads == struc:
-            #Ener += [round(float(ener),2)]
+            # Ener += [round(float(ener),2)]
             Ener = round(float(ener), 3)
 
     EnerInfo.close()
     return Ener, struc
 
 
-#Dir = "../Info/energy_radical"
-#Ener,struc=Exstract_energy_single(Efile=Dir,struc="NH3")
-#print(Ener,struc)
+# Dir = "../Info/energy_radical"
+# Ener,struc=Exstract_energy_single(Efile=Dir,struc="NH3")
+# print(Ener,struc)
 
 
-### 4.Extract adsorption energy
+# 4.Extract adsorption energy
 def Extract_adsE(slab_E, radical_E, tot_E):
-    """
-    Calculates the adsorption energy.
+    """Calculates the adsorption energy.
 
     Parameters
     ----------
     slab_E : float
         The crystal surface energy.
     radical_E : float
         The radical energy.
@@ -187,299 +180,294 @@
     float
         The calculated adsorption energy.
     """
     ads_E = float(tot_E) - float(slab_E) - float(radical_E)
     return round(ads_E, 3)
 
 
-### 5.Get the potcar file
-def get_potcar(poscar, path='/data/jqyang/src/mypps/potpaw_PBE/'):
+# 5.Get the potcar file
+def get_potcar(poscar, path="/data/jqyang/src/mypps/potpaw_PBE/"):
     """Get the POTCAR file for VASP calculation.
 
-      Parameters
-      ----------
-      poscar : str
-          The file path of POSCAR.
-      path : str, optional
-          The path of the pseudopotential files, by default '/data/jqyang/src/mypps/potpaw_PBE/'.
-
-      Returns
-      -------
-      None
-          The function writes the combined POTCAR file.
-
-      Raises
-      ------
-      ValueError
-          If the elements in the structure files are different.
+    Parameters
+    ----------
+    poscar : str
+        The file path of POSCAR.
+    path : str, optional
+        The path of the pseudopotential files, by default '/data/jqyang/src/mypps/potpaw_PBE/'.
+
+    Returns
+    -------
+    None
+        The function writes the combined POTCAR file.
 
-      """
+    Raises
+    ------
+    ValueError
+        If the elements in the structure files are different.
+    """
     # extract the element species:
     list_elem = []
     for i, pos in enumerate(poscar):
-        struc = read(pos, format='vasp')
+        struc = read(pos, format="vasp")
         symbols = struc.get_chemical_symbols()
         dic_sym = dict(Counter(symbols))
         list_elem.append(list(dic_sym.keys()))
     # if num of file, compare them
     if i > 0:
         if list_elem[0] == list_elem[1]:
             list_pot = list_elem[0]
         else:
             print("Elements in structure files are different && please correct! ")
     else:
         list_pot = list_elem[0]
     # extract the potcars file and combines them
-    if os.path.exists('POTCAR'):
-        os.system('rm POTCAR')
-    potcar = open('POTCAR', 'w')
+    if os.path.exists("POTCAR"):
+        os.system("rm POTCAR")
+    potcar = open("POTCAR", "w")
     for j in range(len(list_pot)):
-        path_tmp = os.path.join(path, list_pot[j], 'POTCAR')
+        path_tmp = os.path.join(path, list_pot[j], "POTCAR")
         for line in open(path_tmp):
             potcar.writelines(line)
     potcar.close()
 
 
-### 6. Get the site info
+# 6. Get the site info
 from ase.neighborlist import NeighborList
 from ase.neighborlist import natural_cutoffs
 
 
-#from ase.build import molecule
+# from ase.build import molecule
 def get_site(poscar, mole):
     """Determine the type of adsorption site.
 
-       Parameters
-       ----------
-       poscar : str
-           The name of the POSCAR file.
-       mole : list
-           A list consisting of the chemical formula of the adsorbed molecule
-           and the atoms adsorbed on the point.
-
-       Returns
-       -------
-       tuple
-           A tuple of two lists: binding site types and the chemical symbols for
-           other atoms bound to the binding site.
-
-       """
-    struc = read(poscar, format='vasp')
-    ### molecule and atom info
+    Parameters
+    ----------
+    poscar : str
+        The name of the POSCAR file.
+    mole : list
+        A list consisting of the chemical formula of the adsorbed molecule
+        and the atoms adsorbed on the point.
+
+    Returns
+    -------
+    tuple
+        A tuple of two lists: binding site types and the chemical symbols for
+        other atoms bound to the binding site.
+    """
+    struc = read(poscar, format="vasp")
+    # molecule and atom info
     mol = molecule(mole[0])
     atom_b = mole[1]
 
-    ### POSACR structure analysis
-    ### neighbor list of every atoms
+    # POSACR structure analysis
+    # neighbor list of every atoms
     cutOff = natural_cutoffs(struc)
     nl = NeighborList(cutOff, self_interaction=False, bothways=True)
     nl.update(struc)
     matrix = nl.get_connectivity_matrix()
-    ### list of every atoms : the atom order in poscar, number of binding atoms, the symbol of the atom
+    # list of every atoms : the atom order in poscar, number of binding atoms, the symbol of the atom
     adatom_num = []
     adatom_conn = []
     adatom_symb = []
     for i in range(len(struc.get_positions())):
         indices, offsets = nl.get_neighbors(i)
-        #print(indices)
+        # print(indices)
         if len(indices) < 5:
-            #print('atoms %s is adatom'%(i))
+            # print('atoms %s is adatom'%(i))
             adatom_num += [str(i)]
             adatom_conn += [len(indices)]
             adatom_symb += [struc.get_chemical_symbols()[i]]
-            #for j, offset in zip(indices, offsets):
-            #print(struc.positions[j] + offset @ struc.get_cell())
-    ### the dict: key= the atom order in poscar, the  number of binding atom
+            # for j, offset in zip(indices, offsets):
+            # print(struc.positions[j] + offset @ struc.get_cell())
+    # the dict: key= the atom order in poscar, the  number of binding atom
     dic_adatom = dict(zip(adatom_num, adatom_conn))
     # get connectivity of the atom we studied in adsorbed configuration
     if atom_b in adatom_symb:
         # the atom order of the atom we studied
         atom_b_num = struc.get_chemical_symbols().index(atom_b)
 
     # the binding number of the atom,list of binding atoms of the atom
     # corresponding chemical symbol atom in catalyst
     atom_b_conn_a = dic_adatom.get(str(atom_b_num))
     atom_b_conn, offsets = nl.get_neighbors(atom_b_num)
     atom_b_conn_symb = [struc.get_chemical_symbols()[i] for i in atom_b_conn if i < 36]
-    #print(atom_b,atom_b_conn_a,atom_b_conn,atom_b_conn_symb)
+    # print(atom_b,atom_b_conn_a,atom_b_conn,atom_b_conn_symb)
 
-    ### adsorbed molecule analysis
+    # adsorbed molecule analysis
     cutOff_a = natural_cutoffs(mol)
     nl_a = NeighborList(cutOff_a, self_interaction=False, bothways=True)
     nl_a.update(mol)
     matrix = nl_a.get_connectivity_matrix()
     mol_num = []
     mol_conn = []
     mol_symb = []
     for j in range(len(mol.get_chemical_symbols())):
         indices, offsets = nl_a.get_neighbors(j)
-        #atom number
+        # atom number
         mol_num += [str(j)]
-        #atom connectivity
+        # atom connectivity
         mol_conn += [len(indices)]
-        #atom symbol
+        # atom symbol
         mol_symb += [mol.get_chemical_symbols()[j]]
     dic_mol = dict(zip(mol_num, mol_conn))
     # get connectivity of atom in molecule
     if atom_b in mol_symb:
         atom_b_num = mol.get_chemical_symbols().index(atom_b)
     atom_b_conn_m = dic_mol.get(str(atom_b_num))
 
-    ### calculate binding site type
-    typ = {'0': None, '1': 'top', '2': 'bri', '3': 'hol', '4': '4-fold'}
+    # calculate binding site type
+    typ = {"0": None, "1": "top", "2": "bri", "3": "hol", "4": "4-fold"}
     bind_type = typ.get(str(int(atom_b_conn_a) - int(atom_b_conn_m)))
-    #print(bind_type)
+    # print(bind_type)
     return bind_type, atom_b_conn_symb
 
 
-### 7. To distinguish the surface and bulk atoms,atom binded with or not the surface
+# 7. To distinguish the surface and bulk atoms,atom binded with or not the surface
 from HTMACat.catkit.gen.utils import get_unique_coordinates
 import numpy as np
 
 
 def distinguish_atom_binding(poscar, tol_layer=0.01, tol=0.05, base_layer=4, atoms_layer=9):
-    """
-        Distinguishes different types of atoms in a surface structure and classifies them as adatoms, surface atoms,
-        and subsurface atoms based on their Z coordinates.
+    """Distinguishes different types of atoms in a surface structure and classifies them as
+    adatoms, surface atoms, and subsurface atoms based on their Z coordinates.
+
+    Parameters
+    ----------
+    poscar : str
+        The input structure in POSCAR format
+    tol_layer : float, optional
+        Tolerance for distinguishing the Z coordinate of atoms belonging to different layers. Default is 0.01.
+    tol : float, optional
+        Tolerance for distinguishing the Z coordinate of adatoms and surface atoms. Default is 0.05.
+    base_layer : int, optional
+        The layer number where the surface atoms are located. Default is 4.
+    atoms_layer : int, optional
+        The minimum number of surface atoms required for the structure to be analyzed. Default is 9.
 
-        Parameters
-        ----------
-        poscar : str
-            The input structure in POSCAR format
-        tol_layer : float, optional
-            Tolerance for distinguishing the Z coordinate of atoms belonging to different layers. Default is 0.01.
-        tol : float, optional
-            Tolerance for distinguishing the Z coordinate of adatoms and surface atoms. Default is 0.05.
-        base_layer : int, optional
-            The layer number where the surface atoms are located. Default is 4.
-        atoms_layer : int, optional
-            The minimum number of surface atoms required for the structure to be analyzed. Default is 9.
-
-        Returns
-        -------
-        tuple
-            -adatoms : list
-                A list of the indices of adatoms in the structure.
-            -adatoms_symb : list
-                A list of the chemical symbols of adatoms in the structure.
-            -surfatoms : list
-                A list of the indices of surface atoms in the structure.
-            -surfatoms_symb : list
-                A list of the chemical symbols of surface atoms in the structure.
-            -subsurfatoms : list
-                A list of the indices of subsurface atoms in the structure.
-            -subsurfatoms_symb : list
-                A list of the chemical symbols of subsurface atoms in the structure
-
-        Raises
-        ------
-        ValueError
-            If tol is too large and not able to distinguish the layers, or if the structure cannot be analyzed.
+    Returns
+    -------
+    tuple
+        -adatoms : list
+            A list of the indices of adatoms in the structure.
+        -adatoms_symb : list
+            A list of the chemical symbols of adatoms in the structure.
+        -surfatoms : list
+            A list of the indices of surface atoms in the structure.
+        -surfatoms_symb : list
+            A list of the chemical symbols of surface atoms in the structure.
+        -subsurfatoms : list
+            A list of the indices of subsurface atoms in the structure.
+        -subsurfatoms_symb : list
+            A list of the chemical symbols of subsurface atoms in the structure
 
-        """
+    Raises
+    ------
+    ValueError
+        If tol is too large and not able to distinguish the layers, or if the structure cannot be analyzed.
+    """
 
     if isinstance(poscar, str):
-        struct = read(poscar, format='vasp')
+        struct = read(poscar, format="vasp")
     else:
         struct = poscar
-    #the representative Z coords of every layer
+    # the representative Z coords of every layer
     coordinates_layer = get_unique_coordinates(struct, axis=2, tag=True, tol=tol_layer)
     coordinates = struct.get_scaled_positions()[:, 2]
-    #the dict about the atoms and corresponding layers
+    # the dict about the atoms and corresponding layers
     key_atom = []
     value_layer = []
-    #print(coordinates_layer)
+    # print(coordinates_layer)
     for i, coord in enumerate(coordinates):
         for j, coord_layer in enumerate(coordinates_layer):
             dis = np.abs(coord - coord_layer)
             if dis < tol:
-                #print(f'atom {i+1} belongs to layer {j+1}')
+                # print(f'atom {i+1} belongs to layer {j+1}')
                 key_atom += [i]
                 value_layer += [j + 1]
                 break
             elif j >= base_layer:
-                #print(f'atom {i+1} belongs to layer {j+1}')
+                # print(f'atom {i+1} belongs to layer {j+1}')
                 key_atom += [i]
                 value_layer += [j + 1]
 
-    #if len(key_atom) != (i+1):
+    # if len(key_atom) != (i+1):
     #   raise ValueError('tol is too large and not to distinguish the layers; Please reduce tol!')
     dict_atom_layer = dict(zip(key_atom, value_layer))
-    #print(dict_atom_layer)
+    # print(dict_atom_layer)
     adatoms, adatoms_symb = [], []
     surfatoms, surfatoms_symb = [], []
     subsurfatoms, subsurfatoms_symb = [], []
     for k in range(len(coordinates)):
-        #print(dict_atom_layer.get(k))
+        # print(dict_atom_layer.get(k))
         if int(dict_atom_layer.get(k)) > base_layer:
-            dict_atom_layer[k] = 'adatom'
+            dict_atom_layer[k] = "adatom"
             adatoms += [k]
             adatoms_symb += [struct.get_chemical_symbols()[k]]
         elif dict_atom_layer.get(k) == base_layer:
-            dict_atom_layer[k] = 'surf_atom'
+            dict_atom_layer[k] = "surf_atom"
             surfatoms += [k]
             surfatoms_symb += [struct.get_chemical_symbols()[k]]
         elif dict_atom_layer.get(k) == (base_layer - 1):
-            dict_atom_layer[k] = 'subsurf_atom'
+            dict_atom_layer[k] = "subsurf_atom"
             subsurfatoms += [k]
             subsurfatoms_symb += [struct.get_chemical_symbols()[k]]
         else:
             continue
-    #print(dict_atom_layer)
-    base_element = ['Au', 'Ag', 'Pd', 'Pt', 'Rh', 'Ru', 'Ir', 'Cu', 'Fe', 'Co', 'Ni', 'Zn']
+    # print(dict_atom_layer)
+    base_element = ["Au", "Ag", "Pd", "Pt", "Rh", "Ru", "Ir", "Cu", "Fe", "Co", "Ni", "Zn"]
     if len(surfatoms) > int(atoms_layer):
-        #print('surface atoms >9')
-        #print(surfatoms_symb)
+        # print('surface atoms >9')
+        # print(surfatoms_symb)
         surfatoms_final, surfatoms_symb_final = [], []
         tmp = []
         for n, atom_symb in enumerate(surfatoms_symb):
             if atom_symb not in base_element:
-                #print(atom_symb)
+                # print(atom_symb)
                 adatoms += [surfatoms[n]]
                 adatoms_symb += [atom_symb]
-                #surfatoms.pop(n)
-                #surfatoms_symb.pop(n)
+                # surfatoms.pop(n)
+                # surfatoms_symb.pop(n)
                 tmp += [n]
         for m, atom_symb in enumerate(surfatoms_symb):
             if m not in tmp:
                 surfatoms_final += [surfatoms[m]]
                 surfatoms_symb_final += [surfatoms_symb[m]]
         surfatoms = surfatoms_final
         surfatoms_symb = surfatoms_symb_final
-        #print(surfatoms_symb)
-        ### Ignore structures where Z coord of adatoms < Z coord of surfatoms
+        # print(surfatoms_symb)
+        # Ignore structures where Z coord of adatoms < Z coord of surfatoms
         Z_mean = np.mean([struct.get_scaled_positions()[i][2] for i in surfatoms])
         Z_adatom = np.mean([struct.get_scaled_positions()[i][2] for i in adatoms])
         if Z_adatom <= Z_mean:
             surfatoms = []
             surfatoms_symb = []
-    ### Ignore the structures without standard and integrated surface configurations
+    # Ignore the structures without standard and integrated surface configurations
     elif len(surfatoms) < int(atoms_layer):
-        #raise ValueError(f'{poscar} can not been analyzed!')
+        # raise ValueError(f'{poscar} can not been analyzed!')
         surfatoms = []
         surfatoms_symb = []
-        #return adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb
-    '''
+        # return adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb
+    """
     #extract the atoms and corresponding chemical symbols of specific layer
     layer_atoms=[]
-    layer_atoms_symb=[] 
+    layer_atoms_symb=[]
     for m in range(len(coordinates)):
-        if dict_atom_layer.get(m) == layer:           
+        if dict_atom_layer.get(m) == layer:
            layer_atoms += [m]
            layer_atoms_symb += [struct.get_chemical_symbols()[m]]
     return layer_atoms,layer_atoms_symb
-    '''
+    """
 
     return adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb
 
 
-### get the neighboring atoms fo specific adatoms
+# get the neighboring atoms fo specific adatoms
 def get_atom_neigh(poscar, atom):
-    """
-    Get the neighboring atoms of specific adsorbed atoms.
+    """Get the neighboring atoms of specific adsorbed atoms.
 
     Parameters
     ----------
     poscar : str or pymatgen.Structure
         The VASP file or pymatgen.Structure object containing the lattice structure information.
     atom : str
         The chemical symbol of the specific adsorbed atom.
@@ -487,23 +475,29 @@
     Returns
     -------
     tuple[list,list]
         A tuple of two lists:
 
         - The indices of the nearest neighbor atoms of the specified atom in the lattice structure.
         - The chemical element symbols of the nearest neighbor atoms.
-
     """
 
     if isinstance(poscar, str):
-        struct = read(poscar, format='vasp')
+        struct = read(poscar, format="vasp")
     else:
         struct = poscar
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.03)
+    layer = len(get_unique_coordinates(poscar, axis=2, tag=True, tol=0.01))-1
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.03, base_layer=layer)    # Changed by RxChen, 2023/06/02
     struct_symb = struct.symbols
     atom_symb = chemical_symbols[atom]
 
     atom_index, atom_neighs = [], []
     # whether input atom occur in the bulk
     if atom_symb in struct.get_chemical_symbols():
         cutOff = natural_cutoffs(struct, mult=1.0)
@@ -513,103 +507,108 @@
         for i, adatom_symb in enumerate(adatoms_symb):
             if atom_symb == adatom_symb:
                 indices, offsets = nl.get_neighbors(adatoms[i])
                 for index in indices:
                     atom_index += [index]
                     atom_neighs += [struct.get_chemical_symbols()[index]]
             else:
-                print(f'No {atom_symb} adatom')
+                print(f"No {atom_symb} adatom")
     else:
-        print(f'No {atom_symb} in {struct_symb}')
+        print(f"No {atom_symb} in {struct_symb}")
     return atom_index, atom_neighs
 
 
-### 8. TO get atoms binding with surface among adatoms
+# 8. TO get atoms binding with surface among adatoms
 def get_binding_adatom(poscar):
-    """
-        Determine the adsorbed atoms and the surface atoms to which they bind.
+    """Determine the adsorbed atoms and the surface atoms to which they bind.
 
-        Parameters
-        ----------
-        poscar : str
-            The VASP file path or pymatgen.Structure object.
-
-        Returns
-        -------
-        tuple[list,list,list,list,list,list]
-            A tuple containing the following elements:
-
-            - bind_adatoms :list
-                The list of indices of adsorbed atoms that are bound to surface atoms.
-            - bind_adatoms_symb :list
-                The list of chemical symbols of adsorbed atoms that are bound to surface atoms.
-            - adspecie :list
-                The list of chemical representations of adsorbates.
-            - bind_type_symb :list
-                The list of adsorption types.
-            - bind_surfatoms :list
-                The list of indices of surface atoms that are bound to adsorbed atoms.
-            - bind_surfatoms_symb :list
-                The list of chemical symbols of surface atoms that are bound to adsorbed atoms.
-
-        Notes
-        -----
-        This function extracts adsorbed and surface atoms from the structure, calculates the neighbor list,
-        and determines which adsorbed atoms are bound to which surface atoms. It then extracts the adsorbate species,
-        the adsorption type, and the surface atoms that are bound to each adsorbed atom.
+    Parameters
+    ----------
+    poscar : str
+        The VASP file path or pymatgen.Structure object.
 
-        """
+    Returns
+    -------
+    tuple[list,list,list,list,list,list]
+        A tuple containing the following elements:
+
+        - bind_adatoms :list
+            The list of indices of adsorbed atoms that are bound to surface atoms.
+        - bind_adatoms_symb :list
+            The list of chemical symbols of adsorbed atoms that are bound to surface atoms.
+        - adspecie :list
+            The list of chemical representations of adsorbates.
+        - bind_type_symb :list
+            The list of adsorption types.
+        - bind_surfatoms :list
+            The list of indices of surface atoms that are bound to adsorbed atoms.
+        - bind_surfatoms_symb :list
+            The list of chemical symbols of surface atoms that are bound to adsorbed atoms.
+
+    Notes
+    -----
+    This function extracts adsorbed and surface atoms from the structure, calculates the neighbor list,
+    and determines which adsorbed atoms are bound to which surface atoms. It then extracts the adsorbate species,
+    the adsorption type, and the surface atoms that are bound to each adsorbed atom.
+    """
     # extract surface atoms and adsorbed atoms
-    #adatoms,adatoms_symb=distinguish_atom_binding(poscar,tol=0.05,layer='adatom')
-    #surf_atoms,surf_atom_symb=distinguish_atom_binding(poscar,tol=0.05,layer='surf_atom')
+    # adatoms,adatoms_symb=distinguish_atom_binding(poscar,tol=0.05,layer='adatom')
+    # surf_atoms,surf_atom_symb=distinguish_atom_binding(poscar,tol=0.05,layer='surf_atom')
 
     # neighbor list of atoms in struct
     if isinstance(poscar, str):
-        struct = read(poscar, format='vasp')
+        struct = read(poscar, format="vasp")
     else:
         struct = poscar
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(adatoms_symb,surfatoms_symb)
-    #print(struct.symbols)
+    layer = len(get_unique_coordinates(poscar, axis=2, tag=True, tol=0.01))-1
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05, base_layer=layer)    # Changed by RxChen, 2023/06/02
+    # print(adatoms_symb,surfatoms_symb)
+    # print(struct.symbols)
     cutOff = natural_cutoffs(struct, mult=1.0)
-    #print(cutOff)
+    # print(cutOff)
     nl = NeighborList(cutOff, self_interaction=False, bothways=True)
     nl.update(struct)
-    #### extract the adatoms binded with surface and corresponding surface atoms
+    ## extract the adatoms binded with surface and corresponding surface atoms
     bind_adatoms = []
     bind_adatoms_symb = []
     bind_surfatoms = []
     bind_surfatoms_symb = []
     site_type = []
     site_type2 = []
     site_type_symb = []
-    ### Extract the binded surface atoms and binded adsorbed atoms
+    # Extract the binded surface atoms and binded adsorbed atoms
     for i, atom in enumerate(adatoms):
         indices, offsets = nl.get_neighbors(atom)
         tmp = []
         tmp2 = []
-        #print(indices)
+        # print(indices)
         for index in indices:
-            #print(index)
+            # print(index)
             if index in surfatoms:
                 bind_adatoms += [atom]
                 tmp += [index]
                 tmp2 += [struct.get_chemical_symbols()[index]]
             else:
                 continue
-        #tmp3_symb=[struct.get_chemical_symbols()[i] for i in tmp3]
+        # tmp3_symb=[struct.get_chemical_symbols()[i] for i in tmp3]
         if tmp != []:
             bind_surfatoms += [tmp]
             bind_surfatoms_symb += [tmp2]
             site_type += [len(tmp2)]
-        #print(struct.get_scaled_positions()[atom][0:-1])
+        # print(struct.get_scaled_positions()[atom][0:-1])
     bind_adatoms = list(set(bind_adatoms))
     bind_adatoms_symb = [struct.get_chemical_symbols()[i] for i in bind_adatoms]
-    ### Extract the bind type
+    # Extract the bind type
     item = []
     bind_type_symb = []
     for j, adatom in enumerate(bind_adatoms):
         p1 = struct.get_scaled_positions()[adatom][0:-1]
         item_tmp = []
         for k, atom in enumerate(subsurfatoms):
             p2 = struct.get_scaled_positions()[atom][0:-1]
@@ -617,67 +616,73 @@
                 item_tmp += [True]
             else:
                 item_tmp += [False]
         if any(item_tmp):
             item += [int(1)]
         else:
             item += [int(0)]
-    #print(item)
-    typ = {0: None, 1: 'top', 2: 'bri', 3: 'hol', 4: '4-fold'}
+    # print(item)
+    typ = {0: None, 1: "top", 2: "bri", 3: "hol", 4: "4-fold"}
     for m, bind in enumerate(site_type):
         bind_type = typ.get(bind)
-        if bind_type == 'hol' and item[m] == 0:
-            bind_type_symb += ['fcc']
-        elif bind_type == 'hol' and item[m] == 1:
-            bind_type_symb += ['hcp']
+        if bind_type == "hol" and item[m] == 0:
+            bind_type_symb += ["fcc"]
+        elif bind_type == "hol" and item[m] == 1:
+            bind_type_symb += ["hcp"]
         else:
             bind_type_symb += [bind_type]
 
-    ### Extract the adsorbed species
+    # Extract the adsorbed species
     adspecie = []
     for i, atom in enumerate(bind_adatoms):
         indices, offsets = nl.get_neighbors(atom)
         tmp3 = [atom]
-        #print(indices)
+        # print(indices)
         for index in indices:
             if (index in surfatoms) or (index in subsurfatoms):
                 continue
             else:
                 tmp3 += [index]
-        #print(tmp3)
-        tmp3_symb = ''.join(list([struct.get_chemical_symbols()[i] for i in tmp3]))
+        # print(tmp3)
+        tmp3_symb = "".join(list([struct.get_chemical_symbols()[i] for i in tmp3]))
         Ele = list(dict(Counter(tmp3_symb)).keys())
         Num = list(dict(Counter(tmp3_symb)).values())
-        #print(tmp3_symb)
-        #print(Ele)
-        mol = '*'
+        # print(tmp3_symb)
+        # print(Ele)
+        mol = "*"
         for j, E in enumerate(Ele):
             mol = mol + E
             if Num[j] == 1:
                 continue
             else:
                 mol = mol + str(Num[j])
-        if mol == '*OH2':
-            mol = '*H2O'
+        if mol == "*OH2":
+            mol = "*H2O"
         else:
-            adspecie += [mol.split('*')[1]]
-        #adspecie+=[''.join(list(chain.from_iterable(zip(Ele,Num))))]
-        #mol=molecule(tmp3_symb)[0]
-        #print(mol.symbol)
-    return bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb
+            adspecie += [mol.split("*")[1]]
+        # adspecie+=[''.join(list(chain.from_iterable(zip(Ele,Num))))]
+        # mol=molecule(tmp3_symb)[0]
+        # print(mol.symbol)
+    return (
+        bind_adatoms,
+        bind_adatoms_symb,
+        adspecie,
+        bind_type_symb,
+        bind_surfatoms,
+        bind_surfatoms_symb,
+    )
 
 
-### 9. To get the distance between adatoms
+# 9. To get the distance between adatoms
 from ase.geometry import get_distances
 from HTMACat.catkit.gen import defaults
 
 
 def get_distance_adatoms(poscar, tol=0.1):
-    """
-    Calculate the distance between adsorbed atoms in a VASP file.
+    """Calculate the distance between adsorbed atoms in a VASP file.
 
     Parameters
     ----------
     poscar : str
         The VASP file or structure object.
     tol : float, optional
         A parameter that determines whether atoms are bonded. The default value is 0.1.
@@ -692,110 +697,117 @@
             - dis_matrix : list of float
                 A list of distances between adsorbed atoms.
 
     Raises
     ------
     ValueError
         If there is only one atom in the VASP file.
-
     """
     if isinstance(poscar, str):
-        struct = read(poscar, format='vasp')
+        struct = read(poscar, format="vasp")
     else:
         struct = poscar
-    #struct=read(poscar,format='vasp')
-    bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-        poscar)
-    radii = defaults.get('radii')
+    # struct=read(poscar,format='vasp')
+    (
+        bind_adatoms,
+        bind_adatoms_symb,
+        adspecie,
+        bind_type_symb,
+        bind_surfatoms,
+        bind_surfatoms_symb,
+    ) = get_binding_adatom(poscar)
+    radii = defaults.get("radii")
     radii_adatom = [radii[struct.numbers[i]] for i in bind_adatoms]
     dis_matrix = []  # distcance
     dis_symb_matrix = []  # symbol corresponding distance
     if len(bind_adatoms) < 2:
-        raise ValueError('Only 1 atom and No distance')
+        raise ValueError("Only 1 atom and No distance")
     ## distance when there are 2 adatoms
-    #elif len(bind_adatoms) == 2:
-    #bond_distance=sum(radii_adatom)
-    #print(bond_distance)
-    #dis = get_distances(struct.get_positions()[bind_adatoms[0]],struct.get_positions()[bind_adatoms[1]])[1][0][0]
-    #print(dis)
-    #if abs(dis-bond_distance) < tol:
+    # elif len(bind_adatoms) == 2:
+    # bond_distance=sum(radii_adatom)
+    # print(bond_distance)
+    # dis = get_distances(struct.get_positions()[bind_adatoms[0]],struct.get_positions()[bind_adatoms[1]])[1][0][0]
+    # print(dis)
+    # if abs(dis-bond_distance) < tol:
     #   print('The dis may below the possible bond length')
-    #else:
-    #print(round(dis,3))
-    #return round(dis,3)
+    # else:
+    # print(round(dis,3))
+    # return round(dis,3)
     ## distance when there are above 2 adatoms
     else:
         for i in range(len(bind_adatoms)):
             if (i + 1) > (len(bind_adatoms) - 1):
                 continue
             else:
-                dis_symb = '-'.join([bind_adatoms_symb[i], bind_adatoms_symb[i + 1]])
+                dis_symb = "-".join([bind_adatoms_symb[i], bind_adatoms_symb[i + 1]])
                 bond_distance = radii_adatom[i] + radii_adatom[i + 1]
                 ## get minmum distance of adsorbed atoms
                 p_all = struct.get_scaled_positions()
                 p1_scaled = struct.get_scaled_positions()[bind_adatoms[i]]
                 p2_scaled = struct.get_scaled_positions()[bind_adatoms[i + 1]]
                 # replace the minus coord
                 struct.set_scaled_positions(p_all)
-                #print(p1_scaled[0],p2_scaled[0])
+                # print(p1_scaled[0],p2_scaled[0])
                 if p1_scaled[0] - p2_scaled[0] >= 0.50:
                     p_all[bind_adatoms[i + 1]][0] = p2_scaled[0] + 1
                     struct.set_scaled_positions(p_all)
                 elif p1_scaled[0] - p2_scaled[0] <= -0.50:
                     p_all[bind_adatoms[i]][0] = p1_scaled[0] + 1
                     struct.set_scaled_positions(p_all)
                 if p1_scaled[1] - p2_scaled[1] >= 0.50:
                     p_all[bind_adatoms[i + 1]][1] = p2_scaled[1] + 1
                     struct.set_scaled_positions(p_all)
                 elif p1_scaled[1] - p2_scaled[1] <= -0.50:
                     p_all[bind_adatoms[i]][1] = p1_scaled[1] + 1
                     struct.set_scaled_positions(p_all)
-                dis = get_distances(struct.get_positions()[bind_adatoms[i]],
-                                    struct.get_positions()[bind_adatoms[i + 1]])[1][0][0]
-                #print(struct.get_positions()[bind_adatoms[i]],struct.get_positions()[bind_adatoms[i+1]])
-                #print(get_distances(struct.get_positions()[bind_adatoms[i]],struct.get_positions()[bind_adatoms[i+1]]))
+                dis = get_distances(
+                    struct.get_positions()[bind_adatoms[i]],
+                    struct.get_positions()[bind_adatoms[i + 1]],
+                )[1][0][0]
+                # print(struct.get_positions()[bind_adatoms[i]],struct.get_positions()[bind_adatoms[i+1]])
+                # print(get_distances(struct.get_positions()[bind_adatoms[i]],struct.get_positions()[bind_adatoms[i+1]]))
 
                 ## ignore the configuraton with too near distance
                 if abs(dis - bond_distance) < tol:
-                    print('The dis may below the possible bond length')
+                    print("The dis may below the possible bond length")
                 else:
                     dis_symb_matrix += [dis_symb]
                     dis_matrix += [round(dis, 3)]
     return dis_symb_matrix, dis_matrix
 
 
-### 10. To get the minimum distance between two group
+# 10. To get the minimum distance between two group
 from ase.geometry import get_distances
 
 
 def get_min_distance_group(struct, group1, group2):
-    """
-      Compute the minimum distance between two sets of atoms in a crystal structure.
+    """Compute the minimum distance between two sets of atoms in a crystal structure.
+
+    Parameters
+    ----------
+    struct : ase.Atoms
+        The crystal structure.
+    group1 : list of int
+        Indices of the atoms in the first group.
+    group2 : list of int
+        Indices of the atoms in the second group.
 
-      Parameters
-      ----------
-      struct : ase.Atoms
-          The crystal structure.
-      group1 : list of int
-          Indices of the atoms in the first group.
-      group2 : list of int
-          Indices of the atoms in the second group.
-
-      Returns
-      -------
-      numpy.ndarray
-          A 2D array containing the distances between each pair of atoms in group1 and group2.
-      """
+    Returns
+    -------
+    numpy.ndarray
+        A 2D array containing the distances between each pair of atoms in group1 and group2.
+    """
     p1_scaled = [struct.get_scaled_positions()[i] for i in group1]
     p2_scaled = [struct.get_scaled_positions()[i] for i in group2]
     dis_matrix = get_distances(p1_scaled, p2_scaled)
     return dis_matrix
 
 
-### 11. To peprocess the raw info for descritor construction
+# 11. To peprocess the raw info for descritor construction
+
 
 def Construct_descriptor_info(raw_file, atoms, feature):
     """Construct descriptor information from raw data file.
 
     Parameters
     ----------
     raw_file : str
@@ -829,25 +841,24 @@
     for i, ele in enumerate(atoms):
         line = index_line.index(ele)
         tmp = []
         for j, des in enumerate(feature):
             row = index_row.get(des)
             tmp += [float(matrix_info[line][row])]
         feature_value += [tmp]
-    #return index_line,index_row,matrix_info,feature_value
+    # return index_line,index_row,matrix_info,feature_value
     return feature_value
 
 
-### 12. Extrate the based info:atomic_numbers, atomic_names, atomic_masses, covalent_radii
+# 12. Extrate the based info:atomic_numbers, atomic_names, atomic_masses, covalent_radii
 from ase.data import atomic_numbers, atomic_names, atomic_masses, covalent_radii, vdw_radii
 
 
 def Extract_atomic_info(atoms):
-    """
-    Extracts information related to the provided atoms.
+    """Extracts information related to the provided atoms.
 
     Parameters
     ----------
     atoms : list of int
         List of integers representing the atomic numbers of the atoms.
 
     Returns
@@ -868,18 +879,18 @@
     names_atoms = [atomic_names[i] for i in numbers_atoms]
     radii_atoms = [covalent_radii[i] for i in numbers_atoms]
     mass_atoms = [atomic_masses[i] for i in numbers_atoms]
     vdw_radii_atoms = [vdw_radii[i] for i in numbers_atoms]
     return names_atoms, radii_atoms, mass_atoms, vdw_radii_atoms
 
 
-### 13. Extract the stable adsorption type for single molecule or radical adsorption based on adsorption energy
+# 13. Extract the stable adsorption type for single molecule or radical adsorption based on adsorption energy
 def get_site_stable(Efile, Ecut=-0.1):
-    """
-    Extracts the stable adsorption type for single molecule or radical adsorption based on adsorption energy.
+    """Extracts the stable adsorption type for single molecule or radical adsorption based on
+    adsorption energy.
 
     Parameters
     ----------
     Efile : str
         Path to the file containing adsorption energies.
     Ecut : float, optional
         The maximum energy cut-off for stable adsorption (default is -0.1).
@@ -890,62 +901,68 @@
         - spec_ads: a dictionary with species as keys and a list of possible adsorption types as values.
         - spec_ads_stable: a dictionary with species as keys and the stable adsorption type as values.
         - dir_list_final: a list of directories containing the stable adsorption configurations.
         - spec_ads_stable_surfa: a dictionary with species as keys and the symbol of the surface atom bound to the adsorbate in the stable adsorption configuration as values.
     """
     EnerInfo = open(Efile, "r+")
     species_ads = []
-    typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
+    typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
     for i, ads_ener in enumerate(EnerInfo):
-        species_ads += [ads_ener.split(',')[0].split('_')[-2]]
+        species_ads += [ads_ener.split(",")[0].split("_")[-2]]
     specie_ads = set(species_ads)
     EnerInfo.close()
 
     spec, ads_type, ads_type_stable = [], [], []
     dir_list_final = []
     ads_type_surfa, ads_type_stable_surfa = [], []
 
     for specie in specie_ads:
         ads_type_tmp, energy, dir_list = [], [], []
-        #ads_type_surfa_tmp=[]
+        # ads_type_surfa_tmp=[]
         spec += [specie]
         EnerInfo = open(Efile, "r+")
         for j, ads_ener in enumerate(EnerInfo):
-            ads = ads_ener.split(',')[0]
-            ads1 = ads.split('_')[-2]
-            ener = ads_ener.split(',')[-1].strip()
-            #print(ads1,specie,ads1==specie)
+            ads = ads_ener.split(",")[0]
+            ads1 = ads.split("_")[-2]
+            ener = ads_ener.split(",")[-1].strip()
+            # print(ads1,specie,ads1==specie)
             if ads1 == specie and float(ener) <= float(Ecut):
-                bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-                    f'{ads}/CONTCAR')
-                #bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(f'{ads}/optmk/CONTCAR')
-                #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+                (
+                    bind_adatoms,
+                    bind_adatoms_symb,
+                    adspecie,
+                    bind_type_symb,
+                    bind_surfatoms,
+                    bind_surfatoms_symb,
+                ) = get_binding_adatom(f"{ads}/CONTCAR")
+                # bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(f'{ads}/optmk/CONTCAR')
+                # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
                 if bind_type_symb == []:
-                    bind_type_symb = ['top']
+                    bind_type_symb = ["top"]
                 ads_type_tmp += [typ.get(bind_type_symb[0])]
                 energy += [ener]
-                dir_list += [ads_ener.split(',')[0]]
+                dir_list += [ads_ener.split(",")[0]]
                 ads_type_surfa += [bind_surfatoms_symb[0]]
         EnerInfo.close()
 
         ads_type += [list(set(ads_type_tmp))]
         ads_type_stable += [[ads_type_tmp[energy.index(max(energy))]]]
         dir_list_final += [dir_list[energy.index(max(energy))]]
         ads_type_stable_surfa += [ads_type_surfa[energy.index(max(energy))]]
     spec_ads = dict(zip(spec, ads_type))
     spec_ads_stable = dict(zip(spec, ads_type_stable))
     spec_ads_stable_surfa = dict(zip(spec, ads_type_stable_surfa))
-    #print(ads_type_stable_surfa)
+    # print(ads_type_stable_surfa)
     return spec_ads, spec_ads_stable, dir_list_final, spec_ads_stable_surfa
 
 
-###13-2. Extract the stable adsorption type for single molecule or radical adsorption based on the calculated energy
+#13-2. Extract the stable adsorption type for single molecule or radical adsorption based on the calculated energy
 def get_site_stable_energy(Efile, Ecut=0.0):
-    """
-    Extract the stable adsorption type for single molecule or radical adsorption based on the calculated energy.
+    """Extract the stable adsorption type for single molecule or radical adsorption based on the
+    calculated energy.
 
     Parameters
     ----------
     Efile : str
         The path to the file containing the adsorption energy information.
     Ecut : float, optional
         The cutoff energy for considering stable adsorption types. Default is 0.0.
@@ -955,91 +972,96 @@
     tuple[dict,dict,list]
         The first dictionary contains all the possible adsorption types for each species.
         The second dictionary contains the stable adsorption type for each species.
         The third list contains the corresponding directories for each species' stable adsorption type.
     """
     EnerInfo = open(Efile, "r+")
     species_ads = []
-    typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
+    typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
     for i, ads_ener in enumerate(EnerInfo):
-        species_ads += [ads_ener.split(',')[0].split('_')[-2]]
+        species_ads += [ads_ener.split(",")[0].split("_")[-2]]
     specie_ads = set(species_ads)
     EnerInfo.close()
 
     spec, ads_type, ads_type_stable = [], [], []
     dir_list_final = []
     for specie in specie_ads:
         ads_type_tmp, energy, dir_list = [], [], []
         spec += [specie]
         EnerInfo = open(Efile, "r+")
         for j, ads_ener in enumerate(EnerInfo):
-            ads = ads_ener.split(',')[0]
-            ads1 = ads.split('_')[-2]
-            ener = ads_ener.split(',')[-1].strip()
-            #print(ads1,specie,ads1==specie)
+            ads = ads_ener.split(",")[0]
+            ads1 = ads.split("_")[-2]
+            ener = ads_ener.split(",")[-1].strip()
+            # print(ads1,specie,ads1==specie)
             if ads1 == specie and float(ener) < float(Ecut):
-                bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-                    f'{ads}/CONTCAR')
+                (
+                    bind_adatoms,
+                    bind_adatoms_symb,
+                    adspecie,
+                    bind_type_symb,
+                    bind_surfatoms,
+                    bind_surfatoms_symb,
+                ) = get_binding_adatom(f"{ads}/CONTCAR")
 
                 if bind_type_symb == []:
-                    bind_type_symb = ['top']
+                    bind_type_symb = ["top"]
                 ads_type_tmp += [typ.get(bind_type_symb[0])]
                 energy += [ener]
-                dir_list += [ads_ener.split(',')[0]]
+                dir_list += [ads_ener.split(",")[0]]
         EnerInfo.close()
 
         ads_type += [list(set(ads_type_tmp))]
         ads_type_stable += [[ads_type_tmp[energy.index(max(energy))]]]
         dir_list_final += [dir_list[energy.index(max(energy))]]
     spec_ads = dict(zip(spec, ads_type))
     spec_ads_stable = dict(zip(spec, ads_type_stable))
     return spec_ads, spec_ads_stable, dir_list_final
 
 
-### get the energy of  most stable configurationi for single radical
+# get the energy of  most stable configurationi for single radical
 def get_adsorption_energy_stable(Efile, specie, dop_typ):
-    """get the energy of  most stable configurationi for single radical
+    """Get the energy of  most stable configurationi for single radical.
 
     Parameters
     ----------
     Efile : str
         The name of the file storing energy information.
     specie : str
         The name of the adsorbed species.
     dop_typ : str
         The type of doping.
 
     Returns
     -------
     tuple[list,list]
         A tuple containing the name of the most stable radical and its energy.
-
     """
 
     EnerInfo = open(Efile, "r+")
     dir_spe, dir_ene = [], []
     for i, ads_ener in enumerate(EnerInfo):
-        ads = ads_ener.split(',')[0]
-        ads1 = ads.split('_')[-2]
-        dop = ads.split('_')[-3]
-        ener = ads_ener.split(',')[-1].strip()
-        #if (ads1 == specie) & (dop in dop_typ):
+        ads = ads_ener.split(",")[0]
+        ads1 = ads.split("_")[-2]
+        dop = ads.split("_")[-3]
+        ener = ads_ener.split(",")[-1].strip()
+        # if (ads1 == specie) & (dop in dop_typ):
         if (ads1 == specie) & (dop == dop_typ):
             dir_spe += [ads]
             dir_ene += [float(ener)]
     EnerInfo.close()
     if dir_ene:
         spe = dir_spe[dir_ene.index(min(dir_ene))]
         ene = dir_ene[dir_ene.index(min(dir_ene))]
         return spe, ene
     else:
         return specie, None
 
 
-### get the file name of reaction dir
+# get the file name of reaction dir
 def get_file_name(reaction):
     """
     Given a chemical reaction as a string in the form of 'reactants = products',
     constructs the file name for the corresponding reaction file.
 
     Parameters
     ----------
@@ -1053,77 +1075,75 @@
 
     Examples
     --------
     >>> get_file_name('H2(g) + Cl2(g) = 2HCl(g)')
     'H2+Cl2=2HCl'
 
     """
-    specie_f = reaction.split('=')[0].strip()
-    specie_b = reaction.split('=')[1].strip()
-    ### Construct the reaction name
+    specie_f = reaction.split("=")[0].strip()
+    specie_b = reaction.split("=")[1].strip()
+    # Construct the reaction name
     ##1.Extract the reactant molecule and type (a g s)
     specie_f_list = []
-    for i in range(len(specie_f.split('+'))):
-        specie_f_list += [specie_f.split('+')[i].strip()]
+    for i in range(len(specie_f.split("+"))):
+        specie_f_list += [specie_f.split("+")[i].strip()]
     specie_f_mol = []
     specie_f_typ = []
     for j, specie in enumerate(specie_f_list):
-        specie_f_mol += [specie.split('(', 1)[0].strip()]
-        specie_f_typ += [specie.split('(', 1)[1].split(')')[0].strip()]
+        specie_f_mol += [specie.split("(", 1)[0].strip()]
+        specie_f_typ += [specie.split("(", 1)[1].split(")")[0].strip()]
     ##2.Extract the product molecule and type (a g s)
     specie_b_list = []
-    for i in range(len(specie_b.split('+'))):
-        specie_b_list += [specie_b.split('+')[i].strip()]
+    for i in range(len(specie_b.split("+"))):
+        specie_b_list += [specie_b.split("+")[i].strip()]
     specie_b_mol = []
     specie_b_typ = []
     for j, specie in enumerate(specie_b_list):
-        specie_b_mol += [specie.split('(', 1)[0].strip()]
-        specie_b_typ += specie.split('(', 1)[1].split(')')[0].strip()
+        specie_b_mol += [specie.split("(", 1)[0].strip()]
+        specie_b_typ += specie.split("(", 1)[1].split(")")[0].strip()
     ##3.construct the file name for every reaction
-    File = '+'.join(specie_f_mol) + '=' + '+'.join(specie_b_mol)
+    File = "+".join(specie_f_mol) + "=" + "+".join(specie_b_mol)
     return File
 
 
-### calculate the energy of radicals
+# calculate the energy of radicals
 def cal_Erad(FErad, Radical):
-    """
-     Calculates the energy of a given radical.
+    """Calculates the energy of a given radical.
 
-     Parameters
-     ----------
-     FErad : str
-         The name of the file containing the radical energies.
-     Radical : str
-         The name of the radical to calculate the energy for.
-
-     Returns
-     -------
-     float
-         The energy of the given radical.
-
-     Notes
-     -----
-     The file containing the radical energies should be a comma-separated file,Just like this:Pt_100_CO2_0,-226.43504734
-     """
+    Parameters
+    ----------
+    FErad : str
+        The name of the file containing the radical energies.
+    Radical : str
+        The name of the radical to calculate the energy for.
+
+    Returns
+    -------
+    float
+        The energy of the given radical.
+
+    Notes
+    -----
+    The file containing the radical energies should be a comma-separated file,Just like this:Pt_100_CO2_0,-226.43504734
+    """
     Erad = 0
-    with open(FErad, 'r+') as Eradicals:
+    with open(FErad, "r+") as Eradicals:
         for i, Eradical in enumerate(Eradicals):
-            radical = Eradical.split(',')[0]
-            E = Eradical.split(',')[1].strip()
+            radical = Eradical.split(",")[0]
+            E = Eradical.split(",")[1].strip()
             # find the atom energy
             if Radical == radical:
-                #print(i,radical)
+                # print(i,radical)
                 Erad = float(Erad) + float(E)
     return Erad
 
 
 ## calculate the energy of radical relative to atom energy: ExCyHzO=xEC+yEH+zEO
 def cal_Erad_atom(FErad, Radical):
-    """
-    Calculates the energy of each atom in a given radical.
+    """Calculates the energy of each atom in a given radical.
 
     Parameters
     ----------
     FErad : str
         The name of the file containing the atom energies.
     Radical : str
         The name of the radical to calculate the atom energies for.
@@ -1132,28 +1152,27 @@
     -------
     float
         The total energy of all atoms in the given radical.
     """
     Erad = 0
     rad = molecule(Radical)
     for i in rad.get_chemical_symbols():
-        with open(FErad, 'r+') as Eradicals:
+        with open(FErad, "r+") as Eradicals:
             for j, Eradical in enumerate(Eradicals):
-                radical = Eradical.split(',')[0]
-                E = Eradical.split(',')[1].strip()
+                radical = Eradical.split(",")[0]
+                E = Eradical.split(",")[1].strip()
                 # find the atom energy
                 if i == radical:
-                    #print(i,radical)
+                    # print(i,radical)
                     Erad = float(Erad) + float(E)
     return Erad
 
 
 def cal_Eslab(FEslab, facet):
-    """
-    Calculate the energy of a given slab facet.
+    """Calculate the energy of a given slab facet.
 
     Parameters
     ----------
     FEslab : str
         File path to the file containing the slab energies.
     facet : list
         a List containing the Miller indices of the facet.
@@ -1165,29 +1184,28 @@
 
     Examples
     --------
     >>> cal_Eslab('path/to/file.csv', [1, 0, 0])
     -123.45
     """
     E_slab = 0
-    with open(FEslab, 'r+') as Eslabs:
+    with open(FEslab, "r+") as Eslabs:
         for i, Eslab in enumerate(Eslabs):
-            slab = Eslab.split(',')[0].split('_')[0:-1]
-            E = Eslab.split(',')[1]
+            slab = Eslab.split(",")[0].split("_")[0:-1]
+            E = Eslab.split(",")[1]
             # find the facet energy
             if facet == slab:
-                #print(slab)
+                # print(slab)
                 E_slab = float(E)
     return E_slab
 
 
 ## calculate the adE with  atom energy: E(xCyHzO)ad=ECHOsurf-Esurf-xEC-yEH-zEO
-def cal_Eads(Flist, FErad, FEslab, radicals, Erad_property='radical', Facet_property='all'):
-    """
-    Calculate the adsorption energy based on atom energy.
+def cal_Eads(Flist, FErad, FEslab, radicals, Erad_property="radical", Facet_property="all"):
+    """Calculate the adsorption energy based on atom energy.
 
     Parameters
     ----------
     Flist : str
         The filename of the file that contains the list of adsorption energy configurations.
     FErad : str
         The filename of the file that contains the atom energies of the radicals.
@@ -1204,89 +1222,95 @@
     -------
     None
 
     Outputs
     -------
     adsE_{Erad_property}_{Facet_property} : file
     The file that contains the calculated adsorption energies.
-
     """
-    EnerInfo = open(Flist, 'r+')
-    Foutput = open(f'adsE_{Erad_property}_{Facet_property}', 'w+')
-    #num=0
+    EnerInfo = open(Flist, "r+")
+    Foutput = open(f"adsE_{Erad_property}_{Facet_property}", "w+")
+    # num=0
     for i, ads_ener in enumerate(EnerInfo):
         # extract the facet and radical
-        conf = ads_ener.split(',', 1)[0]
-        conf_facet = conf.split('_')[0:-2]
-        conf_radical = conf.split('_')[-2]
+        conf = ads_ener.split(",", 1)[0]
+        conf_facet = conf.split("_")[0:-2]
+        conf_radical = conf.split("_")[-2]
         # extract the energy of adsorption configuration
-        Eads = ads_ener.split(',', 1)[1].strip()
-        #print(conf)
+        Eads = ads_ener.split(",", 1)[1].strip()
+        # print(conf)
         if Eads:
             E_rad, E_slab = 0, 0
             if conf_radical in radicals:
-                #if conf.split('_')[-3] == 'b1':
+                # if conf.split('_')[-3] == 'b1':
                 #   num=num+1
-                #else:
+                # else:
                 #   num=num
                 ## extract the energy of radical based atom energy
-                if Erad_property == 'atom':
+                if Erad_property == "atom":
                     E_rad = cal_Erad_atom(FErad, conf_radical)
-                elif Erad_property == 'radical':
+                elif Erad_property == "radical":
                     E_rad = cal_Erad(FErad, conf_radical)
                 else:
-                    print('Erad has not the property!')
+                    print("Erad has not the property!")
                     break
 
                 ##  extract the energy of facet
-                with open(FEslab, 'r+') as Eslabs:
+                with open(FEslab, "r+") as Eslabs:
                     for j, Eslab in enumerate(Eslabs):
-                        line1 = Eslab.split('[')[0]
-                        Ftmp = line1.split(',')
-                        conf_slab = Ftmp[0].split('_')[0:-1]
-                        line2 = [eval(i) for i in Eslab.split('[')[1].split(']')[0].split(',')]
-                        #print(Ftmp[2])
-                        #print(Ftmp[2]== 'True')
+                        line1 = Eslab.split("[")[0]
+                        Ftmp = line1.split(",")
+                        conf_slab = Ftmp[0].split("_")[0:-1]
+                        line2 = [eval(i) for i in Eslab.split("[")[1].split("]")[0].split(",")]
+                        # print(Ftmp[2])
+                        # print(Ftmp[2]== 'True')
                         if conf_slab == conf_facet:
-                            poscar = f'./poscar/{conf}.vasp'
-                            adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
+                            poscar = f"./poscar/{conf}.vasp"
+                            (
+                                adatoms,
+                                adatoms_symb,
+                                surfatoms,
+                                surfatoms_symb,
+                                subsurfatoms,
+                                subsurfatoms_symb,
+                            ) = distinguish_atom_binding(
                                 poscar,
                                 tol=0.05,
                                 base_layer=int(Ftmp[3]),
-                                atoms_layer=int(float(Ftmp[4])))
+                                atoms_layer=int(float(Ftmp[4])),
+                            )
                             if line2 == surfatoms_symb:
-                                if Facet_property == 'all':
+                                if Facet_property == "all":
                                     E_slab = Ftmp[1]
-                                elif (Facet_property == 'stable') & (Ftmp[2] == 'True'):
+                                elif (Facet_property == "stable") & (Ftmp[2] == "True"):
                                     E_slab = Ftmp[1]
                                 else:
                                     continue
                             else:
                                 continue
                         else:
                             continue
             else:
                 continue
 
             if E_slab:
                 Eads = Extract_adsE(slab_E=E_slab, radical_E=E_rad, tot_E=Eads)
-                #print(conf,Eads)
-                Foutput.write(f'{conf},{Eads}\n')
+                # print(conf,Eads)
+                Foutput.write(f"{conf},{Eads}\n")
             else:
-                print('NO Eslab')
+                print("NO Eslab")
         else:
-            print(f'{conf} is not calculated!')
-    #print(f'Species: {num}')
+            print(f"{conf} is not calculated!")
+    # print(f'Species: {num}')
     EnerInfo.close()
     Foutput.close()
 
 
-def cal_adE_coad(Flist, FErad, FEslab, Erad_property='radical'):
-    """
-    Calculate the adsorption energy of CO on a surface with multiple radicals
+def cal_adE_coad(Flist, FErad, FEslab, Erad_property="radical"):
+    """Calculate the adsorption energy of CO on a surface with multiple radicals.
 
     Parameters
     ----------
     Flist: str
         File path of a text file that contains the adsorption energy information of the system in each line.
         Each line should be in the following format: facet_radical1_radical2, adsorption_energy, where
         facet_radical1_radical2 is the identifier of the system, and adsorption_energy is the corresponding
@@ -1300,56 +1324,54 @@
     Erad_property: str, optional
         The property used to calculate the radical energy. It can be either 'atom' or 'radical'. Default is 'radical'.
 
     Returns
     -------
     None
     The function writes the calculated adsorption energy for each system to a file named 'adsE_coad_<Erad_property>'.
-
     """
 
-    EnerInfo = open(Flist, 'r+')
-    Foutput = open(f'adsE_coad_{Erad_property}', 'w+')
+    EnerInfo = open(Flist, "r+")
+    Foutput = open(f"adsE_coad_{Erad_property}", "w+")
 
     for i, ads_ener in enumerate(EnerInfo):
-        conf = ads_ener.split(',', 1)[0]
-        Eads = ads_ener.split(',', 1)[1].strip()
-        conf_facet = conf.split('_')[0:-3]
-        conf_radicals = conf.split('_')[-3:-1]
+        conf = ads_ener.split(",", 1)[0]
+        Eads = ads_ener.split(",", 1)[1].strip()
+        conf_facet = conf.split("_")[0:-3]
+        conf_radicals = conf.split("_")[-3:-1]
 
-        #if Eads and len(conf.split('_')) > 4:
-        #if Eads and len(conf.split('_')) > 3:
+        # if Eads and len(conf.split('_')) > 4:
+        # if Eads and len(conf.split('_')) > 3:
         if Eads:
-            #print(Eads,len(conf.split('_')))
+            # print(Eads,len(conf.split('_')))
             E_rad, E_slab = 0, 0
             E_slab = cal_Eslab(FEslab, conf_facet)
-            if Erad_property == 'atom':
+            if Erad_property == "atom":
                 for i, conf_radical in enumerate(conf_radicals):
                     ## extract the energy of radical based atom energy
                     E_rad = float(E_rad) + float(cal_Erad_atom(FErad, conf_radical))
-            elif Erad_property == 'radical':
+            elif Erad_property == "radical":
                 for i, conf_radical in enumerate(conf_radicals):
                     E_rad = float(E_rad) + float(cal_Erad(FErad, conf_radical))
             else:
-                print('Erad has not the property!')
+                print("Erad has not the property!")
                 break
 
             Eads = Extract_adsE(slab_E=E_slab, radical_E=E_rad, tot_E=Eads)
             print(conf, Eads)
-            Foutput.write(f'{conf},{Eads}\n')
+            Foutput.write(f"{conf},{Eads}\n")
         else:
-            print(f'{conf} is not calculated!')
+            print(f"{conf} is not calculated!")
     EnerInfo.close()
     Foutput.close()
 
 
-### TO extract the struct info and energy of specific slab and
+# TO extract the struct info and energy of specific slab and
 def Extract_slab_info_1(Flist, facet):
-    """
-    Extracts structural information and energy of specific slab.
+    """Extracts structural information and energy of specific slab.
 
     Parameters
     ----------
     Flist : str
         File path to the list of slab energies.
     facet : list
         List of strings representing the surface facets to extract information for.
@@ -1371,127 +1393,146 @@
     Notes
     -----
     This function extracts the energy and structural information of a specific slab given a list of energies and the
     surface facets to extract information for. The energy and surface information are extracted for all slabs that match
     the given facet. If there is only one matching slab, the energy and surface information are returned directly. If
     there are multiple matching slabs, the function determines the most stable facet by finding the slab with the lowest
     energy, and returns the energy and surface information for that slab.
-
     """
     E_slab, surf = [], []
-    with open(Flist, 'r+') as Eslabs:
+    with open(Flist, "r+") as Eslabs:
         for i, Eslab in enumerate(Eslabs):
-            conf = Eslab.split(',')[0]
-            slab = Eslab.split(',')[0].split('_')[0:-1]
-            E = Eslab.split(',')[1]
+            conf = Eslab.split(",")[0]
+            slab = Eslab.split(",")[0].split("_")[0:-1]
+            E = Eslab.split(",")[1]
             ## TO extract the energy and surface info
             if facet == slab:
                 E_slab += [float(E)]
                 # TO extract struct info: layers and atom numbers of layer
-                poscar = f'./poscar/{conf}.vasp'
-                struct = read(poscar, format='vasp')
-                layer = len(get_unique_coordinates(struct, axis=2, tag=True, tol=0.01))
+                poscar = f"./poscar/{conf}.vasp"
+                struct = read(poscar, format="vasp")
+                layer = len(get_unique_coordinates(struct, axis=2, tag=True, tol=0.01))-1   # Changed by RxChen, 2023/06/02
                 atoms_layer = int(len(struct.get_chemical_symbols())) / int(layer)
-                adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-                    poscar, tol=0.05, base_layer=layer, atoms_layer=atoms_layer)
+                (
+                    adatoms,
+                    adatoms_symb,
+                    surfatoms,
+                    surfatoms_symb,
+                    subsurfatoms,
+                    subsurfatoms_symb,
+                ) = distinguish_atom_binding(
+                    poscar, tol=0.05, base_layer=layer, atoms_layer=atoms_layer
+                )
                 surf += [surfatoms_symb]
     ## TO find out the most stable facet
     if len(E_slab) == 1:
         pass
     elif len(E_slab) > 1:
         E_stable = min(E_slab)
         surf_stable = surf[E_slab.index(E_stable)]
 
     return E_slab, surf, [E_stable], [surf_stable], [layer, atoms_layer]
 
 
-###TO Extract the struct info and energy of slabs
+#TO Extract the struct info and energy of slabs
 def Extract_slab_info_2(Flist, layer=4):
-    """TO Extract the struct info and energy of slabs
+    """TO Extract the struct info and energy of slabs.
 
     Parameters
     ----------
     Flist: str
         Crystal surface energy information file
     layer: int
         Number of crystal layers, default value is 4
 
     Returns
     -------
     None
-
     """
 
-    Fslab = open('energy_facet_f', 'w+')
-    with open(Flist, 'r+') as Eslabs:
+    Fslab = open("energy_facet_f", "w+")
+    with open(Flist, "r+") as Eslabs:
         for i, Eslab in enumerate(Eslabs):
-            conf = Eslab.split(',')[0]
-            #TO extract energy
-            E = Eslab.split(',')[1]
+            conf = Eslab.split(",")[0]
+            # TO extract energy
+            E = Eslab.split(",")[1]
             E_slab = float(E)
             # TO extract struct info: layers and atom numbers of layer
-            poscar = f'./poscar/{conf}.vasp'
-            struct = read(poscar, format='vasp')
-            layer = len(get_unique_coordinates(struct, axis=2, tag=True, tol=0.01))
+            poscar = f"./poscar/{conf}.vasp"
+            struct = read(poscar, format="vasp")
+            layer = len(get_unique_coordinates(struct, axis=2, tag=True, tol=0.01)) - 1 # Changed by RxChen, 2023/06/02
             atoms_layer = int(len(struct.get_chemical_symbols())) / int(layer)
-            adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-                poscar, tol=0.05, base_layer=layer, atoms_layer=atoms_layer)
+            (
+                adatoms,
+                adatoms_symb,
+                surfatoms,
+                surfatoms_symb,
+                subsurfatoms,
+                subsurfatoms_symb,
+            ) = distinguish_atom_binding(
+                poscar, tol=0.05, base_layer=layer, atoms_layer=atoms_layer
+            )
             surf = surfatoms_symb
 
-            Fslab.write(f'{conf},\t{E_slab},\t{surf}\n')
+            Fslab.write(f"{conf},\t{E_slab},\t{surf}\n")
     Fslab.close()
 
 
-###To identify whether the symmetry is keeped###
+#To identify whether the symmetry is keeped#
 def get_symmetry_surfatoms(poscar, tol=0.3):
-    """
-    Determine whether surface atoms are reconstructed
+    """Determine whether surface atoms are reconstructed.
 
     Parameters
     ----------
     poscar : str or Structure
         Vasp format structure file
     tol : float, optional
         Tolerance for determining whether surface atoms are reconstructed. The default is 0.3.
 
     Returns
     -------
     str
         A sign of whether surface atoms are reconstructed. "When surface atoms are reconstructed,
         'NO' is returned, otherwise 'YES' is returned.".
-
     """
     if isinstance(poscar, str):
-        struct = read(poscar, format='vasp')
+        struct = read(poscar, format="vasp")
     else:
         struct = poscar
-    #struct=read(poscar,format='vasp')
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(surfatoms)
+    # struct=read(poscar,format='vasp')
+    layer = len(get_unique_coordinates(poscar, axis=2, tag=True, tol=0.01))-1    
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05, base_layer=layer)    # Changed by RxChen, 2023/06/02
+    # print(surfatoms)
 
     dis_matrix = []  # distcance
     if len(surfatoms) < 2:
-        #raise ValueError('Only or less than 1 atom and No distance')
-        symmetry_prop = 'NO'
+        # raise ValueError('Only or less than 1 atom and No distance')
+        symmetry_prop = "NO"
         return symmetry_prop
     else:
         # p_all=struct.get_scaled_positions()
         # struct.set_scaled_positions(p_all)
 
         for i, atom1 in enumerate(surfatoms):
             dis = []
-            #print(atom1)
+            # print(atom1)
             for j, atom2 in enumerate(surfatoms):
-                #print(atom2)
+                # print(atom2)
                 if atom1 == atom2:
                     continue
                 else:
                     if isinstance(poscar, str):
-                        struct = read(poscar, format='vasp')
+                        struct = read(poscar, format="vasp")
                     else:
                         struct = poscar
                     p_all = struct.get_scaled_positions()
                     struct.set_scaled_positions(p_all)
 
                     p1_scaled = struct.get_scaled_positions()[surfatoms[i]]
                     p2_scaled = struct.get_scaled_positions()[surfatoms[j]]
@@ -1504,116 +1545,133 @@
                     if p1_scaled[1] - p2_scaled[1] >= 0.50:
                         p_all[surfatoms[j]][1] = p2_scaled[1] + 1
                         struct.set_scaled_positions(p_all)
                     elif p1_scaled[1] - p2_scaled[1] <= -0.50:
                         p_all[surfatoms[i]][1] = p1_scaled[1] + 1
                         struct.set_scaled_positions(p_all)
                     dis += [
-                        get_distances(struct.get_positions()[surfatoms[i]],
-                                      struct.get_positions()[surfatoms[j]])[1][0][0]
+                        get_distances(
+                            struct.get_positions()[surfatoms[i]],
+                            struct.get_positions()[surfatoms[j]],
+                        )[1][0][0]
                     ]
-            #print(dis)
+            # print(dis)
             dis_matrix += [min(dis)]
-        #print(min(dis_matrix),max(dis_matrix),np.mean(dis_matrix))
-        #if max(dis_matrix)-min(dis_matrix) > tol:
+        # print(min(dis_matrix),max(dis_matrix),np.mean(dis_matrix))
+        # if max(dis_matrix)-min(dis_matrix) > tol:
         if abs(np.mean(dis_matrix) - min(dis_matrix)) > tol:
-            symmetry_prop = 'NO'
+            symmetry_prop = "NO"
             return symmetry_prop
         else:
-            symmetry_prop = 'YES'
+            symmetry_prop = "YES"
         return symmetry_prop
 
 
 from HTMACat.catkit.gen import defaults
 from ase.data import atomic_numbers, atomic_names, atomic_masses, covalent_radii, chemical_symbols
 import numpy as np
-if __name__ == '__main__':
-    #get_potcar(['opt/POSstart','opt/POSend'])
-    #bind_type,atom_b_conn_symb=get_site('opt/POSend',['NH2','N'])
-    #Sub_repeat('opt/descriptor-all')
-    #poscar='./opt/CONTCAR-Ag111'
-    #dis_symb_matrix,dis_matrix=get_distance_adatoms(poscar,tol=0.1)
-    #print(dis_symb_matrix,dis_matrix)
-    #poscar='CONTCAR'
-    #adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol=0.05)
-    #print(adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb)
-    #bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(poscar)
-    #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
-    #print(get_symmetry_surfatoms(poscar,tol=0.2))
-    ''' 
-   Efile='ads_final_b1' 
-   spec_ads,spec_ads_stable,dir_list_final, spec_ads_stable_surfa=get_site_stable(Efile,Ecut=-0.1)
-   #print(spec_ads)
-   print(spec_ads_stable, spec_ads_stable_surfa)
-   #print(dir_list_final)
-   '''
-    ''' 
+
+if __name__ == "__main__":
+    # get_potcar(['opt/POSstart','opt/POSend'])
+    # bind_type,atom_b_conn_symb=get_site('opt/POSend',['NH2','N'])
+    # Sub_repeat('opt/descriptor-all')
+    # poscar='./opt/CONTCAR-Ag111'
+    # dis_symb_matrix,dis_matrix=get_distance_adatoms(poscar,tol=0.1)
+    # print(dis_symb_matrix,dis_matrix)
+    # poscar='CONTCAR'
+    # adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol=0.05)
+    # print(adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb)
+    # bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(poscar)
+    # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+    # print(get_symmetry_surfatoms(poscar,tol=0.2))
+    """Efile='ads_final_b1' spec_ads,spec_ads_stable,dir_list_final,
+    spec_ads_stable_surfa=get_site_stable(Efile,Ecut=-0.1)
+
+    #print(spec_ads) print(spec_ads_stable, spec_ads_stable_surfa) #print(dir_list_final)
+    """
+    """
    poscar='CONTCAR'
    atom = atomic_numbers['N']
    atom_index,atom_neighs=get_atom_neigh(poscar,atom)
    print(atom_index,atom_neighs)
-   '''
+   """
 
-    #poscar='Pt_Au_100_b1_N_3/CONTCAR'
-    #bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym = get_binding_adatom(poscar)
-    #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym)
-    #dis_symb_matrix,dis_matrix=get_distance_adatoms('opt/CONTCAR1')
-    #print(dis_symb_matrix,dis_matrix)
-    #adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol_layer=0.01,tol=0.02,base_layer=4,atoms_layer=9)
-    #print( adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb)
+    # poscar='Pt_Au_100_b1_N_3/CONTCAR'
+    # bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym = get_binding_adatom(poscar)
+    # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym)
+    # dis_symb_matrix,dis_matrix=get_distance_adatoms('opt/CONTCAR1')
+    # print(dis_symb_matrix,dis_matrix)
+    # adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol_layer=0.01,tol=0.02,base_layer=4,atoms_layer=9)
+    # print( adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb)
 
-    #atoms=['Au','Ag','Pt','Pd','Rh','Ru','Ir','Cu','N','O','H','Zn','Fe','Co','Ni']
+    # atoms=['Au','Ag','Pt','Pd','Rh','Ru','Ir','Cu','N','O','H','Zn','Fe','Co','Ni']
     atoms = [
-        'Os', 'C', 'Cu', 'Zn', 'Al', 'Sc', 'Ti', 'V', 'Cr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Hf', 'Ta',
-        'W', 'Re'
+        "Os",
+        "C",
+        "Cu",
+        "Zn",
+        "Al",
+        "Sc",
+        "Ti",
+        "V",
+        "Cr",
+        "Y",
+        "Zr",
+        "Nb",
+        "Mo",
+        "Tc",
+        "Hf",
+        "Ta",
+        "W",
+        "Re",
     ]
     names_atom, radii_atoms, mass_atoms, vdw_radii_atoms = Extract_atomic_info(atoms)
-    print(f'{atoms}\n{radii_atoms}\n{vdw_radii_atoms}')
-    ''' 
-   layer_adatoms,layer_adatoms_symb=distinguish_atom_binding('opt/CONTCAR', tol=0.05,layer='adatom')
-   print("adatom:%s%s" %(layer_adatoms,layer_adatoms_symb))
-   layer_surfatoms,layer_surfatoms_symb=distinguish_atom_binding('opt/CONTCAR', tol=0.05,layer='surf_atom')
-   print("surf_atom:%s%s" %(layer_surfatoms,layer_surfatoms_symb)) 
-   #print("surf_atom:%s" %(layer_surfatoms_symb))
-   layer_subsurfatoms,layer_subsurfatoms_symb=distinguish_atom_binding('opt/CONTCAR', tol=0.05,layer='subsurf_atom')
-   print("subsurf_atom:%s%s" %(layer_subsurfatoms,layer_subsurfatoms_symb))
-   '''
-    '''
+    print(f"{atoms}\n{radii_atoms}\n{vdw_radii_atoms}")
+    """layer_adatoms,layer_adatoms_symb=distinguish_atom_binding('opt/CONTCAR',
+    tol=0.05,layer='adatom') print("adatom:%s%s" %(layer_adatoms,layer_adatoms_symb))
+    layer_surfatoms,layer_surfatoms_symb=distinguish_atom_binding('opt/CONTCAR',
+    tol=0.05,layer='surf_atom') print("surf_atom:%s%s" %(layer_surfatoms,layer_surfatoms_symb))
+
+    #print("surf_atom:%s" %(layer_surfatoms_symb))
+    layer_subsurfatoms,layer_subsurfatoms_symb=distinguish_atom_binding('opt/CONTCAR', tol=0.05,layer='subsurf_atom')
+    print("subsurf_atom:%s%s" %(layer_subsurfatoms,layer_subsurfatoms_symb))
+    """
+    """
    #radii = defaults.get('radii')
    #radii_adatom=[radii[i.numbers] for i in layer_atoms_symb]
    #number_adatom=[atomic_numbers[i] for i in layer_atoms_symb]
    radii_adatom=[covalent_radii[i] for i in number_adatom]
    radii_mean = np.mean(radii_adatom)
    print(radii_mean)
-   '''
-    ''' 
-   adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding('opt/CONTCAR-N',tol=0.01)  
+   """
+    """
+   adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding('opt/CONTCAR-N',tol=0.01)
    print("adatom:%s%s" %(adatoms,adatoms_symb))
    print("surf_atom:%s%s" %(surfatoms,surfatoms_symb))
    bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym = get_binding_adatom('opt/CONTCAR-N')
    print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_sym)
-   '''
-    '''
-   descriptor=[]
-   #feature=['Enegativity','Valence_electron','Atomic_radius','Atomic_mass']
-   feature=['Valence_electron','Atomic_radius']
-   feature_value_surf=Construct_descriptor_info('Info/Element_Info',layer_surfatoms_symb,feature)
-   feature_value_subsurf=Construct_descriptor_info('Info/Element_Info',layer_subsurfatoms_symb,feature)
-   feature_value=np.hstack((feature_value_surf,feature_value_subsurf))
-   print(feature_value)
-   descriptor += [np.around(np.mean(feature_value,0),2)]
-   print(descriptor)
-   '''
-    #bind_adatoms,bind_adatoms_symb,bind_type_symb,adspecie,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom('opt/POSend')
-    #print(bind_adatoms,bind_adatoms_symb,bind_type_symb,adspecie,bind_surfatoms,bind_surfatoms_symb)
-
-    #bind_type,atom_b_conn_symb=get_site('opt/CONTCAR',['NH2','N'])
-    #print(bind_type)
-
-    #dis_symb_matrix,dis_matrix=get_distance_adatoms('opt/CONTCAR')
-    #print(dis_symb_matrix,dis_matrix)
-    #s='opt/CONTCAR'
-    #if isinstance(s, str):
-    #print("string")
-    #else:
-    #print("not string")
-    #Sub_repeat('opt/descriptor-all')
+   """
+    """descriptor=[]
+
+    #feature=['Enegativity','Valence_electron','Atomic_radius','Atomic_mass']
+    feature=['Valence_electron','Atomic_radius']
+    feature_value_surf=Construct_descriptor_info('Info/Element_Info',layer_surfatoms_symb,feature)
+    feature_value_subsurf=Construct_descriptor_info('Info/Element_Info',layer_subsurfatoms_symb,feature)
+    feature_value=np.hstack((feature_value_surf,feature_value_subsurf))
+    print(feature_value)
+    descriptor += [np.around(np.mean(feature_value,0),2)]
+    print(descriptor)
+    """
+    # bind_adatoms,bind_adatoms_symb,bind_type_symb,adspecie,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom('opt/POSend')
+    # print(bind_adatoms,bind_adatoms_symb,bind_type_symb,adspecie,bind_surfatoms,bind_surfatoms_symb)
+
+    # bind_type,atom_b_conn_symb=get_site('opt/CONTCAR',['NH2','N'])
+    # print(bind_type)
+
+    # dis_symb_matrix,dis_matrix=get_distance_adatoms('opt/CONTCAR')
+    # print(dis_symb_matrix,dis_matrix)
+    # s='opt/CONTCAR'
+    # if isinstance(s, str):
+    # print("string")
+    # else:
+    # print("not string")
+    # Sub_repeat('opt/descriptor-all')
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/Construct_neb.py` & `HTMACat-1.0.5/HTMACat/NEB/Construct_neb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# -*- coding: UTF-8 -*-
 from ase import io
 from ase.geometry import get_distances, Cell
 from ase.neb import NEB
 from ase.neb import interpolate
 from ase.constraints import FixAtoms
 from ase.visualize import view
 import numpy as np
 
 
-def Construct_neb(struct, method_inter='linear', nimages=6, dcut=0.25, d_scaled=0.5):
-    """
-    Construct a Nudged Elastic Band (NEB) for transitioning between two structures.
+def Construct_neb(struct, method_inter="linear", nimages=6, dcut=0.25, d_scaled=0.5):
+    """Construct a Nudged Elastic Band (NEB) for transitioning between two structures.
 
     Parameters
     ----------
     struct : list
         List of two strings representing the initial and final states in VASP file format.
     method_inter : str, optional
         Method for interpolating the positions of the middle images. Either 'linear' or 'idpp'. Default is 'linear'.
@@ -30,96 +28,98 @@
     images : list
         List of images representing the NEB calculation. The first and last images are the initial and final states, respectively, and the middle images are interpolated.
 
     Examples
     --------
     >>> struct = ['initial.vasp', 'final.vasp']
     >>> images = Construct_neb(struct, method_inter='idpp', nimages=10, dcut=0.2, d_scaled=0.3)s
-
     """
     ###Read initial and final states:
-    initial = io.read(struct[0], format='vasp')
-    final = io.read(struct[1], format='vasp')
+    initial = io.read(struct[0], format="vasp")
+    final = io.read(struct[1], format="vasp")
 
     ###fixed atoms distance and indices,modify the positions
     p1_scaled = initial.get_scaled_positions()
     p2_scaled = final.get_scaled_positions()
     p1 = initial.get_positions()
     p2 = final.get_positions()
 
-    #print(p2[-1],final.get_scaled_positions()[-1])
+    # print(p2[-1],final.get_scaled_positions()[-1])
     length = initial.get_cell_lengths_and_angles()[0:3]
     Mask = []
     Natom = []
     if len(p1) == len(p2):
         for i in range(len(p1)):
             # get the distance of different axises
             # check the distance of every axis is or not larger than 0.5*cell length
             # If larger, add the length to modify the position
             for j in range(3):
                 if (p2_scaled[i][j] - p1_scaled[i][j]) > d_scaled:
-                    if abs(p2_scaled[i][j] - p1_scaled[i][j]) > abs(p2_scaled[i][j] -
-                                                                    (p1_scaled[i][j] + 1)):
+                    if abs(p2_scaled[i][j] - p1_scaled[i][j]) > abs(
+                        p2_scaled[i][j] - (p1_scaled[i][j] + 1)
+                    ):
                         p1_scaled[i][j] = p1_scaled[i][j] + 1
                         initial.set_scaled_positions(p1_scaled)
                     else:
                         pass
                 elif (p2_scaled[i][j] - p1_scaled[i][j]) < -d_scaled:
-                    if abs(p2_scaled[i][j] - p1_scaled[i][j]) > abs(p2_scaled[i][j] + 1 -
-                                                                    p1_scaled[i][j]):
+                    if abs(p2_scaled[i][j] - p1_scaled[i][j]) > abs(
+                        p2_scaled[i][j] + 1 - p1_scaled[i][j]
+                    ):
                         p2_scaled[i][j] = p2_scaled[i][j] + 1
                         final.set_scaled_positions(p2_scaled)
                     else:
                         pass
                 else:
                     continue
 
             # get the Euclidean Distance
-            #vector1,vector2=p1[i],p2[i];dis = np.sqrt(np.sum(np.square(vector1-vector2)))
+            # vector1,vector2=p1[i],p2[i];dis = np.sqrt(np.sum(np.square(vector1-vector2)))
             dis = get_distances(p1[i], p2[i])[1][0][0]
-            #p1_t=np.array([p1_scaled[i][0]*length[0],p1_scaled[i][1]*length[1],p1_scaled[i][2]*length[2]])
-            #p2_t=np.array([p2_scaled[i][0]*length[0],p2_scaled[i][1]*length[1],p2_scaled[i][2]*length[2]])
-            #dis_t= np.sqrt(np.sum(np.square(p1_t-p2_t)))
-            #print(dis,dis_t)
+            # p1_t=np.array([p1_scaled[i][0]*length[0],p1_scaled[i][1]*length[1],p1_scaled[i][2]*length[2]])
+            # p2_t=np.array([p2_scaled[i][0]*length[0],p2_scaled[i][1]*length[1],p2_scaled[i][2]*length[2]])
+            # dis_t= np.sqrt(np.sum(np.square(p1_t-p2_t)))
+            # print(dis,dis_t)
             # according to the dcut(unit:Angstrom),choose the atoms needed to be fixed
             if dis > dcut:
                 Mask += [False]
             else:
                 Mask += [True]
                 Natom += [i]
 
     else:
-        print('The numbers of atoms between two structure are not equal !!!')
-    #view(final)
+        print("The numbers of atoms between two structure are not equal !!!")
+    # view(final)
     ###Make a band consisting of 6 images:
     images = [initial]
     images += [initial.copy() for i in range(nimages)]
     images += [final]
     neb = NEB(images)
     ###Interpolate idpp or linear the potisions of the six middle images:
-    if method_inter == 'linear':
-        neb.interpolate(method='linear')
-    elif method_inter == 'idpp':
-        neb.interpolate(method='idpp')
+    if method_inter == "linear":
+        neb.interpolate(method="linear")
+    elif method_inter == "idpp":
+        neb.interpolate(method="idpp")
     else:
-        print('the interpolate method no exist!')
-        #ima=neb.iterimages()
+        print("the interpolate method no exist!")
+        # ima=neb.iterimages()
 
     ###fixed atoms
     ##method 1:constraint = FixAtoms(indices=Natom)
     ##method 2:constraint = FixAtoms(mask=Mask)
     constraint = FixAtoms(mask=Mask)
     for image in images:
-        #image.calc = Vasp(xc='PBE')
+        # image.calc = Vasp(xc='PBE')
         image.set_constraint(constraint)
     return images
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import os
     from ase.io.vasp import write_vasp, read_vasp
-    os.system('rm -rf 0*')
-    ima = Construct_neb(['POSstart', 'POSend'], method_inter='idpp', d_scaled=0.75, dcut=0.25)
+
+    os.system("rm -rf 0*")
+    ima = Construct_neb(["POSstart", "POSend"], method_inter="idpp", d_scaled=0.75, dcut=0.25)
     for i in range(len(ima)):
-        os.mkdir(f'0{i}', 0o777)
-        write_vasp('0%s/POSCAR' % (i), ima[i], direct=True, sort=[''], vasp5=True)
-    print(f'{int(i)-1} images are constructed')
+        os.mkdir(f"0{i}", 0o777)
+        write_vasp("0%s/POSCAR" % (i), ima[i], direct=True, sort=[""], vasp5=True)
+    print(f"{int(i)-1} images are constructed")
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/Construct_network.py` & `HTMACat-1.0.5/HTMACat/NEB/Construct_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,155 +1,156 @@
-# -*- coding: UTF-8 -*-
-#import math
+# import math
 import os
 from ase import io
 from ase.io.vasp import write_vasp, read_vasp
 from HTMACat.NEB.Construct_neb import Construct_neb
 from HTMACat.NEB.Post_struc import mig_atoms
 import numpy as np
 from HTMACat.Extract_info import *
+
 # Construct reaction network
 ReaInfo = open("reaction", "r+")
 Ads_Ener = open("EnerInfo", "a+")
-Efile = 'energy_list_2.csv'
+Efile = "energy_list_2.csv"
 # to get species involved in the reaction network
-rspe1, rspe2 = Extract_reaction(Efile='reaction')
+rspe1, rspe2 = Extract_reaction(Efile="reaction")
 rspe = np.hstack((rspe1, rspe2))
 
 for index, line in enumerate(ReaInfo):
-    specie_f = line.split('=')[0].strip()
-    specie_b = line.split('=')[1].strip()
-    print('--------------------')
+    specie_f = line.split("=")[0].strip()
+    specie_b = line.split("=")[1].strip()
+    print("--------------------")
     print(line.strip())
     ### Operation on reactant
-    '''
+    """
     1.substract the reactant molecule and type (a g s)
     2.substract the dir and energy of stable configuration
-    '''
+    """
     ##1.substract the product molecule and type (a g s)
     specie_f_list = []
-    for i in range(len(specie_f.split('+'))):
-        specie_f_list += [specie_f.split('+')[i].strip()]
+    for i in range(len(specie_f.split("+"))):
+        specie_f_list += [specie_f.split("+")[i].strip()]
     specie_f_mol = []
     specie_f_typ = []
     for j, specie in enumerate(specie_f_list):
-        specie_f_mol += [specie.split('(', 1)[0].strip()]
-        specie_f_typ += [specie.split('(', 1)[1].split(')')[0].strip()]
+        specie_f_mol += [specie.split("(", 1)[0].strip()]
+        specie_f_typ += [specie.split("(", 1)[1].split(")")[0].strip()]
     print(specie_f_mol)
     ##2.substract the dir and energy of stable configuration
     ads_dir_f = []
     energy_f = []
     EnerInfo = open(f"../surface-adsorption/{Efile}", "r+")
     for i, ads_ener in enumerate(EnerInfo):
-        ads = ads_ener.split(',', 1)[0]
-        ener = ads_ener.split(',', 1)[1].strip()
+        ads = ads_ener.split(",", 1)[0]
+        ener = ads_ener.split(",", 1)[1].strip()
         # to get the reaction species info from the name of poscar
-        for k in range(2, len(ads.split('_'))):
-            tmp = sorted(ads.split('_')[k:-1])
+        for k in range(2, len(ads.split("_"))):
+            tmp = sorted(ads.split("_")[k:-1])
             if np.array([spe in rspe for spe in tmp]).all():
                 ads1 = tmp
                 break
             else:
                 continue
 
-        #if np.array([spe in ads1 for spe in  specie_f_mol]).all():
+        # if np.array([spe in ads1 for spe in  specie_f_mol]).all():
         if ads1 == sorted(specie_f_mol):
             ads_dir_f += [ads]
             energy_f += [ener]
     ener_max_f = max(energy_f)
     ads_dir_max_f = ads_dir_f[energy_f.index(max(energy_f))]
     EnerInfo.close()
 
     ### Operation on product
-    '''
+    """
     1.substract the product molecule and type (a g s)
-    2.substract the dir and energy of stable configuration 
-    '''
+    2.substract the dir and energy of stable configuration
+    """
     ##1.substract the product molecule and type (a g s)
     specie_b_list = []
-    for i in range(len(specie_b.split('+'))):
-        specie_b_list += [specie_b.split('+')[i].strip()]
+    for i in range(len(specie_b.split("+"))):
+        specie_b_list += [specie_b.split("+")[i].strip()]
     specie_b_mol = []
     specie_b_typ = []
     for j, specie in enumerate(specie_b_list):
-        specie_b_mol += [specie.split('(', 1)[0].strip()]
-        specie_b_typ += specie.split('(', 1)[1].split(')')[0].strip()
-    #print(specie_b_mol)
-    #print(specie_b_typ)
+        specie_b_mol += [specie.split("(", 1)[0].strip()]
+        specie_b_typ += specie.split("(", 1)[1].split(")")[0].strip()
+    # print(specie_b_mol)
+    # print(specie_b_typ)
     energy_b = []
     ads_dir_b = []
     EnerInfo = open(f"../surface-adsorption/{Efile}", "r+")
     for i, ads_ener in enumerate(EnerInfo):
-        ads = ads_ener.split(',', 1)[0]
-        ener = ads_ener.split(',', 1)[1].strip()
+        ads = ads_ener.split(",", 1)[0]
+        ener = ads_ener.split(",", 1)[1].strip()
         # to get the reaction species info from the name of poscar
-        for k in range(2, len(ads.split('_'))):
-            tmp = sorted(ads.split('_')[k:-1])
+        for k in range(2, len(ads.split("_"))):
+            tmp = sorted(ads.split("_")[k:-1])
             if np.array([spe in rspe for spe in tmp]).all():
                 ads1 = tmp
                 break
             else:
                 continue
 
-        #if np.array([spe in ads1 for spe in  specie_b_mol]).all():
+        # if np.array([spe in ads1 for spe in  specie_b_mol]).all():
         if ads1 == sorted(specie_b_mol):
             ads_dir_b += [ads]
             energy_b += [ener]
     ener_max_b = max(energy_b)
     ads_dir_max_b = ads_dir_b[energy_b.index(max(energy_b))]
     EnerInfo.close()
     print(ads_dir_max_f, ads_dir_max_b)
     ## output ener info
     Rea = line.strip()
     Spef = ads_dir_max_f
     Ef = str(round(float(ener_max_f), 3))
     Speb = ads_dir_max_b
     Eb = str(round(float(ener_max_b), 3))
     E = str(round((float(ener_max_b) - float(ener_max_f)), 2))
-    Ads_Ener.write(f'{Rea}:\n{Spef}={Ef} eV,{Speb}={Eb} eV,ReaEner={E} eV\n')
+    Ads_Ener.write(f"{Rea}:\n{Spef}={Ef} eV,{Speb}={Eb} eV,ReaEner={E} eV\n")
 
     ### construct dir
     Dir = os.getcwd()
-    File = '+'.join(specie_f_mol) + '=' + '+'.join(specie_b_mol)
+    File = "+".join(specie_f_mol) + "=" + "+".join(specie_b_mol)
     path = os.path.join(Dir, File)
     os.mkdir(path, 0o777)
     Dir1 = os.path.split(Dir)[0]
-    #os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_f}/optmk/CONTCAR ./{File}/POSstart')
-    #os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_b}/optmk/CONTCAR ./{File}/POSend')
-    os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_f}/CONTCAR ./{File}/POSstart')
-    os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_b}/CONTCAR ./{File}/POSend')
+    # os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_f}/optmk/CONTCAR ./{File}/POSstart')
+    # os.system(f'cp {Dir1}/surface-adsorption/{ads_dir_max_b}/optmk/CONTCAR ./{File}/POSend')
+    os.system(f"cp {Dir1}/surface-adsorption/{ads_dir_max_f}/CONTCAR ./{File}/POSstart")
+    os.system(f"cp {Dir1}/surface-adsorption/{ads_dir_max_b}/CONTCAR ./{File}/POSend")
     os.chdir(path)
     Reactlog = open("react.log", "w")
-    Reactlog.write(f'{Rea}:\n{Spef}={Ef} eV,{Speb}={Eb} eV,ReaEner={E} eV\n')
+    Reactlog.write(f"{Rea}:\n{Spef}={Ef} eV,{Speb}={Eb} eV,ReaEner={E} eV\n")
     Reactlog.close
     ### format chansfer and delete the constraint
-    initial = read_vasp('POSstart')
-    final = read_vasp('POSend')
+    initial = read_vasp("POSstart")
+    final = read_vasp("POSend")
     if initial.constraints or final.constraints:
-        write_vasp('POSstart', initial, direct=True, sort=[''], vasp5=True, ignore_constraints=True)
-        write_vasp('POSend', final, direct=True, sort=[''], vasp5=True, ignore_constraints=True)
+        write_vasp(
+            "POSstart", initial, direct=True, sort=[""], vasp5=True, ignore_constraints=True
+        )
+        write_vasp("POSend", final, direct=True, sort=[""], vasp5=True, ignore_constraints=True)
 
     ### construct the cal file
-    os.system('cp POSstart POSCAR')
-    os.system('jointPOTCAR.sh')
-    os.system('rm POSCAR')
-    os.system('cp /data/jqyang/high-throughput/script/infile-neb/* .')
-    print('calc dir is done!')
+    os.system("cp POSstart POSCAR")
+    os.system("jointPOTCAR.sh")
+    os.system("rm POSCAR")
+    os.system("cp /data/jqyang/high-throughput/script/infile-neb/* .")
+    print("calc dir is done!")
     ### construct N images for neb calc
-    mig_atoms(['POSstart', 'POSend'])
-    Images = Construct_neb(struct=['POSstart', 'POSend'],
-                           method_inter='linear',
-                           nimages=6,
-                           dcut=0.75)
-    os.mkdir(f'pos', 0o777)
+    mig_atoms(["POSstart", "POSend"])
+    Images = Construct_neb(
+        struct=["POSstart", "POSend"], method_inter="linear", nimages=6, dcut=0.75
+    )
+    os.mkdir(f"pos", 0o777)
     for i in range(len(Images)):
-        os.mkdir(f'0{i}', 0o777)
-        write_vasp('0%s/POSCAR' % (i), Images[i], direct=True, sort=[''], vasp5=True)
-        write_vasp('pos/POSCAR-0%s' % (i), Images[i], direct=True, sort=[''], vasp5=True)
-    print(f'{int(i)-1} images are constructed')
-    #print('--------------------')
-    #os.system('qsub job.txt')
+        os.mkdir(f"0{i}", 0o777)
+        write_vasp("0%s/POSCAR" % (i), Images[i], direct=True, sort=[""], vasp5=True)
+        write_vasp("pos/POSCAR-0%s" % (i), Images[i], direct=True, sort=[""], vasp5=True)
+    print(f"{int(i)-1} images are constructed")
+    # print('--------------------')
+    # os.system('qsub job.txt')
     os.chdir(Dir)
 
 Ads_Ener.close()
 ReaInfo.close()
-print('NEB construction is done')
+print("NEB construction is done")
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/Dismove.py` & `HTMACat-1.0.5/HTMACat/NEB/Dismove.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 #!/usr/bin/python
-#calculate the atom moving distance between initial and final structure for NEB calculation.
+# calculate the atom moving distance between initial and final structure for NEB calculation.
 #     1.Usage : Dismove.py dcut
 #     2.dcut : when atom moving distance > dcut, the atom id should be exported into Nmoveatom used to NEB calculation.
 #     3.the distance in fraction coord  is exported into POStmp file
 #     4.the distance in real xoord is exported into POStmp2 file
 #     5.the diatance > dcut is exported into POSfinal file
 #     6.the POStmp POStmp2 POSfinal are put into dismove dir
 #     7.the POSstart & POSend are used in vasp coord file (tansforming cif into vasp in vesta)
-#writen by JqYang in 20160512
+# writen by JqYang in 20160512
 #####################################################################################################################
 import os
 import sys
 import linecache
 import math
 
 
 def Dismove(dcut):
-    """
-    calculate the atom moving distance between initial and final structure for NEB calculation.
+    """calculate the atom moving distance between initial and final structure for NEB calculation.
 
     Parameters
     ----------
     dcut:float
         when atom moving distance > dcut, the atom id should be exported into Nmoveatom used to NEB calculation.
 
     Returns
     -------
     None
 
     Notes
     -----
-    This function needs to read two files named POSstart and POSend, and write the processing results to three files: 
-    POStmp, POStmp2, and POSfinal.At the same time, this function will also create a file called Nmovetatom to record 
-    the sequence numbers of atoms whose movement distance is greater than the threshold. It is necessary to ensure that 
-    there is no folder named remove in the current working directory before calling this function, otherwise the folder 
+    This function needs to read two files named POSstart and POSend, and write the processing results to three files:
+    POStmp, POStmp2, and POSfinal.At the same time, this function will also create a file called Nmovetatom to record
+    the sequence numbers of atoms whose movement distance is greater than the threshold. It is necessary to ensure that
+    there is no folder named remove in the current working directory before calling this function, otherwise the folder
     will be deleted.
-
     """
-    #dcut = float(sys.argv[1])
-    POSstart = open('POSstart', 'r')
-    POSend = open('POSend', 'r')
-    POStmp = open('POStmp', 'w')
-    POStmp2 = open('POStmp2', 'w')
+    # dcut = float(sys.argv[1])
+    POSstart = open("POSstart")
+    POSend = open("POSend")
+    POStmp = open("POStmp", "w")
+    POStmp2 = open("POStmp2", "w")
     for i in range(2):
         head = POSstart.readline()
         head2 = POSend.readline()
         POStmp.write(head)
         POStmp2.write(head)
 
-#to x lattice parameter
+    # to x lattice parameter
     head = POSstart.readline()
     head2 = POSend.readline()
     xcoord = head.split()
     xcoord = float(xcoord[0])
     POStmp.write(head)
     POStmp2.write(head)
 
-    #to y lattice parameter
+    # to y lattice parameter
     head = POSstart.readline()
     head2 = POSend.readline()
     ycoord = head.split()
     ycoord = float(ycoord[1])
     POStmp.write(head)
     POStmp2.write(head)
 
-    #to z lattice parameter
+    # to z lattice parameter
     head = POSstart.readline()
     head2 = POSend.readline()
     zcoord = head.split()
     zcoord = float(zcoord[2])
     POStmp.write(head)
     POStmp2.write(head)
 
@@ -78,33 +76,43 @@
     POStmp2.write(head)
 
     head = POSstart.readline()
     head2 = POSend.readline()
     POStmp.write(head)
     POStmp2.write(head)
 
-    #to the number of atoms
+    # to the number of atoms
     Nelement = head.split()
     Tatom = 0
     for i in range(len(Nelement)):
         Tatom = Tatom + int(Nelement[i])
 
     head = POSstart.readline()
     head2 = POSend.readline()
     POStmp.write(head)
     POStmp2.write(head)
 
-    POSftmp = open('POSfinal', 'w')
-    Nmovefile = open('Nmoveatom', 'w')
-    POStmp.write("Natom" + '\t\t\t\t ' + "x" + '\t\t\t\t ' + "y" + '\t\t\t\t ' + "z" + '\n')
-    POStmp2.write("Natom" + '\t\t\t\t ' + "x" + '\t\t\t\t ' + "y" + '\t\t\t\t ' + "z" + '\t\t\t\t' +
-                  "Dmove" + '\n')
-    POSftmp.write("dcut=" + str(dcut) + '\n')
-    POSftmp.write("Natom" + '\t\t\t\t' + "Dmove-final" + '\n')
-    #to atom move distance
+    POSftmp = open("POSfinal", "w")
+    Nmovefile = open("Nmoveatom", "w")
+    POStmp.write("Natom" + "\t\t\t\t " + "x" + "\t\t\t\t " + "y" + "\t\t\t\t " + "z" + "\n")
+    POStmp2.write(
+        "Natom"
+        + "\t\t\t\t "
+        + "x"
+        + "\t\t\t\t "
+        + "y"
+        + "\t\t\t\t "
+        + "z"
+        + "\t\t\t\t"
+        + "Dmove"
+        + "\n"
+    )
+    POSftmp.write("dcut=" + str(dcut) + "\n")
+    POSftmp.write("Natom" + "\t\t\t\t" + "Dmove-final" + "\n")
+    # to atom move distance
     for i in range(int(Tatom)):
         head = POSstart.readline()
         head2 = POSend.readline()
         #     print head2
         head = head.split()
         head2 = head2.split()
         x = float(head2[0]) - float(head[0])
@@ -118,35 +126,48 @@
         if y < -0.5:
             y = y + 1
         z = float(head2[2]) - float(head[2])
         xvalue = float(x) * float(xcoord)
         yvalue = float(y) * float(ycoord)
         zvalue = float(z) * float(zcoord)
         Dmove = math.sqrt(
-            float(xvalue) * float(xvalue) + float(yvalue) * float(yvalue) +
-            float(zvalue) * float(zvalue))
+            float(xvalue) * float(xvalue)
+            + float(yvalue) * float(yvalue)
+            + float(zvalue) * float(zvalue)
+        )
         i = i + 1
         if Dmove > dcut:
-            POSftmp.write('\t\t' + str(i) + '\t\t ' + str(Dmove) + '\n')
-            Nmovefile.write(str(i) + '\t')
-
+            POSftmp.write("\t\t" + str(i) + "\t\t " + str(Dmove) + "\n")
+            Nmovefile.write(str(i) + "\t")
 
-#     print  xvalue
-#     print x
-#     print y
-#     print z
+        #     print  xvalue
+        #     print x
+        #     print y
+        #     print z
         if x != 0 and y != 0 and z != 0:
-            POStmp.write('\t\t' + str(i) + '\t\t ' + str(x) + '\t\t ' + str(y) + '\t\t ' + str(z) +
-                         ' \n')
-            POStmp2.write('\t\t' + str(i) + '\t\t ' + str(xvalue) + '\t\t ' + str(yvalue) +
-                          '\t\t ' + str(zvalue) + '\t\t' + str(Dmove) + ' \n')
+            POStmp.write(
+                "\t\t" + str(i) + "\t\t " + str(x) + "\t\t " + str(y) + "\t\t " + str(z) + " \n"
+            )
+            POStmp2.write(
+                "\t\t"
+                + str(i)
+                + "\t\t "
+                + str(xvalue)
+                + "\t\t "
+                + str(yvalue)
+                + "\t\t "
+                + str(zvalue)
+                + "\t\t"
+                + str(Dmove)
+                + " \n"
+            )
     POSstart.close()
     POSend.close()
     Nmovefile.close()
     POStmp.close()
     POStmp2.close()
     POSftmp.close()
-    os.system('rm -rf dismove')
-    os.system('mkdir dismove')
-    #os.system('pwd')
-    os.system('cp POStmp* POSf* dismove')
-    os.system('rm POStmp* POSf*')
+    os.system("rm -rf dismove")
+    os.system("mkdir dismove")
+    # os.system('pwd')
+    os.system("cp POStmp* POSf* dismove")
+    os.system("rm POStmp* POSf*")
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/Post_struc.py` & `HTMACat-1.0.5/HTMACat/NEB/Post_struc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from ase.io import read
 from catkit.gen.utils import to_gratoms
 from collections import Counter
 import os
 
 
 def mig_atoms(Ffile, dis=[0.50, 0.50, 0.00]):
-    """
-    Migrate atoms in VASP POSCAR files.
+    """Migrate atoms in VASP POSCAR files.
 
     Parameters
     ----------
     Ffile : str
         A string that specifies the filename of the VASP POSCAR file.
     dis : list of float, optional
         A list of three floats that specifies the displacement of each atom
@@ -25,35 +24,34 @@
     This function reads in a VASP POSCAR file, applies a displacement to each
     atom in the file, and writes out a new VASP POSCAR file with the migrated
     atoms. The displacement is specified by the `dis` parameter.
 
     Examples
     --------
     >>> mig_atoms('POSCAR', dis=[0.20, 0.20, 0.20])
-
     """
-    #print(Ffile)
+    # print(Ffile)
     for i, poscar in enumerate(list(Ffile)):
-        poscar_bk = ''.join([poscar, '_bk'])
-        os.system(f'mv {poscar} {poscar_bk}')
+        poscar_bk = "".join([poscar, "_bk"])
+        os.system(f"mv {poscar} {poscar_bk}")
 
-        struc = read(poscar_bk, format='vasp')
+        struc = read(poscar_bk, format="vasp")
         struc2 = to_gratoms(struc)
         symbols = struc2.get_chemical_symbols()
         dic_sym = dict(Counter(symbols))
         Num = sum(list(dic_sym.values()))
         constraint = struc2.constraints
         if constraint:
             Nline = 9
         else:
             Nline = 8
 
-        pos = open(poscar_bk, 'r')
-        #posfile = ''.join([poscar,'-new'])
-        pos_new = open(poscar, 'w')
+        pos = open(poscar_bk)
+        # posfile = ''.join([poscar,'-new'])
+        pos_new = open(poscar, "w")
         for j, line in enumerate(pos):
             if j < Nline:
                 pos_new.write(line)
             elif j >= (int(Nline) + int(Num)):
                 pos.close()
                 pos_new.close()
                 break
@@ -67,21 +65,21 @@
                 if Ytmp > 1:
                     Ytmp = Ytmp - 1
                 if Ztmp > 1:
                     Ztmp = Ztmp - 1
                 coord[0] = str(Xtmp)
                 coord[1] = str(Ytmp)
                 coord[2] = str(Ztmp)
-                coordn = ' '.join(coord)
-                pos_new.write('%s\n' % (coordn))
+                coordn = " ".join(coord)
+                pos_new.write("%s\n" % (coordn))
         pos.close()
         pos_new.close()
-    #os.system('mv POSstart POSstart_bk')
-    #os.system('mv POSstart-new POSstart')
-    #os.system('mv POSend POSend_bk')
-    #os.system('mv POSend-new POSend')
-    #return 0
+    # os.system('mv POSstart POSstart_bk')
+    # os.system('mv POSstart-new POSstart')
+    # os.system('mv POSend POSend_bk')
+    # os.system('mv POSend-new POSend')
+    # return 0
 
 
-#mig_atoms(['optmk/CONTCAR'])
+# mig_atoms(['optmk/CONTCAR'])
 
-#if __name__ == '__main__':
+# if __name__ == '__main__':
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/post_neb.py` & `HTMACat-1.0.5/HTMACat/NEB/post_neb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: UTF-8 -*-
 import matplotlib.pyplot as plt
 import os
 
 
 def calE_neb(nimage=6):
-    """
-    Read the data in the 'react.log' file and calculate the energy barrier information, then return the list of reactants,
-     energy barriers, and energy
+    """Read the data in the 'react.log' file and calculate the energy barrier information, then
+    return the list of reactants, energy barriers, and energy.
 
     Parameters
     ----------
     nimage:int
         how many segments the entire reaction path is divided into,The default value is 6
 
     Returns
@@ -29,22 +27,22 @@
     """
     ## read data and calculate barrier
     Ener_neb = open("react.log", "r+")
     neb_E = []
     neb_B = []
     Ei, Ef, Er = 0, 0, 0
     for i, line in enumerate(Ener_neb):
-        #print(line)
+        # print(line)
         if i == 0:
             reaction = line.strip()
         elif i == 1:
             tmp = line.strip()
-            Ei = tmp.split(',', 2)[0].split('=')[1].split()[0]
-            Ef = tmp.split(',', 2)[1].split('=')[1].split()[0]
-            Ent = tmp.split(',', 2)[2].split('=')[1].split()[0]
+            Ei = tmp.split(",", 2)[0].split("=")[1].split()[0]
+            Ef = tmp.split(",", 2)[1].split("=")[1].split()[0]
+            Ent = tmp.split(",", 2)[2].split("=")[1].split()[0]
             neb_E += [Ei]
             neb_B += [i - 1, round(float(0), 2)]
         elif i < (2 + nimage):
             neb_E += [line.strip()]
             neb_B += [i - 1, round((float(neb_E[i - 1]) - float(neb_E[0])), 2)]
         else:
             i = i - 1
@@ -53,17 +51,16 @@
     neb_B += [i, round(float(Ent), 2)]
     Ener_neb.close()
     return reaction, neb_B, neb_E
 
     ## plot the figure
 
 
-def plt_neb(react, neb, show=True, name='neb'):
-    """
-    It is mainly used to draw the reaction potential energy surface. Its parameters include
+def plt_neb(react, neb, show=True, name="neb"):
+    """It is mainly used to draw the reaction potential energy surface. Its parameters include.
 
     Parameters
     ----------
     react: str
         The reaction equation.
     neb: list
         Potential energy data of the reaction path,
@@ -79,29 +76,29 @@
         The return value includes the potential barrier and reaction heat values in the reaction path.
     """
     X = neb[::2]
     Y = neb[1::2]
     barrier = max(Y)
     enthalpy = Y[-1]
     plt.figure()
-    path = plt.plot(X, Y, 'go-')
+    path = plt.plot(X, Y, "go-")
     for x, y in zip(X, Y):
-        plt.text(x, y, '%.2f' % y, ha='center', va='bottom', fontsize=11)
+        plt.text(x, y, "%.2f" % y, ha="center", va="bottom", fontsize=11)
     plt.xlabel("Reaction Coordination")
     plt.ylabel("Reaction Energy(eV)")
     plt.title("Reaction Pathway")
     plt.legend(labels=[f"{react}:Ea={barrier}eV;Ef={enthalpy}eV"], loc=8)
     if show:
         plt.show()
-        plt.savefig(f'{name}.png', dpi=300, bbox_inches='tight')
+        plt.savefig(f"{name}.png", dpi=300, bbox_inches="tight")
     return barrier, enthalpy
 
 
 ### post processing
-if __name__ == '__main__':
+if __name__ == "__main__":
     react, neb_B, neb_E = calE_neb()
     Ea, Ef = plt_neb(react, neb_B, show=True)
     print(react)
     print("Ea:", Ea)
     print("Ef:", Ef)
     Ener = open("react.log", "a+")
     Ener.write("-----Reaction Info-----\n")
```

### Comparing `HTMACat-1.0.4/HTMACat/NEB/vaspneb6.py` & `HTMACat-1.0.5/HTMACat/NEB/vaspneb6.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,81 +15,79 @@
 
 ###########neb-first################
 
 import os
 
 
 def vaspneb(num, dcut):
-    '''
-   linear interpolate n images with fixing the atoms within the dcut of distance change
-   '''
+    """Linear interpolate n images with fixing the atoms within the dcut of distance change."""
 
 
-dirnametmp = ['00']
-dirname = ''.join(dirnametmp)
-#print dirname
-#os.chdir(dirname)
-os.system('ls > dirnamefile')
+dirnametmp = ["00"]
+dirname = "".join(dirnametmp)
+# print dirname
+# os.chdir(dirname)
+os.system("ls > dirnamefile")
 
-dir = open('dirnamefile', 'r')
+dir = open("dirnamefile")
 firstline = dir.readline()
-#print firstline
+# print firstline
 if dirname in firstline:
-    #os.system('echo 1')
-    os.system('rm -rf 0* con')
-    os.system('mkdir 00 01 02 03 04 05 06 07')
-    os.system('echo it is not a first neb calculation')
-    os.system('echo ')
+    # os.system('echo 1')
+    os.system("rm -rf 0* con")
+    os.system("mkdir 00 01 02 03 04 05 06 07")
+    os.system("echo it is not a first neb calculation")
+    os.system("echo ")
 else:
-    #os.system('echo 2')
-    os.system('mkdir 00 01 02 03 04 05 06 07')
-    os.system('echo it is a first neb calculation')
-    os.system('echo ')
+    # os.system('echo 2')
+    os.system("mkdir 00 01 02 03 04 05 06 07")
+    os.system("echo it is a first neb calculation")
+    os.system("echo ")
 
-os.system('rm -f dirnamefile')
+os.system("rm -f dirnamefile")
 
 ###########neb-boundray################
 
-#import os
-POSstart = open('POSstart', 'r')
-POSend = open('POSend', 'r')
-POSstarttmp = open('POSstarttmp', 'w')
-POSendtmp = open('POSendtmp', 'w')
-#pos = open('pos','w')
+# import os
+POSstart = open("POSstart")
+POSend = open("POSend")
+POSstarttmp = open("POSstarttmp", "w")
+POSendtmp = open("POSendtmp", "w")
+# pos = open('pos','w')
 
 # handle the head of POSstart and POSend
 # handle POSstart
 tmp = POSstart.readline()
-POSstarttmp.write('System = NEB image \n')
+POSstarttmp.write("System = NEB image \n")
 
 for i in range(5):
     head = POSstart.readline()
     POSstarttmp.write(head)
 
-#tmp = POSstart.readline()
+# tmp = POSstart.readline()
 
 head = POSstart.readline()
 POSstarttmp.write(head)
 Nelement = head.split()
 Tatom = 0
 for i in range(len(Nelement)):
     Tatom = Tatom + int(Nelement[i])
 
 head = POSstart.readline()
 POSstarttmp.write(head)
 
 # handle POSend
 tmp = POSend.readline()
-POSendtmp.write('System = NEB image \n')
+POSendtmp.write("System = NEB image \n")
 
 for i in range(5):
     head = POSend.readline()
     POSendtmp.write(head)
 
-#tmp = POSend.readline()
+# tmp = POSend.readline()
 
 head = POSend.readline()
 POSendtmp.write(head)
 Nelement = head.split()
 Tatom = 0
 for i in range(len(Nelement)):
     Tatom = Tatom + int(Nelement[i])
@@ -98,58 +96,58 @@
 POSendtmp.write(head)
 
 # handle the coordinate of POSstart and POSend
 for j in range(Tatom):
     Coor_start = POSstart.readline().split()
     Coor_end = POSend.readline().split()
     for i in range(3):
-        #print Coor_start[i]
-        #print Coor_end[i]
-        #print float(Coor_start[i])
+        # print Coor_start[i]
+        # print Coor_end[i]
+        # print float(Coor_start[i])
         if abs(float(Coor_start[i]) - float(Coor_end[i])) > 0.95:
             #        print j+1
             POSstarttmp.write(Coor_start[i])
-            POSstarttmp.write('  ')
+            POSstarttmp.write("  ")
             POSendtmp.write(Coor_start[i])
-            POSendtmp.write('  ')
+            POSendtmp.write("  ")
         else:
             POSstarttmp.write(Coor_start[i])
-            POSstarttmp.write('  ')
+            POSstarttmp.write("  ")
             POSendtmp.write(Coor_end[i])
-            POSendtmp.write('  ')
-    POSstarttmp.write('\n')
-    POSendtmp.write('\n')
+            POSendtmp.write("  ")
+    POSstarttmp.write("\n")
+    POSendtmp.write("\n")
 
 POSstart.close()
 POSend.close()
 POSstarttmp.close()
 POSendtmp.close()
-#os.system('cat POSstarttmp POSendtmp > pos')
-#pos.close()
-#os.system('rm -f POSstarttmp POSendtmp')
-os.system('echo all atoms have been moved into an unit cell')
+# os.system('cat POSstarttmp POSendtmp > pos')
+# pos.close()
+# os.system('rm -f POSstarttmp POSendtmp')
+os.system("echo all atoms have been moved into an unit cell")
 
 ###########neb-interpolate###############
 
 # suppose we have 8 structures
-#import os
-#os.system('mkdir 00 01 02 03 04 05 06 07')
+# import os
+# os.system('mkdir 00 01 02 03 04 05 06 07')
 rootdir = os.getcwd()
 
 for i in range(8):
     itmp = i
-    dirnametmp = ['0', str(i)]
-    dirname = ''.join(dirnametmp)
+    dirnametmp = ["0", str(i)]
+    dirname = "".join(dirnametmp)
     # print dirname
     os.chdir(dirname)
-    os.system('cp ../POSstarttmp .')
-    os.system('cp ../POSendtmp .')
-    POSstart = open('POSstarttmp', 'r')
-    POSend = open('POSendtmp', 'r')
-    POSCAR = open('POSCAR', 'w')
+    os.system("cp ../POSstarttmp .")
+    os.system("cp ../POSendtmp .")
+    POSstart = open("POSstarttmp")
+    POSend = open("POSendtmp")
+    POSCAR = open("POSCAR", "w")
 
     # handle the head of POSCAR
     for i in range(8):
         head = POSend.readline()
 
     for i in range(6):
         head = POSstart.readline()
@@ -166,58 +164,60 @@
     POSCAR.write(head)
 
     # handle the coordinate of POSCAR
     for i in range(Tatom):
         Coordinatestart = POSstart.readline().split()
         Coordinateend = POSend.readline().split()
         Coordinatetmp = Coordinatestart
-        #print Coordinatetmp[0]
-        #print Coordinatestart[0]
+        # print Coordinatetmp[0]
+        # print Coordinatestart[0]
         for i in range(3):
-            #print Coordinatestart[i]
-            #print Coordinateend[i]
-            #print float(Coor_start[i])
-            Coordinatetmp[i] = float(Coordinatetmp[i]) + float(itmp) * (
-                float(Coordinateend[i]) - float(Coordinatestart[i])) / 7
-            #print Coordinatetmp[i]
+            # print Coordinatestart[i]
+            # print Coordinateend[i]
+            # print float(Coor_start[i])
+            Coordinatetmp[i] = (
+                float(Coordinatetmp[i])
+                + float(itmp) * (float(Coordinateend[i]) - float(Coordinatestart[i])) / 7
+            )
+            # print Coordinatetmp[i]
             POSCAR.write(str(round(Coordinatetmp[i], 6)).ljust(10))
-            POSCAR.write('  ')
-        POSCAR.write('\n')
+            POSCAR.write("  ")
+        POSCAR.write("\n")
 
     POSCAR.close()
     POSstart.close()
     POSend.close()
-    os.system('rm POSstarttmp POSendtmp')
+    os.system("rm POSstarttmp POSendtmp")
     os.chdir(rootdir)
 
-os.system('rm -f POSstarttmp POSendtmp')
-os.system('echo ')
-os.system('echo six images have been generated by linear interpolation')
-os.system('echo ')
+os.system("rm -f POSstarttmp POSendtmp")
+os.system("echo ")
+os.system("echo six images have been generated by linear interpolation")
+os.system("echo ")
 
 ###########neb-selective################
 
 # please write the number of moving atoms in Nmoveatom file
 # like 1 2 3 5
 # you can write 0(-1) in Nmoveatom make all atoms T(F)
 # suppose we have 10 structures
-#import os
+# import os
 rootdir = os.getcwd()
-os.system('mkdir con')
+os.system("mkdir con")
 # Nmoveatom = open('Nmoveatom', 'r')
 
 for i in range(8):
-    dirnametmp = ['0', str(i)]
-    dirname = ''.join(dirnametmp)
+    dirnametmp = ["0", str(i)]
+    dirname = "".join(dirnametmp)
     # print dirname
     os.chdir(dirname)
-    os.system('cp ../Nmoveatom .')
-    POSCAR = open('POSCAR', 'r')
-    POSfinal = open('POStmp', 'w')
-    Nmoveatom = open('Nmoveatom', 'r')
+    os.system("cp ../Nmoveatom .")
+    POSCAR = open("POSCAR")
+    POSfinal = open("POStmp", "w")
+    Nmoveatom = open("Nmoveatom")
     # POSfinal.write('debug')
     # os.chdir(rootdir)
 
     # handle the head of POSCAR
     for i in range(6):
         head = POSCAR.readline()
         POSfinal.write(head)
@@ -225,93 +225,93 @@
     head = POSCAR.readline()
     POSfinal.write(head)
     Nelement = head.split()
     Tatom = 0
     for i in range(len(Nelement)):
         Tatom = Tatom + int(Nelement[i])
 
-    POSfinal.write('Selective Dynamic \n')
+    POSfinal.write("Selective Dynamic \n")
     head = POSCAR.readline()
     POSfinal.write(head)
     # read the number of moving atoms
     Nmatom = Nmoveatom.readline().split()
     Num = []
     for i in range(len(Nmatom)):
         Num = Num + [int(Nmatom[i])]
 
     TMP = 1
     # handle the coordinate of POSCAR
     for i in range(Tatom):
         Coordinate = POSCAR.readline()
-        #print  Coordinate.strip()
+        # print  Coordinate.strip()
         if -2 in Num:
             TMP = -2
             if 0 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   T   T   T \n')
+                POSfinal.write("   T   T   T \n")
                 TMP = 0
             elif -1 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   F   F   F \n')
+                POSfinal.write("   F   F   F \n")
                 TMP = -1
             elif i + 1 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                #POSfinal.write('   T   T   T \n')
-                POSfinal.write('   F   F   F \n')
+                # POSfinal.write('   T   T   T \n')
+                POSfinal.write("   F   F   F \n")
             else:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                #POSfinal.write('   F   F   F \n')
-                POSfinal.write('   T   T   T \n')
+                # POSfinal.write('   F   F   F \n')
+                POSfinal.write("   T   T   T \n")
         else:
             if 0 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   T   T   T \n')
+                POSfinal.write("   T   T   T \n")
                 TMP = 0
             elif -1 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   F   F   F \n')
+                POSfinal.write("   F   F   F \n")
                 TMP = -1
             elif i + 1 in Num:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   T   T   T \n')
+                POSfinal.write("   T   T   T \n")
             else:
-                POSfinal.write('   ')
+                POSfinal.write("   ")
                 POSfinal.write(Coordinate.strip().ljust(34))
-                POSfinal.write('   F   F   F \n')
+                POSfinal.write("   F   F   F \n")
 
     POSCAR.close()
     POSfinal.close()
     Nmoveatom.close()
-    os.system('rm Nmoveatom')
-    os.system('mv POStmp POSCAR')
+    os.system("rm Nmoveatom")
+    os.system("mv POStmp POSCAR")
     os.chdir(rootdir)
 
-os.system('cp 00/POSCAR con/POSCAR0')
-os.system('cp 01/POSCAR con/POSCAR1')
-os.system('cp 02/POSCAR con/POSCAR2')
-os.system('cp 03/POSCAR con/POSCAR3')
-os.system('cp 04/POSCAR con/POSCAR4')
-os.system('cp 05/POSCAR con/POSCAR5')
-os.system('cp 06/POSCAR con/POSCAR6')
-os.system('cp 07/POSCAR con/POSCAR7')
-#os.system('cp 08/POSCAR con/POSCAR8')
-#os.system('cp 09/POSCAR con/POSCAR9')
+os.system("cp 00/POSCAR con/POSCAR0")
+os.system("cp 01/POSCAR con/POSCAR1")
+os.system("cp 02/POSCAR con/POSCAR2")
+os.system("cp 03/POSCAR con/POSCAR3")
+os.system("cp 04/POSCAR con/POSCAR4")
+os.system("cp 05/POSCAR con/POSCAR5")
+os.system("cp 06/POSCAR con/POSCAR6")
+os.system("cp 07/POSCAR con/POSCAR7")
+# os.system('cp 08/POSCAR con/POSCAR8')
+# os.system('cp 09/POSCAR con/POSCAR9')
 
 if TMP == -1:
-    os.system('echo all atoms have been set to fixed')
+    os.system("echo all atoms have been set to fixed")
 elif TMP == 0:
-    os.system('echo all atoms have been set to mobile')
+    os.system("echo all atoms have been set to mobile")
 elif TMP == -2:
-    os.system('echo only the selective atoms have been set to fixed')
+    os.system("echo only the selective atoms have been set to fixed")
 else:
-    os.system('echo only the selective atoms have been set to mobile')
+    os.system("echo only the selective atoms have been set to mobile")
 
-os.system('echo ')
-os.system('echo All settings have done! Congratulations!')
-os.system('echo ')
+os.system("echo ")
+os.system("echo All settings have done! Congratulations!")
+os.system("echo ")
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/build.py` & `HTMACat-1.0.5/HTMACat/catkit/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import HTMACat.catkit as catkit
 import numpy as np
 import ase.build
 import ase
 
 
 def bulk(name, crystalstructure=None, primitive=False, **kwargs):
-    """Return the standard conventional cell of a bulk structure
-    created using ASE. Accepts all keyword arguments for the ase
-    bulk generator.
+    """Return the standard conventional cell of a bulk structure created using ASE. Accepts all
+    keyword arguments for the ase bulk generator.
 
     Parameters
     ----------
     name : Atoms object | str
         Chemical symbol or symbols as in 'MgO' or 'NaCl'.
     crystalstructure : str
         Must be one of sc, fcc, bcc, hcp, diamond, zincblende,
@@ -25,31 +24,24 @@
     standardized_bulk : Gratoms object
         The conventional standard or primitive bulk structure.
     """
     if isinstance(name, str):
         atoms = ase.build.bulk(name, crystalstructure, **kwargs)
     else:
         atoms = name
-    standardized_bulk = catkit.gen.symmetry.get_standardized_cell(
-        atoms, primitive=primitive)
+    standardized_bulk = catkit.gen.symmetry.get_standardized_cell(atoms, primitive=primitive)
 
     return standardized_bulk
 
 
 def surface(
-        elements,
-        size,
-        miller=(1, 1, 1),
-        termination=0,
-        fixed=0,
-        vacuum=10,
-        orthogonal=False,
-        **kwargs):
-    """A helper function to return the surface associated with a
-    given set of input parameters to the general surface generator.
+    elements, size, miller=(1, 1, 1), termination=0, fixed=0, vacuum=10, orthogonal=False, **kwargs
+):
+    """A helper function to return the surface associated with a given set of input parameters to
+    the general surface generator.
 
     Parameters
     ----------
     elements : str or object
         The atomic symbol to be passed to the as bulk builder function
         or an atoms object representing the bulk structure to use.
     size : list (3,)
@@ -71,51 +63,49 @@
     slab : Gratoms object
         Return a slab generated from the specified bulk structure.
     """
     if isinstance(elements, ase.Atoms):
         atoms = elements
     else:
         bkwargs = kwargs.copy()
-        keys = ['crystalstructure', 'a', 'c', 'covera',
-                'u', 'orthorhombic', 'cubic']
+        keys = ["crystalstructure", "a", "c", "covera", "u", "orthorhombic", "cubic"]
         for key in kwargs:
             if key not in keys:
                 del bkwargs[key]
         atoms = ase.build.bulk(elements, **bkwargs)
 
     generator = catkit.gen.surface.SlabGenerator(
         bulk=atoms,
         miller_index=miller,
         layers=size[-1],
         vacuum=vacuum,
         fixed=fixed,
-        layer_type=kwargs.get('layer_type', 'trim'),
-        attach_graph=kwargs.get('attach_graph', True),
-        standardize_bulk=kwargs.get('standardize_bulk', True),
-        tol=kwargs.get('tol', 1e-8)
+        layer_type=kwargs.get("layer_type", "trim"),
+        attach_graph=kwargs.get("attach_graph", True),
+        standardize_bulk=kwargs.get("standardize_bulk", True),
+        tol=kwargs.get("tol", 1e-8),
     )
 
     if len(size) == 2:
         size = size[0]
     elif len(size) == 3 and not orthogonal:
         size = size[:2]
 
     if orthogonal:
-        catkit.gen.defaults['orthogonal'] = True
+        catkit.gen.defaults["orthogonal"] = True
         if isinstance(size, (list, tuple)):
             size = np.prod(size[:2])
 
     slab = generator.get_slab(size=size, iterm=termination)
 
     return slab
 
 
 def molecule(species, bond_index=None, vacuum=0):
-    """Return list of enumerated gas-phase molecule structures based
-    on species and topology.
+    """Return list of enumerated gas-phase molecule structures based on species and topology.
 
     Parameters
     ----------
     species : str
         The chemical symbols to construct a molecule from.
     bond_index : int
         Construct the molecule as though it were adsorbed to a surface
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/__init__.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # Copyright 2017
 # (see accompanying license files for details).
 """Catalysis Generator."""
 
-from collections import MutableMapping
+from collections.abc import MutableMapping
 import numpy as np
 import ase
 
 radicals = np.ones(92)
 radicals[[6, 7, 8, 9, 15, 16]] = [4, 3, 2, 1, 3, 2]
 
 
 class Defaults(MutableMapping, dict):
     """No frills default dictionary class."""
 
     def __init__(self):
-        self.update({
-            'radii': ase.data.covalent_radii.copy(),
-            'radicals': radicals,
-            'orthogonal': False
-        })
+        self.update(
+            {"radii": ase.data.covalent_radii.copy(), "radicals": radicals, "orthogonal": False}
+        )
 
     def __setitem__(self, key, val):
         dict.__setitem__(self, key, val)
 
     def __getitem__(self, key):
         return dict.__getitem__(self, key)
 
+
 defaults = Defaults()
 
 from . import symmetry
 from . import adsorption
 from . import surface
-from . import molecules
 
-__all__ = ['defaults', 'symmetry', 'adsorption', 'surface', 'molecules']
+__all__ = ["defaults", "symmetry", "adsorption", "surface"]
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/adsorption.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/adsorption.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,73 +3,75 @@
 from . import symmetry
 import HTMACat.catkit as catkit
 import matplotlib.pyplot as plt
 import itertools
 import networkx as nx
 import numpy as np
 import scipy
-radii = defaults.get('radii')
 
+radii = defaults.get("radii")
 
-class AdsorptionSites():
+
+class AdsorptionSites:
     """Adsorption site object."""
 
     def __init__(self, slab, surface_atoms=None, tol=1e-5):
-        """Create an extended unit cell of the surface sites for
-        use in identifying other sites.
+        """Create an extended unit cell of the surface sites for use in identifying other sites.
 
         Parameters
         ----------
         slab : Gatoms object
             The slab associated with the adsorption site network to be
             attached.
         tol : float
             Absolute tolerance for floating point errors.
         """
         index, coords, offsets = utils.expand_cell(slab, cutoff=5.0)
         if surface_atoms is None:
             surface_atoms = slab.get_surface_atoms()
         if surface_atoms is None:
-            raise ValueError('Slab must contain surface atoms')
+            raise ValueError("Slab must contain surface atoms")
 
         extended_top = np.where(np.in1d(index, surface_atoms))[0]
 
         self.tol = tol
         self.coordinates = coords[extended_top].tolist()
         self.connectivity = np.ones(extended_top.shape[0]).tolist()
         self.r1_topology = [[i] for i in np.arange(len(extended_top))]
         self.index = index[extended_top]
 
         sites = self._get_higher_coordination_sites(coords[extended_top])
-        self.r2_topology = sites['top'][2]
+        self.r2_topology = sites["top"][2]
 
         # Put data into array format
-        selection = ['bridge', 'hollow', '4fold']
+        selection = ["bridge", "hollow", "4fold"]
         for i, k in enumerate(selection):
             coordinates, r1top, r2top = sites[k]
 
-            if k in ['hollow', '4fold']:
+            if k in ["hollow", "4fold"]:
                 r2top = [[] for _ in coordinates]
 
             self.connectivity += (np.ones(len(coordinates)) * (i + 2)).tolist()
             self.coordinates += coordinates
             self.r1_topology += r1top
             self.r2_topology += r2top
 
         self.coordinates = np.array(self.coordinates)
         self.connectivity = np.array(self.connectivity, dtype=int)
         self.r1_topology = np.array(self.r1_topology, dtype=object)
         self.r2_topology = np.array(self.r2_topology, dtype=object)
         self.frac_coords = np.dot(self.coordinates, np.linalg.pinv(slab.cell))
         self.slab = slab
 
-        screen = (self.frac_coords[:, 0] > 0 - self.tol) & \
-                 (self.frac_coords[:, 0] < 1 - self.tol) & \
-                 (self.frac_coords[:, 1] > 0 - self.tol) & \
-                 (self.frac_coords[:, 1] < 1 - self.tol)
+        screen = (
+            (self.frac_coords[:, 0] > 0 - self.tol)
+            & (self.frac_coords[:, 0] < 1 - self.tol)
+            & (self.frac_coords[:, 1] > 0 - self.tol)
+            & (self.frac_coords[:, 1] < 1 - self.tol)
+        )
 
         self.screen = screen
         self._symmetric_sites = None
 
     def get_connectivity(self, unique=True):
         """Return the number of connections associated with each site."""
         if unique:
@@ -95,20 +97,17 @@
         if unique:
             sel = self.get_symmetric_sites()
         else:
             sel = self.get_periodic_sites()
 
         return topology[sel]
 
-    def _get_higher_coordination_sites(self,
-                                       top_coordinates,
-                                       allow_obtuse=True):
-        """Find all bridge and hollow sites (3-fold and 4-fold) given an
-        input slab based Delaunay triangulation of surface atoms of a
-        super-cell.
+    def _get_higher_coordination_sites(self, top_coordinates, allow_obtuse=True):
+        """Find all bridge and hollow sites (3-fold and 4-fold) given an input slab based Delaunay
+        triangulation of surface atoms of a super-cell.
 
         TODO: Determine if this can be made more efficient by
         removing the 'sites' dictionary.
 
         Parameters
         ----------
         top_coordinates : ndarray (n, 3)
@@ -116,108 +115,106 @@
 
         Returns
         -------
         sites : dict of 3 lists
             Dictionary sites containing positions, points, and neighbor lists.
         """
         sites = {
-            'top': [top_coordinates, [], [[] for _ in top_coordinates]],
-            'bridge': [[], [], []],
-            'hollow': [[], [], []],
-            '4fold': [[], [], []]}
+            "top": [top_coordinates, [], [[] for _ in top_coordinates]],
+            "bridge": [[], [], []],
+            "hollow": [[], [], []],
+            "4fold": [[], [], []],
+        }
 
-        dt = scipy.spatial.Delaunay(sites['top'][0][:, :2])
+        dt = scipy.spatial.Delaunay(sites["top"][0][:, :2])
         neighbors = dt.neighbors
         simplices = dt.simplices
 
         for i, corners in enumerate(simplices):
             cir = scipy.linalg.circulant(corners)
             edges = cir[:, 1:]
 
             # Inner angle of each triangle corner
-            vec = sites['top'][0][edges.T] - sites['top'][0][corners]
+            vec = sites["top"][0][edges.T] - sites["top"][0][corners]
             uvec = vec.T / np.linalg.norm(vec, axis=2).T
             angles = np.sum(uvec.T[0] * uvec.T[1], axis=1)
 
             # Angle types
             right = np.isclose(angles, 0)
-            obtuse = (angles < -self.tol)
+            obtuse = angles < -self.tol
 
             rh_corner = corners[right]
             edge_neighbors = neighbors[i]
 
             if obtuse.any() and not allow_obtuse:
                 # Assumption: All simplices with obtuse angles
                 # are irrelevant boundaries.
                 continue
 
-            bridge = np.sum(sites['top'][0][edges], axis=1) / 2.0
+            bridge = np.sum(sites["top"][0][edges], axis=1) / 2.0
 
             # Looping through corners allows for elimination of
             # redundant points, identification of 4-fold hollows,
             # and collection of bridge neighbors.
             for j, c in enumerate(corners):
                 edge = sorted(edges[j])
 
-                if edge in sites['bridge'][1]:
+                if edge in sites["bridge"][1]:
                     continue
 
                 # Get the bridge neighbors (for adsorption vector)
                 neighbor_simplex = simplices[edge_neighbors[j]]
                 oc = list(set(neighbor_simplex) - set(edge))[0]
 
                 # Right angles potentially indicate 4-fold hollow
                 potential_hollow = edge + sorted([c, oc])
                 if c in rh_corner:
-
-                    if potential_hollow in sites['4fold'][1]:
+                    if potential_hollow in sites["4fold"][1]:
                         continue
 
                     # Assumption: If not 4-fold, this suggests
                     # no hollow OR bridge site is present.
-                    ovec = sites['top'][0][edge] - sites['top'][0][oc]
+                    ovec = sites["top"][0][edge] - sites["top"][0][oc]
                     ouvec = ovec / np.linalg.norm(ovec)
                     oangle = np.dot(*ouvec)
                     oright = np.isclose(oangle, 0)
                     if oright:
-                        sites['4fold'][0] += [bridge[j]]
-                        sites['4fold'][1] += [potential_hollow]
-                        sites['top'][2][c] += [oc]
+                        sites["4fold"][0] += [bridge[j]]
+                        sites["4fold"][1] += [potential_hollow]
+                        sites["top"][2][c] += [oc]
                 else:
-                    sites['bridge'][0] += [bridge[j]]
-                    sites['bridge'][1] += [edge]
-                    sites['bridge'][2] += [[c, oc]]
+                    sites["bridge"][0] += [bridge[j]]
+                    sites["bridge"][1] += [edge]
+                    sites["bridge"][2] += [[c, oc]]
 
-                sites['top'][2][edge[0]] += [edge[1]]
-                sites['top'][2][edge[1]] += [edge[0]]
+                sites["top"][2][edge[0]] += [edge[1]]
+                sites["top"][2][edge[1]] += [edge[0]]
 
             if not right.any() and not obtuse.any():
-                hollow = np.average(sites['top'][0][corners], axis=0)
-                sites['hollow'][0] += [hollow]
-                sites['hollow'][1] += [corners.tolist()]
+                hollow = np.average(sites["top"][0][corners], axis=0)
+                sites["hollow"][0] += [hollow]
+                sites["hollow"][1] += [corners.tolist()]
 
         # For collecting missed bridge neighbors
-        for s in sites['4fold'][1]:
-
+        for s in sites["4fold"][1]:
             edges = itertools.product(s[:2], s[2:])
             for edge in edges:
                 edge = sorted(edge)
-                i = sites['bridge'][1].index(edge)
-                n, m = sites['bridge'][1][i], sites['bridge'][2][i]
+                i = sites["bridge"][1].index(edge)
+                n, m = sites["bridge"][1][i], sites["bridge"][2][i]
                 nn = list(set(s) - set(n + m))
 
                 if len(nn) == 0:
                     continue
-                sites['bridge'][2][i] += [nn[0]]
+                sites["bridge"][2][i] += [nn[0]]
 
         return sites
 
     def get_periodic_sites(self, screen=True):
-        """Return an index of the coordinates which are unique by
-        periodic boundary conditions.
+        """Return an index of the coordinates which are unique by periodic boundary conditions.
 
         Parameters
         ----------
         screen : bool
             Return only sites inside the unit cell.
 
         Returns
@@ -237,16 +234,16 @@
         for p in periodic:
             matched = utils.matching_sites(self.frac_coords[p], coords)
             periodic_match[matched] = p
 
         return periodic_match
 
     def get_symmetric_sites(self, unique=True, screen=True):
-        """Determine the symmetrically unique adsorption sites
-        from a list of fractional coordinates.
+        """Determine the symmetrically unique adsorption sites from a list of fractional
+        coordinates.
 
         Parameters
         ----------
         unique : bool
             Return only the unique symmetrically reduced sites.
         screen : bool
             Return only sites inside the unit cell.
@@ -289,16 +286,15 @@
         if unique:
             return np.unique(symmetry_match)
 
         else:
             return symmetry_match
 
     def get_adsorption_vectors(self, unique=True, screen=True):
-        """Returns the vectors representing the furthest distance from
-        the neighboring atoms.
+        """Returns the vectors representing the furthest distance from the neighboring atoms.
 
         Returns
         -------
         vectors : ndarray (n, 3)
             Adsorption vectors for surface sites.
         """
         top_coords = self.coordinates[self.connectivity == 1]
@@ -314,32 +310,30 @@
         for i, s in enumerate(coords):
             plane_points = np.array(list(r1top[i]) + list(r2top[i]), dtype=int)
             vectors[i] = utils.plane_normal(top_coords[plane_points])
 
         return vectors
 
     def get_adsorption_edges(self, symmetric=True, periodic=True):
-        """Return the edges of adsorption sties defined as all regions
-        with adjacent vertices.
+        """Return the edges of adsorption sties defined as all regions with adjacent vertices.
 
         Parameters
         ----------
         symmetric : bool
             Return only the symmetrically reduced edges.
         periodic : bool
             Return edges which are unique via periodicity.
 
         Returns
         -------
         edges : ndarray (n, 2)
             All edges crossing ridge or vertices indexed by the expanded
             unit slab.
         """
-        vt = scipy.spatial.Voronoi(self.coordinates[:, :2],
-                                   qhull_options='Qbb Qc Qz C{}'.format(1e-2))
+        vt = scipy.spatial.Voronoi(self.coordinates[:, :2], qhull_options=f"Qbb Qc Qz C{1e-2}")
 
         select, lens = [], []
         for i, p in enumerate(vt.point_region):
             select += [vt.regions[p]]
             lens += [len(vt.regions[p])]
 
         dmax = max(lens)
@@ -359,15 +353,15 @@
 
             for v in voi:
                 nr = np.where(regions == v)[0]
 
                 for n in nr:
                     edge = sorted((p, n))
 
-                    if n in uper[:i + 1] or edge in edges:
+                    if n in uper[: i + 1] or edge in edges:
                         continue
 
                     if (np.in1d(per[edge], per[uper[:i]]).any()) and periodic:
                         continue
 
                     sym = sorted(site_id[edge])
                     if sym in symmetry:
@@ -380,18 +374,20 @@
 
         edges = np.array(edges)
         if symmetric:
             edges = edges[uniques]
 
         return edges
 
-    def ex_sites(self, index, select='inner', cutoff=0):
-        """Get site indices inside or outside of a cutoff radii from a
-        provided periodic site index. If two sites are provided, an
-        option to return the mutually inclusive points is also available.
+    def ex_sites(self, index, select="inner", cutoff=0):
+        """Get site indices inside or outside of a cutoff radii from a provided periodic site
+        index.
+
+        If two sites are provided, an option to return the mutually inclusive points is also
+        available.
         """
         per = self.get_periodic_sites(False)
         sym = self.get_symmetric_sites()
         edges = self.get_adsorption_edges(symmetric=False, periodic=False)
         coords = self.coordinates[:, :2]
 
         if isinstance(index, int):
@@ -409,88 +405,76 @@
         norm = np.linalg.norm(diff, axis=2)
         neighbors = np.array(np.where(norm < cutoff))
 
         neighbors = []
         for i in index:
             diff = coords[:, None] - coords[per[i]]
             norm = np.linalg.norm(diff, axis=2)
-            if select == 'mutual' and len(index) == 2:
+            if select == "mutual" and len(index) == 2:
                 neighbors += [np.where(norm < cutoff)[0].tolist()]
             else:
                 neighbors += np.where(norm < cutoff)[0].tolist()
 
-        if select == 'inner':
+        if select == "inner":
             return per[neighbors]
-        elif select == 'outer':
+        elif select == "outer":
             return np.setdiff1d(per, per[neighbors])
-        elif select == 'mutual':
+        elif select == "mutual":
             return np.intersect1d(per[neighbors[0]], per[neighbors[1]])
 
     def plot(self, savefile=None):
         """Create a visualization of the sites."""
         top = self.connectivity == 1
         other = self.connectivity != 1
         dt = scipy.spatial.Delaunay(self.coordinates[:, :2][top])
 
         fig = plt.figure(figsize=(6, 4), frameon=False)
         ax = fig.add_axes([0, 0, 1, 1])
 
         ax.triplot(dt.points[:, 0], dt.points[:, 1], dt.simplices.copy())
-        ax.plot(dt.points[:, 0], dt.points[:, 1], 'o')
-        ax.plot(self.coordinates[:, 0][other], self.coordinates[:, 1][other],
-                'o')
-        ax.axis('off')
+        ax.plot(dt.points[:, 0], dt.points[:, 1], "o")
+        ax.plot(self.coordinates[:, 0][other], self.coordinates[:, 1][other], "o")
+        ax.axis("off")
 
         if savefile:
             plt.savefig(savefile, transparent=True)
         else:
             plt.show()
 
 
 class Builder(AdsorptionSites):
-    """Initial module for creation of 3D slab structures with
-    attached adsorbates.
-    """
+    """Initial module for creation of 3D slab structures with attached adsorbates."""
 
     def __repr__(self):
         formula = self.slab.get_chemical_formula()
-        string = 'Adsorption builder for {} slab.\n'.format(formula)
+        string = f"Adsorption builder for {formula} slab.\n"
         sym = len(self.get_symmetric_sites())
-        string += 'unique adsorption sites: {}\n'.format(sym)
+        string += f"unique adsorption sites: {sym}\n"
         con = self.get_connectivity()
-        string += 'site connectivity: {}\n'.format(con)
+        string += f"site connectivity: {con}\n"
         edges = self.get_adsorption_edges()
-        string += 'unique adsorption edges: {}'.format(len(edges))
+        string += f"unique adsorption edges: {len(edges)}"
 
         return string
 
     def add_adsorbates(self, adsorbates, indices):
-        """ """
+        """"""
         slab = self.slab.copy()
         for i, ads in enumerate(adsorbates):
             bond = np.where(ads.get_tags() == -1)[0][0]
 
             slab = self._single_adsorption(
-                ads,
-                slab=slab,
-                bond=bond,
-                site_index=indices[i],
-                symmetric=False)
+                ads, slab=slab, bond=bond, site_index=indices[i], symmetric=False
+            )
 
         return slab
 
-    def add_adsorbate(
-            self,
-            adsorbate,
-            bonds=None,
-            index=0,
-            auto_construct=True,
-            **kwargs):
-        """Add and adsorbate to a slab. If the auto_constructor flag is False,
-        the atoms object provided will be attached at the active site.
+    def add_adsorbate(self, adsorbate, bonds=None, index=0, auto_construct=True, **kwargs):
+        """Add and adsorbate to a slab. If the auto_constructor flag is False, the atoms object
+        provided will be attached at the active site.
 
         Parameters
         ----------
         adsorbate : gratoms object
             Molecule to connect to the surface.
         bonds : int or list of 2 int
             Index of adsorbate atoms to be bonded.
@@ -507,72 +491,75 @@
             Slab(s) with adsorbate attached.
         """
         if bonds is None:
             # Molecules with tag -1 are designated to bond
             bonds = np.where(adsorbate.get_tags() == -1)[0]
 
         if len(bonds) == 0:
-            raise ValueError('Specify the index of atom to bond.')
+            raise ValueError("Specify the index of atom to bond.")
 
         elif len(bonds) == 1:
             if index == -1:
                 slab = []
                 for i, _ in enumerate(self.get_symmetric_sites()):
-                    slab += [self._single_adsorption(
-                        adsorbate,
-                        bond=bonds[0],
-                        site_index=i,
-                        auto_construct=auto_construct,
-                        **kwargs)]
+                    slab += [
+                        self._single_adsorption(
+                            adsorbate,
+                            bond=bonds[0],
+                            site_index=i,
+                            auto_construct=auto_construct,
+                            **kwargs,
+                        )
+                    ]
             elif isinstance(index, (list, np.ndarray)):
                 slab = []
                 for i in index:
-                    slab += [self._single_adsorption(
-                        adsorbate,
-                        bond=bonds[0],
-                        site_index=i,
-                        auto_construct=auto_construct,
-                        **kwargs)]
+                    slab += [
+                        self._single_adsorption(
+                            adsorbate,
+                            bond=bonds[0],
+                            site_index=i,
+                            auto_construct=auto_construct,
+                            **kwargs,
+                        )
+                    ]
             else:
                 slab = self._single_adsorption(
                     adsorbate,
                     bond=bonds[0],
                     site_index=index,
                     auto_construct=auto_construct,
-                    **kwargs)
+                    **kwargs,
+                )
 
         elif len(bonds) == 2:
             if index == -1:
                 slab = []
                 edges = self.get_adsorption_edges()
                 for i, _ in enumerate(edges):
-                    slab += [self._double_adsorption(
-                        adsorbate,
-                        bonds=bonds,
-                        edge_index=i,
-                        **kwargs)]
+                    slab += [
+                        self._double_adsorption(adsorbate, bonds=bonds, edge_index=i, **kwargs)
+                    ]
             else:
-                slab = self._double_adsorption(
-                    adsorbate,
-                    bonds=bonds,
-                    edge_index=index,
-                    **kwargs)
+                slab = self._double_adsorption(adsorbate, bonds=bonds, edge_index=index, **kwargs)
 
         else:
-            raise ValueError('Only mono- and bidentate adsorption supported.')
+            raise ValueError("Only mono- and bidentate adsorption supported.")
 
         return slab
 
     def _single_adsorption(
             self,
             adsorbate,
             bond,
             slab=None,
             site_index=0,
             auto_construct=True,
+            direction_mode='default', # wzj 20230524 指定确定位向的方式
+            direction_args=[], # wzj 20230524 为后续扩展预留的参数
             symmetric=True):
         """Bond and adsorbate by a single atom."""
         if slab is None:
             slab = self.slab.copy()
         atoms = adsorbate.copy()
         atoms.set_cell(slab.cell)
 
@@ -591,32 +578,39 @@
         numbers = atoms.numbers[bond]
         R = radii[numbers]
         base_position = utils.trilaterate(top_sites[u], r + R, vector)
 
         branches = nx.bfs_successors(atoms.graph, bond)
         atoms.translate(-atoms.positions[bond])
 
+        """ ### zjwang 20230426
         if auto_construct:
             atoms = catkit.gen.molecules.get_3D_positions(atoms, bond)
 
             # Align with the adsorption vector
             atoms.rotate([0, 0, 1], vector)
+        """
+        if auto_construct: ### wzj 20230510
+            if direction_mode == 'default':
+                atoms.rotate([0, 0, 1], vector)
+            elif direction_mode == 'decision_boundary':
+                adsorption_vector, flag = utils.solve_normal_vector_linearsvc(adsorbate.get_positions(), bond)
+                atoms.rotate(adsorption_vector, [0, 0, 1])
 
         atoms.translate(base_position)
         n = len(slab)
         slab += atoms
 
         # Add graph connections
         for metal_index in self.index[u]:
             slab.graph.add_edge(metal_index, bond + n)
 
         return slab
 
-    def _double_adsorption(self, adsorbate,
-                           bonds=None, edge_index=0):
+    def _double_adsorption(self, adsorbate, bonds=None, edge_index=0):
         """Bond and adsorbate by two adjacent atoms."""
         slab = self.slab.copy()
         atoms = adsorbate.copy()
         atoms.set_cell(slab.cell)
 
         numbers = atoms.numbers[bonds]
         R = radii[numbers] * 0.95
@@ -647,14 +641,15 @@
 
         vectors = self.get_adsorption_vectors(screen=False, unique=False)
         uvec1 = vectors[edges[edge_index]]
         uvec2 = np.cross(uvec1, uvec0)
         uvec2 /= -np.linalg.norm(uvec2, axis=1)[:, None]
         uvec1 = np.cross(uvec2, uvec0)
 
+        """ ### zjwang 20230426
         branches0 = list(nx.bfs_successors(atoms.graph, bonds[0]))
         if len(branches0[0][1]) != 0:
             uvec = [-uvec0, uvec1[0], uvec2[0]]
             self._branch_bidentate(atoms, uvec, branches0[0])
             for branch in branches0[1:]:
                 catkit.gen.molecules._branch_molecule(
                     atoms, branch, adsorption=True)
@@ -662,65 +657,66 @@
         branches1 = list(nx.bfs_successors(atoms.graph, bonds[1]))
         if len(branches1[0][1]) != 0:
             uvec = [uvec0, uvec1[0], uvec2[0]]
             self._branch_bidentate(atoms, uvec, branches1[0])
             for branch in branches1[1:]:
                 catkit.gen.molecules._branch_molecule(
                     atoms, branch, adsorption=True)
+        """
 
         n = len(slab)
         slab += atoms
         # Add graph connections
         slab.graph.add_edge(*np.array(bonds) + n)
         for i, u in enumerate(U):
             for metal_index in self.index[u]:
                 slab.graph.add_edge(metal_index, bonds[i] + n)
 
         return slab
 
     def _branch_bidentate(self, atoms, uvec, branch):
-        """Return extended positions for additional adsorbates
-        based on provided unit vectors.
-        """
+        """Return extended positions for additional adsorbates based on provided unit vectors."""
         r, nodes = branch
         num = atoms.numbers[[r] + nodes]
         d = radii[num[1:]] + radii[num[0]]
         c = atoms[r].position
 
         # Single additional atom
         if len(nodes) == 1:
-            coord0 = c + \
-                d[0] * uvec[0] * np.cos(1 / 3. * np.pi) + \
-                d[0] * uvec[1] * np.sin(1 / 3. * np.pi)
+            coord0 = (
+                c
+                + d[0] * uvec[0] * np.cos(1 / 3.0 * np.pi)
+                + d[0] * uvec[1] * np.sin(1 / 3.0 * np.pi)
+            )
             atoms[nodes[0]].position = coord0
 
         # Two branch system
         elif len(nodes) == 2:
-            coord0 = c + \
-                d[0] * uvec[1] * np.cos(1 / 3. * np.pi) + \
-                0.866 * d[0] * uvec[0] * np.cos(1 / 3. * np.pi) + \
-                0.866 * d[0] * uvec[2] * np.sin(1 / 3. * np.pi)
+            coord0 = (
+                c
+                + d[0] * uvec[1] * np.cos(1 / 3.0 * np.pi)
+                + 0.866 * d[0] * uvec[0] * np.cos(1 / 3.0 * np.pi)
+                + 0.866 * d[0] * uvec[2] * np.sin(1 / 3.0 * np.pi)
+            )
             atoms[nodes[0]].position = coord0
 
-            coord1 = c + \
-                d[1] * uvec[1] * np.cos(1 / 3. * np.pi) + \
-                0.866 * d[1] * uvec[0] * np.cos(1 / 3. * np.pi) + \
-                0.866 * d[1] * -uvec[2] * np.sin(1 / 3. * np.pi)
+            coord1 = (
+                c
+                + d[1] * uvec[1] * np.cos(1 / 3.0 * np.pi)
+                + 0.866 * d[1] * uvec[0] * np.cos(1 / 3.0 * np.pi)
+                + 0.866 * d[1] * -uvec[2] * np.sin(1 / 3.0 * np.pi)
+            )
             atoms[nodes[1]].position = coord1
 
         else:
-            raise ValueError('Too many bonded atoms to position correctly.')
+            raise ValueError("Too many bonded atoms to position correctly.")
 
 
-def get_adsorption_sites(slab,
-                         surface_atoms=None,
-                         symmetry_reduced=True,
-                         tol=1e-5):
-    """Get the adsorption sites of a slab as defined by surface
-    symmetries of the surface atoms.
+def get_adsorption_sites(slab, surface_atoms=None, symmetry_reduced=True, tol=1e-5):
+    """Get the adsorption sites of a slab as defined by surface symmetries of the surface atoms.
 
     Parameters
     ----------
     slab : Atoms object
         The slab to find adsorption sites for. Must have surface
         atoms defined.
     surface_atoms : array_like (N,)
@@ -759,16 +755,16 @@
     unique, counts = np.unique(symmetries, return_counts=True)
     symmetry_index = np.arange(len(unique)).repeat(counts)
 
     return coordinates, connectivity, symmetry_index
 
 
 def _get_adsorption_sites(surface_positions, tol=1e-5):
-    """Return the positions and topology of adsorption sites based on the
-    provided 3D positions of surface atoms for a structure.
+    """Return the positions and topology of adsorption sites based on the provided 3D positions of
+    surface atoms for a structure.
 
     This function is intended for internal use only.
 
     Parameters
     ----------
     surface_positions : ndarray (N, 3)
         Cartesian coordinates for the surface atoms of a structure.
@@ -802,15 +798,15 @@
         # Inner angle of each triangle corner
         vec = positions[0][edges.T] - positions[0][corners]
         uvec = vec.T / np.linalg.norm(vec, axis=2).T
         angles = np.sum(uvec.T[0] * uvec.T[1], axis=1)
 
         # Angle types
         right = np.isclose(angles, 0)
-        obtuse = (angles < -tol)
+        obtuse = angles < -tol
 
         rh_corner = corners[right]
         edge_neighbors = neighbors[i]
 
         bridge = np.sum(positions[0][edges], axis=1) / 2
 
         # Looping through corners allows for elimination of
@@ -825,15 +821,14 @@
             # Get the bridge neighbors (for adsorption vector)
             neighbor_simplex = simplices[edge_neighbors[j]]
             oc = list(set(neighbor_simplex) - set(edge))[0]
 
             # Right angles potentially indicate 4-fold hollow
             potential_hollow = edge + sorted([c, oc])
             if c in rh_corner:
-
                 if potential_hollow in r1topology[3]:
                     continue
 
                 # Assumption: If not 4-fold, this suggests
                 # no hollow OR bridge site is present.
                 ovec = positions[0][edge] - positions[0][oc]
                 ouvec = ovec / np.linalg.norm(ovec)
@@ -856,15 +851,14 @@
             hollow = np.average(positions[0][corners], axis=0)
             positions[2] += [hollow]
             r1topology[2] += [corners.tolist()]
             r2topology[2] += []
 
     # For collecting missed bridge neighbors
     for s in r1topology[3]:
-
         edges = itertools.product(s[:2], s[2:])
         for edge in edges:
             edge = sorted(edge)
             i = r1topology[1].index(edge)
             n, m = r1topology[1][i], r2topology[1][i]
             nn = list(set(s) - set(n + m))
 
@@ -875,18 +869,16 @@
     positions = np.array([j for i in positions for j in i])
     r1topology = np.array([j for i in r1topology for j in i])
     r2topology = np.array([j for i in r2topology for j in i])
 
     return positions, r1topology, r2topology
 
 
-def symmetry_equivalent_points(
-        fractional_coordinates, atoms, tol=1e-5):
-    """Return the symmetrically equivalent points from a list of
-    provided fractional coordinates.
+def symmetry_equivalent_points(fractional_coordinates, atoms, tol=1e-5):
+    """Return the symmetrically equivalent points from a list of provided fractional coordinates.
 
     Parameters
     ----------
     fractional_coordinates : ndarray (N ,3)
         Fractional coordinates to find symmetrical equivalence
         between.
     atoms : Atoms object
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/surface.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from __future__ import division
 from .. import Gratoms
 from . import symmetry
 from . import utils
 from . import adsorption
 from . import defaults
 import numpy as np
 import itertools
 import warnings
 import scipy
 import ase
+
 try:
     from math import gcd
 except ImportError:
     from fractions import gcd
 
 
-class SlabGenerator(object):
+class SlabGenerator:
     """Class for generation of slab unit cells from bulk unit cells.
 
     Many surface operations rely upon / are made easier through the
     bulk basis cell they are created from. The SlabGenerator class
     is designed to house these operations.
 
     Return the miller indices associated with the users requested
@@ -62,25 +62,27 @@
         Covert the bulk input to its standard form before and
         produce the cleave from it. This is highly recommended as
         Miller indices are not defined for non-standard cells.
     tol : float
         Tolerance for floating point rounding errors.
     """
 
-    def __init__(self,
-                 bulk,
-                 miller_index,
-                 layers,
-                 vacuum=None,
-                 fixed=None,
-                 layer_type='ang',
-                 attach_graph=True,
-                 standardize_bulk=False,
-                 primitive=True,
-                 tol=1e-8):
+    def __init__(
+        self,
+        bulk,
+        miller_index,
+        layers,
+        vacuum=None,
+        fixed=None,
+        layer_type="ang",
+        attach_graph=True,
+        standardize_bulk=False,
+        primitive=True,
+        tol=1e-8,
+    ):
         self.layers = layers
         self.vacuum = vacuum
         self.fixed = fixed
         self.tol = tol
         self.layer_type = layer_type
         self.standardized = standardize_bulk
         self.primitive = primitive
@@ -89,41 +91,39 @@
         self.slab_basis = None
         self.slab = None
 
         miller_index = np.array(miller_index)
         if len(miller_index) == 4:
             miller_index[[0, 1]] -= miller_index[2]
             miller_index = np.delete(miller_index, 2)
-        miller_index = (miller_index /
-                        utils.list_gcd(miller_index)).astype(int)
+        miller_index = (miller_index / utils.list_gcd(miller_index)).astype(int)
 
         # Store the Miller indices associated with the standard cell.
         self.miller_index = miller_index
 
         if standardize_bulk:
             bulk = symmetry.get_standardized_cell(bulk, tol=1e-2)
         else:
             warnings.warn(
-                ("Not using a standardized bulk will result in an arbitrary "
-                 "Miller index. To get ensure you are using the correct "
-                 "miller index, use standardize_bulk=True"))
+                "Not using a standardized bulk will result in an arbitrary "
+                "Miller index. To get ensure you are using the correct "
+                "miller index, use standardize_bulk=True"
+            )
 
         if primitive:
-            primitive_bulk = symmetry.get_standardized_cell(
-                bulk, primitive=True, tol=1e-2)
-            miller_index = convert_miller_index(
-                miller_index, bulk, primitive_bulk)
+            primitive_bulk = symmetry.get_standardized_cell(bulk, primitive=True, tol=1e-2)
+            miller_index = convert_miller_index(miller_index, bulk, primitive_bulk)
         else:
             primitive_bulk = bulk
 
         self._bulk = self.align_crystal(primitive_bulk, miller_index)
 
     def align_crystal(self, bulk, miller_index):
-        """Return an aligned unit cell from bulk unit cell. This alignment
-        rotates the a and b basis vectors to be parallel to the Miller index.
+        """Return an aligned unit cell from bulk unit cell. This alignment rotates the a and b
+        basis vectors to be parallel to the Miller index.
 
         Parameters
         ----------
         bulk : Atoms object
             Bulk system to be standardized.
         miller_index : list (3,)
             Miller indices to align with the basis vectors.
@@ -133,46 +133,43 @@
         new_bulk : Gratoms object
             Standardized bulk unit cell.
         """
         del bulk.constraints
 
         if len(np.nonzero(miller_index)[0]) == 1:
             mi = max(np.abs(miller_index))
-            new_lattice = scipy.linalg.circulant(
-                miller_index[::-1] / mi).astype(int)
+            new_lattice = scipy.linalg.circulant(miller_index[::-1] / mi).astype(int)
         else:
             h, k, l = miller_index
             p, q = utils.ext_gcd(k, l)
             a1, a2, a3 = bulk.cell
 
-            k1 = np.dot(p * (k * a1 - h * a2) + q * (l * a1 - h * a3),
-                        l * a2 - k * a3)
-            k2 = np.dot(l * (k * a1 - h * a2) - k * (l * a1 - h * a3),
-                        l * a2 - k * a3)
+            k1 = np.dot(p * (k * a1 - h * a2) + q * (l * a1 - h * a3), l * a2 - k * a3)
+            k2 = np.dot(l * (k * a1 - h * a2) - k * (l * a1 - h * a3), l * a2 - k * a3)
 
             if abs(k2) > self.tol:
                 i = -int(np.round(k1 / k2))
                 p, q = p + i * l, q - i * k
 
             a, b = utils.ext_gcd(p * k + q * l, h)
 
             c1 = (p * k + q * l, -p * h, -q * h)
             c2 = np.array((0, l, -k)) // abs(gcd(l, k))
             c3 = (b, a * p, a * q)
             new_lattice = np.array([c1, c2, c3])
 
-        scaled = np.linalg.solve(new_lattice.T,
-                                 bulk.get_scaled_positions().T).T
+        scaled = np.linalg.solve(new_lattice.T, bulk.get_scaled_positions().T).T
         scaled -= np.floor(scaled + self.tol)
 
         new_bulk = Gratoms(
             positions=bulk.positions,
             numbers=bulk.get_atomic_numbers(),
             magmoms=bulk.get_initial_magnetic_moments(),
-            pbc=True)
+            pbc=True,
+        )
 
         if not self.attach_graph:
             del new_bulk._graph
 
         new_bulk.set_scaled_positions(scaled)
         new_bulk.set_cell(np.dot(new_lattice, bulk.cell), scale_atoms=True)
 
@@ -190,32 +187,31 @@
             if new_bulk.cell[i][i] < 0:
                 new_bulk.cell[i] *= -1
         new_bulk.wrap(eps=1e-3)
 
         return new_bulk
 
     def get_unique_terminations(self):
-        """Determine the fractional coordinate shift that will result in
-        a unique surface termination. This is not required if bulk
-        standardization has been performed, since all available z shifts will
-        result in a unique termination for a primitive cell.
+        """Determine the fractional coordinate shift that will result in a unique surface
+        termination. This is not required if bulk standardization has been performed, since all
+        available z shifts will result in a unique termination for a primitive cell.
 
         Returns
         -------
         unique_shift : array (n,)
             Fractional coordinate shifts which will result in unique
             terminations.
         """
         if self.unique_terminations is not None:
             return self.unique_terminations
 
         zcoords = utils.get_unique_coordinates(self._bulk)
 
         if len(zcoords) > 1:
-            itol = self.tol ** -1
+            itol = self.tol**-1
             zdiff = np.cumsum(np.diff(zcoords))
             zdiff = np.floor(zdiff * itol) / itol
 
             sym = symmetry.Symmetry(self._bulk, self.tol)
             rotations, translations = sym.get_symmetry_operations(affine=False)
 
             # Find all symmetries which are rotations about the z-axis
@@ -237,18 +233,17 @@
 
         self.unique_terminations = unique_shift
         self.slab_basis = [None] * len(unique_shift)
 
         return unique_shift
 
     def get_slab_basis(self, iterm=0, maxn=20):
-        """Return a list of all terminations which have been properly shifted
-        and with an appropriate number of layers added. This function is mainly
-        for performance, to prevent looping over other operations which are not
-        related the size of the slab.
+        """Return a list of all terminations which have been properly shifted and with an
+        appropriate number of layers added. This function is mainly for performance, to prevent
+        looping over other operations which are not related the size of the slab.
 
         This step also contains periodically constrained orthogonalization of
         the c basis. This implementation only works if the a anb b basis
         vectors are properly aligned with the x and y axis. This is strictly to
         assist the correct identification of surface atoms.
 
         Only produces the terminations requested as a lazy evaluator.
@@ -278,15 +273,15 @@
             scaled_positions = ibasis.get_scaled_positions()
             scaled_positions[:, 2] -= zshift - self.tol
             ibasis.set_scaled_positions(scaled_positions)
             ibasis.wrap(pbc=True)
 
         bulk_layers = utils.get_unique_coordinates(_basis)
 
-        if self.layer_type != 'trim':
+        if self.layer_type != "trim":
             height = np.abs(self._bulk.cell[2][2])
             minimum_repetitions = np.ceil(self.layers / height)
         else:
             minimum_repetitions = np.ceil(self.layers / len(bulk_layers))
 
         ibasis *= (1, 1, int(minimum_repetitions))
 
@@ -296,15 +291,15 @@
         div = ibasis.cell[2][1] / ibasis.cell[1][1]
         sign = -np.sign(div)
         if sign == 0:
             sign = 1
         m = np.ceil(np.abs(div)) + 1
 
         # Try to be smart and only search a limited space
-        search = np.mgrid[maxn:-maxn-1:-1, sign*m:m-4*sign:-sign, 1:2]
+        search = np.mgrid[maxn : -maxn - 1 : -1, sign * m : m - 4 * sign : -sign, 1:2]
         search = search.T.reshape(-1, 3)
 
         # Need the reciprocal unit cell.
         recp = np.linalg.inv(ibasis.cell).T
         normal = np.dot(self.miller_index, recp)
         normal /= np.linalg.norm(normal)
 
@@ -328,17 +323,18 @@
 
         n = len(ibasis)
         diff = connectivity[:n, n:].sum(axis=1)
         surf_atoms = diff != 0
 
         if np.all(diff):
             warnings.warn(
-                ("Your slab has no bulk atoms and may be too thin "
-                 "to identify surface atoms correctly. This may cause "
-                 "surface adsorption site identification to fail."))
+                "Your slab has no bulk atoms and may be too thin "
+                "to identify surface atoms correctly. This may cause "
+                "surface adsorption site identification to fail."
+            )
 
         # TODO: Graph generation needs to go here once handling of
         # unit cell repetitions is implemented.
         scaled_zpositions = ibasis.get_scaled_positions()[:, 2] + self.tol
         scaled_zpositions = np.round(scaled_zpositions % 1 + self.tol, 4)
 
         indices = np.argwhere(surf_atoms).flatten()
@@ -348,17 +344,16 @@
         ibasis.set_surface_atoms(top=top, bottom=bottom)
 
         self.slab_basis[iterm] = ibasis
 
         return ibasis
 
     def get_slab(self, size=1, iterm=0):
-        """Generate a slab from the bulk structure. This function is meant
-        specifically for selection of an individual termination or enumeration
-        through surfaces of various size.
+        """Generate a slab from the bulk structure. This function is meant specifically for
+        selection of an individual termination or enumeration through surfaces of various size.
 
         This function will orthogonalize the c basis vector and align it
         with the z-axis which breaks bulk symmetry along the z-axis.
 
         Parameters
         ----------
         size : int, array_like (2,) or (2, 2)
@@ -381,18 +376,18 @@
         slab.cell[2] = [0, 0, slab.cell[2][2]]
         slab.set_pbc([1, 1, 0])
 
         if slab.cell[1][0] < 0:
             slab = transform_ab(slab, [[-1, 0], [0, 1]])
 
         # Trim the bottom of the cell, bulk symmetry may be lost
-        if self.layer_type == 'trim':
+        if self.layer_type == "trim":
             zlayers = utils.get_unique_coordinates(slab)
             reverse_sort = np.sort(zlayers)[::-1]
-            ncut = reverse_sort[:self.layers][-1] * slab.cell[2][2]
+            ncut = reverse_sort[: self.layers][-1] * slab.cell[2][2]
 
             zpos = slab.positions[:, 2]
             index = np.arange(len(slab))
             del slab[index[zpos - ncut < -self.tol]]
 
             slab.cell[2][2] -= ncut
             slab.translate([0, 0, -ncut])
@@ -403,27 +398,26 @@
         slab.translate(-translation)
         slab.wrap()
 
         if self.vacuum:
             slab.center(vacuum=self.vacuum, axis=2)
 
         utils.get_unique_coordinates(slab, tag=True)
-        if self.layer_type == 'sym':
+        if self.layer_type == "sym":
             slab = self.make_symmetric(slab)
 
         roundoff = np.isclose(slab.cell, 0)
         slab.cell[roundoff] = 0
 
         ind = np.lexsort(slab.positions.T)
         slab = slab[ind]
 
         if self.fixed:
             tags = slab.get_tags()
-            constraints = ase.constraints.FixAtoms(
-                mask=tags > (tags.max() - self.fixed))
+            constraints = ase.constraints.FixAtoms(mask=tags > (tags.max() - self.fixed))
             slab.set_constraint(constraints)
 
         self.slab = slab
 
         return slab
 
     def adsorption_sites(self, slab, **kwargs):
@@ -437,16 +431,15 @@
 
         Returns
         -------
         output : tuple (n, n) | (n, n, n)
             Coordinates and connectivity of the adsorption sites.
             The symmetry indices can also be returned.
         """
-        output = adsorption.get_adsorption_sites(
-            slab=slab, **kwargs)
+        output = adsorption.get_adsorption_sites(slab=slab, **kwargs)
 
         return output
 
     def set_size(self, slab, size):
         """Set the size of a slab based one of three methods.
 
         1. An integer value performs a search of valid matrix operations
@@ -471,15 +464,15 @@
         supercell : Gratoms object
             Supercell of the requested size.
         """
         supercell = slab
 
         if isinstance(size, (int, np.integer)):
             a = max(int(size / 2), 1) + size % 2 + 1
-            T = np.mgrid[-a:a + 1, -a:a + 1].reshape(2, -1).T
+            T = np.mgrid[-a : a + 1, -a : a + 1].reshape(2, -1).T
 
             metrics = []
             search_space = itertools.product(T, repeat=2)
             for i, M in enumerate(search_space):
                 M = np.array(M)
                 if ~np.isclose(abs(np.linalg.det(M)), size):
                     continue
@@ -494,20 +487,18 @@
                 if angle < 0 or diff < 0:
                     continue
 
                 metrics += [[d.sum(), angle, M]]
 
             if metrics:
                 order = [0, 1]
-                if defaults.get('orthogonal'):
+                if defaults.get("orthogonal"):
                     order = [1, 0]
 
-                matrix = sorted(metrics,
-                                key=lambda x: (
-                                    x[order[0]], x[order[1]]))[0][-1]
+                matrix = sorted(metrics, key=lambda x: (x[order[0]], x[order[1]]))[0][-1]
                 supercell = transform_ab(supercell, matrix)
 
         elif isinstance(size, (list, tuple, np.ndarray)):
             size = np.array(size, dtype=int)
 
             if size.shape == (2,):
                 supercell *= (size[0], size[1], 1)
@@ -521,47 +512,46 @@
             n = len(supercell)
             exsupercell = supercell * (1, 1, 2)
 
             # Look into making bulk more orthogonal
             exsupercell.wrap()
             connectivity = utils.get_voronoi_neighbors(exsupercell)
             edges = utils.connectivity_to_edges(connectivity[:n, :n])
-            supercell.graph.add_weighted_edges_from(edges, weight='bonds')
+            supercell.graph.add_weighted_edges_from(edges, weight="bonds")
 
         return supercell
 
     def make_symmetric(self, slab):
-        """Returns a symmetric slab. Note, this will trim the slab potentially
-        resulting in loss of stoichiometry.
+        """Returns a symmetric slab.
+
+        Note, this will trim the slab potentially resulting in loss of stoichiometry.
         """
         sym = symmetry.Symmetry(slab)
         inversion_symmetric = sym.get_point_group(check_laue=True)[1]
 
         # Trim the cell until it is symmetric
         while not inversion_symmetric:
             tags = slab.get_tags()
             bottom_layer = np.max(tags)
             del slab[tags == bottom_layer]
 
             sym = symmetry.Symmetry(slab)
             inversion_symmetric = sym.get_point_group(check_laue=True)[1]
 
             if len(slab) <= len(self._bulk):
-                warnings.warn('Too many sites removed, please use a larger '
-                              'slab size.')
+                warnings.warn("Too many sites removed, please use a larger " "slab size.")
                 break
 
-
         return slab
 
+
 def transform_ab(slab, matrix, tol=1e-5):
-    """Transform the slab basis vectors parallel to the z-plane
-    by matrix notation. This can result in changing the slabs
-    cell size. This can also result in very unusual slab dimensions,
-    use with caution.
+    """Transform the slab basis vectors parallel to the z-plane by matrix notation. This can result
+    in changing the slabs cell size. This can also result in very unusual slab dimensions, use with
+    caution.
 
     Parameters
     ----------
     slab : Atoms object
         The slab to be transformed.
     matrix : array_like (2, 2)
         The matrix notation transformation of the a and b basis vectors.
@@ -573,17 +563,15 @@
     slab : Atoms object
         Slab after transformation.
     """
     M = np.eye(3)
     M[:2, :2] = np.array(matrix).T
     newcell = np.dot(M, slab.cell)
 
-    scorners_newcell = np.array([
-        [0, 0], [1, 0],
-        [0, 1], [1, 1]])
+    scorners_newcell = np.array([[0, 0], [1, 0], [0, 1], [1, 1]])
 
     corners = np.dot(scorners_newcell, newcell[:2, :2])
     scorners = np.linalg.solve(slab.cell[:2, :2].T, corners.T).T
     rep = np.ceil(scorners.ptp(axis=0)).astype(int)
 
     slab *= (rep[0], rep[1], 1)
     slab.set_cell(newcell)
@@ -599,17 +587,17 @@
         periodic_match[matched] = i
 
     repeated = np.where(periodic_match != original_index)
     del slab[repeated]
 
     # Align the first basis vector with x
     sign = np.sign(slab.cell[2][2])
-    slab.rotate(slab.cell[0], 'x', rotate_cell=True)
+    slab.rotate(slab.cell[0], "x", rotate_cell=True)
     if sign != np.sign(slab.cell[2][2]):
-        slab.arrays['surface_atoms'] *= -1
+        slab.arrays["surface_atoms"] *= -1
 
     if slab.cell[1][1] < 0:
         slab.cell[1] *= -1
     if slab.cell[2][2] < 0:
         slab.translate([0, 0, -slab.cell[2][2]])
         slab.cell[2][2] = -slab.cell[2][2]
 
@@ -617,54 +605,51 @@
 
 
 def convert_miller_index(miller_index, atoms1, atoms2):
     """Return a converted miller index between two atoms objects."""
     recip1 = utils.get_reciprocal_vectors(atoms1)
     recip2 = utils.get_reciprocal_vectors(atoms2)
 
-    converted_index = np.dot(
-        miller_index, np.dot(recip1, np.linalg.inv(recip2)))
+    converted_index = np.dot(miller_index, np.dot(recip1, np.linalg.inv(recip2)))
     converted_index = np.round(converted_index)
-    converted_index = (converted_index /
-                       utils.list_gcd(converted_index)).astype(int)
+    converted_index = (converted_index / utils.list_gcd(converted_index)).astype(int)
     if converted_index[0] < 0:
         converted_index *= -1
 
     return converted_index
 
 
 def generate_indices(max_index):
-    """Return an array of miller indices enumerated up to values
-    plus or minus some maximum. Filters out lists with greatest
-    common divisors greater than one. Only positive values need to
+    """Return an array of miller indices enumerated up to values plus or minus some maximum.
+    Filters out lists with greatest common divisors greater than one. Only positive values need to
     be considered for the first index.
 
     Parameters
     ----------
     max_index : int
         Maximum number that will be considered for a given surface.
 
     Returns
     -------
     unique_index : ndarray (n, 3)
         Unique miller indices
     """
-    grid = np.mgrid[max_index:-1:-1,
-                    max_index:-max_index-1:-1,
-                    max_index:-max_index-1:-1]
+    grid = np.mgrid[
+        max_index:-1:-1, max_index : -max_index - 1 : -1, max_index : -max_index - 1 : -1
+    ]
     index = grid.reshape(3, -1)
     gcd = utils.list_gcd(index)
     unique_index = index.T[np.where(gcd == 1)]
 
     return unique_index
 
 
 def get_unique_indices(bulk, max_index):
-    """Returns an array of miller indices which will produce unique
-    surface terminations based on a provided bulk structure.
+    """Returns an array of miller indices which will produce unique surface terminations based on a
+    provided bulk structure.
 
     Parameters
     ----------
     bulk : Atoms object
         Bulk structure to get the unique miller indices.
     max_index : int
         Maximum number that will be considered for a given surface.
@@ -696,16 +681,16 @@
 
     unique_millers = np.flip(unique_millers, axis=0)
 
     return unique_millers
 
 
 def get_degenerate_indices(bulk, miller_index):
-    """Return the miller indices which are degenerate to a
-    given miller index for a particular bulk structure.
+    """Return the miller indices which are degenerate to a given miller index for a particular bulk
+    structure.
 
     Parameters
     ----------
     bulk : Atoms object
         Bulk structure to get the degenerate miller indices.
     miller_index : array_like (3,)
         Miller index to get the degenerate indices for.
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/symmetry.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/symmetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .. import Gratoms
 import numpy as np
 import spglib
 
 
 def get_standardized_cell(atoms, primitive=False, tol=1e-5):
     """Atoms object interface with spglib primitive cell finder:
-    https://atztogo.github.io/spglib/python-spglib.html#python-spglib
+    https://atztogo.github.io/spglib/python-spglib.html#python-spglib.
 
     The function also builds in limited functionality for initial
     magnetic moments. Only integer values are supported.
 
     Parameters
     ----------
     atoms : object
@@ -44,39 +44,37 @@
     atoms.translate(-atoms[0].position)
     atoms.wrap()
     atoms.set_initial_magnetic_moments(_magmoms)
 
     return atoms
 
 
-class Symmetry():
+class Symmetry:
     """Wrapper for the spglib package."""
 
     def __init__(self, atoms, tol=1e-5, ang_tol=-1):
         """Atoms object interface with spglib symmetry finder:
-        https://atztogo.github.io/spglib/python-spglib.html#python-spglib
+        https://atztogo.github.io/spglib/python-spglib.html#python-spglib.
 
         Parameters
         ----------
         atoms : Atoms object
             Atomic structure to return the symmetry operations for.
         tol : float
             Tolerance for floating point precision errors.
         """
         self.lattice = atoms.cell
         self.positions = atoms.get_scaled_positions()
         self.numbers = atoms.get_atomic_numbers()
         self.magmoms = atoms.get_initial_magnetic_moments()
-        self.modified_numbers = get_modified_spin_symbols(
-            self.numbers, self.magmoms)
+        self.modified_numbers = get_modified_spin_symbols(self.numbers, self.magmoms)
         self.tol = tol
 
         cell = (self.lattice, self.positions, self.modified_numbers)
-        self.data = spglib.get_symmetry_dataset(
-            cell, symprec=tol, angle_tolerance=ang_tol)
+        self.data = spglib.get_symmetry_dataset(cell, symprec=tol, angle_tolerance=ang_tol)
 
     def get_symmetry_operations(self, affine=True):
         """Return the symmetry operations for a given atomic structure.
 
         Parameters
         ----------
         affine : bool
@@ -88,16 +86,16 @@
             Rotation matices of the symmetry operations.
         translations ndarray (N, 3)
             Translation vector components of the symmetry operations.
         affine_matrices ndarray (N, 4, 4)
             Affine matrix operations, combinations of the rotation and
             translation with ones along the diagonal.
         """
-        rotations = self.data['rotations'][1:]
-        translations = self.data['translations'][1:]
+        rotations = self.data["rotations"][1:]
+        translations = self.data["translations"][1:]
 
         if affine:
             affine_matrices = np.zeros((rotations.shape[0], 4, 4))
             affine_matrices[:, :3, :3] = rotations
             affine_matrices[:, -1, :3] = translations
             affine_matrices[:, -1, -1] = 1
             return affine_matrices
@@ -115,56 +113,54 @@
         Returns
         -------
         pointgroup : str
             The pointgroup symmetry of the atomic structure.
         is_laue : bool
             Whether the pointgroup is a laue symmetry.
         """
-        pointgroup = self.data['pointgroup']
+        pointgroup = self.data["pointgroup"]
 
         if check_laue:
-            laue = ['-1', '2/m', 'mmm', '4/m', '4/mmm',
-                    '-3', '-3m', '6/m', '6/mmm', 'm-3', 'm-3m']
+            laue = ["-1", "2/m", "mmm", "4/m", "4/mmm", "-3", "-3m", "6/m", "6/mmm", "m-3", "m-3m"]
             is_laue = pointgroup in laue
 
             return pointgroup, is_laue
 
         return pointgroup
 
     def get_lattice_name(self):
-        """Return the lattice name of an atoms object based
-        on its spacegroup number:
-        https://en.wikipedia.org/wiki/List_of_space_groups
+        """Return the lattice name of an atoms object based on its spacegroup number:
+        https://en.wikipedia.org/wiki/List_of_space_groups.
 
         Returns
         -------
         lattice : str
             The name of the structures lattice.
         """
-        space_group_number = self.data['number']
+        space_group_number = self.data["number"]
 
         if space_group_number in [146, 148, 155, 160, 161, 166, 167]:
-            return 'rhombohedral'
+            return "rhombohedral"
 
         lattices = {
-            'triclinic': 2,
-            'monoclinic': 15,
-            'orthorhombic': 74,
-            'tetragonal': 142,
-            'hexagonal': 194,
-            'cubic': 230}
+            "triclinic": 2,
+            "monoclinic": 15,
+            "orthorhombic": 74,
+            "tetragonal": 142,
+            "hexagonal": 194,
+            "cubic": 230,
+        }
 
         for lattice, max_number in lattices.items():
             if space_group_number <= max_number:
                 return lattice
 
 
 def get_modified_spin_symbols(numbers, magmoms):
-    """Return a representation of atomic symbols which is
-    unique to the magnetic moment as well.
+    """Return a representation of atomic symbols which is unique to the magnetic moment as well.
 
     This is effectivly creating a single integer which contains the
     atomic number and the magnetic moment multiplied by 10.
 
     Parameters
     ----------
     numbers : ndarray (N,)
@@ -187,16 +183,16 @@
     ind = np.where(sign)
     spin_mod_symbols[ind] *= sign[ind]
 
     return spin_mod_symbols
 
 
 def get_unmodified_spin_symbols(spin_mod_symbols):
-    """Return the origional atomic numbers and magnetic moments from
-    the get_modified_spin_symbols function.
+    """Return the origional atomic numbers and magnetic moments from the get_modified_spin_symbols
+    function.
 
     Parameters
     ----------
     spin_mod_symbols : ndarray (N,)
         Joint symbol and spin representation of an atomic structure.
 
     Returns
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/__init__.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
                           matching_sites, get_integer_enumeration,
                           matching_coordinates, get_unique_coordinates)
 from .graph import (connectivity_to_edges, isomorphic_molecules)
 from .vectors import (get_reciprocal_vectors, plane_normal, get_basis_vectors)
 from .utilities import (running_mean, to_gratoms, get_atomic_numbers,
                         get_reference_energies, parse_slice, ext_gcd,
                         list_gcd)
+from .utils_mdnm import (mol_to_graph, solve_normal_vector_linearsvc)
 
 __all__ = ['get_voronoi_neighbors',
            'get_cutoff_neighbors',
            'get_integer_enumeration',
            'trilaterate',
            'get_unique_xy',
            'expand_cell',
@@ -24,8 +25,10 @@
            'plane_normal',
            'running_mean',
            'to_gratoms',
            'get_atomic_numbers',
            'get_reference_energies',
            'parse_slice',
            'ext_gcd',
-           'list_gcd']
+           'list_gcd',
+           'mol_to_graph',
+           'solve_normal_vector_linearsvc']
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/connectivity.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from . import coordinates
 import numpy as np
 import scipy
 import warnings
 
 
 def get_voronoi_neighbors(atoms, cutoff=5.0, return_distances=False):
-    """Return the connectivity matrix from the Voronoi
-    method. Multi-bonding occurs through periodic boundary conditions.
+    """Return the connectivity matrix from the Voronoi method. Multi-bonding occurs through
+    periodic boundary conditions.
 
     Parameters
     ----------
     atoms : atoms object
         Atoms object with the periodic boundary conditions and
         unit cell information to use.
     cutoff : float
@@ -25,30 +25,31 @@
     index, coords, offsets = coordinates.expand_cell(atoms, cutoff=cutoff)
 
     xm, ym, zm = np.max(coords, axis=0) - np.min(coords, axis=0)
 
     L = int(len(offsets) / 2)
     origional_indices = np.arange(L * len(atoms), (L + 1) * len(atoms))
 
-    voronoi = scipy.spatial.Voronoi(coords, qhull_options='QbB Qc Qs')
+    voronoi = scipy.spatial.Voronoi(coords, qhull_options="QbB Qc Qs")
     points = voronoi.ridge_points
 
     connectivity = np.zeros((len(atoms), len(atoms)))
     distances = []
     distance_indices = []
     for i, n in enumerate(origional_indices):
         ridge_indices = np.where(points == n)[0]
         p = points[ridge_indices]
         dist = np.linalg.norm(np.diff(coords[p], axis=1), axis=-1)[:, 0]
         edges = np.sort(index[p])
 
         if not edges.size:
             warnings.warn(
-                ("scipy.spatial.Voronoi returned an atom which has "
-                 "no neighbors. This may result in incorrect connectivity."))
+                "scipy.spatial.Voronoi returned an atom which has "
+                "no neighbors. This may result in incorrect connectivity."
+            )
             continue
 
         unique_edge = np.unique(edges, axis=0)
 
         for j, edge in enumerate(unique_edge):
             indices = np.where(np.all(edge == edges, axis=1))[0]
             d = dist[indices][np.where(dist[indices] < cutoff)[0]]
@@ -65,29 +66,27 @@
             connectivity[v][u] += count
 
     connectivity /= 2
     if not return_distances:
         return connectivity.astype(int)
 
     if len(distances) > 0:
-        distance_indices, unique_idx_idx = \
-            np.unique(distance_indices, axis=0, return_index=True)
+        distance_indices, unique_idx_idx = np.unique(distance_indices, axis=0, return_index=True)
         distance_indices = distance_indices.tolist()
 
         distances = [distances[i] for i in unique_idx_idx]
 
-    pair_distances = {'indices': distance_indices,
-                      'distances': distances}
+    pair_distances = {"indices": distance_indices, "distances": distances}
 
     return connectivity.astype(int), pair_distances
 
 
 def get_cutoff_neighbors(atoms, cutoff=None, scale_cov_radii=1.2, atol=1e-8):
-    """Return the connectivity matrix from a simple radial cutoff.
-    Multi-bonding occurs through periodic boundary conditions.
+    """Return the connectivity matrix from a simple radial cutoff. Multi-bonding occurs through
+    periodic boundary conditions.
 
     Parameters
     ----------
     atoms : atoms object
         Atoms object with the periodic boundary conditions and
         unit cell information to use.
     cutoff : float
@@ -99,15 +98,15 @@
         Absolute tolerance to use when computing distances.
 
     Returns
     -------
     connectivity : ndarray (n, n)
         Number of edges formed between atoms in a system.
     """
-    cov_radii = HTMACat.catkit.gen.defaults.get('radii') * scale_cov_radii
+    cov_radii = HTMACat.catkit.gen.defaults.get("radii") * scale_cov_radii
     numbers = atoms.numbers
     index, coords = coordinates.expand_cell(atoms)[:2]
 
     if cutoff is None:
         radii = cov_radii[numbers]
         radii = np.repeat(radii[:, None], len(index) / len(radii), axis=1)
         radii = radii.T.flatten()
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/coordinates.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/coordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 
 
 def expand_cell(atoms, cutoff=None, padding=None):
-    """Return Cartesian coordinates atoms within a supercell
-    which contains repetitions of the unit cell which contains
-    at least one neighboring atom.
+    """Return Cartesian coordinates atoms within a supercell which contains repetitions of the unit
+    cell which contains at least one neighboring atom.
 
     Parameters
     ----------
     atoms : Atoms object
         Atoms with the periodic boundary conditions and unit cell
         information to use.
     cutoff : float
@@ -28,55 +27,49 @@
         Integer offsets of each unit cell.
     """
     cell = atoms.cell
     pbc = atoms.pbc
     pos = atoms.positions
 
     if padding is None and cutoff is None:
-        diags = np.sqrt((
-            np.dot([[1, 1, 1],
-                    [-1, 1, 1],
-                    [1, -1, 1],
-                    [-1, -1, 1]],
-                   cell)**2).sum(1))
+        diags = np.sqrt(
+            (np.dot([[1, 1, 1], [-1, 1, 1], [1, -1, 1], [-1, -1, 1]], cell) ** 2).sum(1)
+        )
 
         if pos.shape[0] == 1:
-            cutoff = max(diags) / 2.
+            cutoff = max(diags) / 2.0
         else:
             dpos = (pos - pos[:, None]).reshape(-1, 3)
             Dr = np.dot(dpos, np.linalg.inv(cell))
             D = np.dot(Dr - np.round(Dr) * pbc, cell)
             D_len = np.sqrt((D**2).sum(1))
 
-            cutoff = min(max(D_len), max(diags) / 2.)
+            cutoff = min(max(D_len), max(diags) / 2.0)
 
     latt_len = np.sqrt((cell**2).sum(1))
     V = abs(np.linalg.det(cell))
-    padding = pbc * np.array(np.ceil(cutoff * np.prod(latt_len) /
-                                     (V * latt_len)), dtype=int)
+    padding = pbc * np.array(np.ceil(cutoff * np.prod(latt_len) / (V * latt_len)), dtype=int)
 
     offsets = np.mgrid[
-        -padding[0]:padding[0] + 1,
-        -padding[1]:padding[1] + 1,
-        -padding[2]:padding[2] + 1].T
+        -padding[0] : padding[0] + 1, -padding[1] : padding[1] + 1, -padding[2] : padding[2] + 1
+    ].T
     tvecs = np.dot(offsets, cell)
     coords = pos[None, None, None, :, :] + tvecs[:, :, :, None, :]
 
     ncell = np.prod(offsets.shape[:-1])
     index = np.arange(len(atoms))[None, :].repeat(ncell, axis=0).flatten()
     coords = coords.reshape(np.prod(coords.shape[:-1]), 3)
     offsets = offsets.reshape(ncell, 3)
 
     return index, coords, offsets
 
 
 def trilaterate(centers, r, zvector=None):
-    """Find the intersection of two or three spheres. In the case
-    of two sphere intersection, the z-coordinate is assumed to be
-    an intersection of a plane whose normal is aligned with the
+    """Find the intersection of two or three spheres. In the case of two sphere intersection, the
+    z-coordinate is assumed to be an intersection of a plane whose normal is aligned with the
     points and perpendicular to the positive z-coordinate.
 
     If more than three spheres are supplied, the centroid of the
     points is returned (no radii used).
 
     Parameters
     ----------
@@ -104,17 +97,17 @@
         return centroid
 
     vec1 = centers[1] - centers[0]
     uvec1 = vec1 / np.linalg.norm(vec1)
     d = np.linalg.norm(vec1)
 
     if len(r) == 2:
-        x0 = (d**2 - r[0]**2 + r[1]**2)
+        x0 = d**2 - r[0] ** 2 + r[1] ** 2
         x = d - x0 / (2 * d)
-        a = np.sqrt(4 * d**2 * r[1]**2 - x0**2)
+        a = np.sqrt(4 * d**2 * r[1] ** 2 - x0**2)
         z = 0.5 * (1 / d) * a
         if np.isnan(z):
             z = 0.01
         h = z * zvector
         intersection = centers[0] + uvec1 * x + h
 
     elif len(r) == 3:
@@ -122,28 +115,27 @@
         i = np.dot(uvec1, vec2)
         vec2 = vec2 - i * uvec1
 
         uvec2 = vec2 / np.linalg.norm(vec2)
         uvec3 = np.cross(uvec1, uvec2)
         j = np.dot(uvec2, vec2)
 
-        x = (r[0]**2 - r[1]**2 + d**2) / (2 * d)
-        y = (r[0]**2 - r[2]**2 - 2 * i * x + i**2 + j**2) / (2 * j)
-        z = np.sqrt(r[0]**2 - x**2 - y**2)
+        x = (r[0] ** 2 - r[1] ** 2 + d**2) / (2 * d)
+        y = (r[0] ** 2 - r[2] ** 2 - 2 * i * x + i**2 + j**2) / (2 * j)
+        z = np.sqrt(r[0] ** 2 - x**2 - y**2)
         if np.isnan(z):
             z = 0.01
         intersection = centers[0] + x * uvec1 + y * uvec2 + z * uvec3
 
     return intersection
 
 
 def get_unique_xy(xyz_coords, cutoff=0.1):
-    """Return the unique coordinates of an atoms object
-    for the requrested atoms indices. Z-coordinates are projected
-    to maximum z-coordinate by default.
+    """Return the unique coordinates of an atoms object for the requrested atoms indices.
+    Z-coordinates are projected to maximum z-coordinate by default.
 
     Parameters
     ----------
     xyz_coords : ndarray (n, 3)
         Cartesian coordinates to identify unique xy positions from.
     cutoff : float
         Distance in Angstrons to consider xy-coordinate unique within.
@@ -166,17 +158,16 @@
 
     xyz_coords = np.delete(xyz_coords, xy_copies, axis=0)
 
     return xyz_coords
 
 
 def matching_sites(position, comparators, tol=1e-8):
-    """Get the indices of all points in a comparator list that are
-    equal to a given position (with a tolerance), taking into
-    account periodic boundary conditions (adaptation from Pymatgen).
+    """Get the indices of all points in a comparator list that are equal to a given position (with
+    a tolerance), taking into account periodic boundary conditions (adaptation from Pymatgen).
 
     This will only accept a fractional coordinate scheme.
 
     Parameters
     ----------
     position : list (3,)
         Fractional coordinate to compare to list.
@@ -197,17 +188,16 @@
     fdist -= np.round(fdist)
     match = np.where((np.abs(fdist) < tol).all(axis=1))[0]
 
     return match
 
 
 def matching_coordinates(position, comparators, tol=1e-8):
-    """Get the indices of all points in a comparator list that are
-    equal to a given position (with a tolerance), taking into
-    account periodic boundary conditions (adaptation from Pymatgen).
+    """Get the indices of all points in a comparator list that are equal to a given position (with
+    a tolerance), taking into account periodic boundary conditions (adaptation from Pymatgen).
 
     This will only accept a Cartesian coordinate scheme.
     TODO: merge this with matching_sites.
 
     Parameters
     ----------
     position : list (3,)
@@ -228,16 +218,15 @@
     fdist = comparators - position[None, :]
     match = np.where((np.abs(fdist) < tol).all(axis=1))[0]
 
     return match
 
 
 def get_unique_coordinates(atoms, axis=2, tag=False, tol=1e-3):
-    """Return unique coordinate values of a given atoms object
-    for a specified axis.
+    """Return unique coordinate values of a given atoms object for a specified axis.
 
     Parameters
     ----------
     atoms : object
         Atoms object to search for unique values along.
     axis : int (0, 1, or 2)
         Look for unique values along the x, y, or z axis.
@@ -267,16 +256,16 @@
             tags += [np.where(close)[0][0] + 1]
         atoms.set_tags(tags)
 
     return values
 
 
 def get_integer_enumeration(N=3, span=[0, 2]):
-    """Return the enumerated array of a span of integer values.
-    These enumerations are limited to the length N.
+    """Return the enumerated array of a span of integer values. These enumerations are limited to
+    the length N.
 
     For the default span of [0, 2], the enumeration equates to
     the corners of an N-dimensional hypercube.
 
     Parameters
     ----------
     N : int
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/graph.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import networkx as nx
 import numpy as np
 
 
 def connectivity_to_edges(connectivity, indices=None):
-    """Convert a Numpy connectivity matrix into a list of NetworkX
-    compatible edges.
-    """
+    """Convert a Numpy connectivity matrix into a list of NetworkX compatible edges."""
     if indices is None:
         indices = np.arange(connectivity.shape[0], dtype=int)
 
     edges = []
     for i, c in enumerate(connectivity):
-        lower_diagonal = c[:i + 1]
+        lower_diagonal = c[: i + 1]
 
         for j, v in enumerate(lower_diagonal):
             edges += [(indices[i], indices[j], 1)] * int(v)
     return edges
 
 
 def isomorphic_molecules(graph0, graph1):
     """Check whether two molecule graphs are isomorphic."""
-    em = nx.algorithms.isomorphism.numerical_edge_match('bonds', 1)
-    nm = nx.algorithms.isomorphism.numerical_node_match('number', 1)
+    em = nx.algorithms.isomorphism.numerical_edge_match("bonds", 1)
+    nm = nx.algorithms.isomorphism.numerical_node_match("number", 1)
 
     isomorphic = nx.is_isomorphic(graph0, graph1, edge_match=em, node_match=nm)
 
     return isomorphic
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/utilities.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from HTMACat.catkit import Gratoms
 import numpy as np
 import ase
 import re
+
 try:
     from math import gcd
 except ImportError:
     from fractions import gcd
 
 
 def running_mean(array, N=5):
@@ -36,15 +37,15 @@
 def to_gratoms(atoms, edges=None):
     """Convert and atom object to a gratoms object."""
     gratoms = Gratoms(
         numbers=atoms.numbers,
         positions=atoms.positions,
         pbc=atoms.pbc,
         cell=atoms.cell,
-        edges=edges
+        edges=edges,
     )
 
     if atoms.constraints:
         gratoms.set_constraint(atoms.constraints)
 
     return gratoms
 
@@ -62,28 +63,27 @@
     Returns
     -------
     numbers : ndarray (n,)
         Element numbers in associated species.
     counts : ndarray (n,)
         Count of each element in a species.
     """
-    parse = re.findall('[A-Z][a-z]?|[0-9]+', formula)
+    parse = re.findall("[A-Z][a-z]?|[0-9]+", formula)
 
     values = {}
     for i, e in enumerate(parse):
         if e.isdigit():
             values[parse[i - 1]] += int(e) - 1
         else:
             if e not in values:
                 values[e] = 1
             else:
                 values[e] += 1
 
-    numbers = np.array([
-        ase.data.chemical_symbols.index(k) for k in values.keys()])
+    numbers = np.array([ase.data.chemical_symbols.index(k) for k in values.keys()])
     srt = np.argsort(numbers)
     numbers = numbers[srt]
 
     if return_count:
         counts = np.array([v for v in values.values()])[srt]
 
         return numbers, counts
@@ -147,17 +147,16 @@
 
     elif isinstance(slice_name, str):
         if slice_name.isdigit():
             i = int(slice_name)
             _slice = slice(i, i + 1)
 
         else:
-            split = slice_name.split(':')
-            split = [int(_) if _.lstrip('-').isdigit()
-                     else None for _ in split]
+            split = slice_name.split(":")
+            split = [int(_) if _.lstrip("-").isdigit() else None for _ in split]
             _slice = slice(*split)
 
     return _slice
 
 
 def ext_gcd(a, b):
     """Extension of greatest common divisor."""
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gen/utils/vectors.py` & `HTMACat-1.0.5/HTMACat/catkit/gen/utils/vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
     vec /= -np.linalg.norm(vec)
 
     return vec
 
 
 def get_basis_vectors(coordinates):
-    """Return a set of basis vectors for a given array of
-    3D coordinates.
+    """Return a set of basis vectors for a given array of 3D coordinates.
 
     Parameters
     ----------
     coordinates : array_like (3, 3) | (2, 3)
         Cartesian coordinates to determine the basis of. If
         only 2 positions are given 3rd is chosen as the positive
         y-axis.
@@ -57,11 +56,10 @@
         c2 = np.array([0, 1, 0])
 
     basis1 = c0 - c1
     basis2 = np.cross(basis1, c0 - c2)
     basis3 = np.cross(basis1, basis2)
 
     basis_vectors = np.vstack([basis1, basis2, basis3])
-    basis_vectors /= np.linalg.norm(
-        basis_vectors, axis=1, keepdims=True)
+    basis_vectors /= np.linalg.norm(basis_vectors, axis=1, keepdims=True)
 
     return basis_vectors
```

### Comparing `HTMACat-1.0.4/HTMACat/catkit/gratoms.py` & `HTMACat-1.0.5/HTMACat/catkit/gratoms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,78 @@
 import networkx as nx
 import numpy as np
 import ase
 import copy
 import warnings
+
 try:
     from builtins import super
-except(ImportError):
+except ImportError:
     from __builtin__ import super
 
 sym = np.array(ase.data.chemical_symbols)
-em = nx.algorithms.isomorphism.numerical_edge_match('bonds', 1)
-nm = nx.algorithms.isomorphism.numerical_node_match('number', 1)
+em = nx.algorithms.isomorphism.numerical_edge_match("bonds", 1)
+nm = nx.algorithms.isomorphism.numerical_node_match("number", 1)
 
 
 class Gratoms(ase.Atoms):
     """Graph based atoms object.
 
-    An Integrated class for an ASE atoms object with a corresponding
-    Networkx Graph.
+    An Integrated class for an ASE atoms object with a corresponding Networkx Graph.
     """
 
-    def __init__(self,
-                 symbols=None,
-                 positions=None,
-                 numbers=None,
-                 tags=None,
-                 momenta=None,
-                 masses=None,
-                 magmoms=None,
-                 charges=None,
-                 scaled_positions=None,
-                 cell=None,
-                 pbc=None,
-                 celldisp=None,
-                 constraint=None,
-                 calculator=None,
-                 info=None,
-                 edges=None):
+    def __init__(
+        self,
+        symbols=None,
+        positions=None,
+        numbers=None,
+        tags=None,
+        momenta=None,
+        masses=None,
+        magmoms=None,
+        charges=None,
+        scaled_positions=None,
+        cell=None,
+        pbc=None,
+        celldisp=None,
+        constraint=None,
+        calculator=None,
+        info=None,
+        edges=None,
+    ):
         super().__init__(
-            symbols, positions, numbers, tags, momenta,
-            masses, magmoms, charges, scaled_positions, cell,
-            pbc, celldisp, constraint, calculator, info)
+            symbols,
+            positions,
+            numbers,
+            tags,
+            momenta,
+            masses,
+            magmoms,
+            charges,
+            scaled_positions,
+            cell,
+            pbc,
+            celldisp,
+            constraint,
+            calculator,
+            info,
+        )
 
         if isinstance(edges, np.ndarray):
             if self.pbc.any():
                 self._graph = nx.MultiGraph(edges)
             else:
                 self._graph = nx.Graph(edges)
         else:
             if self.pbc.any():
                 self._graph = nx.MultiGraph()
             else:
                 self._graph = nx.Graph()
 
-        nodes = [[i, {'number': n}]
-                 for i, n in enumerate(self.arrays['numbers'])]
+        nodes = [[i, {"number": n}] for i, n in enumerate(self.arrays["numbers"])]
         self._graph.add_nodes_from(nodes)
 
         if isinstance(edges, list):
             self._graph.add_edges_from(edges)
 
     @property
     def graph(self):
@@ -85,63 +99,59 @@
     def connectivity(self):
         connectivity = nx.to_numpy_matrix(self._graph)
         connectivity = np.array(connectivity, dtype=int)
         return connectivity
 
     def get_surface_atoms(self):
         """Return surface atoms."""
-        surf_atoms = np.where(self.get_array('surface_atoms') > 0)[0]
+        surf_atoms = np.where(self.get_array("surface_atoms") > 0)[0]
         return surf_atoms
 
     def set_surface_atoms(self, top, bottom=None):
         """Assign surface atoms."""
         n = np.zeros(len(self))
         if bottom is not None:
             n[bottom] = -1
         # Overwrites bottom indexing
         n[top] = 1
-        self.set_array('surface_atoms', n)
+        self.set_array("surface_atoms", n)
 
     def get_neighbor_symbols(self, u):
         """Get chemical symbols for neighboring atoms of u."""
         neighbors = list(self._graph[u])
 
-        return sym[self.arrays['numbers'][neighbors]]
+        return sym[self.arrays["numbers"][neighbors]]
 
     def is_isomorph(self, other):
         """Check if isomorphic by bond count and atomic number."""
-        isomorphic = nx.is_isomorphic(
-            self._graph, other._graph, edge_match=em, node_match=nm)
+        isomorphic = nx.is_isomorphic(self._graph, other._graph, edge_match=em, node_match=nm)
 
         return isomorphic
 
     def get_chemical_tags(self, rank=2):
-        """Generate a hash descriptive of the chemical formula (rank 0)
-        or include bonding (rank 1).
-        """
-        cnt = np.bincount(self.arrays['numbers'])
-        composition = ','.join(cnt.astype(str))
+        """Generate a hash descriptive of the chemical formula (rank 0) or include bonding (rank
+        1)."""
+        cnt = np.bincount(self.arrays["numbers"])
+        composition = ",".join(cnt.astype(str))
 
         if rank == 1:
             return composition[2:]
 
         for adj in self.adj.items():
-
-            num = self.arrays['numbers'][list(adj[1].keys())]
+            num = self.arrays["numbers"][list(adj[1].keys())]
             cnt += np.bincount(num, minlength=len(cnt))
 
-        bonding = ','.join(cnt.astype(str))
+        bonding = ",".join(cnt.astype(str))
 
         return composition[2:], bonding[2:]
 
     def get_unsaturated_nodes(self, screen=None):
-
         unsaturated = []
         for node, data in self.nodes(data=True):
-            radicals = data['valence']
+            radicals = data["valence"]
 
             if screen in data:
                 continue
 
             if radicals > 0:
                 unsaturated += [node]
 
@@ -151,15 +161,15 @@
         """Return a copy."""
         atoms = self.__class__(cell=self.cell, pbc=self.pbc, info=self.info)
 
         atoms.arrays = {}
         for name, a in self.arrays.items():
             atoms.arrays[name] = a.copy()
         atoms.constraints = copy.deepcopy(self.constraints)
-        if hasattr(self, '_graph'):
+        if hasattr(self, "_graph"):
             atoms._graph = self._graph.copy()
 
         return atoms
 
     def __getitem__(self, i):
         """Return a subset of the atoms.
 
@@ -172,15 +182,15 @@
         indices of the constraints will be shuffled so that they match
         the indexing in the subset returned.
         """
 
         if isinstance(i, (int, np.int64)):
             natoms = len(self)
             if i < -natoms or i >= natoms:
-                raise IndexError('Index out of range.')
+                raise IndexError("Index out of range.")
 
             return ase.Atom(atoms=self, index=i)
         elif isinstance(i, list) and len(i) > 0:
             # Make sure a list of booleans will work correctly and not be
             # interpreted at 0 and 1 indices.
             i = np.array(i)
         elif isinstance(i, slice):
@@ -199,34 +209,32 @@
                 istop = i.stop
 
             istep = i.step if i.step is not None else 1
             i = np.array([i for i in range(istart, istop, istep)])
         conadd = []
         # Constraints need to be deepcopied, but only the relevant ones.
         for con in copy.deepcopy(self.constraints):
-            if isinstance(con, (
-                    ase.constraints.FixConstraint,
-                    ase.constraints.FixBondLengths)):
+            if isinstance(con, (ase.constraints.FixConstraint, ase.constraints.FixBondLengths)):
                 try:
                     con.index_shuffle(self, i)
                     conadd.append(con)
                 except IndexError:
                     pass
 
-        atoms = self.__class__(cell=self.cell, pbc=self.pbc, info=self.info,
-                               celldisp=self._celldisp)
+        atoms = self.__class__(
+            cell=self.cell, pbc=self.pbc, info=self.info, celldisp=self._celldisp
+        )
 
         atoms.arrays = {}
         for name, a in self.arrays.items():
             atoms.arrays[name] = a[i].copy()
 
         # Copy the graph, conserving correct indexing
         if self.nodes:
-            nodes = [[_, {'number': n}]
-                     for _, n in enumerate(self.arrays['numbers'])]
+            nodes = [[_, {"number": n}] for _, n in enumerate(self.arrays["numbers"])]
             atoms.graph.add_nodes_from(nodes)
 
             j = i.tolist()
             for u, v in self.graph.edges():
                 if u not in i or v not in i:
                     continue
                 atoms.graph.add_edge(j.index(u), j.index(v))
@@ -239,51 +247,52 @@
         if isinstance(other, ase.Atom):
             other = self.__class__([other])
 
         n1 = len(self)
         n2 = len(other)
 
         for name, a1 in self.arrays.items():
-            a = np.zeros((n1 + n2, ) + a1.shape[1:], a1.dtype)
+            a = np.zeros((n1 + n2,) + a1.shape[1:], a1.dtype)
             a[:n1] = a1
-            if name == 'masses':
+            if name == "masses":
                 a2 = other.get_masses()
             else:
                 a2 = other.arrays.get(name)
             if a2 is not None:
                 a[n1:] = a2
             self.arrays[name] = a
 
         for name, a2 in other.arrays.items():
             if name in self.arrays:
                 continue
-            a = np.empty((n1 + n2, ) + a2.shape[1:], a2.dtype)
+            a = np.empty((n1 + n2,) + a2.shape[1:], a2.dtype)
             a[n1:] = a2
-            if name == 'masses':
+            if name == "masses":
                 a[:n1] = self.get_masses()[:n1]
             else:
                 a[:n1] = 0
 
             self.set_array(name, a)
 
         if isinstance(other, Gratoms):
-            if isinstance(self._graph, nx.MultiGraph) & \
-               isinstance(other._graph, nx.Graph):
+            if isinstance(self._graph, nx.MultiGraph) & isinstance(other._graph, nx.Graph):
                 other._graph = nx.MultiGraph(other._graph)
 
             self._graph = nx.disjoint_union(self._graph, other._graph)
 
         return self
 
     def __delitem__(self, i):
         from ase.constraints import FixAtoms
+
         for c in self._constraints:
             if not isinstance(c, FixAtoms):
-                raise RuntimeError('Remove constraint using set_constraint() '
-                                   'before deleting atoms.')
+                raise RuntimeError(
+                    "Remove constraint using set_constraint() " "before deleting atoms."
+                )
 
         if isinstance(i, (list, int)):
             # Make sure a list of booleans will work correctly and not be
             # interpreted at 0 and 1 indices.
             i = np.atleast_1d(i)
 
         n = len(self)
@@ -313,25 +322,24 @@
     def __imul__(self, m):
         """In-place repeat of atoms."""
         if isinstance(m, int):
             m = (m, m, m)
 
         for x, vec in zip(m, self.cell):
             if x != 1 and not vec.any():
-                raise ValueError(
-                    'Cannot repeat along undefined lattice vector')
+                raise ValueError("Cannot repeat along undefined lattice vector")
 
         M = np.product(m)
         n = len(self)
 
         for name, a in self.arrays.items():
-            self.arrays[name] = np.tile(a, (M, ) + (1, ) * (len(a.shape) - 1))
+            self.arrays[name] = np.tile(a, (M,) + (1,) * (len(a.shape) - 1))
             cgraph = self._graph.copy()
 
-        positions = self.arrays['positions']
+        positions = self.arrays["positions"]
         i0 = 0
 
         for m0 in range(m[0]):
             for m1 in range(m[1]):
                 for m2 in range(m[2]):
                     i1 = i0 + n
                     positions[i0:i1] += np.dot((m0, m1, m2), self.cell)
```

### Comparing `HTMACat-1.0.4/HTMACat/command.py` & `HTMACat-1.0.5/HTMACat/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 import os
 from HTMACat.model.Construct_adsorption_yaml import *
 from HTMACat.IO import print_templator, out_templator_file
+from HTMACat.__version__ import __title__, __version__
 from pathlib import *
 import shutil
 import typer
 from rich import print
 
 htmat = typer.Typer(add_completion=False)
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def main():
     htmat()
 
 
-@htmat.callback(invoke_without_command=True,
-                no_args_is_help=True,
-                epilog="""+--------------------------------------------------------------------------------------------------------+\n
+@htmat.callback(
+    invoke_without_command=True,
+    no_args_is_help=True,
+    epilog=f"""+--------------------------------------------------------------------------------------------------------+\n
 |                                           HTMACat-Kit                                                  |\n
-|                                          Version: 1.0.4                                                |\n
+|                                          Version: {__version__}                                                |\n
 |    A high-throughput modeling, calculation, and analysis framework for catalytic reaction processes.   |\n
 |              More information, please visit https://stanfordbshan.github.io/HTMACat-kit/.              |\n
 +--------------------------------------------------------------------------------------------------------+""",
-                context_settings=CONTEXT_SETTINGS)
+    context_settings=CONTEXT_SETTINGS,
+)
 def main_command():
     pass
 
 
 @htmat.command(context_settings=CONTEXT_SETTINGS)
-def ads(in_dir: str = typer.Option('./',
-                                   '-i',
-                                   '--inputdir',
-                                   help="relative directory of input file"),
-        out_dir: str = typer.Option('./',
-                                    '-o',
-                                    '--outputdir',
-                                    help="relative directory of output file")):
-    """
-    Construct adsorption configuration
-    """
+def ads(
+    in_dir: str = typer.Option("./", "-i", "--inputdir", help="relative directory of input file"),
+    out_dir: str = typer.Option(
+        "./", "-o", "--outputdir", help="relative directory of output file"
+    ),
+):
+    """Construct adsorption configuration."""
     print("Construct adsorption configuration ... ...")
     wordir = Path(in_dir).resolve()
     outdir = Path(out_dir).resolve()
-    StrucInfo = 'config.yaml'
+    StrucInfo = "config.yaml"
     if not outdir == wordir:
         outdir.mkdir(parents=True, exist_ok=True)
         shutil.copy(wordir / StrucInfo, outdir)
         os.chdir(outdir)
     Construct_adsorption_yaml(StrucInfo)
 
 
 @htmat.command(context_settings=CONTEXT_SETTINGS)
 def templator():
-    """
-    Print out input templator
-    """
+    """Print out input templator."""
     print_templator()
     out_templator_file()
```

### Comparing `HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor.py` & `HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 from HTMACat.configuration import base_info
 
 
-def Construct_descriptor(poscar, feature_surf, feature_ads, feature_site, adspecies, facet='100'):
-    """
-    Construct a descriptor for a given catalytic system based on its geometry and adsorption properties.
+def Construct_descriptor(poscar, feature_surf, feature_ads, feature_site, adspecies, facet="100"):
+    """Construct a descriptor for a given catalytic system based on its geometry and adsorption
+    properties.
 
     Parameters
     ----------
     poscar : str
         The POSCAR file path of the catalyst-adsorbate system.
     feature_surf : list
         A list of strings specifying the features to extract from the surface of the catalytic system. Possible options
@@ -34,183 +33,191 @@
         electron of adsorbate molecule, mean valence electron of binding site atoms, mean atomic radius of binding site atoms,
         and binding type of binding site ('top', 'bridge', 'fcc', 'hcp', or '4-fold').
     """
     descriptor = []
     descriptor_surf = []
     ### the features of catalyst surface : surfce valence electron,surface atomic radius,
     ### surf+subsurf mean valence electron,surf+subsurf mean atomic radius
-    #surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
-    #subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(surfatoms_symb)
+    # surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
+    # subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05)
+    # print(surfatoms_symb)
     ## If NO, The symmetry of surface atoms could be broken
-    if get_symmetry_surfatoms(poscar, tol=0.3) == 'NO':
+    if get_symmetry_surfatoms(poscar, tol=0.3) == "NO":
         print(f"The symmetry of surface atoms of {poscar} could not be keeped!")
-        #return descriptor
+        # return descriptor
     else:
         feature_value_surf = Construct_descriptor_info(base_info, surfatoms_symb, feature_surf)
-        feature_value_subsurf = Construct_descriptor_info(base_info, subsurfatoms_symb,
-                                                          feature_surf)
-        #print(feature_value_surf)
+        feature_value_subsurf = Construct_descriptor_info(
+            base_info, subsurfatoms_symb, feature_surf
+        )
+        # print(feature_value_surf)
         m0, n0 = np.array(feature_value_surf).shape
         m1, n1 = np.array(feature_value_subsurf).shape
-        #print(m0,m1)
+        # print(m0,m1)
         ## Ignore structures without standard or integrated surface configuration
         ## if m0 not equal to m1 menas that the large surface reconstruction occurs and causes the broken of surface.
         if (feature_value_surf != []) and (m0 == m1):
-            #print(feature_value_surf,feature_value_subsurf)
+            # print(feature_value_surf,feature_value_subsurf)
             feature_value = np.hstack((feature_value_surf, feature_value_subsurf))
-            #print(feature_value)
+            # print(feature_value)
             descriptor_surf_tmp = np.around(np.mean(feature_value, 0), 2)
-            facet_coord = {'100': 8, '111': 9}
+            facet_coord = {"100": 8, "111": 9}
             descriptor_surf = np.hstack((descriptor_surf_tmp, [facet_coord.get(facet)]))
             ### the feature of adspecies and binding sites
-            bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-                poscar)
-            #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
-            #print(adspecie,bind_type_symb,bind_surfatoms_symb)
-            #print(bind_type_symb[0])
+            (
+                bind_adatoms,
+                bind_adatoms_symb,
+                adspecie,
+                bind_type_symb,
+                bind_surfatoms,
+                bind_surfatoms_symb,
+            ) = get_binding_adatom(poscar)
+            # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+            # print(adspecie,bind_type_symb,bind_surfatoms_symb)
+            # print(bind_type_symb[0])
             if adspecie == []:
                 print(f"The molecule can not adsorb in the {poscar}!")
             elif len(adspecie) > 1:
                 print(f"More than 1 adspecie are found in {poscar}!")
             elif set(adspecie).intersection(set(adspecies)):
                 ## construct the descriptor of adsorbate: mean enegativity, mean valence_electron
-                #print(adspecie)
+                # print(adspecie)
                 descriptor_ads = []
-                #print(adspecie)
+                # print(adspecie)
                 ads = molecule(adspecie[0])
-                #print(ads)
+                # print(ads)
                 ads_symb = ads.get_chemical_symbols()
                 feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
                 descriptor_ads = np.around(np.mean(feature_value_ads, 0), 2)
-                #print(descriptor_ads)
+                # print(descriptor_ads)
 
                 ## construct the descriptor of site: mean valence electron, mean atomic radius, bind type
                 descriptor_site = []
-                typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
-                typ2 = {None: 0, 'top': 0, 'bri': 0, 'fcc': 0, 'hcp': 1, '4-fold': 0}
+                typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
+                typ2 = {None: 0, "top": 0, "bri": 0, "fcc": 0, "hcp": 1, "4-fold": 0}
                 site_type = np.hstack((typ.get(bind_type_symb[0]), typ2.get(bind_type_symb[0])))
-                feature_value_site = Construct_descriptor_info(base_info, bind_surfatoms_symb[0],
-                                                               feature_site)
+                feature_value_site = Construct_descriptor_info(
+                    base_info, bind_surfatoms_symb[0], feature_site
+                )
                 descriptor_site_tmp = np.around(np.mean(feature_value_site, 0), 2)
                 descriptor_site = np.append(descriptor_site_tmp, site_type)
-                #print(descriptor_site)
+                # print(descriptor_site)
 
                 descriptor = np.hstack((descriptor_surf, descriptor_ads, descriptor_site))
-                #print(descriptor)
+                # print(descriptor)
                 return descriptor
             else:
                 print(adspecie)
                 print(f"{poscar} can not be identified!")
         else:
-            print(f'Surface info of {poscar} can not be obtained ')
+            print(f"Surface info of {poscar} can not be obtained ")
 
 
 from HTMACat.Extract_info import *
 from HTMACat.descriptor.Construct_descriptor import *
 from HTMACat.Base_tools import *
 import os
 import numpy as np
 import operator
-if __name__ == '__main__':
-    feature_surf = ['Valence_electron', 'Atomic_radius']
-    #feature_ads=['Enegativity','Valence_electron']
-    feature_ads = ['Valence_electron', 'Atomic_radius']
-    feature_site = ['Valence_electron', 'Atomic_radius']
-    adspecies = ['NH3', 'NH2', 'NH', 'N', 'O', 'OH', 'H']
-    dop_typ_all = ['1', '2', '3', '4', '1L']
-    facet = '111'
+
+if __name__ == "__main__":
+    feature_surf = ["Valence_electron", "Atomic_radius"]
+    # feature_ads=['Enegativity','Valence_electron']
+    feature_ads = ["Valence_electron", "Atomic_radius"]
+    feature_site = ["Valence_electron", "Atomic_radius"]
+    adspecies = ["NH3", "NH2", "NH", "N", "O", "OH", "H"]
+    dop_typ_all = ["1", "2", "3", "4", "1L"]
+    facet = "111"
     print("----------------------------------------")
     print("Construct descriptor starts:")
     print("1st step: Get the whole 'Descriptor+Ead'")
-    EnerInfo = open('adsE_radical_all', 'r+')
-    file_des = open('descriptor', 'w+')
-    file_all = open('descriptor-all', 'w+')
-    file_log = open('descriptor-log', 'w+')
+    EnerInfo = open("adsE_radical_all", "r+")
+    file_des = open("descriptor", "w+")
+    file_all = open("descriptor-all", "w+")
+    file_log = open("descriptor-log", "w+")
     des, des_all, des_tmp = [], [], []
     for i, Ener in enumerate(EnerInfo):
-        sys = Ener.split(',')[0]
-        ene = Ener.split(',')[-1].strip()
-        sys_all = sys.split('_')
+        sys = Ener.split(",")[0]
+        ene = Ener.split(",")[-1].strip()
+        sys_all = sys.split("_")
         dop_typ = sys_all[-3]
         specie = set(sys_all).intersection(set(adspecies))
         if specie:
             if dop_typ in dop_typ_all:
-                #poscar= f'./{sys}/optmk/CONTCAR'
-                poscar = f'./{sys}/CONTCAR'
+                # poscar= f'./{sys}/optmk/CONTCAR'
+                poscar = f"./{sys}/CONTCAR"
                 print(sys)
-                descriptor = Construct_descriptor(poscar,
-                                                  feature_surf,
-                                                  feature_ads,
-                                                  feature_site,
-                                                  adspecies,
-                                                  facet=facet)
-                #print(descriptor)
+                descriptor = Construct_descriptor(
+                    poscar, feature_surf, feature_ads, feature_site, adspecies, facet=facet
+                )
+                # print(descriptor)
                 if descriptor is None:
-                    tmp = np.hstack(([sys], ['None'], [ene]))
+                    tmp = np.hstack(([sys], ["None"], [ene]))
                     for d in tmp:
                         if d == tmp[-1]:
-                            file_all.write('%s\n' % d)
+                            file_all.write("%s\n" % d)
                         else:
-                            file_all.write('%s\t' % d)
+                            file_all.write("%s\t" % d)
 
                 else:
                     tmp = np.hstack(([sys], descriptor, [ene]))
                     for d in tmp:
                         if d == tmp[-1]:
-                            file_all.write('%s\n' % d)
+                            file_all.write("%s\n" % d)
                         else:
-                            file_all.write('%s\t' % d)
-                    #file_all.writelines('%s\n' %tmp)
+                            file_all.write("%s\t" % d)
+                    # file_all.writelines('%s\n' %tmp)
                     des_tmp += [np.hstack(([sys], descriptor, [ene]))]
     print("2nd: Extrate the repeated values")
     ###Substrate the repeated items according to the feature list
     m, n = np.array(des_tmp).shape
     # Extrate the feature value
     des_feature = [des_tmp[j][1:-1] for j in range(m)]
     # The feaure list after substrate the repeat
-    des_feature_tmp = np.array(list(set([tuple(t) for t in des_feature])))
+    des_feature_tmp = np.array(list({tuple(t) for t in des_feature}))
     k, l = des_feature_tmp.shape
     # The threshold value Ecut of Ead: if Ead > Ecut, ignore it
     Ecut = 0.25
     print(m, k)
     # Output the feature and energy
     if m > k:
         print("Subtrate Repeat Values Starts:")
         for i, d1 in enumerate(des_feature_tmp):
             for j, d2 in enumerate(des_tmp):
                 if all(d1 == d2[1:-1]):
                     tmp = np.hstack((d1, d2[-1]))
-                    tmp2 = np.hstack((d1, [d2[0].split('_')[0]]))
+                    tmp2 = np.hstack((d1, [d2[0].split("_")[0]]))
                     ## output
                     if float(tmp[-1]) < float(Ecut):
                         # output des+ene
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_des.write('%s\n' % d)
+                                file_des.write("%s\n" % d)
                             else:
-                                file_des.write('%s\t' % d)
+                                file_des.write("%s\t" % d)
                         # output des+type: des+'Au'
                         for d in tmp2:
                             if d == tmp2[-1]:
-                                file_log.write('%s\n' % d)
+                                file_log.write("%s\n" % d)
                             else:
-                                file_log.write('%s\t' % d)
+                                file_log.write("%s\t" % d)
                     else:
-                        print(f'Ignore the value {tmp[-1]} >= {Ecut}')
+                        print(f"Ignore the value {tmp[-1]} >= {Ecut}")
 
                     break
                 else:
                     continue
     else:
-        print('No Repeated Value')
+        print("No Repeated Value")
     file_all.close()
     file_des.close()
     print("Subtrate Repeat Values End !")
-    '''
-   print('---------Raw data---------')
-   os.system('cat descriptor-all')
-   print('---------Final data---------')
-   os.system('cat descriptor')
-   '''
+    """print('---------Raw data---------') os.system('cat descriptor-all') print('---------Final
+    data---------') os.system('cat descriptor')"""
```

### Comparing `HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_NEB.py` & `HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_NEB.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 import os
 import numpy as np
 
 
 ### To get the file names of elememtary reaction steps
 def get_file_name(reaction):
-    """
-    This function constructs the file name for a given reaction.
+    """This function constructs the file name for a given reaction.
 
     Parameters
     ----------
     reaction : str
         The string representing the reaction, in the format "reactants = products".
 
     Returns
@@ -19,45 +17,44 @@
     str
         The file name constructed based on the reaction, in the format "reactant1+reactant2+...=product1+product2+...".
 
     Examples
     --------
     >>> get_file_name("2H2 + O2 = 2H2O")
     >>> '2H2+O2=2H2O'
-"""
-    specie_f = reaction.split('=')[0].strip()
-    specie_b = reaction.split('=')[1].strip()
+    """
+    specie_f = reaction.split("=")[0].strip()
+    specie_b = reaction.split("=")[1].strip()
     ### Construct the reaction name
     ##1.Extract the reactant molecule and type (a g s)
     specie_f_list = []
-    for i in range(len(specie_f.split('+'))):
-        specie_f_list += [specie_f.split('+')[i].strip()]
+    for i in range(len(specie_f.split("+"))):
+        specie_f_list += [specie_f.split("+")[i].strip()]
     specie_f_mol = []
     specie_f_typ = []
     for j, specie in enumeratemak(specie_f_list):
-        specie_f_mol += [specie.split('(', 1)[0].strip()]
-        specie_f_typ += [specie.split('(', 1)[1].split(')')[0].strip()]
+        specie_f_mol += [specie.split("(", 1)[0].strip()]
+        specie_f_typ += [specie.split("(", 1)[1].split(")")[0].strip()]
     ##2.Extract the product molecule and type (a g s)
     specie_b_list = []
-    for i in range(len(specie_b.split('+'))):
-        specie_b_list += [specie_b.split('+')[i].strip()]
+    for i in range(len(specie_b.split("+"))):
+        specie_b_list += [specie_b.split("+")[i].strip()]
     specie_b_mol = []
     specie_b_typ = []
     for j, specie in enumerate(specie_b_list):
-        specie_b_mol += [specie.split('(', 1)[0].strip()]
-        specie_b_typ += specie.split('(', 1)[1].split(')')[0].strip()
+        specie_b_mol += [specie.split("(", 1)[0].strip()]
+        specie_b_typ += specie.split("(", 1)[1].split(")")[0].strip()
     ##3.construct the file name for every reaction
-    File = '+'.join(specie_f_mol) + '=' + '+'.join(specie_b_mol)
+    File = "+".join(specie_f_mol) + "=" + "+".join(specie_b_mol)
     return File
 
 
 ### To get info of catalytic surface
 def get_surface_info(poscar, feature_surf, base_info):
-    """
-    Extract surface information from a given POSCAR file.
+    """Extract surface information from a given POSCAR file.
 
     Parameters
     ----------
     poscar : str
         The path to the POSCAR file.
     feature_surf : list
         A list of features to be extracted from the surface. Each feature is a string, and can be one of the following:
@@ -67,37 +64,41 @@
         The path to the file containing the base information about the atoms.
 
     Returns
     ---------
     descriptor_surf : list
         A list of the surface descriptors. The order of the descriptors is the same as the order of the features provided.
         If the structure does not have a standard or integrated surface configuration, an empty list is returned.
-
     """
     ### Extract the surface info
     descriptor_surf = []
-    #base_info='/data3/home/jqyang/high-throughput/script/construction/base-function/codes/Info/Element_Info'
-    #feature_surf=['Valence_electron','Atomic_radius']
-    #feature_surf=['Atomic_radius']
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(surfatoms_symb)
+    # base_info='/data3/home/jqyang/high-throughput/script/construction/base-function/codes/Info/Element_Info'
+    # feature_surf=['Valence_electron','Atomic_radius']
+    # feature_surf=['Atomic_radius']
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05)
+    # print(surfatoms_symb)
     feature_value_surf = Construct_descriptor_info(base_info, surfatoms_symb, feature_surf)
     ## Ignore structures without standard or integrated surface configuration
     if feature_value_surf != []:
         descriptor_surf = np.around(np.mean(feature_value_surf, 0), 2)
-    #print(descriptor_surf)
+    # print(descriptor_surf)
 
     return descriptor_surf
 
 
 ### Extract the site info
 def get_site_info(poscar):
-    """
-    This function extracts site information from a given POSCAR file.
+    """This function extracts site information from a given POSCAR file.
 
     Parameters
     ----------
         poscar (str): The name of the POSCAR file.
 
     Returns
     -------
@@ -106,30 +107,35 @@
     Notes
     -----
     The function extracts the binding adatoms, adspecie, binding type symbols, and binding surface atoms from the POSCAR file.
     The function then assigns numerical values to the binding types based on the following dictionary: {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}.
     The function then adds up the numerical values for each binding type symbol and returns a list of the resulting descriptor.
     """
     descriptor_site = []
-    bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-        poscar)
-    typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
+    (
+        bind_adatoms,
+        bind_adatoms_symb,
+        adspecie,
+        bind_type_symb,
+        bind_surfatoms,
+        bind_surfatoms_symb,
+    ) = get_binding_adatom(poscar)
+    typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
     print(bind_type_symb)
     tmp = 0
     for i in bind_type_symb:
         tmp += int(typ.get(i))
     print(tmp)
     descriptor_site = [tmp]
     return descriptor_site
 
 
 ### Extract the adsorbate info
 def get_adsorbate_info(poscar, feature_ads, base_info):
-    """
-    Extract the adsorbate information from the POSCAR file.
+    """Extract the adsorbate information from the POSCAR file.
 
     Parameters
     ----------
     poscar : str
         The path of the POSCAR file.
     feature_ads : list
         A list of descriptors to calculate for the adsorbate.
@@ -138,164 +144,170 @@
 
     Returns
     -------
         descriptor_ads : list
             A list of the calculated descriptors for the adsorbate.
     """
     ### Extract adsorbate info
-    bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-        poscar)
+    (
+        bind_adatoms,
+        bind_adatoms_symb,
+        adspecie,
+        bind_type_symb,
+        bind_surfatoms,
+        bind_surfatoms_symb,
+    ) = get_binding_adatom(poscar)
     descriptor_ads, descriptor_ads_tmp = [], []
     for i, specie in enumerate(adspecie):
         ads = molecule(specie)
         ads_symb = ads.get_chemical_symbols()
-        #print(ads_symb)
+        # print(ads_symb)
         feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
-        #print(feature_value_ads)
+        # print(feature_value_ads)
         descriptor_ads_tmp += [np.around(np.mean(feature_value_ads, 0), 2)]
     if len(adspecie) == 2:
         descriptor_ads = np.hstack((descriptor_ads_tmp[0], descriptor_ads_tmp[1]))
     else:
         descriptor_ads = np.hstack((descriptor_ads_tmp[0], [0, 0]))
     return descriptor_ads
 
 
-def get_reaction_info(react='react.log', File_adsE='adsE_coad_radical'):
-    """
-    Extract the information of a chemical reaction, including reaction type, reactant info, product info, barrier and 
-    enthalpy. Extract the reactant and product adsorption energy from a file named adsE_coad_radical in the current 
-    directory.
+def get_reaction_info(react="react.log", File_adsE="adsE_coad_radical"):
+    """Extract the information of a chemical reaction, including reaction type, reactant info,
+    product info, barrier and enthalpy. Extract the reactant and product adsorption energy from a
+    file named adsE_coad_radical in the current directory.
 
     Parameters
     ----------
     react : str, optional
         The name of the reaction file, by default 'react.log'.
     File_adsE : str, optional
         The name of the adsorption energy file, by default 'adsE_coad_radical'.
 
     Returns
     -------
     tuple of np.ndarray or None
-        A tuple of descriptor reaction array and reaction barrier. If the NEB of the given file is not calculated, return 
+        A tuple of descriptor reaction array and reaction barrier. If the NEB of the given file is not calculated, return
         None for both values.
-        
+
     Example
     -------
     >>> descriptor_reaction, barrier = get_reaction_info('react.log', 'adsE_coad_radical')
     """
     ### Extract reaction info
     ##1.Extract reaction type,reactant info,product info,barrier & enthalpy
-    react_info = open(react, 'r+')
+    react_info = open(react, "r+")
     reaction_info = react_info.readlines()
     if len(reaction_info) > 2:
         reaction_type = reaction_info[0]
-        reactant_info = reaction_info[1].split(',')[0].split('=')[0]
-        product_info = reaction_info[1].split(',')[1].split('=')[0]
-        #print(reactant_info,product_info)
-        barrier = reaction_info[-3].split(':')[-1].strip()
-        enthalpy = reaction_info[-2].split(':')[-1].strip()
-        #print(barrier,enthalpy)
+        reactant_info = reaction_info[1].split(",")[0].split("=")[0]
+        product_info = reaction_info[1].split(",")[1].split("=")[0]
+        # print(reactant_info,product_info)
+        barrier = reaction_info[-3].split(":")[-1].strip()
+        enthalpy = reaction_info[-2].split(":")[-1].strip()
+        # print(barrier,enthalpy)
         react_info.close()
 
         ##2.extract the reactant and product adsorbed energy
         Ead_reactant, Ead_product = 0, 0
-        #Ead_info=open('../../surface-adsorption/adsE_coad_atom','r+')
-        Ead_info = open(f'../../surface-adsorption/{File_adsE}', 'r+')
+        # Ead_info=open('../../surface-adsorption/adsE_coad_atom','r+')
+        Ead_info = open(f"../../surface-adsorption/{File_adsE}", "r+")
         for k, sys in enumerate(Ead_info):
-            sys_name = sys.split(',')[0]
-            sys_ener = sys.split(',')[1].strip()
+            sys_name = sys.split(",")[0]
+            sys_ener = sys.split(",")[1].strip()
             if sys_name == reactant_info:
                 Ead_reactant = sys_ener
             elif sys_name == product_info:
                 Ead_product = sys_ener
             else:
                 continue
-        #print(Ead_reactant,Ead_product)
+        # print(Ead_reactant,Ead_product)
         Ead_info.close()
         ##Descriptor of Ead and reaction enthalpy
         descriptor_reaction = np.hstack((Ead_reactant, Ead_product, enthalpy))
-        #descriptor_reaction=np.hstack((Ead_reactant,enthalpy))
+        # descriptor_reaction=np.hstack((Ead_reactant,enthalpy))
         return descriptor_reaction, barrier
     else:
-        print(f'NOTE: NEB of {File} is not calculated!')
+        print(f"NOTE: NEB of {File} is not calculated!")
         return None, None
     react_info.close()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     ReaInfo = open("reaction-bk", "r+")
-    des_barr = open('descriptor-barr', 'w+')
-    des_type = open('descriptor-type', 'w+')
-    base_info = '/data3/home/jqyang/high-throughput/script/construction/base-function/codes/Info/Element_Info'
-    feature_surf = ['Valence_electron', 'Atomic_radius']
-    #feature_surf=['Atomic_radius']
-    feature_ads = ['Enegativity', 'Valence_electron']
-    #File_adsE="adsE_coad_radical"
+    des_barr = open("descriptor-barr", "w+")
+    des_type = open("descriptor-type", "w+")
+    base_info = "/data3/home/jqyang/high-throughput/script/construction/base-function/codes/Info/Element_Info"
+    feature_surf = ["Valence_electron", "Atomic_radius"]
+    # feature_surf=['Atomic_radius']
+    feature_ads = ["Enegativity", "Valence_electron"]
+    # File_adsE="adsE_coad_radical"
     for index, line in enumerate(ReaInfo):
         File = get_file_name(line)
         ## enter the dir
         Dir = os.getcwd()
-        Element_type = Dir.split('/')[-3]
-        print(f'Construction for {File} on {Element_type} system starts:')
+        Element_type = Dir.split("/")[-3]
+        print(f"Construction for {File} on {Element_type} system starts:")
         os.chdir(File)
         ### Extract the surface info
-        descriptor_surf = get_surface_info('POSstart', feature_surf, base_info)
+        descriptor_surf = get_surface_info("POSstart", feature_surf, base_info)
         ### Extract reaction info
         descriptor_reaction, barrier = get_reaction_info()
         ### Extract site info
-        descriptor_site1 = get_site_info('POSstart')
-        descriptor_site2 = get_site_info('POSend')
+        descriptor_site1 = get_site_info("POSstart")
+        descriptor_site2 = get_site_info("POSend")
         ### Extract adsorbate info
-        #descriptor_ads=get_adsorbate_info('POSstart',feature_ads,base_info)
-        '''
+        # descriptor_ads=get_adsorbate_info('POSstart',feature_ads,base_info)
+        """
        bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb = get_binding_adatom('POSstart')
        descriptor_ads,descriptor_ads_tmp=[],[]
        for i,specie in enumerate(adspecie):
              ads = molecule(specie)
              ads_symb=ads.get_chemical_symbols()
              #print(ads_symb)
              feature_value_ads=Construct_descriptor_info(base_info,ads_symb,feature_ads)
              #print(feature_value_ads)
              descriptor_ads_tmp += [np.around(np.mean(feature_value_ads,0),2)]
        if len(adspecie) == 2:
           descriptor_ads=np.hstack((descriptor_ads_tmp[0],descriptor_ads_tmp[1]))
        else:
           descriptor_ads=np.hstack((descriptor_ads_tmp[0],[0,0]))
-        '''
+        """
 
         if barrier:
             ### Recombination of descriptor info
             ## Integrated descriptor
             descriptor = np.hstack(
-                (descriptor_surf, descriptor_reaction, descriptor_site1, descriptor_site2))
+                (descriptor_surf, descriptor_reaction, descriptor_site1, descriptor_site2)
+            )
             # descriptor=np.hstack((descriptor_surf,descriptor_reaction,descriptor_site,descriptor_ads))
             ## Descriptor+barrier
             descriptor_barrier = np.hstack((descriptor, barrier))
             ## Descriptor+element type
             descriptor_type = np.hstack((descriptor, Element_type))
             print(descriptor_barrier)
             print(descriptor_type)
 
             ### Output the descriptor
-            #des_barr.write(f'{descriptor_barrier}')
-            #des_type.write(f'{descriptor_type}')
+            # des_barr.write(f'{descriptor_barrier}')
+            # des_type.write(f'{descriptor_type}')
             len_des = len(descriptor_barrier)
             print(len_des)
             for i, d in enumerate(descriptor_barrier):
-                #if d == descriptor_barrier[-1]:
+                # if d == descriptor_barrier[-1]:
                 if i == (int(len_des) - 1):
-                    des_barr.write('%s\n' % d)
+                    des_barr.write("%s\n" % d)
                 else:
-                    des_barr.write('%s\t' % d)
+                    des_barr.write("%s\t" % d)
             for j, d in enumerate(descriptor_type):
-                #if d == descriptor_type[-1]:
+                # if d == descriptor_type[-1]:
                 if j == (int(len_des) - 1):
-                    des_type.write('%s\n' % d)
+                    des_type.write("%s\n" % d)
                 else:
-                    des_type.write('%s\t' % d)
+                    des_type.write("%s\t" % d)
 
-        print(f'Construction for {File} on {Element_type} system end!')
-        print('-----------------------------')
+        print(f"Construction for {File} on {Element_type} system end!")
+        print("-----------------------------")
         os.chdir(Dir)
     ReaInfo.close()
     des_barr.close()
     des_type.close()
```

### Comparing `HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_coad.py` & `HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_coad.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# -*- coding: UTF-8 -*-
-
 from HTMACat.Extract_info import *
 from ase.build import molecule
 from HTMACat.configuration import base_info
 
 
 def Construct_descriptor_coad(poscar, feature_surf, feature_ads, feature_site):
-    """   
-    Construct a descriptor for a catalyst-adsorbate system.
-        
+    """Construct a descriptor for a catalyst-adsorbate system.
+
     Parameters
     ----------
     poscar : str
         The POSCAR file path of the catalyst-adsorbate system.
     feature_surf : list
         A list of features of the catalyst surface for constructing the descriptor.
         The features include:
-        
+
         - surface valence electron
         - surface atomic radius
         - surf+subsurf mean valence electron
         - surf+subsurf mean atomic radius
     feature_ads : list
         A list of features of the adsorbate for constructing the descriptor.
         The features include:
@@ -30,111 +27,124 @@
     feature_site : list
         A list of features of the binding site for constructing the descriptor.
         The features include:
 
         - mean valence electron
         - mean atomic radius
         - binding type
-        
+
     Returns
     -------
     descriptor : numpy.ndarray
         A descriptor array for the catalyst-adsorbate system, including the following features:
 
         - descriptor_surf: the descriptor of the catalyst surface, including the features specified in `feature_surf`.
         - descriptor_ads: the descriptor of the adsorbate, including the features specified in `feature_ads`.
         - descriptor_site: the descriptor of the binding site, including the features specified in `feature_site`.
         - descriptor_distance: the distance of adsorbed species.
 
     Notes
     -----
-    This function first extracts the atom types and coordinates from the POSCAR file of the catalyst-adsorbate system, 
-    and then distinguishes the adsorbate, surface atoms, and subsurface atoms. The features of the surface and 
+    This function first extracts the atom types and coordinates from the POSCAR file of the catalyst-adsorbate system,
+    and then distinguishes the adsorbate, surface atoms, and subsurface atoms. The features of the surface and
     subsurface atoms are calculated based on the `feature_surf` input list, while the features of the adsorbate and
-    binding site are calculated based on the `feature_ads` and `feature_site` input lists, respectively. If multiple 
-    adsorbates are found in the system, the descriptors are constructed for each adsorbate and then combined into a 
+    binding site are calculated based on the `feature_ads` and `feature_site` input lists, respectively. If multiple
+    adsorbates are found in the system, the descriptors are constructed for each adsorbate and then combined into a
     single descriptor. If no adsorbate is found, an error message will be printed.
-
     """
     descriptor = []
     descriptor_surf = []
-    typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
-    typ2 = {None: 0, 'top': 0, 'bri': 0, 'fcc': 0, 'hcp': 1, '4-fold': 0}
+    typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
+    typ2 = {None: 0, "top": 0, "bri": 0, "fcc": 0, "hcp": 1, "4-fold": 0}
 
     ## the features of catalyst surface : surfce valence electron,surface atomic radius, surf+subsurf mean valence electron,surf+subsurf mean atomic radius
     # surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
     # subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05)
     feature_value_surf = Construct_descriptor_info(base_info, surfatoms_symb, feature_surf)
     feature_value_subsurf = Construct_descriptor_info(base_info, subsurfatoms_symb, feature_surf)
 
     ## Ignore structures without standard or integrated surface configuration
     if feature_value_surf != []:
         feature_value = np.hstack((feature_value_surf, feature_value_subsurf))
-        #print(feature_value)
+        # print(feature_value)
         descriptor_surf = np.around(np.mean(feature_value, 0), 2)
         ## the feature of adspecies and binding sites
-        bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-            poscar)
+        (
+            bind_adatoms,
+            bind_adatoms_symb,
+            adspecie,
+            bind_type_symb,
+            bind_surfatoms,
+            bind_surfatoms_symb,
+        ) = get_binding_adatom(poscar)
         # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
         # print(adspecie,bind_type_symb,bind_surfatoms_symb)
         # print(bind_type_symb[0])
         # print(adspecie)
         if adspecie == []:
             print(f"The molecule can not adsorb on the {poscar}!")
         elif len(adspecie) > 1:
-            #print(f"More then 1 adspecie are found in {poscar}!")
-            sys_ad = poscar.split('/')[1].split('_')[-3:-1]
+            # print(f"More then 1 adspecie are found in {poscar}!")
+            sys_ad = poscar.split("/")[1].split("_")[-3:-1]
             if sorted(sys_ad) != sorted(adspecie):
                 print(f"Adsorbed configuration reconstruct on {poscar}!")
             else:
                 ## construct the descriptor of adsorbate: mean enegativity, mean valence_electron
                 descriptor_ads, descriptor_ads_tmp = [], []
                 for i, specie in enumerate(adspecie):
                     ads = molecule(specie)
                     ads_symb = ads.get_chemical_symbols()
-                    #print(ads_symb)
+                    # print(ads_symb)
                     feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
-                    #print(feature_value_ads)
+                    # print(feature_value_ads)
                     descriptor_ads_tmp += [np.around(np.mean(feature_value_ads, 0), 2)]
                 descriptor_ads = np.hstack((descriptor_ads_tmp[0], descriptor_ads_tmp[1]))
 
                 ## construct the descriptor of site: mean valence electron, mean atomic radius, bind type
                 descriptor_site = []
                 site_type, descriptor_site_tmp, descriptor_site_tmp2 = [], [], []
                 # typ={None:0,'top':1,'bri':2,'fcc':3,'hcp':3,'4-fold':4}
                 # typ2={None:0,'top':0,'bri':0,'fcc':0,'hcp':1,'4-fold':0}
                 for j, typ_site in enumerate(bind_type_symb):
                     descriptor_site_tmp += [np.hstack((typ.get(typ_site), typ2.get(typ_site)))]
-                    feature_value_site = Construct_descriptor_info(base_info,
-                                                                   bind_surfatoms_symb[j],
-                                                                   feature_site)
+                    feature_value_site = Construct_descriptor_info(
+                        base_info, bind_surfatoms_symb[j], feature_site
+                    )
                     descriptor_site_tmp += [np.around(np.mean(feature_value_site, 0), 2)]
-                    #print(len(descriptor_site_tmp))
+                    # print(len(descriptor_site_tmp))
                     descriptor_site_tmp2 += [
                         np.hstack((descriptor_site_tmp[0], descriptor_site_tmp[1]))
                     ]
-                    #print(descriptor_site)
+                    # print(descriptor_site)
                 descriptor_site = np.hstack((descriptor_site_tmp2[0], descriptor_site_tmp2[1]))
                 # print(descriptor_site)
 
                 ## construct the descriptor:distance of adsorbed species
                 dis_symb, descriptor_distance = dis_symb_matrix, dis_matrix = get_distance_adatoms(
-                    poscar)
+                    poscar
+                )
                 descriptor = np.hstack(
-                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance))
+                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance)
+                )
                 # print(descriptor)
                 return descriptor
 
         else:
             ## construct the descriptor of adsorbate: mean enegativity, mean valence_electron
-            sys_ad = poscar.split('/')[1].split('_')[-3:-1]
+            sys_ad = poscar.split("/")[1].split("_")[-3:-1]
             adspecie_tmp = sys_ad
-            #print(adspecie_tmp)
+            # print(adspecie_tmp)
             descriptor_ads, descriptor_ads_tmp = [], []
             for i, specie in enumerate(adspecie_tmp):
                 ads = molecule(specie)
                 ads_symb = ads.get_chemical_symbols()
                 # print(ads_symb)
                 feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
                 # print(feature_value_ads)
@@ -143,16 +153,17 @@
 
             ## construct the descriptor of site: mean valence electron, mean atomic radius, bind type
             descriptor_site = []
             site_type, descriptor_site_tmp, descriptor_site_tmp2 = [], [], []
 
             for j, typ_site in enumerate(bind_type_symb):
                 descriptor_site_tmp += [np.hstack((typ.get(typ_site), typ2.get(typ_site)))]
-                feature_value_site = Construct_descriptor_info(base_info, bind_surfatoms_symb[j],
-                                                               feature_site)
+                feature_value_site = Construct_descriptor_info(
+                    base_info, bind_surfatoms_symb[j], feature_site
+                )
                 descriptor_site_tmp += [np.around(np.mean(feature_value_site, 0), 2)]
                 # print(len(descriptor_site_tmp))
                 descriptor_site_tmp2 += [
                     np.hstack((descriptor_site_tmp[0], descriptor_site_tmp[1]))
                 ]
             # print(descriptor_site_tmp2)
             descriptor_site1 = descriptor_site_tmp2[0]
@@ -164,150 +175,162 @@
             # print(np.hstack((site2_type,site2_surfatom_feature)))
 
             if adspecie[0] == adspecie_tmp[0]:
                 descriptor_site = np.hstack((descriptor_site1, site2_type, site2_surfatom_feature))
                 ## construct the descriptor:distance of adsorbed species
                 descriptor_distance = [0]
                 descriptor = np.hstack(
-                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance))
+                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance)
+                )
                 # print(descriptor)
                 # return descriptor
             elif adspecie[0] == adspecie_tmp[1]:
                 descriptor_site = np.hstack((site2_type, site2_surfatom_feature, descriptor_site1))
                 ## construct the descriptor:distance of adsorbed species
                 descriptor_distance = [0]
                 descriptor = np.hstack(
-                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance))
+                    (descriptor_surf, descriptor_ads, descriptor_site, descriptor_distance)
+                )
                 # print(descriptor)
                 # return descriptor
             else:
-                print(f'Adsorbed configuration changes on {poscar}!')
+                print(f"Adsorbed configuration changes on {poscar}!")
     else:
-        print(f'Surface info of {poscar} can not be obtained ')
+        print(f"Surface info of {poscar} can not be obtained ")
 
 
 from HTMACat.Extract_info import *
 from HTMACat.Base_tools import *
 import os
 import numpy as np
 import operator
-if __name__ == '__main__':
-    feature_surf = ['Valence_electron', 'Atomic_radius']
+
+if __name__ == "__main__":
+    feature_surf = ["Valence_electron", "Atomic_radius"]
     # feature_surf=['Atomic_radius']
-    feature_ads = ['Enegativity', 'Valence_electron']
-    feature_site = ['Valence_electron', 'Atomic_radius']
+    feature_ads = ["Enegativity", "Valence_electron"]
+    feature_site = ["Valence_electron", "Atomic_radius"]
     # feature_site=['Atomic_radius']
     adspecies = [
-        'NH3_OH', 'NH3_O', 'NH2_O', 'NH2_OH', 'NH2_H2O', 'NH_O', 'NH_OH', 'NH_H2O', 'N_O', 'N_OH',
-        'N_H2O', 'N_N', 'N_NO', 'O_O'
+        "NH3_OH",
+        "NH3_O",
+        "NH2_O",
+        "NH2_OH",
+        "NH2_H2O",
+        "NH_O",
+        "NH_OH",
+        "NH_H2O",
+        "N_O",
+        "N_OH",
+        "N_H2O",
+        "N_N",
+        "N_NO",
+        "O_O",
     ]
     print("----------------------------------------")
     print("Construct descriptor starts:")
     print("1st step: Get the whole 'Descriptor+Ead'")
 
-    file_des = open('descriptor-coad', 'w+')
-    file_all = open('descriptor-coad-all', 'w+')
-    file_log = open('descriptor-coad-log', 'w+')
+    file_des = open("descriptor-coad", "w+")
+    file_all = open("descriptor-coad-all", "w+")
+    file_log = open("descriptor-coad-log", "w+")
 
-    EnerInfo = open('adsE_coad', 'r+')
+    EnerInfo = open("adsE_coad", "r+")
     des, des_all, des_tmp = [], [], []
     for i, Ener in enumerate(EnerInfo):
-        sys = Ener.split(',')[0]
-        ene = Ener.split(',')[-1].strip()
-        poscar = f'./{sys}/optmk/CONTCAR'
+        sys = Ener.split(",")[0]
+        ene = Ener.split(",")[-1].strip()
+        poscar = f"./{sys}/optmk/CONTCAR"
         # poscar= f'./{sys}/CONTCAR'
 
         if adspecies != []:
-            sys_all = '_'.join(sys.split('_')[-3:-1])
+            sys_all = "_".join(sys.split("_")[-3:-1])
 
-            specie = set([sys_all]).intersection(set(adspecies))
+            specie = {sys_all}.intersection(set(adspecies))
             # print(set([sys_all]),set(adspecies),specie)
             if specie:
                 print(sys)
-                descriptor = Construct_descriptor_coad(poscar, feature_surf, feature_ads,
-                                                       feature_site)
+                descriptor = Construct_descriptor_coad(
+                    poscar, feature_surf, feature_ads, feature_site
+                )
                 if descriptor is None:
-                    tmp = np.hstack(([sys], ['None'], [ene]))
+                    tmp = np.hstack(([sys], ["None"], [ene]))
                     for d in tmp:
                         if d == tmp[-1]:
-                            file_all.write('%s\n' % d)
+                            file_all.write("%s\n" % d)
                         else:
-                            file_all.write('%s\t' % d)
+                            file_all.write("%s\t" % d)
                 else:
                     tmp = np.hstack(([sys], descriptor, [ene]))
                     for d in tmp:
                         if d == tmp[-1]:
-                            file_all.write('%s\n' % d)
+                            file_all.write("%s\n" % d)
                         else:
-                            file_all.write('%s\t' % d)
-                # file_all.writelines('%s\n' %tmp)
+                            file_all.write("%s\t" % d)
+                    # file_all.writelines('%s\n' %tmp)
                     des_tmp += [np.hstack(([sys], descriptor, [ene]))]
         else:
             print(sys)
             descriptor = Construct_descriptor_coad(poscar, feature_surf, feature_ads, feature_site)
             if descriptor is None:
-                tmp = np.hstack(([sys], ['None'], [ene]))
+                tmp = np.hstack(([sys], ["None"], [ene]))
                 for d in tmp:
                     if d == tmp[-1]:
-                        file_all.write('%s\n' % d)
+                        file_all.write("%s\n" % d)
                     else:
-                        file_all.write('%s\t' % d)
+                        file_all.write("%s\t" % d)
             else:
                 tmp = np.hstack(([sys], descriptor, [ene]))
                 for d in tmp:
                     if d == tmp[-1]:
-                        file_all.write('%s\n' % d)
+                        file_all.write("%s\n" % d)
                     else:
-                        file_all.write('%s\t' % d)
-                #file_all.writelines('%s\n' %tmp)
+                        file_all.write("%s\t" % d)
+                # file_all.writelines('%s\n' %tmp)
                 des_tmp += [tmp]
-    #print(des_tmp[0])
+    # print(des_tmp[0])
     print("2nd: Extrate the repeated values")
     ###Substrate the repeated items according to the feature list
     m, n = np.array(des_tmp).shape
     # Extrate the feature value
     des_feature = [des_tmp[j][1:-1] for j in range(m)]
     # The feaure list after substrate the repeat
-    des_feature_tmp = np.array(list(set([tuple(t) for t in des_feature])))
+    des_feature_tmp = np.array(list({tuple(t) for t in des_feature}))
     k, l = des_feature_tmp.shape
     # The threshold value Ecut of Ead: if Ead > Ecut, ignore it
     Ecut = 0.25
     # Output the feature and energy
     if m > k:
         print("Subtrate Repeat Values Starts:")
         for i, d1 in enumerate(des_feature_tmp):
             for j, d2 in enumerate(des_tmp):
                 if all(d1 == d2[1:-1]):
                     tmp = np.hstack((d1, d2[-1]))
-                    tmp2 = np.hstack((d1, [d2[0].split('_')[0]]))
+                    tmp2 = np.hstack((d1, [d2[0].split("_")[0]]))
                     ## output
                     if float(tmp[-1]) < float(Ecut):
                         # output des+ene
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_des.write('%s\n' % d)
+                                file_des.write("%s\n" % d)
                             else:
-                                file_des.write('%s\t' % d)
+                                file_des.write("%s\t" % d)
                         # output des+type: des+'Au'
                         for d in tmp2:
                             if d == tmp2[-1]:
-                                file_log.write('%s\n' % d)
+                                file_log.write("%s\n" % d)
                             else:
-                                file_log.write('%s\t' % d)
+                                file_log.write("%s\t" % d)
                     else:
-                        print(f'Ignore the value {tmp[-1]} >= {Ecut}')
+                        print(f"Ignore the value {tmp[-1]} >= {Ecut}")
 
                     break
                 else:
                     continue
     else:
-        print('No Repeated Value')
+        print("No Repeated Value")
     file_all.close()
     file_des.close()
     file_log.close()
     print("Subtrate Repeat Values End !")
-    '''
-   print('---------Raw data---------')
-   os.system('cat descriptor-all')
-   print('---------Final data---------')
-   os.system('cat descriptor')
-   '''
+    """print('---------Raw data---------') os.system('cat descriptor-all') print('---------Final
+    data---------') os.system('cat descriptor')"""
```

### Comparing `HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_surface.py` & `HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_surface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,161 +1,170 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 from HTMACat.configuration import base_info
 
 
-def Construct_descriptor(poscar, feature_surf, feature_ads, feature_site, adspecies, facet='100'):
+def Construct_descriptor(poscar, feature_surf, feature_ads, feature_site, adspecies, facet="100"):
     descriptor = []
     descriptor_surf = []
     ### the features of catalyst surface : surfce valence electron,surface atomic radius,
     ### surf+subsurf mean valence electron,surf+subsurf mean atomic radius
-    #surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
-    #subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(surfatoms_symb)
+    # surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
+    # subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05)
+    # print(surfatoms_symb)
     ## If NO, The symmetry of surface atoms could be broken
-    if get_symmetry_surfatoms(poscar, tol=0.3) == 'NO':
+    if get_symmetry_surfatoms(poscar, tol=0.3) == "NO":
         print(f"The symmetry of surface atoms of {poscar} could not be keeped!")
-        #return descriptor
+        # return descriptor
     else:
         feature_value_surf = Construct_descriptor_info(base_info, surfatoms_symb, feature_surf)
-        feature_value_subsurf = Construct_descriptor_info(base_info, subsurfatoms_symb,
-                                                          feature_surf)
-        #print(feature_value_surf)
+        feature_value_subsurf = Construct_descriptor_info(
+            base_info, subsurfatoms_symb, feature_surf
+        )
+        # print(feature_value_surf)
         m0, n0 = np.array(feature_value_surf).shape
         m1, n1 = np.array(feature_value_subsurf).shape
-        #print(m0,m1)
+        # print(m0,m1)
         ## Ignore structures without standard or integrated surface configuration
         ## if m0 not equal to m1 menas that the large surface reconstruction occurs and causes the broken of surface.
         if (feature_value_surf != []) and (m0 == m1):
-            #print(feature_value_surf,feature_value_subsurf)
+            # print(feature_value_surf,feature_value_subsurf)
             feature_value = np.hstack((feature_value_surf, feature_value_subsurf))
-            #print(feature_value)
+            # print(feature_value)
             descriptor_surf_tmp = np.around(np.mean(feature_value, 0), 2)
-            facet_coord = {'100': 8, '111': 9}
+            facet_coord = {"100": 8, "111": 9}
             descriptor_surf = np.hstack((descriptor_surf_tmp, [facet_coord.get(facet)]))
             ### the feature of adspecies and binding sites
-            bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-                poscar)
-            #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
-            #print(adspecie,bind_type_symb,bind_surfatoms_symb)
-            #print(bind_type_symb[0])
+            (
+                bind_adatoms,
+                bind_adatoms_symb,
+                adspecie,
+                bind_type_symb,
+                bind_surfatoms,
+                bind_surfatoms_symb,
+            ) = get_binding_adatom(poscar)
+            # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+            # print(adspecie,bind_type_symb,bind_surfatoms_symb)
+            # print(bind_type_symb[0])
             if adspecie == []:
                 print(f"The molecule can not adsorb in the {poscar}!")
             elif len(adspecie) > 1:
                 print(f"More than 1 adspecie are found in {poscar}!")
             elif set(adspecie).intersection(set(adspecies)):
                 ## construct the descriptor of adsorbate: mean enegativity, mean valence_electron
-                #print(adspecie)
+                # print(adspecie)
                 descriptor_ads = []
-                #print(adspecie)
+                # print(adspecie)
                 ads = molecule(adspecie[0])
-                #print(ads)
+                # print(ads)
                 ads_symb = ads.get_chemical_symbols()
                 feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
                 descriptor_ads = np.around(np.mean(feature_value_ads, 0), 2)
-                #print(descriptor_ads)
+                # print(descriptor_ads)
 
                 ## construct the descriptor of site: mean valence electron, mean atomic radius, bind type
                 descriptor_site = []
-                typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
-                typ2 = {None: 0, 'top': 0, 'bri': 0, 'fcc': 0, 'hcp': 1, '4-fold': 0}
+                typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
+                typ2 = {None: 0, "top": 0, "bri": 0, "fcc": 0, "hcp": 1, "4-fold": 0}
                 site_type = np.hstack((typ.get(bind_type_symb[0]), typ2.get(bind_type_symb[0])))
-                feature_value_site = Construct_descriptor_info(base_info, bind_surfatoms_symb[0],
-                                                               feature_site)
+                feature_value_site = Construct_descriptor_info(
+                    base_info, bind_surfatoms_symb[0], feature_site
+                )
                 descriptor_site_tmp = np.around(np.mean(feature_value_site, 0), 2)
                 descriptor_site = np.append(descriptor_site_tmp, site_type)
-                #print(descriptor_site)
+                # print(descriptor_site)
 
                 descriptor = np.hstack((descriptor_surf, descriptor_ads, descriptor_site))
-                #print(descriptor)
+                # print(descriptor)
                 return descriptor
             else:
                 print(adspecie)
                 print(f"{poscar} can not be identified!")
         else:
-            print(f'Surface info of {poscar} can not be obtained ')
+            print(f"Surface info of {poscar} can not be obtained ")
 
 
 from HTMACat.Extract_info import *
-#from Construct_descriptor import *
-#from Base_tools import *
+
+# from Construct_descriptor import *
+# from Base_tools import *
 import os
 import numpy as np
 import operator
 
 
-#if __name__ == '__main__':
+# if __name__ == '__main__':
 def Construct_des_module(adspecies, facet, dop_typ_all):
-    """
-    Constructs the descriptor module for a given set of adsorbates on a surface with a particular facet and doping type.
+    """Constructs the descriptor module for a given set of adsorbates on a surface with a
+    particular facet and doping type.
 
     Parameters
     ----------
     adspecies : list of str
         A list of adsorbate species to consider.
     facet : str
         The surface facet to consider.
     dop_typ_all : list of str
         A list of doping types to consider.
 
     Returns
     -------
     None
         The function writes the descriptor and energy information to an output file.
-
     """
-    feature_surf = ['Valence_electron', 'Atomic_radius']
-    #feature_ads=['Enegativity','Valence_electron']
-    feature_ads = ['Valence_electron', 'Atomic_radius']
-    feature_site = ['Valence_electron', 'Atomic_radius']
-
-    #adspecies=['N']
-    #facet='111'
-    #dop_typ_all = ['1','2','3','1L','b1']
+    feature_surf = ["Valence_electron", "Atomic_radius"]
+    # feature_ads=['Enegativity','Valence_electron']
+    feature_ads = ["Valence_electron", "Atomic_radius"]
+    feature_site = ["Valence_electron", "Atomic_radius"]
+
+    # adspecies=['N']
+    # facet='111'
+    # dop_typ_all = ['1','2','3','1L','b1']
 
-    file_all = open('descriptor-all-2', 'w+')
+    file_all = open("descriptor-all-2", "w+")
     for typ in dop_typ_all:
-
         print("----------------------------------------")
         print("1st step: Get the whole 'Descriptor+Ead'")
 
-        EnerInfo = open(f'ads_final_{typ}', 'r+')
+        EnerInfo = open(f"ads_final_{typ}", "r+")
 
         for i, Ener in enumerate(EnerInfo):
-            sys = Ener.split(',')[0]
-            ene = Ener.split(',')[-1].strip()
-            sys_all = sys.split('_')
+            sys = Ener.split(",")[0]
+            ene = Ener.split(",")[-1].strip()
+            sys_all = sys.split("_")
             dop_typ = sys_all[-3]
             base = sys_all[0]
             specie = set(sys_all).intersection(set(adspecies))
             if specie:
                 if dop_typ in dop_typ_all:
-                    #poscar= f'./{sys}/optmk/CONTCAR'
-                    poscar = f'./{sys}/CONTCAR'
+                    # poscar= f'./{sys}/optmk/CONTCAR'
+                    poscar = f"./{sys}/CONTCAR"
                     print(sys)
-                    descriptor = Construct_descriptor(poscar,
-                                                      feature_surf,
-                                                      feature_ads,
-                                                      feature_site,
-                                                      adspecies,
-                                                      facet=facet)
-                    #print(descriptor)
+                    descriptor = Construct_descriptor(
+                        poscar, feature_surf, feature_ads, feature_site, adspecies, facet=facet
+                    )
+                    # print(descriptor)
                     if descriptor is None:
-                        tmp = np.hstack(([sys], ['None'], [ene], [base]))
+                        tmp = np.hstack(([sys], ["None"], [ene], [base]))
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_all.write('%s\n' % d)
+                                file_all.write("%s\n" % d)
                             else:
-                                file_all.write('%s\t' % d)
+                                file_all.write("%s\t" % d)
 
                     else:
                         tmp = np.hstack(([sys], descriptor, [ene], [base]))
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_all.write('%s\n' % d)
+                                file_all.write("%s\n" % d)
                             else:
-                                file_all.write('%s\t' % d)
-                        #file_all.writelines('%s\n' %tmp)
+                                file_all.write("%s\t" % d)
+                        # file_all.writelines('%s\n' %tmp)
         EnerInfo.close()
     file_all.close()
```

### Comparing `HTMACat-1.0.4/HTMACat/descriptor/Construct_descriptor_surface_single.py` & `HTMACat-1.0.5/HTMACat/descriptor/Construct_descriptor_surface_single.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,152 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 from HTMACat.configuration import base_info
 
 
-def Construct_descriptor(poscar,
-                         feature_surf,
-                         feature_ads,
-                         feature_site,
-                         adspecies,
-                         facet='100',
-                         label='all'):
+def Construct_descriptor(
+    poscar, feature_surf, feature_ads, feature_site, adspecies, facet="100", label="all"
+):
     descriptor = []
     descriptor_surf = []
     ### the features of catalyst surface : surfce valence electron,surface atomic radius,
     ### surf+subsurf mean valence electron,surf+subsurf mean atomic radius
-    #surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
-    #subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
-    adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
-        poscar, tol=0.05)
-    #print(surfatoms_symb)
+    # surfatoms,surfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='surf_atom')
+    # subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar, tol=0.03,layer='subsurf_atom')
+    (
+        adatoms,
+        adatoms_symb,
+        surfatoms,
+        surfatoms_symb,
+        subsurfatoms,
+        subsurfatoms_symb,
+    ) = distinguish_atom_binding(poscar, tol=0.05)
+    # print(surfatoms_symb)
     ## If NO, The symmetry of surface atoms could be broken
-    if get_symmetry_surfatoms(poscar, tol=0.3) == 'NO':
+    if get_symmetry_surfatoms(poscar, tol=0.3) == "NO":
         print(f"The symmetry of surface atoms of {poscar} could not be keeped!")
-        #return descriptor
+        # return descriptor
     else:
         feature_value_surf = Construct_descriptor_info(base_info, surfatoms_symb, feature_surf)
-        feature_value_subsurf = Construct_descriptor_info(base_info, subsurfatoms_symb,
-                                                          feature_surf)
-        #print(feature_value_surf)
+        feature_value_subsurf = Construct_descriptor_info(
+            base_info, subsurfatoms_symb, feature_surf
+        )
+        # print(feature_value_surf)
         m0, n0 = np.array(feature_value_surf).shape
         m1, n1 = np.array(feature_value_subsurf).shape
-        #print(m0,m1)
+        # print(m0,m1)
         ## Ignore structures without standard or integrated surface configuration
         ## if m0 not equal to m1 menas that the large surface reconstruction occurs and causes the broken of surface.
         if (feature_value_surf != []) and (m0 == m1):
-            #print(feature_value_surf,feature_value_subsurf)
+            # print(feature_value_surf,feature_value_subsurf)
             feature_value = np.hstack((feature_value_surf, feature_value_subsurf))
-            #print(feature_value)
+            # print(feature_value)
             descriptor_surf_tmp = np.around(np.mean(feature_value, 0), 2)
-            facet_coord = {'100': 8, '111': 9}
+            facet_coord = {"100": 8, "111": 9}
             descriptor_surf = np.hstack((descriptor_surf_tmp, [facet_coord.get(facet)]))
 
-            if label == 'surface':
+            if label == "surface":
                 return descriptor_surf
             else:
                 ### the feature of adspecies and binding sites
-                bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = get_binding_adatom(
-                    poscar)
-                #print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
-                #print(adspecie,bind_type_symb,bind_surfatoms_symb)
-                #print(bind_type_symb[0])
+                (
+                    bind_adatoms,
+                    bind_adatoms_symb,
+                    adspecie,
+                    bind_type_symb,
+                    bind_surfatoms,
+                    bind_surfatoms_symb,
+                ) = get_binding_adatom(poscar)
+                # print(bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+                # print(adspecie,bind_type_symb,bind_surfatoms_symb)
+                # print(bind_type_symb[0])
                 if adspecie == []:
                     print(f"The molecule can not adsorb in the {poscar}!")
                 elif len(adspecie) > 1:
                     print(f"More than 1 adspecie are found in {poscar}!")
                 elif set(adspecie).intersection(set(adspecies)):
                     ## construct the descriptor of adsorbate: mean enegativity, mean valence_electron
-                    #print(adspecie)
+                    # print(adspecie)
                     descriptor_ads = []
-                    #print(adspecie)
+                    # print(adspecie)
                     ads = molecule(adspecie[0])
-                    #print(ads)
+                    # print(ads)
                     ads_symb = ads.get_chemical_symbols()
                     feature_value_ads = Construct_descriptor_info(base_info, ads_symb, feature_ads)
                     descriptor_ads = np.around(np.mean(feature_value_ads, 0), 2)
-                    #print(descriptor_ads)
+                    # print(descriptor_ads)
 
                     ## construct the descriptor of site: mean valence electron, mean atomic radius, bind type
                     descriptor_site = []
-                    typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
-                    typ2 = {None: 0, 'top': 0, 'bri': 0, 'fcc': 0, 'hcp': 1, '4-fold': 0}
-                    site_type = np.hstack((typ.get(bind_type_symb[0]), typ2.get(bind_type_symb[0])))
-                    feature_value_site = Construct_descriptor_info(base_info,
-                                                                   bind_surfatoms_symb[0],
-                                                                   feature_site)
+                    typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
+                    typ2 = {None: 0, "top": 0, "bri": 0, "fcc": 0, "hcp": 1, "4-fold": 0}
+                    site_type = np.hstack(
+                        (typ.get(bind_type_symb[0]), typ2.get(bind_type_symb[0]))
+                    )
+                    feature_value_site = Construct_descriptor_info(
+                        base_info, bind_surfatoms_symb[0], feature_site
+                    )
                     descriptor_site_tmp = np.around(np.mean(feature_value_site, 0), 2)
                     descriptor_site = np.append(descriptor_site_tmp, site_type)
-                    #print(descriptor_site)
+                    # print(descriptor_site)
 
                     descriptor = np.hstack((descriptor_surf, descriptor_ads, descriptor_site))
-                    #print(descriptor)
+                    # print(descriptor)
                     return descriptor
                 else:
                     print(adspecie)
                     print(f"{poscar} can not be identified!")
         else:
-            print(f'Surface info of {poscar} can not be obtained ')
+            print(f"Surface info of {poscar} can not be obtained ")
 
 
 def Construct_descriptor_info_E(ele, facet, specie, facet_dop=True):
-    """
-    Construct descriptor information based on element, crystal plane and doping species class.
-
-    Parameters
-    ----------
-    ele : str
-        The chemical symbol of an element.
-    facet : str
-        crystal face
-    specie : str
-        The chemical symbol of the dopant.
-    facet_dop : bool, optional
-        Whether the doping type is included (default True).
-
-    Returns
-    -------
-    str
-        The energy value in the descriptor information.
-
-    Notes
-    -----
-   If 'facet_dop' is True, the doping type will be included when building descriptor information.
+    """Construct descriptor information based on element, crystal plane and doping species class.
 
+     Parameters
+     ----------
+     ele : str
+         The chemical symbol of an element.
+     facet : str
+         crystal face
+     specie : str
+         The chemical symbol of the dopant.
+     facet_dop : bool, optional
+         Whether the doping type is included (default True).
+
+     Returns
+     -------
+     str
+         The energy value in the descriptor information.
+
+     Notes
+     -----
+    If 'facet_dop' is True, the doping type will be included when building descriptor information.
     """
-    with open('/data3/home/jqyang/general-script/energy_single', 'r+') as Efile:
+    with open("/data3/home/jqyang/general-script/energy_single", "r+") as Efile:
         f1 = Efile.readline().split()
         EN, EO, label = [], [], []
         f2 = Efile.readlines()
         for i, sys in enumerate(f2):
             EN.append(sys.split()[0])
             EO.append(sys.split()[1])
             label.append(sys.split()[2].strip())
         if facet_dop:
-            lab = f'{ele}_{facet}'
-            #print(label[0],specie)
+            lab = f"{ele}_{facet}"
+            # print(label[0],specie)
             for j, l in enumerate(label):
                 if (lab == l) and (f1[0] == specie):
                     return EN[j]
                 elif (lab == l) and (f1[1] == specie):
                     return EO[j]
                 else:
                     continue
         else:
-            lab = f'{ele}'
+            lab = f"{ele}"
             for j, ls in enumerate(label):
-                l = ls.split('_')[0]
+                l = ls.split("_")[0]
                 if (lab == l) and (f1[0] == specie):
                     return EN[j]
                 elif (lab == l) and (f1[1] == specie):
                     return EO[j]
                 else:
                     continue
 
@@ -146,99 +154,98 @@
 from HTMACat.Extract_info import *
 import os
 import numpy as np
 import operator
 
 
 def Construct_des_module(adspecies, facet, dop_typ_all):
-    """
-    Constructs the descriptor module for a given set of adsorbates on a surface with a particular facet and doping type.
+    """Constructs the descriptor module for a given set of adsorbates on a surface with a
+    particular facet and doping type.
 
     Parameters
     ----------
     adspecies : list of str
         A list of adsorbate species to consider.
     facet : str
         The surface facet to consider.
     dop_typ_all : list of str
         A list of doping types to consider.
 
     Returns
     -------
     None
         The function writes the descriptor and energy information to an output file.
-
     """
-    feature_surf = ['Valence_electron', 'Atomic_radius']
-    #feature_ads=['Enegativity','Valence_electron']
-    feature_ads = ['Valence_electron', 'Atomic_radius']
-    feature_site = ['Valence_electron', 'Atomic_radius']
-
-    #adspecies=['N']
-    #facet='111'
-    #dop_typ_all = ['1','2','3','1L','b1']
+    feature_surf = ["Valence_electron", "Atomic_radius"]
+    # feature_ads=['Enegativity','Valence_electron']
+    feature_ads = ["Valence_electron", "Atomic_radius"]
+    feature_site = ["Valence_electron", "Atomic_radius"]
+
+    # adspecies=['N']
+    # facet='111'
+    # dop_typ_all = ['1','2','3','1L','b1']
 
-    file_all = open('descriptor-all-2', 'w+')
+    file_all = open("descriptor-all-2", "w+")
     for typ in dop_typ_all:
-
         print("----------------------------------------")
         print("Construct descriptor {facet} {dop} starts:")
         print("1st step: Get the whole 'Descriptor+Ead'")
 
-        EnerInfo = open(f'ads_final_{typ}', 'r+')
+        EnerInfo = open(f"ads_final_{typ}", "r+")
 
         for i, Ener in enumerate(EnerInfo):
-            sys = Ener.split(',')[0]
-            ene = Ener.split(',')[-1].strip()
-            sys_all = sys.split('_')
+            sys = Ener.split(",")[0]
+            ene = Ener.split(",")[-1].strip()
+            sys_all = sys.split("_")
             dop_typ = sys_all[-3]
             base = sys_all[0]
             base2 = sys_all[1]
             facet3 = sys_all[2]
             specie = list(set(sys_all).intersection(set(adspecies)))
             if specie:
                 if (dop_typ in dop_typ_all) and (facet == facet3):
-                    #poscar= f'./{sys}/optmk/CONTCAR'
-                    poscar = f'./{sys}/CONTCAR'
-                    #print(sys,specie[0])
+                    # poscar= f'./{sys}/optmk/CONTCAR'
+                    poscar = f"./{sys}/CONTCAR"
+                    # print(sys,specie[0])
                     E1 = Construct_descriptor_info_E(base, facet, specie[0])
                     E2 = Construct_descriptor_info_E(base2, facet, specie[0])
-                    descriptor = Construct_descriptor(poscar,
-                                                      feature_surf,
-                                                      feature_ads,
-                                                      feature_site,
-                                                      adspecies,
-                                                      facet=facet,
-                                                      label='surface')
-                    #print(descriptor)
-                    if dop_typ == '1L':
+                    descriptor = Construct_descriptor(
+                        poscar,
+                        feature_surf,
+                        feature_ads,
+                        feature_site,
+                        adspecies,
+                        facet=facet,
+                        label="surface",
+                    )
+                    # print(descriptor)
+                    if dop_typ == "1L":
                         dop_typ = 9
                     if descriptor is None:
-                        tmp = np.hstack(([sys], ['None'], [ene], [base]))
+                        tmp = np.hstack(([sys], ["None"], [ene], [base]))
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_all.write('%s\n' % d)
+                                file_all.write("%s\n" % d)
                             else:
-                                file_all.write('%s\t' % d)
+                                file_all.write("%s\t" % d)
 
                     else:
                         tmp = np.hstack(([sys], [E1], [E2], [dop_typ], descriptor, [ene], [base]))
                         for d in tmp:
                             if d == tmp[-1]:
-                                file_all.write('%s\n' % d)
+                                file_all.write("%s\n" % d)
                             else:
-                                file_all.write('%s\t' % d)
-                        #file_all.writelines('%s\n' %tmp)
+                                file_all.write("%s\t" % d)
+                        # file_all.writelines('%s\n' %tmp)
         EnerInfo.close()
     file_all.close()
 
 
 def Construct_des_module_2(adspecies, facet, dop_typ_all):
-    """
-    Construct descriptor module for a given adsorbate species, facet, and dopant type(s).
+    """Construct descriptor module for a given adsorbate species, facet, and dopant type(s).
 
     Parameters
     ----------
     adspecies : str
         The adsorbate species to construct the descriptor for.
     facet : str
         The facet to construct the descriptor for.
@@ -253,77 +260,79 @@
     Notes
     -----
     This function reads energy information from a file named 'all' and uses the function Construct_descriptor_info_E to
     obtain information on the energy of a given adsorbate on a given facet and dopant type. The function Construct_descriptor
     is then used to construct a descriptor for a given system, and the descriptor is written to a file named
     'descriptor-{facet}-{adspecies[0]}'.
     """
-    feature_surf = ['Valence_electron', 'Atomic_radius']
-    feature_ads = ['Valence_electron', 'Atomic_radius']
-    feature_site = ['Valence_electron', 'Atomic_radius']
+    feature_surf = ["Valence_electron", "Atomic_radius"]
+    feature_ads = ["Valence_electron", "Atomic_radius"]
+    feature_site = ["Valence_electron", "Atomic_radius"]
 
-    file_all = open(f'descriptor-{facet}-{adspecies[0]}', 'w+')
-    #for typ in dop_typ_all:
+    file_all = open(f"descriptor-{facet}-{adspecies[0]}", "w+")
+    # for typ in dop_typ_all:
 
     print("----------------------------------------")
     print("Construct descriptor {facet} {dop} starts:")
     print("1st step: Get the whole 'Descriptor'")
 
-    EnerInfo = open(f'all', 'r+')
+    EnerInfo = open(f"all", "r+")
     for i, Ener in enumerate(EnerInfo):
-        sys = Ener.split('.')[0]
-        sys_all = sys.split('_')
+        sys = Ener.split(".")[0]
+        sys_all = sys.split("_")
         dop_typ = sys_all[-2]
 
         base = sys_all[0]
         base2 = sys_all[1]
         facet3 = sys_all[2]
 
         if (dop_typ in dop_typ_all) and (facet == facet3):
-            #poscar= f'./{sys}/optmk/CONTCAR'
-            poscar = f'./{sys}.vasp'
+            # poscar= f'./{sys}/optmk/CONTCAR'
+            poscar = f"./{sys}.vasp"
             print(sys)
             E1 = Construct_descriptor_info_E(base, facet, adspecies[0], facet_dop=True)
             E2 = Construct_descriptor_info_E(base2, facet, adspecies[0], facet_dop=False)
-            descriptor = Construct_descriptor(poscar,
-                                              feature_surf,
-                                              feature_ads,
-                                              feature_site,
-                                              adspecies,
-                                              facet=facet,
-                                              label='surface')
+            descriptor = Construct_descriptor(
+                poscar,
+                feature_surf,
+                feature_ads,
+                feature_site,
+                adspecies,
+                facet=facet,
+                label="surface",
+            )
 
             ### construct descriptor ##
-            if dop_typ == '1L':
+            if dop_typ == "1L":
                 dop_typ = 9
             if descriptor is None:
-                tmp = np.hstack(([sys], ['None'], [base]))
+                tmp = np.hstack(([sys], ["None"], [base]))
                 for d in tmp:
                     if d == tmp[-1]:
-                        file_all.write('%s\n' % d)
+                        file_all.write("%s\n" % d)
                     else:
-                        file_all.write('%s\t' % d)
+                        file_all.write("%s\t" % d)
 
             else:
                 tmp = np.hstack(([sys], [E1], [E2], [dop_typ], descriptor, [base]))
                 for d in tmp:
                     if d == tmp[-1]:
-                        file_all.write('%s\n' % d)
+                        file_all.write("%s\n" % d)
                     else:
-                        file_all.write('%s\t' % d)
-                #file_all.writelines('%s\n' %tmp)
+                        file_all.write("%s\t" % d)
+                # file_all.writelines('%s\n' %tmp)
     EnerInfo.close()
     file_all.close()
 
 
-if __name__ == '__main__':
-    #E=Construct_descriptor_info_E('Co','0001','N',facet_dop=False)
-    adspecies = ['N', 'O']
-    #facet='100'
-    #dop_typ_all=['1','2','4','1L']
+if __name__ == "__main__":
+    # E=Construct_descriptor_info_E('Co','0001','N',facet_dop=False)
+    adspecies = ["N", "O"]
+    # facet='100'
+    # dop_typ_all=['1','2','4','1L']
     for specie in adspecies:
-        #facet='111'
-        #dop_typ_all=['1','2','3','1L']
-        facet = '100'
-        dop_typ_all = ['1', '2', '4', '1L']
+        # facet='111'
+        # dop_typ_all=['1','2','3','1L']
+        facet = "100"
+        dop_typ_all = ["1", "2", "4", "1L"]
 
         Construct_des_module_2([specie], facet, dop_typ_all)
```

### Comparing `HTMACat-1.0.4/HTMACat/model/Ads.py` & `HTMACat-1.0.5/HTMACat/model/Ads.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,44 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sat Mar 18 09:00:12 2023
+"""Created on Sat Mar 18 09:00:12 2023.
 
 @author: YuxiaoLan
 """
 
 from HTMACat.catkit.gen.adsorption import Builder
 from HTMACat.catkit.gratoms import *
 from rdkit import Chem
 from rdkit.Chem import AllChem, rdMolDescriptors
 import math
 from HTMACat.Extract_info import *
-from HTMACat.catkit.build import molecule
 from HTMACat.model.Substrate import Slab
 from HTMACat.catkit.gen.adsorption import AdsorptionSites
 from HTMACat.model.Structure import Structure
 import networkx.algorithms.isomorphism as iso
-
-class Species(object):
-    def __init__(self, form, sml=False):
-        self.SML = sml
-        self.form = form.strip()
-
-    def get_formular(self):
-        return self.form
-
-    def out_file_name(self):
-        ads1 = self.get_formular()
-        if self.SML:
-            mole = Chem.AddHs(Chem.MolFromSmiles(ads1))
-            ads1 = rdMolDescriptors.CalcMolFormula(mole)
-        return ads1
-
-    def out_print(self):
-        return self.form
-
-    def MolToNXGraph(self, m):
-        """
-        Convert a molecule object to a graph.
-        Parameters
-        ----------
-        m : mol
-            The RDKit molecule object to be converted into a networkx graph.
-        Returns
-        ----------
-        G : Graph
-            The networkx Graph object derived from m.
-        """
-        G = nx.Graph()
-        for i_n in range(m.GetNumAtoms()):
-            G.add_nodes_from([(i_n, {'number':m.GetAtomWithIdx(i_n).GetAtomicNum()})])
-        bonds = [m.GetBondWithIdx(k) for k in range(len(m.GetBonds()))]
-        edges = []
-        for edge in bonds:
-            edges.append((edge.GetBeginAtomIdx(),edge.GetEndAtomIdx()))
-        G.add_edges_from(edges)
-        return G
-
-    def get_molecule(self):
-        ads1 = self.get_formular()
-        if self.SML:
-            mole = Chem.AddHs(Chem.MolFromSmiles(ads1))
-            G = self.MolToNXGraph(mole)
-            ads1_list = molecule(rdMolDescriptors.CalcMolFormula(mole))
-            ads_molecule = ads1_list[0]
-            for ads_ in ads1_list:
-                nm = iso.categorical_node_match('number', 6)
-                if nx.is_isomorphic(ads_._graph, G, node_match=nm):
-                    ads_molecule = ads_
-                    break
-        else:
-            ads_molecule = molecule(ads1)[0]
-        return ads_molecule
+from ase import Atoms
+from HTMACat.model.Species import init_from_ads, ABS_Species
 
 
 class Adsorption(Structure):
     def __init__(self, species: list, sites: list, spec_ads_stable=None, substrate=Slab()):
         if spec_ads_stable is None:
-            spec_ads_stable = {'NH3': [1], 'NH2': [2], 'NH': [2, 4], 'N': [2, 4], 'O': [2, 4],
-                               'OH': [2, 4], 'NO': [2, 4], 'H2O': [1], 'H': [2, 4]}
+            spec_ads_stable = {
+                "NH3": [1],
+                "NH2": [2],
+                "NH": [2, 4],
+                "N": [2, 4],
+                "O": [2, 4],
+                "OH": [2, 4],
+                "NO": [2, 4],
+                "H2O": [1],
+                "H": [2, 4],
+            }
         assert isinstance(species, list), "species should be a list of Species class"
-        assert isinstance(species[0], Species), "species should be a list of Species class"
+        assert isinstance(species[0], ABS_Species), "species should be a list of Species class"
         assert isinstance(sites, list), "sites should be a list"
         assert sites[0] in ['1', '2'], 'Supports only "1" "2" adsorption sites type for ads!'
-        assert len(species) == len(sites), "The species number and the sites number is not equal"
         self.species = species
         self.sites = sites
         self.spec_ads_stable = spec_ads_stable
         self.substrate = substrate
 
     def set_species(self, species):
         self.species = species
@@ -95,72 +46,96 @@
     def add_species(self, species):
         self.species.append(species)
 
     def add_sites(self, sites):
         self.sites.append(sites)
 
     def get_sites(self):
-        return ' '.join(self.sites)
+        return self.sites # ' '.join(self.sites)
 
     def out_file_name(self):
         ads = []
         ads_str = self.species[0].out_file_name()
         substrate_str = self.substrate.out_file_name()
-        vasp_file_str: str = '_'.join([substrate_str, ads_str])
+        vasp_file_str: str = "_".join([substrate_str, ads_str])
         return vasp_file_str
 
     def out_print(self):
         species_str = []
         for i in range(len(self.species)):
             species_str.append(self.species[i].out_print())
 
-        species_str = ' and '.join(species_str)
+        species_str = " and ".join(species_str)
         substrate_str = self.substrate.out_print()
-        print_str = "%s adsorption on %s" % (species_str, substrate_str)
+        print_str = f"{species_str} adsorption on {substrate_str}"
         return print_str
 
     def construct(self):
-        if self.get_sites() == '1':
-            slabs_ads = self.Construct_single_adsorption()
-        elif self.get_sites() == '2':
+        if self.get_sites()[0] == '1':
+            if len(self.get_sites()) == 1:
+                slabs_ads = self.Construct_single_adsorption()
+            else:
+                ele = ''.join(self.get_sites()[1:]) ### wzj 20230518
+                slabs_ads = self.Construct_single_adsorption(ele=ele)
+        elif self.get_sites()[0] == '2':
             slabs_ads = self.Construct_double_adsorption()
         else:
             raise ValueError('Supports only "1" "2" adsorption sites for ads!')
 
         if self.substrate.is_dope():
             slabs_ads = self.remove_same(slabs_ads)
 
         return slabs_ads
 
     def remove_same(self, slabs_ads):
         # To choose the config whose neighbor list includes the doped atoms
-        p1 = self.substrate.property['p1']
-        p1_symb = self.substrate.property['p1_symb']
+        p1 = self.substrate.property["p1"]
+        p1_symb = self.substrate.property["p1_symb"]
         slabs_ads_near = []
         for slb in slabs_ads:
-            bind_adatoms, bind_adatoms_symb, bind_type_symb, adspecie, bind_surfatoms, bind_surfatoms_symb = \
-                get_binding_adatom(slb)
-            if self.get_sites() == '1' and (set(p1_symb) & set(bind_surfatoms_symb[0])):
+            (
+                bind_adatoms,
+                bind_adatoms_symb,
+                bind_type_symb,
+                adspecie,
+                bind_surfatoms,
+                bind_surfatoms_symb,
+            ) = get_binding_adatom(slb)
+            if self.get_sites() == "1" and (set(p1_symb) & set(bind_surfatoms_symb[0])):
                 slabs_ads_near += [slb]
-            elif self.get_sites() == '2' and \
-                    (set(p1_symb) & set(bind_surfatoms_symb[0])) or (set(p1_symb) & set(bind_surfatoms_symb[0])):
+            elif (
+                self.get_sites() == "2"
+                and (set(p1_symb) & set(bind_surfatoms_symb[0]))
+                or (set(p1_symb) & set(bind_surfatoms_symb[0]))
+            ):
                 slabs_ads_near += [slb]
         return slabs_ads_near
 
-    def Construct_single_adsorption(self):
+    def Construct_single_adsorption(self, ele=None):
         # generate surface adsorption configuration
         slab_ad = []
         slabs = self.substrate.construct()
         for i, slab in enumerate(slabs):
             site = AdsorptionSites(slab)
             coordinates = site.get_coordinates()
             builder = Builder(slab)
             ads_use = self.species[0].get_molecule()
-            for j, coord in enumerate(coordinates):
-                slab_ad += [builder._single_adsorption(ads_use, bond=0, site_index=j)]
+            if not ele is None:
+                chemical_symbols = np.array(ads_use.get_chemical_symbols())
+                bond_atom_ids = chemical_symbols[chemical_symbols==ele]
+                bond_atom_ids = np.where(chemical_symbols==ele)[0]
+                ### print('bond_atom_ids =', bond_atom_ids, bond_atom_ids.shape)
+                for j, coord in enumerate(coordinates):
+                    for bond_id in bond_atom_ids:
+                        slab_ad += [builder._single_adsorption(ads_use, bond=bond_id, site_index=j, direction_mode='decision_boundary')]
+                        #if len(bond_atom_ids) > 1:
+                        #    slab_ad += [builder._single_adsorption(ads_use, bond=bond_id, site_index=j, direction_mode='decision_boundary', direction_args=bond_atom_ids)]
+            else:
+                for j, coord in enumerate(coordinates):
+                    slab_ad += [builder._single_adsorption(ads_use, bond=0, site_index=j)]
         return slab_ad
 
     def Construct_double_adsorption(self):
         slab_ad = []
         slabs = self.substrate.construct()
         for i, slab in enumerate(slabs):
             site = AdsorptionSites(slab)
@@ -168,56 +143,67 @@
             ads_use = self.species[0].get_molecule()
             edges = site.get_adsorption_edges()
             for j, edge01 in enumerate(edges):
                 slab_ad += [builder._double_adsorption(ads_use, bonds=[0, 1], edge_index=j)]
         return slab_ad
 
     @classmethod
-    def from_input_dict(cls, init_dict):
-        spec1 = Species(init_dict['value'][0], init_dict['SML'])
-        sites = str(init_dict['value'][1])
-        substrate = init_dict['substrate']
-        return cls([spec1], [sites], substrate=substrate)
+    def from_input(cls, init_list, substrates, species_dict=None):
+        ads = []
+        for i in init_list:
+            spec1 = init_from_ads(i[0], species_dict)
+            sites1 = str(i[1])
+            for j in substrates:
+                ads.append(cls([spec1], list(sites1), substrate=j))
+        return ads
 
 
 class Coadsorption(Adsorption):
     def __init__(self, species: list, sites: list, spec_ads_stable=None, substrate=Slab()):
         super().__init__(species, sites, spec_ads_stable, substrate)
-        assert len(species) == 2, 'Coads need Two adsorption Species, but %d was given' % len(species)
+        assert len(species) == 2, "Coads need Two adsorption Species, but %d was given" % len(
+            species
+        )
 
     def construct(self):
-        if self.get_sites() == '1 1':
+        if self.get_sites() == "1 1":
             slabs_ads = self.Construct_coadsorption_11()
-        elif self.get_sites() == '1 2':
+        elif self.get_sites() == "1 2":
             slabs_ads = self.Construct_coadsorption_12()
-        elif self.get_sites() == '2 2':
+        elif self.get_sites() == "2 2":
             slabs_ads = self.Construct_coadsorption_22()
         else:
             raise ValueError('Supports only "1 1" "1 2" "2 2" adsorption sites for coads!')
         if self.substrate.is_dope():
             slabs_ads = self.remove_same(slabs_ads)
         return slabs_ads
 
     def out_file_name(self):
         ads = []
         for every_species in self.species:
             ads.append(every_species.out_file_name())
-        ads_str = '_'.join(ads)
+        ads_str = "_".join(ads)
         substrate_str = self.substrate.out_file_name()
-        vasp_file_str = '_'.join([substrate_str, ads_str])
+        vasp_file_str = "_".join([substrate_str, ads_str])
         return vasp_file_str
 
     def remove_same(self, slabs_ads):
         # To choose the config whose neighbor list includes the doped atoms
-        p1 = self.substrate.property['p1']
-        p1_symb = self.substrate.property['p1_symb']
+        p1 = self.substrate.property["p1"]
+        p1_symb = self.substrate.property["p1_symb"]
         slabs_ads_near = []
         for slb in slabs_ads:
-            bind_adatoms, bind_adatoms_symb, bind_type_symb, adspecie, bind_surfatoms, bind_surfatoms_symb = \
-                get_binding_adatom(slb)
+            (
+                bind_adatoms,
+                bind_adatoms_symb,
+                bind_type_symb,
+                adspecie,
+                bind_surfatoms,
+                bind_surfatoms_symb,
+            ) = get_binding_adatom(slb)
             bind_surfatoms_symb_all = sum(bind_surfatoms_symb, [])
             if set(p1_symb) & set(bind_surfatoms_symb_all):
                 slabs_ads_near += [slb]
         return slabs_ads_near
 
     def Construct_coadsorption_11(self):
         slab_ad = []
@@ -228,44 +214,57 @@
             site01 = AdsorptionSites(slab)
             builder01 = Builder(slab)
             coordinate01 = site01.get_coordinates()
             # generate surface adsorption configuration
             ads1_use = self.species[0].get_molecule()
             ads2_use = self.species[1].get_molecule()
             for k, sitetype in enumerate(site01.get_symmetric_sites()):
-                slab = builder01._single_adsorption(ads1_use, bond=0, site_index=k, auto_construct=True)
+                slab = builder01._single_adsorption(
+                    ads1_use, bond=0, site_index=k, auto_construct=True
+                )
                 coord01 = site01.get_coordinates()[k]
                 site02 = AdsorptionSites(slab)
                 coordinates02 = site02.get_coordinates()
                 for j, coord02 in enumerate(coordinates02):
                     dis = np.linalg.norm(coord01 - coord02)
                     if dis < float(dis_inter[0]):
                         continue
                     elif dis > float(dis_inter[1]):
                         continue
                     else:
                         builder02 = Builder(slab)
-                        slab_ad += [builder02._single_adsorption(ads2_use, bond=0, site_index=j, auto_construct=True)]
+                        slab_ad += [
+                            builder02._single_adsorption(
+                                ads2_use, bond=0, site_index=j, auto_construct=True
+                            )
+                        ]
 
-        typ = {None: 0, 'top': 1, 'bri': 2, 'fcc': 3, 'hcp': 3, '4-fold': 4}
+        typ = {None: 0, "top": 1, "bri": 2, "fcc": 3, "hcp": 3, "4-fold": 4}
         # view(slab_ad)
         slab_ad_final = []
         for j, adslab in enumerate(slab_ad):
-            bind_adatoms, bind_adatoms_symb, adspecie, bind_type_symb, bind_surfatoms, bind_surfatoms_symb = \
-                get_binding_adatom(adslab)
+            (
+                bind_adatoms,
+                bind_adatoms_symb,
+                adspecie,
+                bind_type_symb,
+                bind_surfatoms,
+                bind_surfatoms_symb,
+            ) = get_binding_adatom(adslab)
             adspecie_tmp, bind_type_symb_tmp = [], []
             for k, spe in enumerate(adspecie):
                 if spe in ads_type.keys():
                     adspecie_tmp += [spe]
                     bind_type_symb_tmp += [bind_type_symb[k]]
             if len(adspecie_tmp) < 2:
                 # print('Can not identify the config!')
                 slab_ad_final += [adslab]
             elif typ.get(bind_type_symb_tmp[0]) in ads_type.get(adspecie_tmp[0]) and typ.get(
-                    bind_type_symb_tmp[1]) in ads_type.get(adspecie_tmp[1]):
+                bind_type_symb_tmp[1]
+            ) in ads_type.get(adspecie_tmp[1]):
                 slab_ad_final += [adslab]
         return slab_ad_final
 
     def Construct_coadsorption_12(self):
         slab_ad = []
         slabs = self.substrate.construct()
         dis_inter = self.substrate.get_dis_inter()
@@ -306,15 +305,17 @@
                     dis = min(dis1, dis2)
 
                     if dis < dis_inter[0]:
                         continue
                     elif dis > dis_inter[1]:
                         continue
                     else:
-                        slab_ad += [builder02._double_adsorption(ads2_use, bonds=[0, 1], edge_index=j)]
+                        slab_ad += [
+                            builder02._double_adsorption(ads2_use, bonds=[0, 1], edge_index=j)
+                        ]
         return slab_ad
 
     def Construct_coadsorption_22(self):
         slab_ad = []
         dis_inter = self.substrate.get_dis_inter()
         slabs = self.substrate.construct()
         for i, slab in enumerate(slabs):
@@ -353,39 +354,57 @@
                     coord10 = dic_site02.get(edge[0])
                     coord11 = dic_site02.get(edge[1])
                     if not coord10 is None:
                         dis1 = np.linalg.norm(coord01 - coord10)
                     else:
                         dis1 = dis_inter[0] + 0.1
                     if not coord11 is None:
-                        dis2 = math.hypot(coord00[0] - coord11[0], coord00[1] - coord11[1], coord00[2] - coord11[2])
+                        dis2 = math.hypot(
+                            coord00[0] - coord11[0],
+                            coord00[1] - coord11[1],
+                            coord00[2] - coord11[2],
+                        )
                     else:
                         dis2 = dis_inter[1] + 0.1
                     dis = min(dis1, dis2)
 
                     if dis < dis_inter[0]:
                         continue
                     elif dis > dis_inter[1]:
                         continue
                     else:
-                        slab_ad += [builder02._double_adsorption(ads2_use, bonds=[0, 1], edge_index=j)]
+                        slab_ad += [
+                            builder02._double_adsorption(ads2_use, bonds=[0, 1], edge_index=j)
+                        ]
         return slab_ad
 
     @classmethod
-    def from_input_dict(cls, init_dict):
-        spec1 = Species(init_dict['value'][0], init_dict['SML'])
-        spec2 = Species(init_dict['value'][1], init_dict['SML'])
-        sites1 = str(init_dict['value'][2])
-        sites2 = str(init_dict['value'][3])
-        substrate = init_dict['substrate']
-        return cls([spec1, spec2], [sites1, sites2], substrate=substrate)
-
-
-def ads_from_input(init_dict):
-    # ads_init_dict = {'SML':False,'type':[],'value':[]}
-    if init_dict['type'] == 'coads':
-        ads = Coadsorption.from_input_dict(init_dict)
-    elif init_dict['type'] == 'ads':
-        ads = Adsorption.from_input_dict(init_dict)
-    else:
-        raise TypeError('Supports only "Ads" and "Coads" adsorption type!')
+    def from_input(cls, init_list, substrates, species_dict=None):
+        ads = []
+        for i in init_list:
+            spec1 = init_from_ads(i[0], species_dict)
+            spec2 = init_from_ads(i[1], species_dict)
+            sites1 = str(i[2])
+            sites2 = str(i[3])
+            for j in substrates:
+                ads.append(cls([spec1, spec2], [sites1, sites2], substrate=j))
+        return ads
+
+
+def ads_from_input(ads_model, substrate, species_dict=None):
+    ads = []
+    new_ads = []
+    ads_type_list = ["ads", "coads"]
+    for key, value in ads_model.items():
+        if key == "coads":
+            new_ads = Coadsorption.from_input(value, substrate, species_dict)
+        elif key == "ads":
+            new_ads = Adsorption.from_input(value, substrate, species_dict)
+        else:
+            msg = ",".join(ads_type_list)
+            warn_msg = (
+                "Only support species type: %s, Your input %s part in Species will be dismiss"
+                % (msg, key)
+            )
+            raise Warning(warn_msg)
+        ads = ads + new_ads
     return ads
```

### Comparing `HTMACat-1.0.4/HTMACat/post/Extract_adener.py` & `HTMACat-1.0.5/HTMACat/post/Extract_adener.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 import os
 import csv
-if __name__ == '__main__':
-    species = ['NH3', 'NH2', 'NH', 'N', 'O', 'OH', 'H2O', 'O2', 'H', 'NO', 'N2', 'N2O']
-    Efile = 'adsE_radical'
-    facets = ['100', '111']
-    ele = [['Ag', 'Au', 'Ir', 'Cu', 'Pd', 'Pt', 'Rh'],
-           ['Ag', 'Au', 'Ir', 'Cu', 'Pd', 'Pt', 'Rh', 'Ru']]
+
+if __name__ == "__main__":
+    species = ["NH3", "NH2", "NH", "N", "O", "OH", "H2O", "O2", "H", "NO", "N2", "N2O"]
+    Efile = "adsE_radical"
+    facets = ["100", "111"]
+    ele = [
+        ["Ag", "Au", "Ir", "Cu", "Pd", "Pt", "Rh"],
+        ["Ag", "Au", "Ir", "Cu", "Pd", "Pt", "Rh", "Ru"],
+    ]
     ### extract the adsorption energy of the most stable configuration
     for i, facet in enumerate(facets):
         for j in ele[i]:
             Dir = os.getcwd()
-            Dir1 = f'/data3/home/jqyang/surface/{j}/{facet}/surface-adsorption/'
+            Dir1 = f"/data3/home/jqyang/surface/{j}/{facet}/surface-adsorption/"
             os.chdir(Dir1)
-            print(f'------{j}--{facet}------')
-            fads = open('ads_final', 'w+')
+            print(f"------{j}--{facet}------")
+            fads = open("ads_final", "w+")
             for specie in species:
-                print(f'{specie}')
+                print(f"{specie}")
                 spe, ene = get_adsorption_energy_stable(Efile, specie)
-                fads.write(f'{spe},{ene}\n')
+                fads.write(f"{spe},{ene}\n")
             fads.close()
             os.chdir(Dir)
     ### extract the adsorption energy of the most stable configuration
-    fads0 = open('ads_all.csv', 'w+')
+    fads0 = open("ads_all.csv", "w+")
     writer = csv.writer(fads0)
-    writer.writerow(['sys', 'Eads'])
+    writer.writerow(["sys", "Eads"])
     for specie in species:
         for i, facet in enumerate(facets):
             for j in ele[i]:
                 Dir = os.getcwd()
-                Dir1 = f'/data3/home/jqyang/surface/{j}/{facet}/surface-adsorption/'
+                Dir1 = f"/data3/home/jqyang/surface/{j}/{facet}/surface-adsorption/"
                 os.chdir(Dir1)
-                fads1 = open('ads_final', 'r+')
+                fads1 = open("ads_final", "r+")
                 for k, ads_ene in enumerate(fads1):
-                    spe = ads_ene.split(',')[0]
-                    ene = ads_ene.split(',')[1].strip()
-                    if len(spe.split('_')) < 2:
-                        spe1 = spe.split('_')[0]
+                    spe = ads_ene.split(",")[0]
+                    ene = ads_ene.split(",")[1].strip()
+                    if len(spe.split("_")) < 2:
+                        spe1 = spe.split("_")[0]
                     else:
-                        spe1 = spe.split('_')[-2]
-                    #ene=ads_ene.split(',')[1].strip()
+                        spe1 = spe.split("_")[-2]
+                    # ene=ads_ene.split(',')[1].strip()
                     print(spe1, ene)
                     if spe1 == specie:
                         tmp = [spe, ene]
                         writer.writerow(tmp)
                 fads1.close()
                 os.chdir(Dir)
     fads0.close()
```

### Comparing `HTMACat-1.0.4/HTMACat/post/Extract_adener_alloy.py` & `HTMACat-1.0.5/HTMACat/post/Extract_adener_alloy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 import os
 import csv
-if __name__ == '__main__':
-    #species=['N','O']
-    #species=['NH3','NH2','NH','N','O','OH','H','H2O','O2','NO','N2O','N2']
-    species = ['NH3', 'NH2', 'NH', 'N', 'O', 'OH', 'H']
-    #dop_typs=['1','1L','2','4']
-    dop_typs = ['1', '1L', '2', '3']
-    Efile = 'adsE_radical_all'
-    facets = ['111']
-    ele = [['Ag', 'Au', 'Cu', 'Pd', 'Pt', 'Ir', 'Rh']]
-    #facets=['100','111']
-    #ele=[['Ag','Au','Ir','Cu','Pd','Pt','Rh'],['Ag','Au','Ir','Cu','Pd','Pt','Rh','Ru']]
+
+if __name__ == "__main__":
+    # species=['N','O']
+    # species=['NH3','NH2','NH','N','O','OH','H','H2O','O2','NO','N2O','N2']
+    species = ["NH3", "NH2", "NH", "N", "O", "OH", "H"]
+    # dop_typs=['1','1L','2','4']
+    dop_typs = ["1", "1L", "2", "3"]
+    Efile = "adsE_radical_all"
+    facets = ["111"]
+    ele = [["Ag", "Au", "Cu", "Pd", "Pt", "Ir", "Rh"]]
+    # facets=['100','111']
+    # ele=[['Ag','Au','Ir','Cu','Pd','Pt','Rh'],['Ag','Au','Ir','Cu','Pd','Pt','Rh','Ru']]
 
     for dop_typ in dop_typs:
         ### extract the adsorption energy of the most stable configuration
         for i, facet in enumerate(facets):
             for j in ele[i]:
-                if j == 'Ru':
+                if j == "Ru":
                     continue
                 else:
                     for k in ele[i]:
                         if j == k:
                             continue
                         else:
                             Dir = os.getcwd()
-                            Dir1 = f'/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/'
+                            Dir1 = f"/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/"
                             os.chdir(Dir1)
-                            print(f'------{j}{k}--{facet}------')
-                            fads = open(f'ads_final_{dop_typ}', 'w+')
+                            print(f"------{j}{k}--{facet}------")
+                            fads = open(f"ads_final_{dop_typ}", "w+")
                             for specie in species:
-                                #print(dop_typ)
-                                print(f'{specie}')
+                                # print(dop_typ)
+                                print(f"{specie}")
                                 spe, ene = get_adsorption_energy_stable(Efile, specie, dop_typ)
-                                #poscar=f'{spe}/CONTCAR'
-                                #bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(poscar)
-                                fads.write(f'{spe},{ene}\n')
-                                #print(spe,ene,bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
+                                # poscar=f'{spe}/CONTCAR'
+                                # bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb=get_binding_adatom(poscar)
+                                fads.write(f"{spe},{ene}\n")
+                                # print(spe,ene,bind_adatoms,bind_adatoms_symb,adspecie,bind_type_symb,bind_surfatoms,bind_surfatoms_symb)
                             fads.close()
                             os.chdir(Dir)
         ### extract the adsorption energy of the most stable configuration
-        fads0 = open(f'ads_all_alloy_{facets[0]}_{dop_typ}.csv', 'w+')
+        fads0 = open(f"ads_all_alloy_{facets[0]}_{dop_typ}.csv", "w+")
         writer = csv.writer(fads0)
-        writer.writerow(['sys', 'Eads'])
+        writer.writerow(["sys", "Eads"])
         for specie in species:
             for i, facet in enumerate(facets):
                 for j in ele[i]:
-                    if j == 'Ru':
+                    if j == "Ru":
                         continue
                     else:
                         for k in ele[i]:
                             if j == k:
                                 continue
                             else:
                                 Dir = os.getcwd()
-                                Dir1 = f'/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/'
+                                Dir1 = f"/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/"
                                 os.chdir(Dir1)
-                                fads1 = open(f'ads_final_{dop_typ}', 'r+')
+                                fads1 = open(f"ads_final_{dop_typ}", "r+")
                                 for m, ads_ene in enumerate(fads1):
-                                    spe = ads_ene.split(',')[0]
-                                    ene = ads_ene.split(',')[1].strip()
-                                    if len(spe.split('_')) < 2:
-                                        spe1 = spe.split('_')[0]
+                                    spe = ads_ene.split(",")[0]
+                                    ene = ads_ene.split(",")[1].strip()
+                                    if len(spe.split("_")) < 2:
+                                        spe1 = spe.split("_")[0]
                                     else:
-                                        spe1 = spe.split('_')[-2]
-                                        typ = spe.split('_')[-3]
+                                        spe1 = spe.split("_")[-2]
+                                        typ = spe.split("_")[-3]
 
                                     if (spe1 == specie) & (typ == dop_typ):
                                         tmp = [spe, ene]
                                         writer.writerow(tmp)
                                 fads1.close()
                                 os.chdir(Dir)
         fads0.close()
 
         ### to arrange the binding energy info
-        fads2 = open(f'ads_all_alloy_{facets[0]}_{dop_typ}_arr.csv', 'w+')
+        fads2 = open(f"ads_all_alloy_{facets[0]}_{dop_typ}_arr.csv", "w+")
         writer2 = csv.writer(fads2)
-        writer2.writerow(['sys', 'E(NH3)', 'E(NH2)', 'E(NH)', 'E(N)', 'E(O)', 'E(OH)', 'E(H)'])
+        writer2.writerow(["sys", "E(NH3)", "E(NH2)", "E(NH)", "E(N)", "E(O)", "E(OH)", "E(H)"])
 
         for i, facet in enumerate(facets):
             for j in ele[i]:
-                if j == 'Ru':
+                if j == "Ru":
                     continue
                 else:
                     for k in ele[i]:
                         if j == k:
                             continue
                         else:
                             Dir = os.getcwd()
-                            Dir1 = f'/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/'
+                            Dir1 = f"/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/"
                             os.chdir(Dir1)
-                            name = '_'.join([j, k, facet, dop_typ])
+                            name = "_".join([j, k, facet, dop_typ])
                             row = []
                             row += [name]
 
                             for specie in species:
-                                fads1 = open(f'ads_final_{dop_typ}', 'r+')
+                                fads1 = open(f"ads_final_{dop_typ}", "r+")
                                 for m, ads_ene in enumerate(fads1):
-                                    spe = ads_ene.split(',')[0]
-                                    ene = ads_ene.split(',')[1].strip()
-                                    if len(spe.split('_')) < 2:
-                                        spe1 = spe.split('_')[0]
+                                    spe = ads_ene.split(",")[0]
+                                    ene = ads_ene.split(",")[1].strip()
+                                    if len(spe.split("_")) < 2:
+                                        spe1 = spe.split("_")[0]
                                     else:
-                                        spe1 = spe.split('_')[-2]
-                                        typ = spe.split('_')[-3]
+                                        spe1 = spe.split("_")[-2]
+                                        typ = spe.split("_")[-3]
                                     if (spe1 == specie) & (typ == dop_typ):
                                         row += [ene]
                                 fads1.close()
                             os.chdir(Dir)
-                            #row +=['\n']
+                            # row +=['\n']
                             writer2.writerow(row)
         fads2.close()
```

### Comparing `HTMACat-1.0.4/HTMACat/post/Extract_adener_site.py` & `HTMACat-1.0.5/HTMACat/post/Extract_adener_site.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 import os
 import csv
-if __name__ == '__main__':
-    species = ['N', 'O']
-    dop_typs = ['b1']
-    Efile = 'ads_final_b1'
 
-    facets = ['100']
-    ele = [['Ag', 'Au', 'Cu', 'Pd', 'Pt', 'Ir', 'Rh', 'Ru']]
+if __name__ == "__main__":
+    species = ["N", "O"]
+    dop_typs = ["b1"]
+    Efile = "ads_final_b1"
+
+    facets = ["100"]
+    ele = [["Ag", "Au", "Cu", "Pd", "Pt", "Ir", "Rh", "Ru"]]
 
     for dop_typ in dop_typs:
         ### extract the adsorption energy of the most stable configuration
-        fads0 = open(f'ads_all_alloy_{facets[0]}_{dop_typ}_site.csv', 'w+')
+        fads0 = open(f"ads_all_alloy_{facets[0]}_{dop_typ}_site.csv", "w+")
         writer = csv.writer(fads0)
-        writer.writerow(['sys', 'site', 'surfatoms'])
+        writer.writerow(["sys", "site", "surfatoms"])
         for specie in species:
             for i, facet in enumerate(facets):
                 for j in ele[i]:
-                    if j == 'Ru':
+                    if j == "Ru":
                         continue
                     else:
                         for k in ele[i]:
                             if j == k:
                                 continue
                             else:
                                 Dir = os.getcwd()
-                                Dir1 = f'/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/'
+                                Dir1 = f"/data3/home/jqyang/surface/{j}{k}/{facet}/surface-adsorption/"
                                 os.chdir(Dir1)
-                                print(f'{j}{k}-{facet}')
-                                spec_ads, spec_ads_stable, dir_list_final, spec_ads_stable_surfa = get_site_stable(
-                                    Efile, Ecut=-0.1)
+                                print(f"{j}{k}-{facet}")
+                                (
+                                    spec_ads,
+                                    spec_ads_stable,
+                                    dir_list_final,
+                                    spec_ads_stable_surfa,
+                                ) = get_site_stable(Efile, Ecut=-0.1)
                                 for k, sys in enumerate(dir_list_final):
-                                    spe = (sys.split('_')[-2])
-                                    dop = (sys.split('_')[-3])
+                                    spe = sys.split("_")[-2]
+                                    dop = sys.split("_")[-3]
                                     if (spe == specie) & (dop in dop_typ):
                                         tmp = [
                                             sys,
                                             spec_ads_stable.get(spe),
-                                            spec_ads_stable_surfa.get(spe)
+                                            spec_ads_stable_surfa.get(spe),
                                         ]
                                         writer.writerow(tmp)
 
                                 os.chdir(Dir)
         fads0.close()
```

### Comparing `HTMACat-1.0.4/HTMACat/post/Extract_cal_fre.py` & `HTMACat-1.0.5/HTMACat/post/Extract_cal_fre.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,92 @@
-# -*- coding: UTF-8 -*-
 from ase import io
 from ase.constraints import FixAtoms
 import os
 from ase.io.vasp import write_vasp, read_vasp
 
 
 def get_file_name(reaction):
-    specie_f = reaction.split('=')[0].strip()
-    specie_b = reaction.split('=')[1].strip()
+    specie_f = reaction.split("=")[0].strip()
+    specie_b = reaction.split("=")[1].strip()
     ### Construct the reaction name
     ##1.Extract the reactant molecule and type (a g s)
     specie_f_list = []
-    for i in range(len(specie_f.split('+'))):
-        specie_f_list += [specie_f.split('+')[i].strip()]
+    for i in range(len(specie_f.split("+"))):
+        specie_f_list += [specie_f.split("+")[i].strip()]
     specie_f_mol = []
     specie_f_typ = []
     for j, specie in enumerate(specie_f_list):
-        specie_f_mol += [specie.split('(', 1)[0].strip()]
-        specie_f_typ += [specie.split('(', 1)[1].split(')')[0].strip()]
+        specie_f_mol += [specie.split("(", 1)[0].strip()]
+        specie_f_typ += [specie.split("(", 1)[1].split(")")[0].strip()]
     ##2.Extract the product molecule and type (a g s)
     specie_b_list = []
-    for i in range(len(specie_b.split('+'))):
-        specie_b_list += [specie_b.split('+')[i].strip()]
+    for i in range(len(specie_b.split("+"))):
+        specie_b_list += [specie_b.split("+")[i].strip()]
     specie_b_mol = []
     specie_b_typ = []
     for j, specie in enumerate(specie_b_list):
-        specie_b_mol += [specie.split('(', 1)[0].strip()]
-        specie_b_typ += specie.split('(', 1)[1].split(')')[0].strip()
+        specie_b_mol += [specie.split("(", 1)[0].strip()]
+        specie_b_typ += specie.split("(", 1)[1].split(")")[0].strip()
     ##3.construct the file name for every reaction
-    File = '+'.join(specie_f_mol) + '=' + '+'.join(specie_b_mol)
+    File = "+".join(specie_f_mol) + "=" + "+".join(specie_b_mol)
     return File
 
 
-def get_adspecie_dir(react='react.log'):
+def get_adspecie_dir(react="react.log"):
     ### Extract reaction info
     ##1.Extract reaction type,reactant info,product info,barrier & enthalpy
-    react_info = open(react, 'r+')
+    react_info = open(react, "r+")
     reaction_info = react_info.readlines()
     if len(reaction_info) > 2:
         reaction_type = reaction_info[0]
-        reactant_info = reaction_info[1].split(',')[0].split('=')[0]
-        product_info = reaction_info[1].split(',')[1].split('=')[0]
-        #print(reactant_info,product_info)
+        reactant_info = reaction_info[1].split(",")[0].split("=")[0]
+        product_info = reaction_info[1].split(",")[1].split("=")[0]
+        # print(reactant_info,product_info)
         return reactant_info, product_info
     react_info.close()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     ### Extract the dir
     ReaInfo = open("reaction-bk", "r+")
     dir_list = []
     for index, line in enumerate(ReaInfo):
         File = get_file_name(line)
         Dir = os.getcwd()
         os.chdir(File)
-        reactant_info, product_info = get_adspecie_dir(react='react.log')
+        reactant_info, product_info = get_adspecie_dir(react="react.log")
         dir_list += [reactant_info, product_info]
         os.chdir(Dir)
     ReaInfo.close()
-    #print(len(dir_list))
-    #print(len(list(set(dir_list))))
+    # print(len(dir_list))
+    # print(len(list(set(dir_list))))
     dir_list = list(set(dir_list))
 
     ### output ###
     Flist = open("file_list", "w+")
     for i in dir_list:
-        Flist.write(f'{i}\n')
+        Flist.write(f"{i}\n")
     Flist.close()
     ### construct cal dir
     dcut = 0.68
     Dir_temp = os.getcwd()
     for j in dir_list:
         print(j)
-        os.chdir(f'../test/{j}')
-        os.system('rm -rf fre-cal')
-        #os.chdir(f'../surface-adsorption/{Dir}')
-        os.system('cp -r optmk fre-cal')
-        os.chdir('fre-cal')
+        os.chdir(f"../test/{j}")
+        os.system("rm -rf fre-cal")
+        # os.chdir(f'../surface-adsorption/{Dir}')
+        os.system("cp -r optmk fre-cal")
+        os.chdir("fre-cal")
         print(os.getcwd())
-        os.system('mv CONTCAR POSCAR')
-        pos = io.read('POSCAR', format='vasp')
+        os.system("mv CONTCAR POSCAR")
+        pos = io.read("POSCAR", format="vasp")
         Mask = []
         for j in pos.get_scaled_positions():
             z = j[2]
             if float(z) > float(dcut):
                 Mask += [False]
             else:
                 Mask += [True]
         constraint = FixAtoms(mask=Mask)
         pos.set_constraint(constraint)
-        write_vasp('POSCAR', pos, direct=True, sort=[''], vasp5=True)
+        write_vasp("POSCAR", pos, direct=True, sort=[""], vasp5=True)
         os.chdir(Dir_temp)
```

### Comparing `HTMACat-1.0.4/HTMACat/post/cal_adsE.py` & `HTMACat-1.0.5/HTMACat/post/cal_adsE.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,179 +1,180 @@
-# -*- coding: UTF-8 -*-
 from HTMACat.Extract_info import *
 import sys
 
 
 ## calculate the energy of radical
 def cal_Erad(FErad, Radical):
     Erad = 0
-    with open(FErad, 'r+') as Eradicals:
+    with open(FErad, "r+") as Eradicals:
         for i, Eradical in enumerate(Eradicals):
-            radical = Eradical.split(',')[0]
-            E = Eradical.split(',')[1].strip()
+            radical = Eradical.split(",")[0]
+            E = Eradical.split(",")[1].strip()
             # find the atom energy
             if Radical == radical:
-                #print(i,radical)
+                # print(i,radical)
                 Erad = float(Erad) + float(E)
     return Erad
 
 
 ## calculate the energy of radical relative to atom energy: ExCyHzO=xEC+yEH+zEO
 def cal_Erad_atom(FErad, Radical):
     Erad = 0
     rad = molecule(Radical)
     for i in rad.get_chemical_symbols():
-        with open(FErad, 'r+') as Eradicals:
+        with open(FErad, "r+") as Eradicals:
             for j, Eradical in enumerate(Eradicals):
-                radical = Eradical.split(',')[0]
-                E = Eradical.split(',')[1].strip()
+                radical = Eradical.split(",")[0]
+                E = Eradical.split(",")[1].strip()
                 # find the atom energy
                 if i == radical:
-                    #print(i,radical)
+                    # print(i,radical)
                     Erad = float(Erad) + float(E)
     return Erad
 
 
 def cal_Eslab(FEslab, facet):
     E_slab = 0
-    with open(FEslab, 'r+') as Eslabs:
+    with open(FEslab, "r+") as Eslabs:
         for i, Eslab in enumerate(Eslabs):
-            slab = Eslab.split(',')[0].split('_')[0:-1]
-            E = Eslab.split(',')[1]
+            slab = Eslab.split(",")[0].split("_")[0:-1]
+            E = Eslab.split(",")[1]
             # find the facet energy
             if facet == slab:
-                #print(slab)
+                # print(slab)
                 E_slab = float(E)
     return E_slab
 
 
 ## calculate the adE with  atom energy: E(xCyHzO)ad=ECHOsurf-Esurf-xEC-yEH-zEO
-def cal_Eads(Flist, FErad, FEslab, radicals, Erad_property='radical', Facet_property='all'):
-    EnerInfo = open(Flist, 'r+')
-    Foutput = open(f'adsE_{Erad_property}_{Facet_property}', 'w+')
-    #num=0
+def cal_Eads(Flist, FErad, FEslab, radicals, Erad_property="radical", Facet_property="all"):
+    EnerInfo = open(Flist, "r+")
+    Foutput = open(f"adsE_{Erad_property}_{Facet_property}", "w+")
+    # num=0
     for i, ads_ener in enumerate(EnerInfo):
         # extract the facet and radical
-        conf = ads_ener.split(',', 1)[0]
-        conf_facet = conf.split('_')[0:-2]
-        conf_radical = conf.split('_')[-2]
+        conf = ads_ener.split(",", 1)[0]
+        conf_facet = conf.split("_")[0:-2]
+        conf_radical = conf.split("_")[-2]
         # extract the energy of adsorption configuration
-        Eads = ads_ener.split(',', 1)[1].strip()
+        Eads = ads_ener.split(",", 1)[1].strip()
         print(conf)
         if Eads:
             E_rad, E_slab = 0, 0
             if conf_radical in radicals:
-                #if conf.split('_')[-3] == 'b1':
+                # if conf.split('_')[-3] == 'b1':
                 #   num=num+1
-                #else:
+                # else:
                 #   num=num
                 ## extract the energy of radical based atom energy
-                if Erad_property == 'atom':
+                if Erad_property == "atom":
                     E_rad = cal_Erad_atom(FErad, conf_radical)
-                elif Erad_property == 'radical':
+                elif Erad_property == "radical":
                     E_rad = cal_Erad(FErad, conf_radical)
                 else:
-                    print('Erad has not the property!')
+                    print("Erad has not the property!")
                     break
 
                 ##  extract the energy of facet
-                with open(FEslab, 'r+') as Eslabs:
+                with open(FEslab, "r+") as Eslabs:
                     for j, Eslab in enumerate(Eslabs):
-                        line1 = Eslab.split('[')[0]
-                        Ftmp = line1.split(',')
-                        conf_slab = Ftmp[0].split('_')[0:-1]
-                        line2 = [eval(i) for i in Eslab.split('[')[1].split(']')[0].split(',')]
-                        #print(Ftmp[2])
-                        #print(Ftmp[2]== 'True')
+                        line1 = Eslab.split("[")[0]
+                        Ftmp = line1.split(",")
+                        conf_slab = Ftmp[0].split("_")[0:-1]
+                        line2 = [eval(i) for i in Eslab.split("[")[1].split("]")[0].split(",")]
+                        # print(Ftmp[2])
+                        # print(Ftmp[2]== 'True')
                         if conf_slab == conf_facet:
-                            poscar = f'./poscar/{conf}.vasp'
-                            adatoms, adatoms_symb, surfatoms, surfatoms_symb, subsurfatoms, subsurfatoms_symb = distinguish_atom_binding(
+                            poscar = f"./poscar/{conf}.vasp"
+                            (
+                                adatoms,
+                                adatoms_symb,
+                                surfatoms,
+                                surfatoms_symb,
+                                subsurfatoms,
+                                subsurfatoms_symb,
+                            ) = distinguish_atom_binding(
                                 poscar,
                                 tol=0.05,
                                 base_layer=int(Ftmp[3]),
-                                atoms_layer=int(float(Ftmp[4])))
+                                atoms_layer=int(float(Ftmp[4])),
+                            )
                             if line2 == surfatoms_symb:
-                                if Facet_property == 'all':
+                                if Facet_property == "all":
                                     E_slab = Ftmp[1]
-                                elif (Facet_property == 'stable') & (Ftmp[2] == 'True'):
+                                elif (Facet_property == "stable") & (Ftmp[2] == "True"):
                                     E_slab = Ftmp[1]
                                 else:
                                     continue
                             else:
                                 continue
                         else:
                             continue
             else:
                 continue
 
             if E_slab:
                 Eads = Extract_adsE(slab_E=E_slab, radical_E=E_rad, tot_E=Eads)
-                #print(conf,Eads)
-                Foutput.write(f'{conf},{Eads}\n')
+                # print(conf,Eads)
+                Foutput.write(f"{conf},{Eads}\n")
             else:
-                print('NO Eslab')
+                print("NO Eslab")
         else:
-            print(f'{conf} is not calculated!')
-    #print(f'Species: {num}')
+            print(f"{conf} is not calculated!")
+    # print(f'Species: {num}')
     EnerInfo.close()
     Foutput.close()
 
 
-def cal_adE_coad(Flist, FErad, FEslab, Erad_property='radical'):
-    EnerInfo = open(Flist, 'r+')
-    Foutput = open(f'adsE_coad_{Erad_property}', 'w+')
+def cal_adE_coad(Flist, FErad, FEslab, Erad_property="radical"):
+    EnerInfo = open(Flist, "r+")
+    Foutput = open(f"adsE_coad_{Erad_property}", "w+")
 
     for i, ads_ener in enumerate(EnerInfo):
+        conf = ads_ener.split(",", 1)[0]
+        Eads = ads_ener.split(",", 1)[1].strip()
+        conf_facet = conf.split("_")[0:-3]
+        conf_radicals = conf.split("_")[-3:-1]
 
-        conf = ads_ener.split(',', 1)[0]
-        Eads = ads_ener.split(',', 1)[1].strip()
-        conf_facet = conf.split('_')[0:-3]
-        conf_radicals = conf.split('_')[-3:-1]
-
-        #if Eads and len(conf.split('_')) > 4:
-        #if Eads and len(conf.split('_')) > 3:
+        # if Eads and len(conf.split('_')) > 4:
+        # if Eads and len(conf.split('_')) > 3:
         if Eads:
-            #print(Eads,len(conf.split('_')))
+            # print(Eads,len(conf.split('_')))
             E_rad, E_slab = 0, 0
             E_slab = cal_Eslab(FEslab, conf_facet)
-            if Erad_property == 'atom':
+            if Erad_property == "atom":
                 for i, conf_radical in enumerate(conf_radicals):
                     ## extract the energy of radical based atom energy
                     E_rad = float(E_rad) + float(cal_Erad_atom(FErad, conf_radical))
-            elif Erad_property == 'radical':
+            elif Erad_property == "radical":
                 for i, conf_radical in enumerate(conf_radicals):
                     E_rad = float(E_rad) + float(cal_Erad(FErad, conf_radical))
             else:
-                print('Erad has not the property!')
+                print("Erad has not the property!")
                 break
 
             Eads = Extract_adsE(slab_E=E_slab, radical_E=E_rad, tot_E=Eads)
             print(conf, Eads)
-            Foutput.write(f'{conf},{Eads}\n')
+            Foutput.write(f"{conf},{Eads}\n")
         else:
-            print(f'{conf} is not calculated!')
+            print(f"{conf} is not calculated!")
     EnerInfo.close()
     Foutput.close()
 
 
-if __name__ == '__main__':
-    '''
-   poscar=f'./poscar/Au_Cu_100_b1_N_7.vasp'
-   adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsurfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol=0.05,base_layer=4,atoms_layer=8)
-   print(surfatoms_symb)
-   '''
+if __name__ == "__main__":
+    """poscar=f'./poscar/Au_Cu_100_b1_N_7.vasp' adatoms,adatoms_symb,surfatoms,surfatoms_symb,subsu
+    rfatoms,subsurfatoms_symb=distinguish_atom_binding(poscar,tol=0.05,base_layer=4,atoms_layer=8)
+    print(surfatoms_symb)"""
 
     Flist = "energy_list.csv"
     FErad = "/data3/home/jqyang/general-script/energy_radical"
     FEslab = "/data3/home/jqyang/general-script/energy_facet_f"
-    #radicals=['NH3','NH2','NH','N','O','OH','H2O','O2','NO','N2O','N2','H']
-    #radicals=['N','O']
-    #radicals=['NH3','NH2','NH','N','O','OH','H','H2O','O2','NO','N2O','N2']
-    radicals = ['NH3', 'NH2', 'NH', 'N', 'O', 'OH', 'H', 'NO', 'N2O', 'N2']
-    #cal_Eads(Flist,FErad,FEslab,radicals,Erad_property='radical',Facet_property='all')
-    cal_Eads(Flist, FErad, FEslab, radicals, Erad_property='radical', Facet_property='stable')
-    '''
-   Flist="energy_list_coad.csv"
-   FErad="/data3/home/jqyang/general-script/energy_radical"
-   FEslab="/data3/home/jqyang/general-script/energy_facet"
-   cal_adE_coad(Flist,FErad,FEslab,Erad_property='radical')
-   '''
+    # radicals=['NH3','NH2','NH','N','O','OH','H2O','O2','NO','N2O','N2','H']
+    # radicals=['N','O']
+    # radicals=['NH3','NH2','NH','N','O','OH','H','H2O','O2','NO','N2O','N2']
+    radicals = ["NH3", "NH2", "NH", "N", "O", "OH", "H", "NO", "N2O", "N2"]
+    # cal_Eads(Flist,FErad,FEslab,radicals,Erad_property='radical',Facet_property='all')
+    cal_Eads(Flist, FErad, FEslab, radicals, Erad_property="radical", Facet_property="stable")
+    """Flist="energy_list_coad.csv" FErad="/data3/home/jqyang/general-script/energy_radical"
+    FEslab="/data3/home/jqyang/general-script/energy_facet"
+    cal_adE_coad(Flist,FErad,FEslab,Erad_property='radical')"""
```

### Comparing `HTMACat-1.0.4/HTMACat.egg-info/SOURCES.txt` & `HTMACat-1.0.5/HTMACat.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 HTMACat/Base_tools.py
 HTMACat/Extract_info.py
 HTMACat/IO.py
 HTMACat/__init__.py
+HTMACat/__version__.py
 HTMACat/command.py
 HTMACat/configuration.py
 HTMACat.egg-info/PKG-INFO
 HTMACat.egg-info/SOURCES.txt
 HTMACat.egg-info/dependency_links.txt
 HTMACat.egg-info/entry_points.txt
 HTMACat.egg-info/requires.txt
@@ -23,33 +24,40 @@
 HTMACat/NEB/vaspneb6.py
 HTMACat/catkit/__init__.py
 HTMACat/catkit/build.py
 HTMACat/catkit/gratoms.py
 HTMACat/catkit/data/__init__.py
 HTMACat/catkit/gen/__init__.py
 HTMACat/catkit/gen/adsorption.py
-HTMACat/catkit/gen/molecules.py
 HTMACat/catkit/gen/surface.py
 HTMACat/catkit/gen/symmetry.py
 HTMACat/catkit/gen/utils/__init__.py
 HTMACat/catkit/gen/utils/connectivity.py
 HTMACat/catkit/gen/utils/coordinates.py
 HTMACat/catkit/gen/utils/graph.py
 HTMACat/catkit/gen/utils/utilities.py
+HTMACat/catkit/gen/utils/utils_mdnm.py
 HTMACat/catkit/gen/utils/vectors.py
 HTMACat/descriptor/Construct_descriptor.py
 HTMACat/descriptor/Construct_descriptor_NEB.py
 HTMACat/descriptor/Construct_descriptor_coad.py
 HTMACat/descriptor/Construct_descriptor_surface.py
 HTMACat/descriptor/Construct_descriptor_surface_single.py
 HTMACat/descriptor/__init__.py
 HTMACat/model/Ads.py
 HTMACat/model/Construct_adsorption_yaml.py
+HTMACat/model/Species.py
 HTMACat/model/Structure.py
 HTMACat/model/Substrate.py
 HTMACat/model/__init__.py
 HTMACat/post/Extract_adener.py
 HTMACat/post/Extract_adener_alloy.py
 HTMACat/post/Extract_adener_site.py
 HTMACat/post/Extract_cal_fre.py
 HTMACat/post/__init__.py
-HTMACat/post/cal_adsE.py
+HTMACat/post/cal_adsE.py
+test/test_IO.py
+test/test_adsorption.py
+test/test_bulk.py
+test/test_coadsorption.py
+test/test_slab.py
+test/test_species.py
```

### Comparing `HTMACat-1.0.4/LICENSE` & `HTMACat-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <http://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

