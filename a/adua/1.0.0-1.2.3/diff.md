# Comparing `tmp/adua-1.0.0.tar.gz` & `tmp/adua-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adua-1.0.0.tar", last modified: Thu May 25 13:38:39 2023, max compression
+gzip compressed data, was "adua-1.2.3.tar", last modified: Sat Jun  3 13:03:40 2023, max compression
```

## Comparing `adua-1.0.0.tar` & `adua-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:38:39.925731 adua-1.0.0/
--rw-rw-rw-   0        0        0     1043 2023-05-25 13:13:32.000000 adua-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      254 2023-05-25 13:38:39.912935 adua-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2023-05-25 13:17:50.000000 adua-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:38:39.885731 adua-1.0.0/adua/
--rw-rw-rw-   0        0        0     4296 2023-05-25 13:04:33.000000 adua-1.0.0/adua/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:38:39.907942 adua-1.0.0/adua.egg-info/
--rw-rw-rw-   0        0        0      254 2023-05-25 13:38:39.000000 adua-1.0.0/adua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-25 13:38:39.000000 adua-1.0.0/adua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:38:39.000000 adua-1.0.0/adua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-25 13:38:39.000000 adua-1.0.0/adua.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-25 13:38:39.000000 adua-1.0.0/adua.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:38:39.925731 adua-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-05-25 13:30:51.000000 adua-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:03:40.516701 adua-1.2.3/
+-rw-rw-rw-   0        0        0     1043 2023-05-25 13:13:32.000000 adua-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-06-03 13:03:40.515674 adua-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-05-25 13:17:50.000000 adua-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 13:03:40.504307 adua-1.2.3/adua/
+-rw-rw-rw-   0        0        0     4025 2023-06-03 12:54:50.000000 adua-1.2.3/adua/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-06-03 11:57:06.000000 adua-1.2.3/adua/facerec.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:03:40.514075 adua-1.2.3/adua.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-03 13:03:40.000000 adua-1.2.3/adua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-03 13:03:40.000000 adua-1.2.3/adua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 13:03:40.000000 adua-1.2.3/adua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-03 13:03:40.000000 adua-1.2.3/adua.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-03 13:03:40.000000 adua-1.2.3/adua.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 13:03:40.516701 adua-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-06-03 12:58:37.000000 adua-1.2.3/setup.py
```

### Comparing `adua-1.0.0/LICENSE` & `adua-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adua-1.0.0/README.md` & `adua-1.2.3/README.md`

 * *Files identical despite different names*

