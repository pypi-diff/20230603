# Comparing `tmp/Chiplotle3-0.4.2.tar.gz` & `tmp/Chiplotle3-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chiplotle3-0.4.2.tar", last modified: Wed May  4 21:20:47 2022, max compression
+gzip compressed data, was "Chiplotle3-0.4.3.tar", last modified: Sat Jun  3 12:21:04 2023, max compression
```

## Comparing `Chiplotle3-0.4.2.tar` & `Chiplotle3-0.4.3.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.136343 Chiplotle3-0.4.2/
--rw-r--r--   0 cyprienh   (501) staff       (20)    35147 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/LICENSE
--rw-r--r--   0 cyprienh   (501) staff       (20)     2036 2022-05-04 21:20:47.136660 Chiplotle3-0.4.2/PKG-INFO
--rw-r--r--   0 cyprienh   (501) staff       (20)     1509 2022-05-04 21:20:06.000000 Chiplotle3-0.4.2/README.md
--rw-r--r--   0 cyprienh   (501) staff       (20)       84 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/pyproject.toml
--rw-r--r--   0 cyprienh   (501) staff       (20)     1064 2022-05-04 21:20:47.138528 Chiplotle3-0.4.2/setup.cfg
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.020250 Chiplotle3-0.4.2/src/
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.027734 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/
--rw-r--r--   0 cyprienh   (501) staff       (20)     2036 2022-05-04 21:20:46.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/PKG-INFO
--rw-r--r--   0 cyprienh   (501) staff       (20)    10488 2022-05-04 21:20:47.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/SOURCES.txt
--rw-r--r--   0 cyprienh   (501) staff       (20)        1 2022-05-04 21:20:46.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/dependency_links.txt
--rw-r--r--   0 cyprienh   (501) staff       (20)       81 2022-05-04 21:20:46.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/entry_points.txt
--rw-r--r--   0 cyprienh   (501) staff       (20)       28 2022-05-04 21:20:46.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/requires.txt
--rw-r--r--   0 cyprienh   (501) staff       (20)       11 2022-05-04 21:20:46.000000 Chiplotle3-0.4.2/src/Chiplotle3.egg-info/top_level.txt
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.028105 Chiplotle3-0.4.2/src/chiplotle3/
--rw-r--r--   0 cyprienh   (501) staff       (20)     1482 2022-05-04 20:57:34.000000 Chiplotle3-0.4.2/src/chiplotle3/__init__.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.028800 Chiplotle3-0.4.2/src/chiplotle3/core/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/__init__.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.032055 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      860 2022-05-04 21:00:12.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/_run_chiplotle.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      937 2022-05-04 21:00:03.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/_run_chiplotle_virtual.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      339 2022-05-04 21:20:30.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/cfg.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      771 2022-05-04 21:00:14.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/get_config_value.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1002 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/initialize_files.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      332 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/read_config_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2909 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/write_config_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)       78 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/cfg/write_log_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      734 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/errors.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.033479 Chiplotle3-0.4.2/src/chiplotle3/core/imports/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/imports/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      529 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/imports/get_functions_in_module.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1005 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/imports/package_import.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      212 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/imports/remove_modules_from_namespace.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.034948 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      492 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/formatdecorator.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      118 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/interface.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.035747 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/margins/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/margins/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      723 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/margins/interface.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.036372 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/parentage/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/parentage/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      865 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/parentage/interface.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      528 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/core/visitor.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.039624 Chiplotle3-0.4.2/src/chiplotle3/examples/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3168 2022-05-04 20:57:40.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece.py
--rwxr-xr-x   0 cyprienh   (501) staff       (20)     4606 2022-05-04 20:57:43.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece_file.py
--rwxr-xr-x   0 cyprienh   (501) staff       (20)     3610 2022-05-04 20:59:08.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece_virtual.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2149 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/importing_an_hpgl_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1748 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_data-to-path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      623 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_virtual_generic.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      891 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_virtual_specific.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.040459 Chiplotle3-0.4.2/src/chiplotle3/fonts/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/fonts/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     5214 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/fonts/dorkbot.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.040924 Chiplotle3-0.4.2/src/chiplotle3/geometry/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/__init__.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.049127 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/
--rw-r--r--   0 cyprienh   (501) staff       (20)      141 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      903 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/affixformatvisitor.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     9083 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinate.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     4240 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinatearray.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1491 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinatearraypropertiesmixin.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3295 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/group.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2929 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/hpglformatvisitor.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3246 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/label.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      258 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/layer.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1655 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/layersvisitor.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      126 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/metadata.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2217 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      901 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/polygon.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1030 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/shape.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1397 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/shapepropertiesmixin.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      604 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/tagsvisitor.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3169 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/core/transformlock.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.069503 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/
--rw-r--r--   0 cyprienh   (501) staff       (20)      446 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3040 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/annotation.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1095 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arc_circle.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1889 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arc_ellipse.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1072 2022-05-04 20:58:31.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arrow.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2297 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/bezier_path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      949 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/catmull_path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      595 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/circle.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      724 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/cross.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      973 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/donut.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1258 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/ellipse.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      919 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/fan.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      640 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/frame.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1435 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/grid.py
--rw-r--r--   0 cyprienh   (501) staff       (20)       87 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/group.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      480 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/isosceles.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      275 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/label.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      105 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/layer.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      405 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/line.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      968 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/line_displaced.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      778 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/lock_group.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      299 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1893 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/path_linear.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1567 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/radial_ruler.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      747 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/random_walk_cartesian.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      639 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/random_walk_polar.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      601 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/rectangle.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1746 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/ruler.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2807 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/spiral_archimedean.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1871 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/spiral_logarithmic.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      180 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/square.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2802 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/star_crisscross.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1547 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/star_outline.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1228 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/supershape.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      442 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/symmetric_polygon_side_length.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      824 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/target.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.073674 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/
--rw-r--r--   0 cyprienh   (501) staff       (20)      109 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      747 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/arrange_shapes_on_path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      251 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/center_at.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1238 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/noise.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      867 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/offset.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1796 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/perpendicular_displace.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1540 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/perpendicular_noise.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      968 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/rotate.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      959 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/scale.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1073 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/transformvisitor.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.075428 Chiplotle3-0.4.2/src/chiplotle3/hpgl/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/__init__.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.079373 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1021 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/arc.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      520 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/hpgl.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      347 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/hpglescape.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      733 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/hpglprimitive.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1241 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/penplot.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1321 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/positional.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1006 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/twopoint.py
--rw-r--r--   0 cyprienh   (501) staff       (20)    44032 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/commands.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.081496 Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/
--rw-r--r--   0 cyprienh   (501) staff       (20)       83 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      454 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/filltype.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      996 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/linetype.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1241 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/pen.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2672 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/label.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1273 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/hpgl/pen.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.090511 Chiplotle3-0.4.2/src/chiplotle3/plotters/
--rw-r--r--   0 cyprienh   (501) staff       (20)      717 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     9993 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/baseplotter.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      756 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx2000.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      756 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx2200.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      754 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx3300.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     7549 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/drawingplotter.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      680 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/dxy1300.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      673 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/dxy880.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      678 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7475a.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      853 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7550a.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      184 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7575a.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      728 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7576a.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      773 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7585b.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      910 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7595a.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      910 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7596a.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.091906 Chiplotle3-0.4.2/src/chiplotle3/plotters/interactive/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/interactive/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     6415 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/interactive/interactive_commands.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.095107 Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      234 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/marginshard.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      236 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/marginssoft.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2525 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/plottermargins.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      663 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/plotters/plotter.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.095532 Chiplotle3-0.4.2/src/chiplotle3/tools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      195 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/__init__.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.100135 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      244 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1038 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_bounding_rectangle.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      698 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_center.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      299 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_centroid.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2341 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_line_intersection.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1156 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_minmax_coordinates.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1153 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_radius.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1284 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_shape_intersections.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1058 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_width_height.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      783 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/scale.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.107221 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      109 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      771 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/convert_coordinates_to_hpgl_absolute_path.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1502 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/convert_relatives_to_absolutes.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1020 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_all_coordinates.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      791 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_bounding_box.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      582 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_centroid.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     2829 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/inflate_hpgl_string.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      469 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/is_primitive_absolute.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1587 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/parse_hpgl_string.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1202 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/pens_updown_to_papr.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      706 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/pr_to_pa.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     3705 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/relativize.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      998 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/rotate_hpglprimitives.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      419 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/scale.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      552 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/transpose.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.110229 Chiplotle3-0.4.2/src/chiplotle3/tools/io/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      602 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/_open_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1470 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/export.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      681 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/import_hpgl_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      633 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/save_hpgl.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      664 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/io/view.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.114642 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      104 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/flat_list_to_dovetail_pairs.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      462 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/flat_list_to_pairs.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      444 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/flatten.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      266 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/is_flat_list.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      107 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/isiterable.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      133 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/iterabletools/ispair.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.116251 Chiplotle3-0.4.2/src/chiplotle3/tools/logtools/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/logtools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      211 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/logtools/apply_logger.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      746 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/logtools/get_logger.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.123873 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1399 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/bezier_interpolation.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1197 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/catmull_interpolation.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      272 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/cumsum.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      267 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/difference.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      748 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/factors.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      344 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/interpolate_cosine.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      322 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/interpolate_exponential.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      228 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/interpolate_linear.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      399 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/lcm.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      589 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/pascal_row.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      423 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/polar_to_xy.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1748 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/rotate_2d.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      814 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/rotate_3d.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      656 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/superformula.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      679 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/xy_to_polar.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.126893 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      109 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/cm_to_pu.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      134 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/in_to_pu.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      103 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/mm_to_pu.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      102 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/pu_to_cm.py
--rw-r--r--   0 cyprienh   (501) staff       (20)       98 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/pu_to_in.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      101 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/measuretools/pu_to_mm.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.130524 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1273 2022-05-04 21:01:09.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/_instantiate_plotter.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      520 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_plotter_from_id.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      856 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_plotters.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1449 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_virtual_plotter.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1090 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/interactive_choose_plotter.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1277 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/interactive_plot_layers.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1710 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/search_and_instantiate_plotters.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.135179 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/
--rw-r--r--   0 cyprienh   (501) staff       (20)      110 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      692 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/instantiate_serial_from_config_file.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1332 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/interactive_open_serial.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      626 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      589 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_from_list.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      549 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_linux.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      735 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_windows.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      551 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/sniff_ports_for_plotters.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     6132 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/virtual_serial_port.py
--rw-r--r--   0 cyprienh   (501) staff       (20)     1130 2022-05-04 20:56:06.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/what_plotter_in_port.py
-drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2022-05-04 21:20:47.135927 Chiplotle3-0.4.2/src/chiplotle3/tools/shapetools/
--rw-r--r--   0 cyprienh   (501) staff       (20)        0 2022-05-04 20:53:13.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/shapetools/__init__.py
--rw-r--r--   0 cyprienh   (501) staff       (20)      871 2022-05-04 20:58:30.000000 Chiplotle3-0.4.2/src/chiplotle3/tools/shapetools/get_shapes_with_tag.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.129951 Chiplotle3-0.4.3/
+-rw-r--r--   0 cyprienh   (501) staff       (20)    35147 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/LICENSE
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1999 2023-06-03 12:21:04.130252 Chiplotle3-0.4.3/PKG-INFO
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1509 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/README.md
+-rw-r--r--   0 cyprienh   (501) staff       (20)       84 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/pyproject.toml
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1064 2023-06-03 12:21:04.131549 Chiplotle3-0.4.3/setup.cfg
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.827389 Chiplotle3-0.4.3/src/
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.843912 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1999 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/PKG-INFO
+-rw-r--r--   0 cyprienh   (501) staff       (20)    10488 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/SOURCES.txt
+-rw-r--r--   0 cyprienh   (501) staff       (20)        1 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/dependency_links.txt
+-rw-r--r--   0 cyprienh   (501) staff       (20)       81 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/entry_points.txt
+-rw-r--r--   0 cyprienh   (501) staff       (20)       28 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/requires.txt
+-rw-r--r--   0 cyprienh   (501) staff       (20)       11 2023-06-03 12:21:03.000000 Chiplotle3-0.4.3/src/Chiplotle3.egg-info/top_level.txt
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.844692 Chiplotle3-0.4.3/src/chiplotle3/
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1482 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/__init__.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.847346 Chiplotle3-0.4.3/src/chiplotle3/core/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/__init__.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.855126 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      860 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/_run_chiplotle.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      937 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/_run_chiplotle_virtual.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      339 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/cfg.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      771 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/get_config_value.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1002 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/initialize_files.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      332 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/read_config_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2909 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/write_config_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)       78 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/cfg/write_log_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      734 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/errors.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.859313 Chiplotle3-0.4.3/src/chiplotle3/core/imports/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/imports/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      529 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/imports/get_functions_in_module.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1005 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/imports/package_import.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      212 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/imports/remove_modules_from_namespace.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.861859 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      492 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/formatdecorator.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      118 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/interface.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.863278 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/margins/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/margins/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      723 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/margins/interface.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.864982 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/parentage/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/parentage/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      865 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/parentage/interface.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      528 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/core/visitor.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.872872 Chiplotle3-0.4.3/src/chiplotle3/examples/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3168 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece.py
+-rwxr-xr-x   0 cyprienh   (501) staff       (20)     4606 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece_file.py
+-rwxr-xr-x   0 cyprienh   (501) staff       (20)     3610 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece_virtual.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2149 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/importing_an_hpgl_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1748 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_data-to-path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      623 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_virtual_generic.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      891 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_virtual_specific.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.874627 Chiplotle3-0.4.3/src/chiplotle3/fonts/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/fonts/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     5214 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/fonts/dorkbot.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.876008 Chiplotle3-0.4.3/src/chiplotle3/geometry/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/__init__.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.894991 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      141 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      903 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/affixformatvisitor.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     9083 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinate.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     4240 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinatearray.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1491 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinatearraypropertiesmixin.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3295 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/group.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2929 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/hpglformatvisitor.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3246 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/label.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      258 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/layer.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1655 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/layersvisitor.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      126 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/metadata.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2217 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      901 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/polygon.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1030 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/shape.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1397 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/shapepropertiesmixin.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      604 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/tagsvisitor.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3169 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/core/transformlock.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.983096 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      446 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3040 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/annotation.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1095 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arc_circle.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1889 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arc_ellipse.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1072 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arrow.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2297 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/bezier_path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      949 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/catmull_path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      595 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/circle.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      724 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/cross.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      973 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/donut.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1258 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/ellipse.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      919 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/fan.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      640 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/frame.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1435 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/grid.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)       87 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/group.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      480 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/isosceles.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      275 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/label.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      105 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/layer.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      405 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/line.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      968 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/line_displaced.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      778 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/lock_group.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      299 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1893 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/path_linear.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1567 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/radial_ruler.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      747 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/random_walk_cartesian.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      639 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/random_walk_polar.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      601 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/rectangle.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1746 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/ruler.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2807 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/spiral_archimedean.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1871 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/spiral_logarithmic.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      180 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/square.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2802 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/star_crisscross.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1547 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/star_outline.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1228 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/supershape.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      442 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/symmetric_polygon_side_length.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      824 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/target.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.994971 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      109 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      747 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/arrange_shapes_on_path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      251 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/center_at.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1238 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/noise.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      867 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/offset.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1796 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/perpendicular_displace.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1540 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/perpendicular_noise.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      968 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/rotate.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      959 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/scale.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1073 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/transformvisitor.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:03.998277 Chiplotle3-0.4.3/src/chiplotle3/hpgl/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/__init__.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.005321 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1021 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/arc.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      520 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/hpgl.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      347 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/hpglescape.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      733 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/hpglprimitive.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1241 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/penplot.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1321 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/positional.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1006 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/twopoint.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)    44032 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/commands.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.009599 Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/
+-rw-r--r--   0 cyprienh   (501) staff       (20)       83 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      454 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/filltype.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      996 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/linetype.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1241 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/pen.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2672 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/label.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1273 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/hpgl/pen.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.027573 Chiplotle3-0.4.3/src/chiplotle3/plotters/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      717 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     9993 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/baseplotter.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      756 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx2000.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      756 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx2200.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      754 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx3300.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     7549 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/drawingplotter.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      680 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/dxy1300.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      673 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/dxy880.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      678 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7475a.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      853 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7550a.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      184 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7575a.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      728 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7576a.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      773 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7585b.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      910 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7595a.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      910 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7596a.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.029409 Chiplotle3-0.4.3/src/chiplotle3/plotters/interactive/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/interactive/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     6415 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/interactive/interactive_commands.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.033585 Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      234 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/marginshard.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      236 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/marginssoft.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2525 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/plottermargins.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      663 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/plotters/plotter.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.034841 Chiplotle3-0.4.3/src/chiplotle3/tools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      195 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/__init__.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.046312 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      244 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1038 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_bounding_rectangle.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      698 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_center.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      299 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_centroid.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2341 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_line_intersection.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1156 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_minmax_coordinates.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1153 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_radius.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1284 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_shape_intersections.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1058 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_width_height.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      783 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/scale.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.062333 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      109 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      771 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/convert_coordinates_to_hpgl_absolute_path.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1502 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/convert_relatives_to_absolutes.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1020 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_all_coordinates.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      791 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_bounding_box.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      582 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_centroid.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     2829 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/inflate_hpgl_string.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      469 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/is_primitive_absolute.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1587 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/parse_hpgl_string.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1202 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/pens_updown_to_papr.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      706 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/pr_to_pa.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     3705 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/relativize.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      998 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/rotate_hpglprimitives.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      419 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/scale.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      552 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/transpose.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.068976 Chiplotle3-0.4.3/src/chiplotle3/tools/io/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      602 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/_open_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1486 2023-06-03 12:06:38.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/export.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      681 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/import_hpgl_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      633 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/save_hpgl.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      664 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/io/view.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.076913 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      104 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/flat_list_to_dovetail_pairs.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      462 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/flat_list_to_pairs.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      444 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/flatten.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      266 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/is_flat_list.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      107 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/isiterable.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      133 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/iterabletools/ispair.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.079753 Chiplotle3-0.4.3/src/chiplotle3/tools/logtools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/logtools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      211 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/logtools/apply_logger.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      746 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/logtools/get_logger.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.097226 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1399 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/bezier_interpolation.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1197 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/catmull_interpolation.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      272 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/cumsum.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      267 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/difference.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      748 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/factors.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      344 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/interpolate_cosine.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      322 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/interpolate_exponential.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      228 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/interpolate_linear.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      399 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/lcm.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      589 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/pascal_row.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      423 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/polar_to_xy.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1748 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/rotate_2d.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      814 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/rotate_3d.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      656 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/superformula.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      679 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/xy_to_polar.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.104043 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      109 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/cm_to_pu.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      134 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/in_to_pu.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      103 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/mm_to_pu.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      102 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/pu_to_cm.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)       98 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/pu_to_in.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      101 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/measuretools/pu_to_mm.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.115228 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1273 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/_instantiate_plotter.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      520 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_plotter_from_id.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      856 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_plotters.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1449 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_virtual_plotter.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1090 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/interactive_choose_plotter.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1277 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/interactive_plot_layers.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1710 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/search_and_instantiate_plotters.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.126414 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)      110 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      692 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/instantiate_serial_from_config_file.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1332 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/interactive_open_serial.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      626 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      589 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_from_list.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      549 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_linux.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      735 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_windows.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      551 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/sniff_ports_for_plotters.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     6132 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/virtual_serial_port.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)     1130 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/what_plotter_in_port.py
+drwxr-xr-x   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:21:04.128924 Chiplotle3-0.4.3/src/chiplotle3/tools/shapetools/
+-rw-r--r--   0 cyprienh   (501) staff       (20)        0 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/shapetools/__init__.py
+-rw-r--r--   0 cyprienh   (501) staff       (20)      871 2023-06-03 12:03:51.000000 Chiplotle3-0.4.3/src/chiplotle3/tools/shapetools/get_shapes_with_tag.py
```

### Comparing `Chiplotle3-0.4.2/LICENSE` & `Chiplotle3-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/PKG-INFO` & `Chiplotle3-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: Chiplotle3
-Version: 0.4.2
+Version: 0.4.3
 Summary: Chiplotle is an HPGL Python API.
 Home-page: http://music.columbia.edu/cmc/chiplotle
 Author: Víctor Adán and Douglas Repetto
 Author-email: chiplotle@music.columbia.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,9 +26,7 @@
 - On MacOS using M1 processor, you might need to reinstall Numpy for the library to work, to do so `pip uninstall numpy` and `pip install numpy`.
 
 Find all there is to know about Chiplotle at:
 http://music.columbia.edu/cmc/chiplotle
 
 The code for this version of Chiplotle is available at:
 https://github.com/cyprienh/chiplotle3
-
-
```

### Comparing `Chiplotle3-0.4.2/README.md` & `Chiplotle3-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/setup.cfg` & `Chiplotle3-0.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Chiplotle3
-version = 0.4.2
+version = 0.4.3
 author = Víctor Adán and Douglas Repetto
 author_email = chiplotle@music.columbia.edu
 description = Chiplotle is an HPGL Python API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://music.columbia.edu/cmc/chiplotle
 classifiers =
```

### Comparing `Chiplotle3-0.4.2/src/Chiplotle3.egg-info/PKG-INFO` & `Chiplotle3-0.4.3/src/Chiplotle3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: Chiplotle3
-Version: 0.4.2
+Version: 0.4.3
 Summary: Chiplotle is an HPGL Python API.
 Home-page: http://music.columbia.edu/cmc/chiplotle
 Author: Víctor Adán and Douglas Repetto
 Author-email: chiplotle@music.columbia.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,9 +26,7 @@
 - On MacOS using M1 processor, you might need to reinstall Numpy for the library to work, to do so `pip uninstall numpy` and `pip install numpy`.
 
 Find all there is to know about Chiplotle at:
 http://music.columbia.edu/cmc/chiplotle
 
 The code for this version of Chiplotle is available at:
 https://github.com/cyprienh/chiplotle3
-
-
```

### Comparing `Chiplotle3-0.4.2/src/Chiplotle3.egg-info/SOURCES.txt` & `Chiplotle3-0.4.3/src/Chiplotle3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/__init__.py` & `Chiplotle3-0.4.3/src/chiplotle3/__init__.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/cfg/_run_chiplotle.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/cfg/_run_chiplotle.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/cfg/_run_chiplotle_virtual.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/cfg/_run_chiplotle_virtual.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/cfg/get_config_value.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/cfg/get_config_value.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/cfg/initialize_files.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/cfg/initialize_files.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/cfg/write_config_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/cfg/write_config_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/errors.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/errors.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/imports/get_functions_in_module.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/imports/get_functions_in_module.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/imports/package_import.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/imports/package_import.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/margins/interface.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/margins/interface.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/interfaces/parentage/interface.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/interfaces/parentage/interface.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/core/visitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/core/visitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/abstract_masterpiece_virtual.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/abstract_masterpiece_virtual.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/importing_an_hpgl_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/importing_an_hpgl_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_data-to-path.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_data-to-path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_virtual_generic.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_virtual_generic.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/examples/liveplot_virtual_specific.py` & `Chiplotle3-0.4.3/src/chiplotle3/examples/liveplot_virtual_specific.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/fonts/dorkbot.py` & `Chiplotle3-0.4.3/src/chiplotle3/fonts/dorkbot.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/affixformatvisitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/affixformatvisitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinate.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinate.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinatearray.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinatearray.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/coordinatearraypropertiesmixin.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/coordinatearraypropertiesmixin.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/group.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/group.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/hpglformatvisitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/hpglformatvisitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/label.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/label.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/layersvisitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/layersvisitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/path.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/polygon.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/polygon.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/shape.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/shape.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/shapepropertiesmixin.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/shapepropertiesmixin.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/tagsvisitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/tagsvisitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/core/transformlock.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/core/transformlock.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/annotation.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/annotation.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arc_circle.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arc_circle.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arc_ellipse.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arc_ellipse.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/arrow.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/arrow.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/bezier_path.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/bezier_path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/catmull_path.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/catmull_path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/circle.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/cross.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/cross.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/donut.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/donut.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/ellipse.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/ellipse.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/fan.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/fan.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/frame.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/frame.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/grid.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/grid.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/line_displaced.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/line_displaced.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/lock_group.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/lock_group.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/path_linear.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/path_linear.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/radial_ruler.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/radial_ruler.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/random_walk_cartesian.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/random_walk_cartesian.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/random_walk_polar.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/random_walk_polar.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/rectangle.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/rectangle.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/ruler.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/ruler.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/spiral_archimedean.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/spiral_archimedean.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/spiral_logarithmic.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/spiral_logarithmic.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/star_crisscross.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/star_crisscross.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/star_outline.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/star_outline.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/supershape.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/supershape.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/shapes/target.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/shapes/target.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/arrange_shapes_on_path.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/arrange_shapes_on_path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/noise.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/offset.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/offset.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/perpendicular_displace.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/perpendicular_displace.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/perpendicular_noise.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/perpendicular_noise.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/rotate.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/rotate.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/scale.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/scale.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/geometry/transforms/transformvisitor.py` & `Chiplotle3-0.4.3/src/chiplotle3/geometry/transforms/transformvisitor.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/arc.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/arc.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/hpgl.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/hpgl.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/hpglprimitive.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/hpglprimitive.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/penplot.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/penplot.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/positional.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/positional.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/abstract/twopoint.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/abstract/twopoint.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/commands.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/commands.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/linetype.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/linetype.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/formatters/pen.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/formatters/pen.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/label.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/label.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/hpgl/pen.py` & `Chiplotle3-0.4.3/src/chiplotle3/hpgl/pen.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/__init__.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/__init__.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/baseplotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/baseplotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx2000.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx2000.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx2200.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx2200.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/dpx3300.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/dpx3300.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/drawingplotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/drawingplotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/dxy1300.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/dxy1300.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/dxy880.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/dxy880.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7475a.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7475a.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7550a.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7550a.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7576a.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7576a.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7585b.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7585b.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7595a.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7595a.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/hp7596a.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/hp7596a.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/interactive/interactive_commands.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/interactive/interactive_commands.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/margins/plottermargins.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/margins/plottermargins.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/plotters/plotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/plotters/plotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_bounding_rectangle.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_bounding_rectangle.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_center.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_center.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_line_intersection.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_line_intersection.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_minmax_coordinates.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_minmax_coordinates.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_radius.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_radius.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_shape_intersections.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_shape_intersections.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/get_width_height.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/get_width_height.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/geometrytools/scale.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/geometrytools/scale.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/convert_coordinates_to_hpgl_absolute_path.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/convert_coordinates_to_hpgl_absolute_path.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/convert_relatives_to_absolutes.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/convert_relatives_to_absolutes.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_all_coordinates.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_all_coordinates.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_bounding_box.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_bounding_box.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/get_centroid.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/get_centroid.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/inflate_hpgl_string.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/inflate_hpgl_string.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/parse_hpgl_string.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/parse_hpgl_string.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/pens_updown_to_papr.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/pens_updown_to_papr.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/pr_to_pa.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/pr_to_pa.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/relativize.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/relativize.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/rotate_hpglprimitives.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/rotate_hpglprimitives.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/hpgltools/transpose.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/hpgltools/transpose.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/io/_open_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/io/_open_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/io/export.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/io/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    cmd = 'hp2xx --truesize -p 1 -m %s -f "%s" "%s"' % (fmt, imgfile, htmlfile)
    p = subprocess.Popen(cmd, 
                         shell  = True,
                         stdout = subprocess.PIPE, 
                         stderr = subprocess.PIPE)
    stdout, stderr = p.communicate( )
 
-   if 'not found' in stderr:
+   if 'not found' in stderr.decode("utf-8"):
       print(_hp2xxError())
    
    return imgfile
 
 
 def _hp2xxError():
    msg = '''ATTENTION: hp2xx is not installed in your system.
```

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/io/import_hpgl_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/io/import_hpgl_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/io/save_hpgl.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/io/save_hpgl.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/io/view.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/io/view.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/logtools/get_logger.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/logtools/get_logger.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/bezier_interpolation.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/bezier_interpolation.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/catmull_interpolation.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/catmull_interpolation.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/factors.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/factors.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/pascal_row.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/pascal_row.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/rotate_2d.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/rotate_2d.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/rotate_3d.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/rotate_3d.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/superformula.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/superformula.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/mathtools/xy_to_polar.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/mathtools/xy_to_polar.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/_instantiate_plotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/_instantiate_plotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_plotter_from_id.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_plotter_from_id.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_plotters.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_plotters.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/instantiate_virtual_plotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/instantiate_virtual_plotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/interactive_choose_plotter.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/interactive_choose_plotter.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/interactive_plot_layers.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/interactive_plot_layers.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/plottertools/search_and_instantiate_plotters.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/plottertools/search_and_instantiate_plotters.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/instantiate_serial_from_config_file.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/instantiate_serial_from_config_file.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/interactive_open_serial.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/interactive_open_serial.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_from_list.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_from_list.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_linux.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_linux.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/scan_serial_ports_windows.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/scan_serial_ports_windows.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/sniff_ports_for_plotters.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/sniff_ports_for_plotters.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/virtual_serial_port.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/virtual_serial_port.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/serialtools/what_plotter_in_port.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/serialtools/what_plotter_in_port.py`

 * *Files identical despite different names*

### Comparing `Chiplotle3-0.4.2/src/chiplotle3/tools/shapetools/get_shapes_with_tag.py` & `Chiplotle3-0.4.3/src/chiplotle3/tools/shapetools/get_shapes_with_tag.py`

 * *Files identical despite different names*

