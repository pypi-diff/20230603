# Comparing `tmp/rendersrt-0.0.2.tar.gz` & `tmp/rendersrt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.2.tar", last modified: Thu May 25 13:34:39 2023, max compression
+gzip compressed data, was "rendersrt-0.0.3.tar", last modified: Fri Jun  2 22:26:17 2023, max compression
```

## Comparing `rendersrt-0.0.2.tar` & `rendersrt-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:34:39.051425 rendersrt-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1561 2023-05-25 13:34:39.052175 rendersrt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:34:39.008717 rendersrt-0.0.2/rendersrt/
--rw-rw-rw-   0        0        0     8045 2023-05-25 13:32:23.000000 rendersrt-0.0.2/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:34:39.049177 rendersrt-0.0.2/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1561 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 13:34:38.000000 rendersrt-0.0.2/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-05-25 13:34:39.054421 rendersrt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-05-25 07:38:45.000000 rendersrt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.460647 rendersrt-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1561 2023-06-02 22:26:17.460647 rendersrt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.435173 rendersrt-0.0.3/rendersrt/
+-rw-rw-rw-   0        0        0     9265 2023-06-02 22:26:06.000000 rendersrt-0.0.3/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:26:17.458398 rendersrt-0.0.3/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1561 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 22:26:17.000000 rendersrt-0.0.3/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-02 22:26:17.463641 rendersrt-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-06-02 22:10:10.000000 rendersrt-0.0.3/setup.py
```

### Comparing `rendersrt-0.0.2/LICENSE` & `rendersrt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.2/PKG-INFO` & `rendersrt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.2
+Version: 0.0.3
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.2/README.md` & `rendersrt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.2/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.3/rendersrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.2
+Version: 0.0.3
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

