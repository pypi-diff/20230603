# Comparing `tmp/metaindex-2.2.1.tar.gz` & `tmp/metaindex-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaindex-2.2.1.tar", last modified: Sun May 28 07:52:38 2023, max compression
+gzip compressed data, was "metaindex-2.2.2.tar", last modified: Sat Jun  3 09:04:18 2023, max compression
```

## Comparing `metaindex-2.2.1.tar` & `metaindex-2.2.2.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.773471 metaindex-2.2.1/
--rw-r--r--   0 robert    (1000) robert    (1000)     6054 2023-05-28 07:52:08.000000 metaindex-2.2.1/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.2.1/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.2.1/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-05-28 07:52:38.773471 metaindex-2.2.1/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4141 2023-05-28 06:12:37.000000 metaindex-2.2.1/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.753471 metaindex-2.2.1/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.2.1/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.753471 metaindex-2.2.1/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.760138 metaindex-2.2.1/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/addons.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/cmdoptions.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/cmdusage.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/configuration.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/description.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/extrametadata.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/indexers.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.2.1/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/doctrees/reference.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/doctrees/searchsyntax.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/doctrees/synopsis.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/doctrees/usage.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.763471 metaindex-2.2.1/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.763471 metaindex-2.2.1/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.1/doc/build/html/_sources/addons.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.1/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.2.1/doc/build/html/_sources/cmdoptions.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.2.1/doc/build/html/_sources/cmdusage.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.2.1/doc/build/html/_sources/configuration.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.1/doc/build/html/_sources/description.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.1/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.1/doc/build/html/_sources/extrametadata.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.1/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.2.1/doc/build/html/_sources/indexers.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.1/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.1/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.1/doc/build/html/_sources/reference.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.1/doc/build/html/_sources/searchsyntax.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.1/doc/build/html/_sources/synopsis.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.1/doc/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.766805 metaindex-2.2.1/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.2.1/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/addons.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/cmdusage.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/configuration.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/description.html
--rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/extrametadata.html
--rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/indexers.html
--rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/searchsyntax.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/synopsis.html
--rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.2.1/doc/build/html/usage.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.2.1/doc/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.2.1/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.2.1/doc/metaindex.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.2.1/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.1/doc/source/addons.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.1/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5307 2023-05-28 07:32:15.000000 metaindex-2.2.1/doc/source/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.2.1/doc/source/cmdusage.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.2.1/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.2.1/doc/source/configuration.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.1/doc/source/description.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.1/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.1/doc/source/extrametadata.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.1/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     8208 2023-05-28 07:47:46.000000 metaindex-2.2.1/doc/source/indexers.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.1/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.1/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.1/doc/source/reference.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.1/doc/source/searchsyntax.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.1/doc/source/synopsis.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.1/doc/source/usage.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.2.1/examples/indexing.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    38113 2023-05-28 07:52:38.000000 metaindex-2.2.1/man/metaindex.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.2.1/metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    16060 2023-05-27 16:53:24.000000 metaindex-2.2.1/metaindex/cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12458 2023-05-27 07:57:02.000000 metaindex-2.2.1/metaindex/cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.2.1/metaindex/client.py
--rw-r--r--   0 robert    (1000) robert    (1000)    24347 2023-05-27 19:11:56.000000 metaindex-2.2.1/metaindex/configuration.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/metaindex/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex/docs/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)    56492 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex/docs/metaindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.2.1/metaindex/find.py
--rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.2.1/metaindex/fuse.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.2.1/metaindex/humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15319 2023-05-28 07:14:07.000000 metaindex-2.2.1/metaindex/indexer.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/metaindex/indexers/
--rw-r--r--   0 robert    (1000) robert    (1000)      512 2023-05-27 08:36:14.000000 metaindex-2.2.1/metaindex/indexers/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.2.1/metaindex/indexers/abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.2.1/metaindex/indexers/audio.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4956 2023-05-23 18:18:09.000000 metaindex-2.2.1/metaindex/indexers/collections.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6714 2023-05-27 16:39:21.000000 metaindex-2.2.1/metaindex/indexers/comicbook.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.2.1/metaindex/indexers/epub.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4742 2023-05-27 16:27:19.000000 metaindex-2.2.1/metaindex/indexers/filetags.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4435 2023-05-27 16:28:19.000000 metaindex-2.2.1/metaindex/indexers/gpx.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3061 2023-05-27 18:49:01.000000 metaindex-2.2.1/metaindex/indexers/html.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3801 2023-05-28 07:41:25.000000 metaindex-2.2.1/metaindex/indexers/images.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2788 2023-05-27 18:54:57.000000 metaindex-2.2.1/metaindex/indexers/ooxml.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2876 2023-05-27 18:56:00.000000 metaindex-2.2.1/metaindex/indexers/opendocument.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3353 2023-05-27 19:11:05.000000 metaindex-2.2.1/metaindex/indexers/pdf.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-05-19 08:45:31.000000 metaindex-2.2.1/metaindex/indexers/ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4004 2023-05-28 07:13:11.000000 metaindex-2.2.1/metaindex/json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.2.1/metaindex/logger.py
--rw-r--r--   0 robert    (1000) robert    (1000)     9458 2023-05-28 07:33:08.000000 metaindex-2.2.1/metaindex/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7317 2023-05-28 07:42:39.000000 metaindex-2.2.1/metaindex/ocr.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2757 2023-05-27 16:14:29.000000 metaindex-2.2.1/metaindex/opf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-27 09:09:18.000000 metaindex-2.2.1/metaindex/proto.py
--rw-r--r--   0 robert    (1000) robert    (1000)    27524 2023-05-27 08:10:45.000000 metaindex-2.2.1/metaindex/server.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6061 2023-05-28 06:55:58.000000 metaindex-2.2.1/metaindex/shared.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.2.1/metaindex/stores.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-28 07:52:10.000000 metaindex-2.2.1/metaindex/version.py
--rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.2.1/metaindex/xmlproxy.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4053 2023-05-28 07:02:39.000000 metaindex-2.2.1/metaindex/yaml.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/metaindex.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      235 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-28 07:52:38.000000 metaindex-2.2.1/metaindex.egg-info/top_level.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.770138 metaindex-2.2.1/misc/
--rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.2.1/misc/metaindex.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.773471 metaindex-2.2.1/misc/ranger_metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.2.1/misc/ranger_metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.2.1/misc/ranger_metaindex/linemode.py
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-28 07:52:38.773471 metaindex-2.2.1/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     3664 2023-05-21 10:28:55.000000 metaindex-2.2.1/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-28 07:52:38.773471 metaindex-2.2.1/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.2.1/tests/test_abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.2.1/tests/test_cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.2.1/tests/test_cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.2.1/tests/test_cleanup.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.2.1/tests/test_collect.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.2.1/tests/test_humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.2.1/tests/test_indexers.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.2.1/tests/test_json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.2.1/tests/test_ruleindexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/
+-rw-r--r--   0 robert    (1000) robert    (1000)     6147 2023-06-03 09:03:31.000000 metaindex-2.2.2/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.2.2/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.2.2/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-03 09:04:18.100041 metaindex-2.2.2/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4141 2023-05-28 06:12:37.000000 metaindex-2.2.2/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.083375 metaindex-2.2.2/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.2.2/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.080041 metaindex-2.2.2/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.086708 metaindex-2.2.2/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/addons.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/cmdoptions.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/cmdusage.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/configuration.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/description.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/extrametadata.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/indexers.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/reference.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/searchsyntax.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/synopsis.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/usage.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.090041 metaindex-2.2.2/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.093375 metaindex-2.2.2/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.2/doc/build/html/_sources/addons.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.2/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.2.2/doc/build/html/_sources/cmdoptions.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.2.2/doc/build/html/_sources/cmdusage.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.2.2/doc/build/html/_sources/configuration.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.2/doc/build/html/_sources/description.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.2/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.2/doc/build/html/_sources/extrametadata.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.2/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.2.2/doc/build/html/_sources/indexers.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.2/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.2/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.2/doc/build/html/_sources/reference.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.2/doc/build/html/_sources/searchsyntax.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.2/doc/build/html/_sources/synopsis.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.2/doc/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/addons.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/cmdusage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/configuration.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/description.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/extrametadata.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/indexers.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/searchsyntax.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/synopsis.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/usage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.2.2/doc/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.2.2/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.2.2/doc/metaindex.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.2.2/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.2/doc/source/addons.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.2/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5307 2023-05-28 07:32:15.000000 metaindex-2.2.2/doc/source/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.2.2/doc/source/cmdusage.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.2.2/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.2.2/doc/source/configuration.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.2/doc/source/description.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.2/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.2/doc/source/extrametadata.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.2/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     8208 2023-05-28 07:47:46.000000 metaindex-2.2.2/doc/source/indexers.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.2/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.2/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.2/doc/source/reference.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.2/doc/source/searchsyntax.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.2/doc/source/synopsis.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.2/doc/source/usage.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.2.2/examples/indexing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    38113 2023-06-03 09:04:17.000000 metaindex-2.2.2/man/metaindex.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.2.2/metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    16060 2023-05-27 16:53:24.000000 metaindex-2.2.2/metaindex/cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12461 2023-06-03 08:58:55.000000 metaindex-2.2.2/metaindex/cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/client.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    24347 2023-05-27 19:11:56.000000 metaindex-2.2.2/metaindex/configuration.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-06-03 09:04:17.000000 metaindex-2.2.2/metaindex/docs/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    56492 2023-06-03 09:04:17.000000 metaindex-2.2.2/metaindex/docs/metaindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/find.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.2.2/metaindex/fuse.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.2.2/metaindex/humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15319 2023-05-28 07:14:07.000000 metaindex-2.2.2/metaindex/indexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/indexers/
+-rw-r--r--   0 robert    (1000) robert    (1000)      512 2023-05-27 08:36:14.000000 metaindex-2.2.2/metaindex/indexers/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.2.2/metaindex/indexers/abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.2.2/metaindex/indexers/audio.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4956 2023-05-23 18:18:09.000000 metaindex-2.2.2/metaindex/indexers/collections.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6714 2023-05-27 16:39:21.000000 metaindex-2.2.2/metaindex/indexers/comicbook.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.2.2/metaindex/indexers/epub.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4742 2023-05-27 16:27:19.000000 metaindex-2.2.2/metaindex/indexers/filetags.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4435 2023-05-27 16:28:19.000000 metaindex-2.2.2/metaindex/indexers/gpx.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3061 2023-05-27 18:49:01.000000 metaindex-2.2.2/metaindex/indexers/html.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3801 2023-05-28 07:41:25.000000 metaindex-2.2.2/metaindex/indexers/images.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2788 2023-05-27 18:54:57.000000 metaindex-2.2.2/metaindex/indexers/ooxml.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2876 2023-05-27 18:56:00.000000 metaindex-2.2.2/metaindex/indexers/opendocument.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3353 2023-05-27 19:11:05.000000 metaindex-2.2.2/metaindex/indexers/pdf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-05-19 08:45:31.000000 metaindex-2.2.2/metaindex/indexers/ruleindexer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4004 2023-05-28 07:13:11.000000 metaindex-2.2.2/metaindex/json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.2.2/metaindex/logger.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9458 2023-05-28 07:33:08.000000 metaindex-2.2.2/metaindex/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7317 2023-05-28 07:42:39.000000 metaindex-2.2.2/metaindex/ocr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2757 2023-05-27 16:14:29.000000 metaindex-2.2.2/metaindex/opf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-06-03 08:59:37.000000 metaindex-2.2.2/metaindex/proto.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    27524 2023-05-27 08:10:45.000000 metaindex-2.2.2/metaindex/server.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6061 2023-06-03 08:58:47.000000 metaindex-2.2.2/metaindex/shared.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/stores.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-06-03 09:03:39.000000 metaindex-2.2.2/metaindex/version.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.2.2/metaindex/xmlproxy.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4053 2023-05-28 07:02:39.000000 metaindex-2.2.2/metaindex/yaml.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      235 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/top_level.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/misc/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.2.2/misc/metaindex.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/misc/ranger_metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.2.2/misc/ranger_metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.2.2/misc/ranger_metaindex/linemode.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-03 09:04:18.100041 metaindex-2.2.2/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     3664 2023-05-21 10:28:55.000000 metaindex-2.2.2/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.2.2/tests/test_abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.2.2/tests/test_cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.2.2/tests/test_cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.2.2/tests/test_cleanup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.2.2/tests/test_collect.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.2.2/tests/test_humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.2.2/tests/test_indexers.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.2.2/tests/test_json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.2.2/tests/test_ruleindexer.py
```

### Comparing `metaindex-2.2.1/CHANGELOG.md` & `metaindex-2.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+## 2.2.2
+### Fixed
+- Fixed issues with `last_modified` and the new unified timestamp format
+
 ## 2.2.1
 ### Changed
 - `date` field in sidecar files will be split into `date` and `time` upon loading, if possible, and saved as a merged `date` field upon saving
 
 ### Fixed
 - Overriding values by setting them to `none`/`null` in the sidecar file was not actually doing anything
 - Language hinting for OCR was too demanding; now also short ISO 639 codes work
```

### Comparing `metaindex-2.2.1/LICENSE` & `metaindex-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/PKG-INFO` & `metaindex-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.2.1
+Version: 2.2.2
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.2.1/README.md` & `metaindex-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/Makefile` & `metaindex-2.2.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/addons.doctree` & `metaindex-2.2.2/doc/build/doctrees/addons.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/changelog.doctree` & `metaindex-2.2.2/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/cmdoptions.doctree` & `metaindex-2.2.2/doc/build/doctrees/cmdoptions.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/cmdusage.doctree` & `metaindex-2.2.2/doc/build/doctrees/cmdusage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/configuration.doctree` & `metaindex-2.2.2/doc/build/doctrees/configuration.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/description.doctree` & `metaindex-2.2.2/doc/build/doctrees/description.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/environment.pickle` & `metaindex-2.2.2/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/examples.doctree` & `metaindex-2.2.2/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/extrametadata.doctree` & `metaindex-2.2.2/doc/build/doctrees/extrametadata.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/index.doctree` & `metaindex-2.2.2/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/indexers.doctree` & `metaindex-2.2.2/doc/build/doctrees/indexers.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/install.doctree` & `metaindex-2.2.2/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/license.doctree` & `metaindex-2.2.2/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/reference.doctree` & `metaindex-2.2.2/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/searchsyntax.doctree` & `metaindex-2.2.2/doc/build/doctrees/searchsyntax.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/synopsis.doctree` & `metaindex-2.2.2/doc/build/doctrees/synopsis.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/doctrees/usage.doctree` & `metaindex-2.2.2/doc/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/addons.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/addons.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/cmdoptions.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/cmdoptions.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/cmdusage.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/cmdusage.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/configuration.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/description.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/description.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/examples.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/extrametadata.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/extrametadata.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/indexers.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/indexers.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/install.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/reference.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_sources/searchsyntax.rst.txt` & `metaindex-2.2.2/doc/build/html/_sources/searchsyntax.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/basic.css` & `metaindex-2.2.2/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/doctools.js` & `metaindex-2.2.2/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/jquery-3.5.1.js` & `metaindex-2.2.2/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/jquery.js` & `metaindex-2.2.2/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/language_data.js` & `metaindex-2.2.2/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/nature.css` & `metaindex-2.2.2/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/pygments.css` & `metaindex-2.2.2/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/searchtools.js` & `metaindex-2.2.2/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/underscore-1.13.1.js` & `metaindex-2.2.2/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/_static/underscore.js` & `metaindex-2.2.2/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/addons.html` & `metaindex-2.2.2/doc/build/html/addons.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/changelog.html` & `metaindex-2.2.2/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/cmdoptions.html` & `metaindex-2.2.2/doc/build/html/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/cmdusage.html` & `metaindex-2.2.2/doc/build/html/cmdusage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/configuration.html` & `metaindex-2.2.2/doc/build/html/configuration.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/description.html` & `metaindex-2.2.2/doc/build/html/description.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/examples.html` & `metaindex-2.2.2/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/extrametadata.html` & `metaindex-2.2.2/doc/build/html/extrametadata.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/genindex.html` & `metaindex-2.2.2/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/index.html` & `metaindex-2.2.2/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/indexers.html` & `metaindex-2.2.2/doc/build/html/indexers.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/install.html` & `metaindex-2.2.2/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/license.html` & `metaindex-2.2.2/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/objects.inv` & `metaindex-2.2.2/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/reference.html` & `metaindex-2.2.2/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/search.html` & `metaindex-2.2.2/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/searchindex.js` & `metaindex-2.2.2/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/searchsyntax.html` & `metaindex-2.2.2/doc/build/html/searchsyntax.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/synopsis.html` & `metaindex-2.2.2/doc/build/html/synopsis.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/build/html/usage.html` & `metaindex-2.2.2/doc/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/cmdoptions.rst` & `metaindex-2.2.2/doc/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/make.bat` & `metaindex-2.2.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/metaindex.rst` & `metaindex-2.2.2/doc/metaindex.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/addons.rst` & `metaindex-2.2.2/doc/source/addons.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/cmdoptions.rst` & `metaindex-2.2.2/doc/source/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/cmdusage.rst` & `metaindex-2.2.2/doc/source/cmdusage.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/conf.py` & `metaindex-2.2.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/configuration.rst` & `metaindex-2.2.2/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/description.rst` & `metaindex-2.2.2/doc/source/description.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/examples.rst` & `metaindex-2.2.2/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/extrametadata.rst` & `metaindex-2.2.2/doc/source/extrametadata.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/indexers.rst` & `metaindex-2.2.2/doc/source/indexers.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/install.rst` & `metaindex-2.2.2/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/reference.rst` & `metaindex-2.2.2/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/doc/source/searchsyntax.rst` & `metaindex-2.2.2/doc/source/searchsyntax.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/examples/indexing.py` & `metaindex-2.2.2/examples/indexing.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/man/metaindex.1` & `metaindex-2.2.2/man/metaindex.1`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/cache.py` & `metaindex-2.2.2/metaindex/cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/cacheentry.py` & `metaindex-2.2.2/metaindex/cacheentry.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             raise TypeError()
 
     @classmethod
     def from_dict(cls, data):
         """Recreate a CacheEntry from data, as generated by 'as_dict'"""
         that = cls(data['path'],
                    data.get('metadata', {}),
-                   strpdt(data.get('last_modified', '000010101T000000')),
+                   strpdt(data.get('last_modified', '0001-01-01 00:00:00')),
                    data.get('rpath', None),
                    data.get('slbl', None))
         that.mimetype = data.get('mime', None)
         return that
 
     def __lt__(self, other):
         return str(self.path) < str(other.path)
```

### Comparing `metaindex-2.2.1/metaindex/client.py` & `metaindex-2.2.2/metaindex/client.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/configuration.py` & `metaindex-2.2.2/metaindex/configuration.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/docs/cmdoptions.html` & `metaindex-2.2.2/metaindex/docs/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/docs/metaindex.html` & `metaindex-2.2.2/metaindex/docs/metaindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/find.py` & `metaindex-2.2.2/metaindex/find.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/fuse.py` & `metaindex-2.2.2/metaindex/fuse.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/humanizer.py` & `metaindex-2.2.2/metaindex/humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexer.py` & `metaindex-2.2.2/metaindex/indexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/__init__.py` & `metaindex-2.2.2/metaindex/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/abc.py` & `metaindex-2.2.2/metaindex/indexers/abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/audio.py` & `metaindex-2.2.2/metaindex/indexers/audio.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/collections.py` & `metaindex-2.2.2/metaindex/indexers/collections.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/comicbook.py` & `metaindex-2.2.2/metaindex/indexers/comicbook.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/epub.py` & `metaindex-2.2.2/metaindex/indexers/epub.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/filetags.py` & `metaindex-2.2.2/metaindex/indexers/filetags.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/gpx.py` & `metaindex-2.2.2/metaindex/indexers/gpx.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/html.py` & `metaindex-2.2.2/metaindex/indexers/html.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/images.py` & `metaindex-2.2.2/metaindex/indexers/images.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/ooxml.py` & `metaindex-2.2.2/metaindex/indexers/ooxml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/opendocument.py` & `metaindex-2.2.2/metaindex/indexers/opendocument.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/pdf.py` & `metaindex-2.2.2/metaindex/indexers/pdf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/indexers/ruleindexer.py` & `metaindex-2.2.2/metaindex/indexers/ruleindexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/json.py` & `metaindex-2.2.2/metaindex/json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/logger.py` & `metaindex-2.2.2/metaindex/logger.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/main.py` & `metaindex-2.2.2/metaindex/main.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/ocr.py` & `metaindex-2.2.2/metaindex/ocr.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/opf.py` & `metaindex-2.2.2/metaindex/opf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/proto.py` & `metaindex-2.2.2/metaindex/proto.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/server.py` & `metaindex-2.2.2/metaindex/server.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/shared.py` & `metaindex-2.2.2/metaindex/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def strfdt(timestamp):
     """Return the strftime'd timestamp
 
     This function will also ensure that the returned value has the correct
     amount of leading zeroes, for example when the datetime should be 0001-01-01.
     """
     text = timestamp.strftime(TIMESTAMP_FORMAT)
-    return "0"*max(0, 15-len(text)) + text
+    return "0"*max(0, 19-len(text)) + text
 
 
 def strpdt(text):
     return datetime.datetime.strptime(text, TIMESTAMP_FORMAT)
 
 
 def find_files(paths, recursive=True, ignore_dirs=None):
```

### Comparing `metaindex-2.2.1/metaindex/stores.py` & `metaindex-2.2.2/metaindex/stores.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/xmlproxy.py` & `metaindex-2.2.2/metaindex/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex/yaml.py` & `metaindex-2.2.2/metaindex/yaml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/metaindex.egg-info/PKG-INFO` & `metaindex-2.2.2/metaindex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.2.1
+Version: 2.2.2
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.2.1/metaindex.egg-info/SOURCES.txt` & `metaindex-2.2.2/metaindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/misc/metaindex.conf` & `metaindex-2.2.2/misc/metaindex.conf`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/misc/ranger_metaindex/linemode.py` & `metaindex-2.2.2/misc/ranger_metaindex/linemode.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/setup.py` & `metaindex-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_abc.py` & `metaindex-2.2.2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_cache.py` & `metaindex-2.2.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_cacheentry.py` & `metaindex-2.2.2/tests/test_cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_cleanup.py` & `metaindex-2.2.2/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_collect.py` & `metaindex-2.2.2/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_humanizer.py` & `metaindex-2.2.2/tests/test_humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_indexers.py` & `metaindex-2.2.2/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_json.py` & `metaindex-2.2.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.1/tests/test_ruleindexer.py` & `metaindex-2.2.2/tests/test_ruleindexer.py`

 * *Files identical despite different names*

