# Comparing `tmp/dist_buble-1.0.tar.gz` & `tmp/dist_buble-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist_buble-1.0.tar", last modified: Sat Jun  3 15:42:16 2023, max compression
+gzip compressed data, was "dist_buble-1.1.tar", last modified: Sat Jun  3 15:57:57 2023, max compression
```

## Comparing `dist_buble-1.0.tar` & `dist_buble-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 15:42:16.558113 dist_buble-1.0/
--rw-rw-rw-   0        0        0      107 2023-06-03 15:42:16.562133 dist_buble-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 15:42:16.550113 dist_buble-1.0/dist_buble/
--rw-rw-rw-   0        0        0      330 2023-06-02 12:21:22.000000 dist_buble-1.0/dist_buble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 15:42:16.558113 dist_buble-1.0/dist_buble.egg-info/
--rw-rw-rw-   0        0        0      107 2023-06-03 15:42:16.000000 dist_buble-1.0/dist_buble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-03 15:42:16.000000 dist_buble-1.0/dist_buble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 15:42:16.000000 dist_buble-1.0/dist_buble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 15:42:16.000000 dist_buble-1.0/dist_buble.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-06-03 15:42:16.000000 dist_buble-1.0/dist_buble.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 15:42:16.562133 dist_buble-1.0/setup.cfg
--rw-rw-rw-   0        0        0      199 2023-06-02 17:14:22.000000 dist_buble-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 15:57:57.409531 dist_buble-1.1/
+-rw-rw-rw-   0        0        0      107 2023-06-03 15:57:57.409531 dist_buble-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 15:57:57.401632 dist_buble-1.1/dist_buble/
+-rw-rw-rw-   0        0        0      476 2023-06-03 15:54:35.000000 dist_buble-1.1/dist_buble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 15:57:57.409531 dist_buble-1.1/dist_buble.egg-info/
+-rw-rw-rw-   0        0        0      107 2023-06-03 15:57:57.000000 dist_buble-1.1/dist_buble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-03 15:57:57.000000 dist_buble-1.1/dist_buble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 15:57:57.000000 dist_buble-1.1/dist_buble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 15:42:16.000000 dist_buble-1.1/dist_buble.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-06-03 15:57:57.000000 dist_buble-1.1/dist_buble.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 15:57:57.413534 dist_buble-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      199 2023-06-03 15:57:05.000000 dist_buble-1.1/setup.py
```

