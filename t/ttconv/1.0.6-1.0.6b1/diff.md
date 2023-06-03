# Comparing `tmp/ttconv-1.0.6.tar.gz` & `tmp/ttconv-1.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\projects\ttconv\ttconv-repo\dist\.tmp-y658k9vv\ttconv-1.0.6.tar", last modified: Sat Jun  3 18:50:34 2023, max compression
+gzip compressed data, was "Z:\projects\ttconv\ttconv-repo\dist\.tmp-w249rgxa\ttconv-1.0.6b1.tar", last modified: Tue Jan  3 18:12:40 2023, max compression
```

## Comparing `ttconv-1.0.6.tar` & `ttconv-1.0.6b1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:36.000000 ttconv-1.0.6/
--rw-rw-rw-   0        0        0     1307 2021-10-11 17:26:33.000000 ttconv-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     9142 2023-06-03 18:50:36.000000 ttconv-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8154 2023-01-13 10:29:19.000000 ttconv-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 18:50:36.000000 ttconv-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-06-03 18:41:04.000000 ttconv-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:33.000000 ttconv-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:33.000000 ttconv-1.0.6/src/main/
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:33.000000 ttconv-1.0.6/src/main/python/
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:33.000000 ttconv-1.0.6/src/main/python/ttconv/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/__init__.py
--rw-rw-rw-   0        0        0     3280 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/config.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:34.000000 ttconv-1.0.6/src/main/python/ttconv/filters/
--rw-rw-rw-   0        0        0     1597 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/filters/__init__.py
--rw-rw-rw-   0        0        0     3168 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/filters/default_style_properties.py
--rw-rw-rw-   0        0        0     3100 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/filters/merge_paragraphs.py
--rw-rw-rw-   0        0        0     2589 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/filters/merge_regions.py
--rw-rw-rw-   0        0        0     2708 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/filters/supported_style_properties.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:34.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:33.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/__init__.py
--rw-rw-rw-   0        0        0    13236 2023-01-14 04:29:13.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/attributes.py
--rw-rw-rw-   0        0        0     2731 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/config.py
--rw-rw-rw-   0        0        0    50347 2023-01-14 06:56:35.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/elements.py
--rw-rw-rw-   0        0        0     1734 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/namespaces.py
--rw-rw-rw-   0        0        0     2054 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/reader.py
--rw-rw-rw-   0        0        0    33907 2023-01-14 06:56:35.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/style_properties.py
--rw-rw-rw-   0        0        0     9024 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/utils.py
--rw-rw-rw-   0        0        0     3464 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/imsc/writer.py
--rw-rw-rw-   0        0        0    44407 2023-01-14 06:55:43.000000 ttconv-1.0.6/src/main/python/ttconv/isd.py
--rw-rw-rw-   0        0        0    33484 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/model.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:35.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/
--rw-rw-rw-   0        0        0     2555 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/attribute_codes.py
--rw-rw-rw-   0        0        0     3641 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/control_codes.py
--rw-rw-rw-   0        0        0     3224 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/mid_row_codes.py
--rw-rw-rw-   0        0        0     5711 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/preambles_address_codes.py
--rw-rw-rw-   0        0        0    10066 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/special_characters.py
--rw-rw-rw-   0        0        0     4592 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/codes/standard_characters.py
--rw-rw-rw-   0        0        0     2677 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/config.py
--rw-rw-rw-   0        0        0     8693 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/content.py
--rw-rw-rw-   0        0        0     3209 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/disassembly.py
--rw-rw-rw-   0        0        0     1732 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/dump.py
--rw-rw-rw-   0        0        0     6127 2022-06-09 17:44:38.000000 ttconv-1.0.6/src/main/python/ttconv/scc/line.py
--rw-rw-rw-   0        0        0    19826 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/paragraph.py
--rw-rw-rw-   0        0        0    25285 2023-06-03 18:39:45.000000 ttconv-1.0.6/src/main/python/ttconv/scc/reader.py
--rw-rw-rw-   0        0        0     2402 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/style.py
--rw-rw-rw-   0        0        0     3410 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/utils.py
--rw-rw-rw-   0        0        0     3438 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/scc/word.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:35.000000 ttconv-1.0.6/src/main/python/ttconv/srt/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/srt/__init__.py
--rw-rw-rw-   0        0        0     3654 2021-10-13 14:17:36.000000 ttconv-1.0.6/src/main/python/ttconv/srt/paragraph.py
--rw-rw-rw-   0        0        0     7837 2021-10-13 14:27:18.000000 ttconv-1.0.6/src/main/python/ttconv/srt/reader.py
--rw-rw-rw-   0        0        0     2908 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/srt/style.py
--rw-rw-rw-   0        0        0     7155 2021-10-13 14:17:36.000000 ttconv-1.0.6/src/main/python/ttconv/srt/writer.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:35.000000 ttconv-1.0.6/src/main/python/ttconv/stl/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/stl/__init__.py
--rw-rw-rw-   0        0        0     3512 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/stl/config.py
--rw-rw-rw-   0        0        0    16385 2022-12-03 05:21:03.000000 ttconv-1.0.6/src/main/python/ttconv/stl/datafile.py
--rw-rw-rw-   0        0        0    10018 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/stl/iso6937.py
--rw-rw-rw-   0        0        0     2483 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/stl/reader.py
--rw-rw-rw-   0        0        0     8714 2021-10-11 17:26:34.000000 ttconv-1.0.6/src/main/python/ttconv/stl/tf.py
--rw-rw-rw-   0        0        0    22185 2023-02-02 06:04:29.000000 ttconv-1.0.6/src/main/python/ttconv/style_properties.py
--rw-rw-rw-   0        0        0    11327 2021-10-11 17:26:35.000000 ttconv-1.0.6/src/main/python/ttconv/time_code.py
--rw-rw-rw-   0        0        0    12897 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/tt.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:35.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/
--rw-rw-rw-   0        0        0        0 2021-10-11 17:26:35.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/__init__.py
--rw-rw-rw-   0        0        0     1901 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/config.py
--rw-rw-rw-   0        0        0     1880 2021-10-11 17:26:35.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/css_class.py
--rw-rw-rw-   0        0        0     4563 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/cue.py
--rw-rw-rw-   0        0        0    17505 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/reader.py
--rw-rw-rw-   0        0        0     4243 2021-10-11 17:26:35.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/style.py
--rw-rw-rw-   0        0        0     7798 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/tokenizer.py
--rw-rw-rw-   0        0        0    10059 2023-01-13 10:29:19.000000 ttconv-1.0.6/src/main/python/ttconv/vtt/writer.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:50:35.000000 ttconv-1.0.6/ttconv.egg-info/
--rw-rw-rw-   0        0        0     9142 2023-06-03 18:50:33.000000 ttconv-1.0.6/ttconv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2536 2023-06-03 18:50:33.000000 ttconv-1.0.6/ttconv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 18:50:33.000000 ttconv-1.0.6/ttconv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-03 18:50:33.000000 ttconv-1.0.6/ttconv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 18:50:33.000000 ttconv-1.0.6/ttconv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:36.524205 ttconv-1.0.6b1/
+-rw-rw-rw-   0        0        0     1307 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/LICENSE.txt
+-rw-rw-rw-   0        0        0     9021 2023-01-03 18:12:40.659091 ttconv-1.0.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     8031 2023-01-02 21:45:21.000000 ttconv-1.0.6b1/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-03 18:12:40.674732 ttconv-1.0.6b1/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2023-01-03 17:04:17.000000 ttconv-1.0.6b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:36.414825 ttconv-1.0.6b1/src/
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:36.414825 ttconv-1.0.6b1/src/main/
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:36.414825 ttconv-1.0.6b1/src/main/python/
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:37.539929 ttconv-1.0.6b1/src/main/python/ttconv/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/__init__.py
+-rw-rw-rw-   0        0        0     3280 2022-04-25 21:50:50.000000 ttconv-1.0.6b1/src/main/python/ttconv/config.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:37.805586 ttconv-1.0.6b1/src/main/python/ttconv/filters/
+-rw-rw-rw-   0        0        0     1597 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/filters/__init__.py
+-rw-rw-rw-   0        0        0     3168 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/filters/default_style_properties.py
+-rw-rw-rw-   0        0        0     3100 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/filters/merge_paragraphs.py
+-rw-rw-rw-   0        0        0     2589 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/filters/merge_regions.py
+-rw-rw-rw-   0        0        0     2708 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/filters/supported_style_properties.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:38.493164 ttconv-1.0.6b1/src/main/python/ttconv/imsc/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:33.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/__init__.py
+-rw-rw-rw-   0        0        0    13236 2021-12-09 15:54:37.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/attributes.py
+-rw-rw-rw-   0        0        0     2731 2022-01-19 14:22:54.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/config.py
+-rw-rw-rw-   0        0        0    50347 2021-12-09 15:54:37.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/elements.py
+-rw-rw-rw-   0        0        0     1734 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/namespaces.py
+-rw-rw-rw-   0        0        0     2054 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/reader.py
+-rw-rw-rw-   0        0        0    33907 2022-01-19 14:22:54.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/style_properties.py
+-rw-rw-rw-   0        0        0     9024 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/utils.py
+-rw-rw-rw-   0        0        0     3464 2022-04-14 03:48:58.000000 ttconv-1.0.6b1/src/main/python/ttconv/imsc/writer.py
+-rw-rw-rw-   0        0        0    44407 2021-12-27 04:21:28.000000 ttconv-1.0.6b1/src/main/python/ttconv/isd.py
+-rw-rw-rw-   0        0        0    33484 2022-12-12 04:40:47.000000 ttconv-1.0.6b1/src/main/python/ttconv/model.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:39.165387 ttconv-1.0.6b1/src/main/python/ttconv/scc/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:39.524825 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/
+-rw-rw-rw-   0        0        0     2497 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/__init__.py
+-rw-rw-rw-   0        0        0     4537 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/attribute_codes.py
+-rw-rw-rw-   0        0        0     3657 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/control_codes.py
+-rw-rw-rw-   0        0        0     3252 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/mid_row_codes.py
+-rw-rw-rw-   0        0        0     5711 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/preambles_address_codes.py
+-rw-rw-rw-   0        0        0    10100 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/special_characters.py
+-rw-rw-rw-   0        0        0     4592 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/standard_characters.py
+-rw-rw-rw-   0        0        0     2677 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/config.py
+-rw-rw-rw-   0        0        0     8693 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/content.py
+-rw-rw-rw-   0        0        0     3209 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/disassembly.py
+-rw-rw-rw-   0        0        0     1732 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/dump.py
+-rw-rw-rw-   0        0        0     6127 2022-06-09 17:44:38.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/line.py
+-rw-rw-rw-   0        0        0    19826 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/paragraph.py
+-rw-rw-rw-   0        0        0    25273 2022-02-27 23:02:40.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/reader.py
+-rw-rw-rw-   0        0        0     2402 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/style.py
+-rw-rw-rw-   0        0        0     3410 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/utils.py
+-rw-rw-rw-   0        0        0     3438 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/scc/word.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:39.885280 ttconv-1.0.6b1/src/main/python/ttconv/srt/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/srt/__init__.py
+-rw-rw-rw-   0        0        0     3654 2021-10-13 14:17:36.000000 ttconv-1.0.6b1/src/main/python/ttconv/srt/paragraph.py
+-rw-rw-rw-   0        0        0     7837 2021-10-13 14:27:18.000000 ttconv-1.0.6b1/src/main/python/ttconv/srt/reader.py
+-rw-rw-rw-   0        0        0     2908 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/srt/style.py
+-rw-rw-rw-   0        0        0     7155 2021-10-13 14:17:36.000000 ttconv-1.0.6b1/src/main/python/ttconv/srt/writer.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:40.236350 ttconv-1.0.6b1/src/main/python/ttconv/stl/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/__init__.py
+-rw-rw-rw-   0        0        0     3512 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/config.py
+-rw-rw-rw-   0        0        0    16385 2022-12-03 05:21:03.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/datafile.py
+-rw-rw-rw-   0        0        0    10018 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/iso6937.py
+-rw-rw-rw-   0        0        0     2483 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/reader.py
+-rw-rw-rw-   0        0        0     8714 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/stl/tf.py
+-rw-rw-rw-   0        0        0    22185 2021-10-11 17:26:34.000000 ttconv-1.0.6b1/src/main/python/ttconv/style_properties.py
+-rw-rw-rw-   0        0        0    11327 2021-10-11 17:26:35.000000 ttconv-1.0.6b1/src/main/python/ttconv/time_code.py
+-rw-rw-rw-   0        0        0    12897 2022-12-09 00:09:20.000000 ttconv-1.0.6b1/src/main/python/ttconv/tt.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:40.502803 ttconv-1.0.6b1/src/main/python/ttconv/vtt/
+-rw-rw-rw-   0        0        0        0 2021-10-11 17:26:35.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/__init__.py
+-rw-rw-rw-   0        0        0     1808 2022-01-19 14:22:54.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/config.py
+-rw-rw-rw-   0        0        0     1880 2021-10-11 17:26:35.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/css_class.py
+-rw-rw-rw-   0        0        0     4514 2022-01-19 14:22:54.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/cue.py
+-rw-rw-rw-   0        0        0    17505 2023-01-03 16:36:32.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/reader.py
+-rw-rw-rw-   0        0        0     4243 2021-10-11 17:26:35.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/style.py
+-rw-rw-rw-   0        0        0     7798 2023-01-02 04:25:37.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/tokenizer.py
+-rw-rw-rw-   0        0        0    10026 2022-01-19 14:22:54.000000 ttconv-1.0.6b1/src/main/python/ttconv/vtt/writer.py
+drwxrwxrwx   0        0        0        0 2023-01-03 18:12:40.627822 ttconv-1.0.6b1/ttconv.egg-info/
+-rw-rw-rw-   0        0        0     9021 2023-01-03 18:12:36.000000 ttconv-1.0.6b1/ttconv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2536 2023-01-03 18:12:36.000000 ttconv-1.0.6b1/ttconv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-03 18:12:36.000000 ttconv-1.0.6b1/ttconv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-01-03 18:12:36.000000 ttconv-1.0.6b1/ttconv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-01-03 18:12:36.000000 ttconv-1.0.6b1/ttconv.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ttconv-1.0.6/LICENSE.txt` & `ttconv-1.0.6b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/PKG-INFO` & `ttconv-1.0.6b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttconv
-Version: 1.0.6
+Version: 1.0.6b1
 Summary: Library for conversion of common timed text formats
 Home-page: https://github.com/sandflow/ttconv
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/ttconv/issues
 Project-URL: Source, https://github.com/sandflow/ttconv
 Keywords: ttml,timed text,caption,subtitle,imsc,scc,srt,stl,smpte-tt,conversion,vtt,webvtt,608
@@ -200,22 +200,14 @@
 
 `"line_position" : true | false`
 
 `true` means that the VTT writer outputs line and line alignment cue settings
 
 Default: `false`
 
-#### cue_id
-
-`"cue_id" : true | false`
-
-`true` means that the VTT writer outputs cue identifiers
-
-Default: `true`
-
 ### Library
 
 The overall architecture of the library is as follows:
 
 * Reader modules validate and convert input files into instances of the canonical model (see `ttconv.imsc.reader.to_model()` for
   example);
 * Filter modules transform instances of the canonical data model, e.g. all text styling and positioning might be removed from an
```

### Comparing `ttconv-1.0.6/README.md` & `ttconv-1.0.6b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -177,22 +177,14 @@
 
 `"line_position" : true | false`
 
 `true` means that the VTT writer outputs line and line alignment cue settings
 
 Default: `false`
 
-#### cue_id
-
-`"cue_id" : true | false`
-
-`true` means that the VTT writer outputs cue identifiers
-
-Default: `true`
-
 ### Library
 
 The overall architecture of the library is as follows:
 
 * Reader modules validate and convert input files into instances of the canonical model (see `ttconv.imsc.reader.to_model()` for
   example);
 * Filter modules transform instances of the canonical data model, e.g. all text styling and positioning might be removed from an
```

### Comparing `ttconv-1.0.6/setup.py` & `ttconv-1.0.6b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
-    name='ttconv',
-    version='1.0.6',
+    name='ttconv', 
+    version='1.0.6-beta.1',
     description='Library for conversion of common timed text formats',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sandflow/ttconv',
     author='Sandflow Consulting LLC',
     author_email='info@sandflow.com',
     classifiers=[
@@ -26,15 +26,15 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Multimedia'
     ],
     keywords='ttml, timed text, caption, subtitle, imsc, scc, srt, stl, smpte-tt, conversion, vtt, webvtt, 608',
 
-    package_dir={'ttconv': 'src/main/python/ttconv'},
+    package_dir={'ttconv': 'src/main/python/ttconv'}, 
 
     packages=find_packages(where='src/main/python'),
 
     python_requires='>=3.7, <4',
 
     project_urls={
         'Bug Reports': 'https://github.com/sandflow/ttconv/issues',
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/config.py` & `ttconv-1.0.6b1/src/main/python/ttconv/config.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/filters/__init__.py` & `ttconv-1.0.6b1/src/main/python/ttconv/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/filters/default_style_properties.py` & `ttconv-1.0.6b1/src/main/python/ttconv/filters/default_style_properties.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/filters/merge_paragraphs.py` & `ttconv-1.0.6b1/src/main/python/ttconv/filters/merge_paragraphs.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/filters/merge_regions.py` & `ttconv-1.0.6b1/src/main/python/ttconv/filters/merge_regions.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/filters/supported_style_properties.py` & `ttconv-1.0.6b1/src/main/python/ttconv/filters/supported_style_properties.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/attributes.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/attributes.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/config.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/config.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/elements.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/elements.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/namespaces.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/namespaces.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/reader.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/reader.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/style_properties.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/style_properties.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/utils.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/utils.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/imsc/writer.py` & `ttconv-1.0.6b1/src/main/python/ttconv/imsc/writer.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/isd.py` & `ttconv-1.0.6b1/src/main/python/ttconv/isd.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/model.py` & `ttconv-1.0.6b1/src/main/python/ttconv/model.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/__init__.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """SCC Codes"""
 
-from enum import Enum
-from typing import Tuple
 from ttconv.style_properties import NamedColors
 
 SCC_COLOR_MAPPING = {
   0x00: NamedColors.white.value,
   0x01: NamedColors.white.value,
   0x02: NamedColors.green.value,
   0x03: NamedColors.green.value,
@@ -43,24 +41,24 @@
   0x0A: NamedColors.yellow.value,
   0x0B: NamedColors.yellow.value,
   0x0C: NamedColors.magenta.value,
   0x0D: NamedColors.magenta.value
 }
 
 
-class SccCode(Enum):
+class SccCode:
   """SCC codes base definition class"""
 
   def __init__(self, channel_1: int, channel_2: int):
     if channel_1 > 0xFFFF or channel_2 > 0xFFFF:
       raise ValueError("Expected 2-bytes values")
 
     self._channel_1 = channel_1
     self._channel_2 = channel_2
 
-  def get_values(self) -> Tuple[int, int]:
+  def get_values(self) -> (int, int):
     """Returns SCC Code values"""
     return self._channel_1, self._channel_2
 
   def contains_value(self, value: int) -> bool:
     """Returns whether the specified value is contained into the SCC code channels values"""
     return value in self.get_values()
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/attribute_codes.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/attribute_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """SCC Background and Foreground Attribute Codes"""
 
 from __future__ import annotations
 
+from enum import Enum
 from typing import Optional
 
 from ttconv.scc.codes import SccCode
 from ttconv.style_properties import ColorType, NamedColors, TextDecorationType
 
 
-class SccAttributeCode(SccCode):
+class SccAttributeCode(SccCode, Enum):
   """SCC Foreground and Background Attribute Codes definition"""
   BWO = (0x1020, 0x1820, ColorType((0xFF, 0xFF, 0xFF, 0xFF)))  # Background White, Opaque
   BWS = (0x1021, 0x1821, ColorType((0xFF, 0xFF, 0xFF, 0x88)))  # Background White, Semi-transparent
   BGO = (0x1022, 0x1822, ColorType((0x00, 0xFF, 0x00, 0xFF)))  # Background Green, Opaque
   BGS = (0x1023, 0x1823, ColorType((0x00, 0xFF, 0x00, 0x88)))  # Background Green, Semi-transparent
   BBO = (0x1024, 0x1824, ColorType((0x00, 0x00, 0xFF, 0xFF)))  # Background Blue, Opaque
   BBS = (0x1025, 0x1825, ColorType((0x00, 0x00, 0xFF, 0x88)))  # Background Blue, Semi-transparent
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/control_codes.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/control_codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """SCC Control Codes"""
 
 from __future__ import annotations
 
 import typing
+from enum import Enum
 
 from ttconv.scc.codes import SccCode
 
 
-class SccControlCode(SccCode):
+class SccControlCode(SccCode, Enum):
   """SCC Control Code definition"""
   AOF = (0x1422, 0x1C22, 0x1522, 0x1D22)  # Reserved (formerly Alarm Off)
   AON = (0x1423, 0x1C23, 0x1523, 0x1D23)  # Reserved (formerly Alarm On)
   BS = (0x1421, 0x1C21, 0x1521, 0x1D21)  # Backspace
   CR = (0x142D, 0x1C2D, 0x152D, 0x1D2D)  # Carriage Return
   DER = (0x1424, 0x1C24, 0x1524, 0x1D24)  # Delete to End of Row
   EDM = (0x142C, 0x1C2C, 0x152C, 0x1D2C)  # Erase Displayed Memory
@@ -59,15 +60,15 @@
     self._channel_1_field_2 = channel_1_field_2
     self._channel_2_field_2 = channel_2_field_2
 
   def get_name(self) -> str:
     """Retrieves Control Code name"""
     return self.name
 
-  def get_values(self) -> typing.Tuple[int, int, int, int]:
+  def get_values(self) -> (int, int, int, int):
     """Returns SCC Control Code values"""
     return self._channel_1, self._channel_2, self._channel_1_field_2, self._channel_2_field_2
 
   @staticmethod
   def find(value: int) -> typing.Optional[SccControlCode]:
     """Find the Control Code corresponding to the specified value"""
     for control_code in list(SccControlCode):
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/mid_row_codes.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/mid_row_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """SCC Mid Row Codes"""
 
 from __future__ import annotations
 
 import typing
+from enum import Enum
 
 from ttconv.scc.codes import SccCode, SCC_COLOR_MAPPING
 from ttconv.style_properties import FontStyleType, TextDecorationType, ColorType
 
 
-class SccMidRowCode(SccCode):
+class SccMidRowCode(SccCode, Enum):
   """SCC Mid-Row Code values"""
   WHITE = (0x1120, 0x1920)
   WHITE_UNDERLINE = (0x1121, 0x1921)
   GREEN = (0x1122, 0x1922)
   GREEN_UNDERLINE = (0x1123, 0x1923)
   BLUE = (0x1124, 0x1924)
   BLUE_UNDERLINE = (0x1125, 0x1925)
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/preambles_address_codes.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/preambles_address_codes.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/special_characters.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/special_characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """SCC Special and Extended characters"""
 
 from __future__ import annotations
 
 import typing
+from enum import Enum
 
 from ttconv.scc.codes import SccCode
 
 
-class SccSpecialCharacter(SccCode):
+class SccSpecialCharacter(SccCode, Enum):
   """SCC Special character definition"""
 
   # Special characters specified in CEA-608
   REGISTERED_MARK_SYMBOL = (0x1130, 0x1930, '\u00AE')  # ® Registered mark symbol
   DEGREE_SIGN = (0x1131, 0x1931, '\u00B0')  # ° Degree sign
   VULGAR_FRACTION_ONE_HALF = (0x1132, 0x1932, '\u00BD')  # ¿ Inverse question mark
   INVERTED_QUESTION_MARK = (0x1133, 0x1933, '\u00BF')  # ½ Vulgar one half fraction
@@ -66,15 +67,15 @@
     """Find the special character corresponding to the specified value"""
     for spec_char in list(SccSpecialCharacter):
       if spec_char.contains_value(value):
         return spec_char
     return None
 
 
-class SccExtendedCharacter(SccCode):
+class SccExtendedCharacter(SccCode, Enum):
   """SCC Extended character definition"""
 
   # Spanish extended characters
   LATIN_CAPITAL_LETTER_A_WITH_ACUTE = (0x1220, 0x1A20, '\u00C1')  # Á capital A with acute accent
   LATIN_CAPITAL_LETTER_E_WITH_ACUTE = (0x1221, 0x1A21, '\u00C9')  # É capital E with acute accent
   LATIN_CAPITAL_LETTER_O_WITH_ACUTE = (0x1222, 0x1A22, '\u00D3')  # Ó capital O with acute accent
   LATIN_CAPITAL_LETTER_U_WITH_ACUTE = (0x1223, 0x1A23, '\u00DA')  # Ú capital U with acute accent
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/codes/standard_characters.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/codes/standard_characters.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/config.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/config.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/content.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/content.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/disassembly.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/disassembly.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/dump.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/dump.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/line.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/line.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/paragraph.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/paragraph.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/reader.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """SCC reader"""
 
 from __future__ import annotations
 
 import copy
 import logging
-from typing import Optional, Tuple
+from typing import Optional
 
 from ttconv.model import ContentDocument, Body, Div, CellResolutionType, ActiveAreaType
 from ttconv.scc.codes.attribute_codes import SccAttributeCode
 from ttconv.scc.codes.control_codes import SccControlCode
 from ttconv.scc.codes.mid_row_codes import SccMidRowCode
 from ttconv.scc.codes.preambles_address_codes import SccPreambleAddressCode
 from ttconv.scc.codes.special_characters import SccSpecialCharacter, SccExtendedCharacter
@@ -72,15 +72,15 @@
     # Caption style (Pop-on, Roll-up, Paint-on) currently processed
     self.current_style: Optional[SccCaptionStyle] = None
 
     # Roll-up caption number of lines
     self.roll_up_depth: int = 0
 
     # Cursor position in the active area
-    self.active_cursor: Tuple[int, int] = (0, 0)
+    self.active_cursor: (int, int) = (0, 0)
 
     self.current_text_decoration = None
     self.current_color = None
     self.current_font_style = None
 
     # Text alignment
     self.text_alignment = TextAlignment.AUTO if config is None else config.text_align
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/style.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/style.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/utils.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/utils.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/scc/word.py` & `ttconv-1.0.6b1/src/main/python/ttconv/scc/word.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/srt/paragraph.py` & `ttconv-1.0.6b1/src/main/python/ttconv/srt/paragraph.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/srt/reader.py` & `ttconv-1.0.6b1/src/main/python/ttconv/srt/reader.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/srt/style.py` & `ttconv-1.0.6b1/src/main/python/ttconv/srt/style.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/srt/writer.py` & `ttconv-1.0.6b1/src/main/python/ttconv/srt/writer.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/stl/config.py` & `ttconv-1.0.6b1/src/main/python/ttconv/stl/config.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/stl/datafile.py` & `ttconv-1.0.6b1/src/main/python/ttconv/stl/datafile.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/stl/iso6937.py` & `ttconv-1.0.6b1/src/main/python/ttconv/stl/iso6937.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/stl/reader.py` & `ttconv-1.0.6b1/src/main/python/ttconv/stl/reader.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/stl/tf.py` & `ttconv-1.0.6b1/src/main/python/ttconv/stl/tf.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/style_properties.py` & `ttconv-1.0.6b1/src/main/python/ttconv/style_properties.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/time_code.py` & `ttconv-1.0.6b1/src/main/python/ttconv/time_code.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/tt.py` & `ttconv-1.0.6b1/src/main/python/ttconv/tt.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/config.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,10 +36,7 @@
   
   @classmethod
   def name(cls):
     return "vtt_writer"
 
   # outputs `line` and `line alignment` cue settings
   line_position: bool = field(default=False, metadata={"decoder": bool})
-
-  # outputs cue identifier
-  cue_id: bool = field(default=True, metadata={"decoder": bool})
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/css_class.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/css_class.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/cue.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/cue.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """WebVTT line alignment cue setting"""
     start = "start"
     center = "center"
     end = "end"
 
   _EOL_SEQ_RE = re.compile(r"\n{2,}")
 
-  def __init__(self, identifier: Optional[int] = None):
+  def __init__(self, identifier: int):
     self._id: int = identifier
     self._begin: Optional[ClockTime] = None
     self._end: Optional[ClockTime] = None
     self._text: str = ""
     self._line: int = None
     self._align: VttCue.LineAlignment = None
 
@@ -114,15 +114,15 @@
       raise ValueError("VTT paragraph end time code must be greater than the begin time code.")
 
     return str(self)
 
   def __str__(self) -> str:
 
     # cue identifier
-    t = f"{self._id}\n" if self._id is not None else ""
+    t = f"{self._id}\n"
     
     # cue timing
     t += f"{self._begin} --> {self._end}"
 
     # cue line position
     if self._line is not None:
       t += f" line:{self._line}%"
```

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/reader.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/reader.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/style.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/style.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/tokenizer.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ttconv-1.0.6/src/main/python/ttconv/vtt/writer.py` & `ttconv-1.0.6b1/src/main/python/ttconv/vtt/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
       self._paragraphs[-1].append_text(element.get_text())
 
   def process_p(self, region: ISD.Region, element: model.P, begin: Fraction, end: Optional[Fraction]):
     """Process p element"""
 
     self._captions_counter += 1
 
-    cue = VttCue(self._captions_counter if self._config.cue_id else None)
+    cue = VttCue(self._captions_counter)
     cue.set_begin(begin)
     cue.set_end(end)
 
     if self._config.line_position:
       display_align = region.get_style(StyleProperties.DisplayAlign)
       position: PositionType = region.get_style(StyleProperties.Position)
       extent: ExtentType = region.get_style(StyleProperties.Extent)
```

### Comparing `ttconv-1.0.6/ttconv.egg-info/PKG-INFO` & `ttconv-1.0.6b1/ttconv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttconv
-Version: 1.0.6
+Version: 1.0.6b1
 Summary: Library for conversion of common timed text formats
 Home-page: https://github.com/sandflow/ttconv
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/ttconv/issues
 Project-URL: Source, https://github.com/sandflow/ttconv
 Keywords: ttml,timed text,caption,subtitle,imsc,scc,srt,stl,smpte-tt,conversion,vtt,webvtt,608
@@ -200,22 +200,14 @@
 
 `"line_position" : true | false`
 
 `true` means that the VTT writer outputs line and line alignment cue settings
 
 Default: `false`
 
-#### cue_id
-
-`"cue_id" : true | false`
-
-`true` means that the VTT writer outputs cue identifiers
-
-Default: `true`
-
 ### Library
 
 The overall architecture of the library is as follows:
 
 * Reader modules validate and convert input files into instances of the canonical model (see `ttconv.imsc.reader.to_model()` for
   example);
 * Filter modules transform instances of the canonical data model, e.g. all text styling and positioning might be removed from an
```

### Comparing `ttconv-1.0.6/ttconv.egg-info/SOURCES.txt` & `ttconv-1.0.6b1/ttconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

