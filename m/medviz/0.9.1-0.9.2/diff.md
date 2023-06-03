# Comparing `tmp/medviz-0.9.1.tar.gz` & `tmp/medviz-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.9.1.tar", last modified: Thu Jun  1 17:25:03 2023, max compression
+gzip compressed data, was "medviz-0.9.2.tar", last modified: Sat Jun  3 02:13:53 2023, max compression
```

## Comparing `medviz-0.9.1.tar` & `medviz-0.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-0.9.1/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-0.9.1/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-01 17:25:03.472003 medviz-0.9.1/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.9.1/README.rst
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-01 05:24:31.000000 medviz-0.9.1/VERSION
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2043 2023-06-01 05:52:20.000000 medviz-0.9.1/medviz/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      549 2023-05-31 20:21:50.000000 medviz-0.9.1/medviz/bowel.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      218 2023-05-23 22:19:22.000000 medviz-0.9.1/medviz/bowel2.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/collage/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-0.9.1/medviz/collage/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-0.9.1/medviz/collage/compute_collage.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-0.9.1/medviz/collage/main.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-0.9.1/medviz/collage/stats.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/example.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1620 2023-05-15 18:19:57.000000 medviz-0.9.1/medviz/fat_mul.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/multimodal/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-0.9.1/medviz/multimodal/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-0.9.1/medviz/multimodal/save_dicom_metadata.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-0.9.1/medviz/multimodal/stats.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/nifti/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4331 2023-06-01 05:36:49.000000 medviz-0.9.1/medviz/nifti/helper.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/pkg2/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/pkg2/example.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-0.9.1/medviz/plots/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.9.1/medviz/plots/_plot_image.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/gif/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-0.9.1/medviz/plots/gif/gif.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-0.9.1/medviz/plots/helper_plot.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-0.9.1/medviz/plots/layered_plot2D.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/plot2d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-0.9.1/medviz/plots/plot2d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot2d/image_mask_annotated.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1831 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot2d/image_masks.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1633 2023-05-24 02:54:03.000000 medviz-0.9.1/medviz/plots/plot2d/images.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1891 2023-05-24 02:59:58.000000 medviz-0.9.1/medviz/plots/plot2d/masks.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/plot3d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      114 2023-05-25 02:26:37.000000 medviz-0.9.1/medviz/plots/plot3d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot3d/image_mask_annotated.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2390 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot3d/images.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-0.9.1/medviz/plots/plot3d/layered_plot.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/preprocess/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-14 03:50:56.000000 medviz-0.9.1/medviz/preprocess/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2015 2023-06-01 05:55:48.000000 medviz-0.9.1/medviz/preprocess/mask.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1753 2023-06-01 05:56:55.000000 medviz-0.9.1/medviz/preprocess/match_image_mask.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/utils/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      570 2023-06-01 05:14:13.000000 medviz-0.9.1/medviz/utils/__init__.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.9.1/medviz/utils/array_profile.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.9.1/medviz/utils/array_threshold.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      152 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/utils/custom_type.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-0.9.1/medviz/utils/helper_mask.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2448 2023-05-24 04:53:08.000000 medviz-0.9.1/medviz/utils/helper_path.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.9.1/medviz/utils/log.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-0.9.1/medviz/utils/reader.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.9.1/medviz/utils/utility.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1331 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      190 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-0.9.1/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-01 17:25:03.472003 medviz-0.9.1/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.9.1/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-0.9.2/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-0.9.2/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-03 02:13:53.548121 medviz-0.9.2/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.9.2/README.rst
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-03 02:13:47.000000 medviz-0.9.2/VERSION
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2043 2023-06-01 05:52:20.000000 medviz-0.9.2/medviz/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      549 2023-05-31 20:21:50.000000 medviz-0.9.2/medviz/bowel.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      218 2023-05-23 22:19:22.000000 medviz-0.9.2/medviz/bowel2.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/collage/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-0.9.2/medviz/collage/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-0.9.2/medviz/collage/compute_collage.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-0.9.2/medviz/collage/main.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-0.9.2/medviz/collage/stats.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/example.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1620 2023-05-15 18:19:57.000000 medviz-0.9.2/medviz/fat_mul.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/multimodal/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-0.9.2/medviz/multimodal/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-0.9.2/medviz/multimodal/save_dicom_metadata.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-0.9.2/medviz/multimodal/stats.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/nifti/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4332 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/nifti/helper.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/pkg2/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/pkg2/example.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-0.9.2/medviz/plots/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.9.2/medviz/plots/_plot_image.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/gif/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-0.9.2/medviz/plots/gif/gif.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-0.9.2/medviz/plots/helper_plot.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-0.9.2/medviz/plots/layered_plot2D.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/plot2d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-0.9.2/medviz/plots/plot2d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot2d/image_mask_annotated.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1831 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot2d/image_masks.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1633 2023-05-24 02:54:03.000000 medviz-0.9.2/medviz/plots/plot2d/images.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1891 2023-05-24 02:59:58.000000 medviz-0.9.2/medviz/plots/plot2d/masks.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/plot3d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      114 2023-05-25 02:26:37.000000 medviz-0.9.2/medviz/plots/plot3d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot3d/image_mask_annotated.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2390 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot3d/images.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-0.9.2/medviz/plots/plot3d/layered_plot.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/preprocess/
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       87 2023-06-03 02:09:03.000000 medviz-0.9.2/medviz/preprocess/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2071 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/preprocess/mask.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2764 2023-06-03 02:10:07.000000 medviz-0.9.2/medviz/preprocess/match_image_mask.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/utils/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      571 2023-06-03 02:07:23.000000 medviz-0.9.2/medviz/utils/__init__.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.9.2/medviz/utils/array_profile.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.9.2/medviz/utils/array_threshold.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      152 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/utils/custom_type.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-0.9.2/medviz/utils/helper_mask.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2583 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/utils/helper_path.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.9.2/medviz/utils/log.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-0.9.2/medviz/utils/reader.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.9.2/medviz/utils/utility.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1331 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      190 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/top_level.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-0.9.2/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-03 02:13:53.548121 medviz-0.9.2/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.9.2/setup.py
```

### Comparing `medviz-0.9.1/LICENSE` & `medviz-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/PKG-INFO` & `medviz-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.9.1
+Version: 0.9.2
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.9.1/README.rst` & `medviz-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/__init__.py` & `medviz-0.9.2/medviz/__init__.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/bowel.py` & `medviz-0.9.2/medviz/bowel.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/collage/compute_collage.py` & `medviz-0.9.2/medviz/collage/compute_collage.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/collage/main.py` & `medviz-0.9.2/medviz/collage/main.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/collage/stats.py` & `medviz-0.9.2/medviz/collage/stats.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/fat_mul.py` & `medviz-0.9.2/medviz/fat_mul.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/multimodal/save_dicom_metadata.py` & `medviz-0.9.2/medviz/multimodal/save_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/nifti/helper.py` & `medviz-0.9.2/medviz/nifti/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
-from ..utils import save_path_dir, significant_slice_idx
 
 from medviz.utils.helper_mask import significant_slice_idx_data
 
+from ..utils import save_path_dir, significant_slice_idx
+
 
 def nifti_to_hu(file_path: str or Path):
     """
     read the image and convert it to hu image
     :param file_path: file path
     :return: hu image
     """
```

### Comparing `medviz-0.9.1/medviz/plots/_plot_image.py` & `medviz-0.9.2/medviz/plots/_plot_image.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/gif/gif.py` & `medviz-0.9.2/medviz/plots/gif/gif.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/helper_plot.py` & `medviz-0.9.2/medviz/plots/helper_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/layered_plot2D.py` & `medviz-0.9.2/medviz/plots/layered_plot2D.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot2d/image_mask_annotated.py` & `medviz-0.9.2/medviz/plots/plot2d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot2d/image_masks.py` & `medviz-0.9.2/medviz/plots/plot2d/image_masks.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot2d/images.py` & `medviz-0.9.2/medviz/plots/plot2d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot2d/masks.py` & `medviz-0.9.2/medviz/plots/plot2d/masks.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot3d/image_mask_annotated.py` & `medviz-0.9.2/medviz/plots/plot3d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot3d/images.py` & `medviz-0.9.2/medviz/plots/plot3d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/plots/plot3d/layered_plot.py` & `medviz-0.9.2/medviz/plots/plot3d/layered_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/preprocess/mask.py` & `medviz-0.9.2/medviz/preprocess/mask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from pathlib import Path
 
 import pandas as pd
 
-from ..utils import save_path_file, path_in, get_characteristics,significant_slice_idx
+from ..utils import get_characteristics, path_in, save_path_file, significant_slice_idx
+
 
 def generate_mask_schema(
-    dataset_path: str or Path,
+    masks_path: str or Path,
     id_func=lambda x: x,
-    # mask_extension=".nii",
     mask_extension=None,
-    # mask_type=None,
     save_path: str or Path = Path("./output/mask_profile.csv"),
 ):
     df_dict = {
         "id": [],
         "path": [],
         "shape": [],
         "data_type": [],
         "values": [],
         "mask_type": [],
         "most_value_nonzero_slices": [],
         "num_nonzero_slices": [],
     }
 
-    dataset_path = path_in(dataset_path, env=True)
+    dataset_path = path_in(masks_path, env=False)
 
     if mask_extension is None:
         extensions = set()
 
         for file_path in dataset_path.rglob("*"):
             if file_path.is_file():
                 file_extension = file_path.suffix.lower()
 
                 extensions.add(file_extension)
 
-        mask_extension = extensions
-        exit()
+        for extension in extensions:
+            if extension in [".nii", ".nii.gz", ".dcm"]:
+                mask_extension = extension
+                break
 
     mask_paths = dataset_path.glob(rf"**/*{mask_extension}")
 
     for mask_path in mask_paths:
         # try:
         id = id_func(mask_path.stem)
         print(id)
```

### Comparing `medviz-0.9.1/medviz/utils/__init__.py` & `medviz-0.9.2/medviz/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .custom_type import PathType
 from .utility import now
 from .array_profile import profile
 from .array_threshold import compute_thresholds
+
 # from .helper_path import path_in, save_path_file, save_path_dir
 
 from .helper_mask import (
     get_characteristics,
     significant_slice_idx,
     significant_slice_idx_data,
     mask_path_to_data_ax,
```

### Comparing `medviz-0.9.1/medviz/utils/array_profile.py` & `medviz-0.9.2/medviz/utils/array_profile.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/utils/array_threshold.py` & `medviz-0.9.2/medviz/utils/array_threshold.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/utils/helper_mask.py` & `medviz-0.9.2/medviz/utils/helper_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/utils/helper_path.py` & `medviz-0.9.2/medviz/utils/helper_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from os import getenv
 from pathlib import Path
 
+from .utility import now
+
 
 def path_in(path: str or Path, env: bool = False) -> Path:
     if isinstance(path, str):
         path = Path(path)
 
     if not isinstance(path, Path):
         raise TypeError(f"The input must be string or Path, not {type(path)}")
@@ -54,34 +56,36 @@
     if not path.parent.exists():
         print("The output path doesn't exist but no worries I'm making it.")
         path.parent.mkdir(parents=True)
 
     return path
 
 
-def save_path_file(save_path: str or Path, suffix: str or None) -> Path:
+def save_path_file(save_path: str or Path, suffix: str or None = None) -> Path:
     if isinstance(save_path, str):
         save_path = Path(save_path)
 
     if not isinstance(save_path, Path):
         raise TypeError(f"save_path must be a str or Path, not {type(save_path)}")
 
     if not save_path.suffix:
         save_path = save_path.with_suffix(suffix)
 
     if not save_path.parent.exists():
         save_path.parent.mkdir(parents=True)
+    elif save_path.exists():
+        save_path = save_path.with_stem(save_path.stem + "_" + now())
 
     return save_path
 
 
 def save_path_dir(save_path: str or Path) -> Path:
     if isinstance(save_path, str):
         save_path = Path(save_path)
 
     if not isinstance(save_path, Path):
-        raise TypeError(f"save_path must be a str or Path, not {type(save_path)}")
+        raise TypeError(f"save_path must be a STRING or PATH, not {type(save_path)}")
 
     if not save_path.exists():
         save_path.mkdir(parents=True)
 
     return save_path
```

### Comparing `medviz-0.9.1/medviz/utils/log.py` & `medviz-0.9.2/medviz/utils/log.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz/utils/reader.py` & `medviz-0.9.2/medviz/utils/reader.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/medviz.egg-info/PKG-INFO` & `medviz-0.9.2/medviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.9.1
+Version: 0.9.2
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.9.1/medviz.egg-info/SOURCES.txt` & `medviz-0.9.2/medviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medviz-0.9.1/pyproject.toml` & `medviz-0.9.2/pyproject.toml`

 * *Files identical despite different names*

