# Comparing `tmp/cyberdrop-dl-4.2.58.tar.gz` & `tmp/cyberdrop-dl-4.2.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.58.tar", last modified: Wed May 31 14:15:13 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.59.tar", last modified: Sat Jun  3 18:20:28 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.58.tar` & `cyberdrop-dl-4.2.59.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.879376 cyberdrop-dl-4.2.58/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-31 14:15:13.879376 cyberdrop-dl-4.2.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.871376 cyberdrop-dl-4.2.58/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.875376 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.875376 cyberdrop-dl-4.2.58/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.875376 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.879376 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.879376 cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:15:13.871376 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 14:15:13.000000 cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 14:15:13.879376 cyberdrop-dl-4.2.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:15:04.000000 cyberdrop-dl-4.2.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.256317 cyberdrop-dl-4.2.59/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/setup.py
```

### Comparing `cyberdrop-dl-4.2.58/LICENSE` & `cyberdrop-dl-4.2.59/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/PKG-INFO` & `cyberdrop-dl-4.2.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.58
+Version: 4.2.59
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.58 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.59 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.58/README.md` & `cyberdrop-dl-4.2.59/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,15 +68,22 @@
             "ratelimit": 50,
             "throttle": 0.5,
         },
         "Runtime": {
             "allow_insecure_connections": False,
             "attempts": 10,
             "block_sub_folders": False,
+            "check_for_partial_files_and_empty_dirs": True,
             "disable_attempt_limit": False,
+            "filesize_minimum_images": 0,
+            "filesize_minimum_other": 0,
+            "filesize_minimum_videos": 0,
+            "filesize_maximum_images": 0,
+            "filesize_maximum_other": 0,
+            "filesize_maximum_videos": 0,
             "include_id": False,
             "max_concurrent_threads": 0,
             "max_concurrent_domains": 0,
             "max_concurrent_albums": 0,
             "max_concurrent_downloads_per_domain": 4,
             "output_errored_urls": False,
             "output_unsupported_urls": False,
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 await f.write(chunk)
                 if isinstance(update_progress, functools.partial):
                     await update_progress(len(chunk))
                 else:
                     update_progress(len(chunk))
 
     async def _download(self, media: MediaItem, current_throttle: float, proxy: str, headers: Dict,
-                        save_content: Callable[[aiohttp.StreamReader, int], Coroutine[Any, Any, None]]) -> None:
+                        save_content: Callable[[aiohttp.StreamReader], Coroutine[Any, Any, None]], file: Path) -> None:
         headers['Referer'] = str(media.referer)
         headers['user-agent'] = self.client.user_agent
 
         assert media.url.host is not None
         await self._throttle(current_throttle, media.url.host)
 
         async with self.client_session.get(media.url, headers=headers, ssl=self.client.ssl_context,
@@ -153,21 +153,19 @@
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="No content-type in response header")
             if resp.url in self.bunkr_maintenance:
                 raise DownloadFailure(code=HTTPStatus.SERVICE_UNAVAILABLE, message="Bunkr under maintenance")
             if any(s in content_type.lower() for s in ('html', 'text')):
                 logger.debug("Server for %s is experiencing issues, you are being ratelimited, or cookies have expired", media.url)
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="Unexpectedly got text as response")
 
-            size = int(resp.headers.get('Content-Length', '0'))
-            if not size:
-                content_range = resp.headers.get('Content-Range', '')  # <unit> <range-start>-<range-end>/<size>
-                if content_range:
-                    with contextlib.suppress(ValueError):
-                        size = int(content_range.split('/')[1])
-            await save_content(resp.content, size)
+            if resp.status != HTTPStatus.PARTIAL_CONTENT:
+                if file.is_file():
+                    file.unlink()
+
+            await save_content(resp.content)
 
     async def _throttle(self, delay: float, host: str) -> None:
         """Throttles requests to domains by a parameter amount of time"""
         if delay is None or delay == 0:
             return
 
         key = f'throttle:{host}'
@@ -183,31 +181,30 @@
             remaining = delay - elapsed + 0.1
             await asyncio.sleep(remaining)
 
     async def download_file(self, Progress_Master: ProgressMaster, media: MediaItem, file: Path,
                             current_throttle: float, resume_point: int, proxy: str, headers: Dict,
                             file_task: TaskID) -> None:
 
-        async def save_content(content: aiohttp.StreamReader, size: int) -> None:
-            await Progress_Master.FileProgress.update_file_length(file_task, size + resume_point)
+        async def save_content(content: aiohttp.StreamReader) -> None:
             await Progress_Master.FileProgress.advance_file(file_task, resume_point)
             await self._append_content(file, content, functools.partial(Progress_Master.FileProgress.advance_file, file_task))
 
-        await self._download(media, current_throttle, proxy, headers, save_content)
+        await self._download(media, current_throttle, proxy, headers, save_content, file)
 
     async def old_download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
-                                proxy: str, headers: Dict):
+                                proxy: str, headers: Dict, size: int) -> None:
 
-        async def save_content(content: aiohttp.StreamReader, size: int) -> None:
+        async def save_content(content: aiohttp.StreamReader) -> None:
             task_description = adjust_title(f"{media.url.host}: {media.filename}")
             with tqdm(total=size + resume_point, unit_scale=True, unit='B', leave=False,
                       initial=resume_point, desc=task_description) as progress:
                 await self._append_content(file, content, lambda chunk_len: progress.update(chunk_len))
 
-        await self._download(media, current_throttle, proxy, headers, save_content)
+        await self._download(media, current_throttle, proxy, headers, save_content, file)
 
     async def get_filesize(self, url: URL, referer: str, current_throttle: float) -> int:
         headers = {'Referer': referer, 'user-agent': self.client.user_agent}
 
         assert url.host is not None
         await self._throttle(current_throttle, url.host)
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context,
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Class for specific selectors of supported domains"""
     domain: str
     posts_selectors: List[str] = field(init=False)
     next_page_selector: str = field(init=False)
 
     def __post_init__(self):
         if self.domain == "coomer":
-            self.posts_selectors = ['h2[class=post-card__heading] a']
+            self.posts_selectors = ['article[class=post-card ] a']
             self.next_page_selector = 'a[title="Next page"]'
         elif self.domain == "kemono":
             self.posts_selectors = ['article[class="post-card post-card--preview"] a', 'article[class="post-card"] a']
             self.next_page_selector = 'a[class=next]'
 
 
 class CoomenoCrawler:
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from random import gauss
 from typing import TYPE_CHECKING, Any, Dict, Tuple, Coroutine, List, Optional
 
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
+    FILE_FORMATS,
     clear,
     log,
     logger,
 )
 from cyberdrop_dl.base_functions.data_classes import (
     AlbumItem,
     CascadeItem,
@@ -86,26 +87,64 @@
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
 
+        # Filesize limits
+        self.filesize_minimum_images = args["Runtime"]["filesize_minimum_images"]
+        self.filesize_minimum_other = args["Runtime"]["filesize_minimum_other"]
+        self.filesize_minimum_videos = args["Runtime"]["filesize_minimum_videos"]
+        self.filesize_maximum_images = args["Runtime"]["filesize_maximum_images"]
+        self.filesize_maximum_other = args["Runtime"]["filesize_maximum_other"]
+        self.filesize_maximum_videos = args["Runtime"]["filesize_maximum_videos"]
+
         # Concurrency Limits
-        self.threads_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_threads"]) if args["Runtime"]["max_concurrent_threads"] else None
-        self.domains_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_domains"]) if args["Runtime"]["max_concurrent_domains"] else None
-        self.albums_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_albums"]) if args["Runtime"]["max_concurrent_albums"] else None
+        self.threads_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_threads"]) if args["Runtime"][
+            "max_concurrent_threads"] else None
+        self.domains_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_domains"]) if args["Runtime"][
+            "max_concurrent_domains"] else None
+        self.albums_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_albums"]) if args["Runtime"][
+            "max_concurrent_albums"] else None
 
         # API Keys
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
     def get_throttle(self, domain: str) -> float:
         """Get the throttle for a domain"""
         return self.delay.get(domain, self.client.throttle)
 
+    async def check_filesize_limits(self, media: MediaItem, content_size: int) -> bool:
+        if media.ext in FILE_FORMATS['Images']:
+            if self.filesize_minimum_images and self.filesize_maximum_images:
+                if content_size < self.filesize_minimum_images or content_size > self.filesize_maximum_images:
+                    return False
+            if content_size < self.filesize_minimum_images:
+                return False
+            if self.filesize_maximum_images and content_size > self.filesize_maximum_images:
+                return False
+        elif media.ext in FILE_FORMATS['Videos']:
+            if self.filesize_minimum_videos and self.filesize_maximum_videos:
+                if content_size < self.filesize_minimum_videos or content_size > self.filesize_maximum_videos:
+                    return False
+            if content_size < self.filesize_minimum_videos:
+                return False
+            if self.filesize_maximum_videos and content_size > self.filesize_maximum_videos:
+                return False
+        else:
+            if self.filesize_minimum_other and self.filesize_maximum_other:
+                if content_size < self.filesize_minimum_other or content_size > self.filesize_maximum_other:
+                    return False
+            if content_size < self.filesize_minimum_other:
+                return False
+            if self.filesize_maximum_other and content_size > self.filesize_maximum_other:
+                return False
+        return True
+
 
 class Downloader:
     """Downloader class, directs downloading for domain objects"""
 
     def __init__(self, domain: str, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
         self.domain = domain
         self.throttle = CDL_Helper.get_throttle(domain)
@@ -152,33 +191,43 @@
 
             if url_path not in self.current_attempt:
                 self.current_attempt[url_path] = 0
 
             complete_file = (self.CDL_Helper.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-            complete_file, partial_file, proceed = await self.check_file_exists(complete_file, partial_file, media,
-                                                                                album, url_path, original_filename,
-                                                                                self.throttle)
+            complete_file, partial_file, proceed, expected_size = await self.check_file_exists(complete_file,
+                                                                                               partial_file, media,
+                                                                                               album, url_path,
+                                                                                               original_filename,
+                                                                                               self.throttle)
+
             fake_download = self.CDL_Helper.mark_downloaded or not proceed
 
             await self.CDL_Helper.SQL_Helper.update_pre_download(complete_file, media.filename, url_path,
                                                                  original_filename)
 
+            filesize_check = await self.CDL_Helper.check_filesize_limits(media, expected_size)
+            if not filesize_check:
+                log(f"Filesize out of specified range: {media.url}", quiet=True)
+                await self.CDL_Helper.files.add_skipped()
+                await self.Progress_Master.AlbumProgress.advance_album(album_task)
+                return
+
             await self.CDL_Helper.SQL_Helper.sql_insert_temp(str(partial_file))
             resume_point = partial_file.stat().st_size if partial_file.exists() else 0
 
             assert media.url.host is not None
             headers = {}
             if self.CDL_Helper.pixeldrain_api_key and "pixeldrain" in media.url.host:
                 headers["Authorization"] = await basic_auth("Cyberdrop-DL", self.CDL_Helper.pixeldrain_api_key)
-            if resume_point:
-                headers['Range'] = f'bytes={resume_point}-'
 
-            file_task = await self.Progress_Master.FileProgress.add_file(media.filename)
+            headers['Range'] = f'bytes={resume_point}-'
+
+            file_task = await self.Progress_Master.FileProgress.add_file(media.filename, expected_size)
 
             if not await self.CDL_Helper.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
                 await self.download_session.download_file(self.Progress_Master, media, partial_file, self.throttle,
                                                           resume_point, self.CDL_Helper.proxy, headers, file_task)
                 partial_file.rename(complete_file)
 
             await self.CDL_Helper.SQL_Helper.mark_complete(url_path, original_filename)
@@ -231,32 +280,34 @@
                     return
 
                 logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     def can_retry(self, url_path: str) -> bool:
-        return self.CDL_Helper.disable_attempt_limit or self.current_attempt[url_path] < self.CDL_Helper.allowed_attempts - 1
+        return self.CDL_Helper.disable_attempt_limit or self.current_attempt[
+            url_path] < self.CDL_Helper.allowed_attempts - 1
 
     async def handle_failed(self, media: MediaItem, e: Any) -> None:
         await self.CDL_Helper.files.add_failed()
         await self.CDL_Helper.error_writer.write_errored_download(media.url, media.referer, e.message)
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
-                                url_path: str, original_filename: str, current_throttle: float):
+                                url_path: str, original_filename: str,
+                                current_throttle: float) -> tuple[Path, Path, bool, int]:
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
-            if not complete_file.exists() and not partial_file.exists():
-                break
-
             if not expected_size:
                 expected_size = await self.download_session.get_filesize(media.url, str(media.referer),
                                                                          current_throttle)
+            if not complete_file.exists() and not partial_file.exists():
+                break
+
             if complete_file.exists() and complete_file.stat().st_size == expected_size:
                 proceed = False
                 break
 
             downloaded_filename = await self.CDL_Helper.SQL_Helper.get_downloaded_filename(url_path, original_filename)
             if not downloaded_filename:
                 complete_file, partial_file = await self.iterate_filename(complete_file, media, album)
@@ -274,15 +325,15 @@
                         complete_file, partial_file = await self.iterate_filename(complete_file, media, album)
                 break
 
             media.filename = downloaded_filename
             complete_file = (self.CDL_Helper.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-        return complete_file, partial_file, proceed
+        return complete_file, partial_file, proceed, expected_size
 
     async def iterate_filename(self, complete_file: Path, media: MediaItem, album: str) -> Tuple[Path, Path]:
         for iterations in itertools.count(1):
             filename = f"{complete_file.stem} ({iterations}){media.ext}"
             temp_complete_file = (self.CDL_Helper.download_dir / album / filename)
             if not temp_complete_file.exists() and not await self.CDL_Helper.SQL_Helper.check_filename(filename):
                 media.filename = filename
@@ -362,15 +413,16 @@
         download_tasks = []
         for media in album_obj.media:
             download_tasks.append(self.start_file(downloader, album_task, domain, album, media))
         await asyncio.gather(*download_tasks)
         await self.Progress_Master.DomainProgress.advance_domain(domain_task)
         await self.Progress_Master.AlbumProgress.mark_album_completed(album_task)
 
-    async def start_file(self, downloader: Downloader, album_task: TaskID, domain: str, album: str, media: MediaItem) -> None:
+    async def start_file(self, downloader: Downloader, album_task: TaskID, domain: str, album: str,
+                         media: MediaItem) -> None:
         """Handler for files and the progress bars for it"""
         if media.complete or await self.CDL_Helper.SQL_Helper.check_complete_singular(domain, media.url):
             log(f"Previously Downloaded: {media.filename}", quiet=True)
             await self.CDL_Helper.files.add_skipped()
             await self.Progress_Master.AlbumProgress.advance_album(album_task)
             return
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from random import gauss
 from typing import TYPE_CHECKING, Any, Dict
 
 import aiohttp.client_exceptions
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
+    FILE_FORMATS,
     ErrorFileWriter,
     clear,
     log,
     logger,
 )
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, DomainItem, FileLock, ForumItem, MediaItem
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
@@ -81,14 +82,21 @@
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
         self.exclude_audio = args["Ignore"]["exclude_audio"]
         self.exclude_images = args["Ignore"]["exclude_images"]
         self.exclude_videos = args["Ignore"]["exclude_videos"]
         self.exclude_other = args["Ignore"]["exclude_other"]
 
+        self.filesize_minimum_images = args["Ignore"]["filesize_minimum_images"]
+        self.filesize_minimum_videos = args["Ignore"]["filesize_minimum_videos"]
+        self.filesize_minimum_other = args["Ignore"]["filesize_minimum_other"]
+        self.filesize_maximum_images = args["Ignore"]["filesize_maximum_images"]
+        self.filesize_maximum_videos = args["Ignore"]["filesize_maximum_videos"]
+        self.filesize_maximum_other = args["Ignore"]["filesize_maximum_other"]
+
         self.block_sub_folders = args['Runtime']['block_sub_folders']
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
@@ -145,38 +153,46 @@
 
             current_throttle = self.client.throttle
 
             original_filename = media.filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-            complete_file, partial_file, proceed = await self.check_file_exists(complete_file, partial_file, media,
-                                                                                album, url_path, original_filename,
-                                                                                current_throttle)
+            complete_file, partial_file, proceed, expected_size = await self.check_file_exists(complete_file,
+                                                                                               partial_file, media,
+                                                                                               album, url_path,
+                                                                                               original_filename,
+                                                                                               current_throttle)
             fake_download = self.mark_downloaded or not proceed
 
             await self.SQL_Helper.update_pre_download(complete_file, media.filename, url_path, original_filename)
 
+            filesize_check = await self.check_filesize_limits(media, expected_size)
+            if not filesize_check:
+                log(f"Filesize out of range: {media.filename}", quiet=True)
+                self.files.add_skipped()
+                return
+
             await self.SQL_Helper.sql_insert_temp(str(partial_file))
             resume_point = partial_file.stat().st_size if partial_file.exists() else 0
 
             assert media.url.host is not None
             for key, value in self.delay.items():
                 if key in media.url.host:
                     current_throttle = value
 
             headers = {}
             if self.pixeldrain_api_key and "pixeldrain" in media.url.host:
                 headers["Authorization"] = await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)
-            if resume_point:
-                headers['Range'] = f'bytes={resume_point}-'
+
+            headers['Range'] = f'bytes={resume_point}-'
 
             if not await self.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
                 await self.download_session.old_download_file(media, partial_file, current_throttle, resume_point,
-                                                              self.proxy, headers)
+                                                              self.proxy, headers, expected_size)
                 partial_file.rename(complete_file)
 
             await self.SQL_Helper.mark_complete(url_path, original_filename)
             if media.url.parts[-1] in self.current_attempt:
                 self.current_attempt.pop(media.url.parts[-1])
 
             if fake_download:
@@ -223,27 +239,55 @@
     def can_retry(self, url_path: str) -> bool:
         return self.disable_attempt_limit or self.current_attempt[url_path] < self.allowed_attempts - 1
 
     async def handle_failed(self, media: MediaItem, e: Any) -> None:
         self.files.add_failed()
         await self.error_writer.write_errored_download(media.url, media.referer, e.message)
 
+    async def check_filesize_limits(self, media: MediaItem, content_size: int) -> bool:
+        if media.ext in FILE_FORMATS['Images']:
+            if self.filesize_minimum_images and self.filesize_maximum_images:
+                if content_size < self.filesize_minimum_images or content_size > self.filesize_maximum_images:
+                    return False
+            if content_size < self.filesize_minimum_images:
+                return False
+            if self.filesize_maximum_images and content_size > self.filesize_maximum_images:
+                return False
+        elif media.ext in FILE_FORMATS['Videos']:
+            if self.filesize_minimum_videos and self.filesize_maximum_videos:
+                if content_size < self.filesize_minimum_videos or content_size > self.filesize_maximum_videos:
+                    return False
+            if content_size < self.filesize_minimum_videos:
+                return False
+            if self.filesize_maximum_videos and content_size > self.filesize_maximum_videos:
+                return False
+        else:
+            if self.filesize_minimum_other and self.filesize_maximum_other:
+                if content_size < self.filesize_minimum_other or content_size > self.filesize_maximum_other:
+                    return False
+            if content_size < self.filesize_minimum_other:
+                return False
+            if self.filesize_maximum_other and content_size > self.filesize_maximum_other:
+                return False
+        return True
+
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str,
-                                current_throttle: float) -> tuple[Path, Path, bool]:
+                                current_throttle: float) -> tuple[Path, Path, bool, int]:
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
-            if not complete_file.exists() and not partial_file.exists():
-                break
-
             if not expected_size:
                 expected_size = await self.download_session.get_filesize(media.url, str(media.referer),
                                                                          current_throttle)
+
+            if not complete_file.exists() and not partial_file.exists():
+                break
+
             if complete_file.exists() and complete_file.stat().st_size == expected_size:
                 proceed = False
                 break
 
             downloaded_filename = await self.SQL_Helper.get_downloaded_filename(url_path, original_filename)
             if not downloaded_filename:
                 for iterations in itertools.count(1):
@@ -264,15 +308,15 @@
                     partial_file.rename(complete_file)
                 break
 
             media.filename = downloaded_filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-        return complete_file, partial_file, proceed
+        return complete_file, partial_file, proceed, expected_size
 
 
 async def old_download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client,
                               error_writer: ErrorFileWriter) -> None:
     """Handler for forum threads and the progress bars for it"""
     total_files = await Forums.get_total()
     with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
@@ -283,8 +327,8 @@
             for domain, domain_obj in Cascade.domains.items():
                 downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files, error_writer)
                 tasks.append(downloader.start_domain())
             await asyncio.gather(*tasks)
 
     await clear()
     log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
-              f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
+        f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import contextlib
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple
 
 from rich.console import Group
 from rich.panel import Panel
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
@@ -299,20 +299,20 @@
 class FileProgress:
     def __init__(self, progressions: Progressions, visible_tasks_limit: int):
         self.file_progress = progressions.file_progress
         self.color = "plum3"
         self.type_str = "Files"
         self.progress = _Progress(self.file_progress, progressions.file_progress_overflow, self.color, "Files", visible_tasks_limit)
 
-    async def add_file(self, file: str) -> TaskID:
+    async def add_file(self, file: str, expected_size: Optional[int]) -> TaskID:
         task_description = file.split('/')[-1]
         task_description = task_description.encode("ascii", "ignore").decode().strip()
         task_description = adjust_title(task_description)
 
-        task_id = await self.progress.add_task(task_description.upper(), 0)
+        task_id = await self.progress.add_task(task_description.upper(), expected_size if expected_size else 0)
         await self.progress.redraw()
         return task_id
 
     async def update_file_length(self, task_id: TaskID, length: int) -> None:
         await self.progress.update_total(task_id, length)
 
     async def advance_file(self, task_id: TaskID, increment: int) -> None:
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,22 @@
 
     # Runtime arguments
     config_group = config_data["Runtime"]
     runtime_opts = parser.add_argument_group("Runtime options")
     runtime_opts.add_argument("--allow-insecure-connections", help="allows insecure connections from content hosts", action="store_true")
     runtime_opts.add_argument("--attempts", type=int, help="number of attempts to download each file (default: %(default)s)", default=config_group["attempts"])
     runtime_opts.add_argument("--block-sub-folders", help="block sub folders from being created", action="store_true")
+    runtime_opts.add_argument("--check-for-partial-files-and-empty-dirs", type=bool, default=config_group["check_for_partial_files_and_empty_dirs"], help="checks for partial files and empty directories after completing (default: %(default)s)")
     runtime_opts.add_argument("--disable-attempt-limit", help="disables the attempt limitation", action="store_true")
+    runtime_opts.add_argument("--filesize_maximum_images", type=int, default=config_group["filesize_maximum_images"], help="maximum filesize for images (default: %(default)s)")
+    runtime_opts.add_argument("--filesize_maximum_videos", type=int, default=config_group["filesize_maximum_videos"], help="maximum filesize for videos (default: %(default)s)")
+    runtime_opts.add_argument("--filesize_maximum_other", type=int, default=config_group["filesize_maximum_other"], help="maximum filesize for other files (default: %(default)s)")
+    runtime_opts.add_argument("--filesize_minimum_images", type=int, default=config_group["filesize_minimum_images"], help="minimum filesize for images (default: %(default)s)")
+    runtime_opts.add_argument("--filesize_minimum_videos", type=int, default=config_group["filesize_minimum_videos"], help="minimum filesize for videos (default: %(default)s)")
+    runtime_opts.add_argument("--filesize_minimum_other", type=int, default=config_group["filesize_minimum_other"], help="minimum filesize for other files (default: %(default)s)")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
     runtime_opts.add_argument("--max-concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
@@ -273,26 +280,27 @@
             log("Sorting Downloads")
             sorter = Sorter(args['Files']['output_folder'], args['Sorting']['sort_directory'],
                             args['Sorting']['sorted_audio'], args['Sorting']['sorted_images'],
                             args['Sorting']['sorted_videos'], args['Sorting']['sorted_others'])
             await sorter.sort()
 
         log("")
-        log("Checking for incomplete downloads")
-        partial_downloads = any(f.is_file() for f in args['Files']['output_folder'].rglob("*.part"))
-        temp_downloads = any(Path(f).is_file() for f in await SQL_Helper.get_temp_names())
-
-        log('Purging empty directories')
-        await purge_dir(args['Files']['output_folder'])
+        if args['Runtime']['check_for_partial_files_and_empty_dirs']:
+            log("Checking for incomplete downloads")
+            partial_downloads = any(f.is_file() for f in args['Files']['output_folder'].rglob("*.part"))
+            temp_downloads = any(Path(f).is_file() for f in await SQL_Helper.get_temp_names())
+
+            log('Purging empty directories')
+            await purge_dir(args['Files']['output_folder'])
+            if partial_downloads:
+                log('There are partial downloads in the downloads folder.', style="yellow")
+            if temp_downloads:
+                log('There are partial downloads from this run, please re-run the program.', style="yellow")
 
         log('Finished downloading. Enjoy :)')
-        if partial_downloads:
-            log('There are partial downloads in the downloads folder.', style="yellow")
-        if temp_downloads:
-            log('There are partial downloads from this run, please re-run the program.', style="yellow")
 
     log('')
     log("If you enjoy using this program, please consider buying the developer a coffee :)\nhttps://www.buymeacoffee.com/juleswinnft", style="green")
 
 
 def main(args=None):
     if not args:
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.58
+Version: 4.2.59
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.58 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.59 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.58/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.58/setup.cfg` & `cyberdrop-dl-4.2.59/setup.cfg`

 * *Files identical despite different names*

