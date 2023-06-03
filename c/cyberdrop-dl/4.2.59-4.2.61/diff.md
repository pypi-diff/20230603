# Comparing `tmp/cyberdrop-dl-4.2.59.tar.gz` & `tmp/cyberdrop-dl-4.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.59.tar", last modified: Sat Jun  3 18:20:28 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.61.tar", last modified: Sat Jun  3 18:32:46 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.59.tar` & `cyberdrop-dl-4.2.61.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.256317 cyberdrop-dl-4.2.59/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:20:28.260317 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 18:20:28.000000 cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-03 18:20:28.264317 cyberdrop-dl-4.2.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:20:16.000000 cyberdrop-dl-4.2.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.131500 cyberdrop-dl-4.2.61/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-03 18:32:46.131500 cyberdrop-dl-4.2.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18207 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.119500 cyberdrop-dl-4.2.61/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.123500 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.123500 cyberdrop-dl-4.2.61/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.127500 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.131500 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.131500 cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:32:46.119500 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 18:32:46.000000 cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-03 18:32:46.131500 cyberdrop-dl-4.2.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:32:35.000000 cyberdrop-dl-4.2.61/setup.py
```

### Comparing `cyberdrop-dl-4.2.59/LICENSE` & `cyberdrop-dl-4.2.61/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/PKG-INFO` & `cyberdrop-dl-4.2.61/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.59
+Version: 4.2.61
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -145,14 +145,20 @@
 --only-hosts            only allows downloads and scraping from these hosts
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
+--filesize-maximum-images               maximum filesize for images
+--filesize-maximum-videos               maximum filesize for videos
+--filesize-maximum-other                maximum filesize for other files
+--filesize-minimum-images               minimum filesize for images
+--filesize-minimum-videos               minimum filesize for videos
+--filesize-minimum-other                minimum filesize for other files
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.59 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.61 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -127,58 +127,63 @@
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
-disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --max-concurrent-threads number of threads to
-download simultaneously --max-concurrent-domains number of domains to download
-simultaneously --max-concurrent-albums number of albums to download
-simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-throttle this is a throttle between requests during the downloading phase, the
-number is in seconds --output-last-forum-post outputs the last post of a forum
-scrape to use as a starting point for future runs --scrape-single-post scrapes
-a single post from a forum thread --separate-posts separates forum scraping
-into folders by post number --gofile-api-key api key for premium gofile --
-gofile-website-token website token for gofile --pixeldrain-api-key api key for
-premium pixeldrain --nudostar-username username to login to nudostar --
-nudostar-password password to login to nudostar --simpcity-username username to
-login to simpcity --simpcity-password password to login to simpcity --
-socialmediagirls-username username to login to socialmediagirls --
-socialmediagirls-password password to login to socialmediagirls --xbunker-
-username username to login to xbunker --xbunker-password password to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table --visible-rows-threads number of visible
-rows to use for the threads table --visible-rows-domains number of visible rows
-to use for the domains table --visible-rows-albums number of visible rows to
-use for the albums table --visible-rows-files number of visible rows to use for
-the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
-"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
-"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
-"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
-"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
-"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+disable-attempt-limit disables the attempt limitation --filesize-maximum-images
+maximum filesize for images --filesize-maximum-videos maximum filesize for
+videos --filesize-maximum-other maximum filesize for other files --filesize-
+minimum-images minimum filesize for images --filesize-minimum-videos minimum
+filesize for videos --filesize-minimum-other minimum filesize for other files -
+-include-id include the ID in the download folder name --max-concurrent-threads
+number of threads to download simultaneously --max-concurrent-domains number of
+domains to download simultaneously --max-concurrent-albums number of albums to
+download simultaneously --max-concurrent-downloads-per-domain number of
+simultaneous downloads per domain --skip-download-mark-completed sets the
+scraped files as downloaded without downloading --output-errored-urls sets the
+failed urls to be output to the errored urls file --output-unsupported-urls
+sets the unsupported urls to be output to the unsupported urls file --proxy
+HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port] --
+remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --throttle this is a throttle between
+requests during the downloading phase, the number is in seconds --output-last-
+forum-post outputs the last post of a forum scrape to use as a starting point
+for future runs --scrape-single-post scrapes a single post from a forum thread
+--separate-posts separates forum scraping into folders by post number --gofile-
+api-key api key for premium gofile --gofile-website-token website token for
+gofile --pixeldrain-api-key api key for premium pixeldrain --nudostar-username
+username to login to nudostar --nudostar-password password to login to nudostar
+--simpcity-username username to login to simpcity --simpcity-password password
+to login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
+socialmediagirls --xbunker-username username to login to xbunker --xbunker-
+password password to login to xbunker --apply-jdownloader enables sending
+unsupported URLs to a running jdownloader2 instance to download --jdownloader-
+username username to login to jdownloader --jdownloader-password password to
+login to jdownloader --jdownloader-device device name to login to for
+jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table --
+visible-rows-threads number of visible rows to use for the threads table --
+visible-rows-domains number of visible rows to use for the domains table --
+visible-rows-albums number of visible rows to use for the albums table --
+visible-rows-files number of visible rows to use for the files table ``` `--
+only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.59/README.md` & `cyberdrop-dl-4.2.61/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,20 @@
 --only-hosts            only allows downloads and scraping from these hosts
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
+--filesize-maximum-images               maximum filesize for images
+--filesize-maximum-videos               maximum filesize for videos
+--filesize-maximum-other                maximum filesize for other files
+--filesize-minimum-images               minimum filesize for images
+--filesize-minimum-videos               minimum filesize for videos
+--filesize-minimum-other                minimum filesize for other files
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
```

#### html2text {}

```diff
@@ -121,58 +121,63 @@
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
-disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --max-concurrent-threads number of threads to
-download simultaneously --max-concurrent-domains number of domains to download
-simultaneously --max-concurrent-albums number of albums to download
-simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-throttle this is a throttle between requests during the downloading phase, the
-number is in seconds --output-last-forum-post outputs the last post of a forum
-scrape to use as a starting point for future runs --scrape-single-post scrapes
-a single post from a forum thread --separate-posts separates forum scraping
-into folders by post number --gofile-api-key api key for premium gofile --
-gofile-website-token website token for gofile --pixeldrain-api-key api key for
-premium pixeldrain --nudostar-username username to login to nudostar --
-nudostar-password password to login to nudostar --simpcity-username username to
-login to simpcity --simpcity-password password to login to simpcity --
-socialmediagirls-username username to login to socialmediagirls --
-socialmediagirls-password password to login to socialmediagirls --xbunker-
-username username to login to xbunker --xbunker-password password to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table --visible-rows-threads number of visible
-rows to use for the threads table --visible-rows-domains number of visible rows
-to use for the domains table --visible-rows-albums number of visible rows to
-use for the albums table --visible-rows-files number of visible rows to use for
-the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
-"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
-"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
-"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
-"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
-"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+disable-attempt-limit disables the attempt limitation --filesize-maximum-images
+maximum filesize for images --filesize-maximum-videos maximum filesize for
+videos --filesize-maximum-other maximum filesize for other files --filesize-
+minimum-images minimum filesize for images --filesize-minimum-videos minimum
+filesize for videos --filesize-minimum-other minimum filesize for other files -
+-include-id include the ID in the download folder name --max-concurrent-threads
+number of threads to download simultaneously --max-concurrent-domains number of
+domains to download simultaneously --max-concurrent-albums number of albums to
+download simultaneously --max-concurrent-downloads-per-domain number of
+simultaneous downloads per domain --skip-download-mark-completed sets the
+scraped files as downloaded without downloading --output-errored-urls sets the
+failed urls to be output to the errored urls file --output-unsupported-urls
+sets the unsupported urls to be output to the unsupported urls file --proxy
+HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port] --
+remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --throttle this is a throttle between
+requests during the downloading phase, the number is in seconds --output-last-
+forum-post outputs the last post of a forum scrape to use as a starting point
+for future runs --scrape-single-post scrapes a single post from a forum thread
+--separate-posts separates forum scraping into folders by post number --gofile-
+api-key api key for premium gofile --gofile-website-token website token for
+gofile --pixeldrain-api-key api key for premium pixeldrain --nudostar-username
+username to login to nudostar --nudostar-password password to login to nudostar
+--simpcity-username username to login to simpcity --simpcity-password password
+to login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
+socialmediagirls --xbunker-username username to login to xbunker --xbunker-
+password password to login to xbunker --apply-jdownloader enables sending
+unsupported URLs to a running jdownloader2 instance to download --jdownloader-
+username username to login to jdownloader --jdownloader-password password to
+login to jdownloader --jdownloader-device device name to login to for
+jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table --
+visible-rows-threads number of visible rows to use for the threads table --
+visible-rows-domains number of visible rows to use for the domains table --
+visible-rows-albums number of visible rows to use for the albums table --
+visible-rows-files number of visible rows to use for the files table ``` `--
+only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,20 +61,20 @@
     config_group = config_data["Runtime"]
     runtime_opts = parser.add_argument_group("Runtime options")
     runtime_opts.add_argument("--allow-insecure-connections", help="allows insecure connections from content hosts", action="store_true")
     runtime_opts.add_argument("--attempts", type=int, help="number of attempts to download each file (default: %(default)s)", default=config_group["attempts"])
     runtime_opts.add_argument("--block-sub-folders", help="block sub folders from being created", action="store_true")
     runtime_opts.add_argument("--check-for-partial-files-and-empty-dirs", type=bool, default=config_group["check_for_partial_files_and_empty_dirs"], help="checks for partial files and empty directories after completing (default: %(default)s)")
     runtime_opts.add_argument("--disable-attempt-limit", help="disables the attempt limitation", action="store_true")
-    runtime_opts.add_argument("--filesize_maximum_images", type=int, default=config_group["filesize_maximum_images"], help="maximum filesize for images (default: %(default)s)")
-    runtime_opts.add_argument("--filesize_maximum_videos", type=int, default=config_group["filesize_maximum_videos"], help="maximum filesize for videos (default: %(default)s)")
-    runtime_opts.add_argument("--filesize_maximum_other", type=int, default=config_group["filesize_maximum_other"], help="maximum filesize for other files (default: %(default)s)")
-    runtime_opts.add_argument("--filesize_minimum_images", type=int, default=config_group["filesize_minimum_images"], help="minimum filesize for images (default: %(default)s)")
-    runtime_opts.add_argument("--filesize_minimum_videos", type=int, default=config_group["filesize_minimum_videos"], help="minimum filesize for videos (default: %(default)s)")
-    runtime_opts.add_argument("--filesize_minimum_other", type=int, default=config_group["filesize_minimum_other"], help="minimum filesize for other files (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-maximum-images", type=int, default=config_group["filesize_maximum_images"], help="maximum filesize for images (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-maximum-videos", type=int, default=config_group["filesize_maximum_videos"], help="maximum filesize for videos (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-maximum-other", type=int, default=config_group["filesize_maximum_other"], help="maximum filesize for other files (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-minimum-images", type=int, default=config_group["filesize_minimum_images"], help="minimum filesize for images (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-minimum-videos", type=int, default=config_group["filesize_minimum_videos"], help="minimum filesize for videos (default: %(default)s)")
+    runtime_opts.add_argument("--filesize-minimum-other", type=int, default=config_group["filesize_minimum_other"], help="minimum filesize for other files (default: %(default)s)")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
     runtime_opts.add_argument("--max-concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
```

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.61/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.59
+Version: 4.2.61
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -145,14 +145,20 @@
 --only-hosts            only allows downloads and scraping from these hosts
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
+--filesize-maximum-images               maximum filesize for images
+--filesize-maximum-videos               maximum filesize for videos
+--filesize-maximum-other                maximum filesize for other files
+--filesize-minimum-images               minimum filesize for images
+--filesize-minimum-videos               minimum filesize for videos
+--filesize-minimum-other                minimum filesize for other files
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.59 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.61 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -127,58 +127,63 @@
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
-disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --max-concurrent-threads number of threads to
-download simultaneously --max-concurrent-domains number of domains to download
-simultaneously --max-concurrent-albums number of albums to download
-simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-throttle this is a throttle between requests during the downloading phase, the
-number is in seconds --output-last-forum-post outputs the last post of a forum
-scrape to use as a starting point for future runs --scrape-single-post scrapes
-a single post from a forum thread --separate-posts separates forum scraping
-into folders by post number --gofile-api-key api key for premium gofile --
-gofile-website-token website token for gofile --pixeldrain-api-key api key for
-premium pixeldrain --nudostar-username username to login to nudostar --
-nudostar-password password to login to nudostar --simpcity-username username to
-login to simpcity --simpcity-password password to login to simpcity --
-socialmediagirls-username username to login to socialmediagirls --
-socialmediagirls-password password to login to socialmediagirls --xbunker-
-username username to login to xbunker --xbunker-password password to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table --visible-rows-threads number of visible
-rows to use for the threads table --visible-rows-domains number of visible rows
-to use for the domains table --visible-rows-albums number of visible rows to
-use for the albums table --visible-rows-files number of visible rows to use for
-the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
-"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
-"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
-"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
-"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
-"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+disable-attempt-limit disables the attempt limitation --filesize-maximum-images
+maximum filesize for images --filesize-maximum-videos maximum filesize for
+videos --filesize-maximum-other maximum filesize for other files --filesize-
+minimum-images minimum filesize for images --filesize-minimum-videos minimum
+filesize for videos --filesize-minimum-other minimum filesize for other files -
+-include-id include the ID in the download folder name --max-concurrent-threads
+number of threads to download simultaneously --max-concurrent-domains number of
+domains to download simultaneously --max-concurrent-albums number of albums to
+download simultaneously --max-concurrent-downloads-per-domain number of
+simultaneous downloads per domain --skip-download-mark-completed sets the
+scraped files as downloaded without downloading --output-errored-urls sets the
+failed urls to be output to the errored urls file --output-unsupported-urls
+sets the unsupported urls to be output to the unsupported urls file --proxy
+HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port] --
+remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --throttle this is a throttle between
+requests during the downloading phase, the number is in seconds --output-last-
+forum-post outputs the last post of a forum scrape to use as a starting point
+for future runs --scrape-single-post scrapes a single post from a forum thread
+--separate-posts separates forum scraping into folders by post number --gofile-
+api-key api key for premium gofile --gofile-website-token website token for
+gofile --pixeldrain-api-key api key for premium pixeldrain --nudostar-username
+username to login to nudostar --nudostar-password password to login to nudostar
+--simpcity-username username to login to simpcity --simpcity-password password
+to login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
+socialmediagirls --xbunker-username username to login to xbunker --xbunker-
+password password to login to xbunker --apply-jdownloader enables sending
+unsupported URLs to a running jdownloader2 instance to download --jdownloader-
+username username to login to jdownloader --jdownloader-password password to
+login to jdownloader --jdownloader-device device name to login to for
+jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table --
+visible-rows-threads number of visible rows to use for the threads table --
+visible-rows-domains number of visible rows to use for the domains table --
+visible-rows-albums number of visible rows to use for the albums table --
+visible-rows-files number of visible rows to use for the files table ``` `--
+only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.59/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.61/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.59/setup.cfg` & `cyberdrop-dl-4.2.61/setup.cfg`

 * *Files identical despite different names*

