# Comparing `tmp/replicPy-0.1.0.tar.gz` & `tmp/replicPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicPy-0.1.0.tar", last modified: Thu Apr 13 09:16:52 2023, max compression
+gzip compressed data, was "replicPy-0.1.1.tar", last modified: Sat Jun  3 08:19:07 2023, max compression
```

## Comparing `replicPy-0.1.0.tar` & `replicPy-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:16:52.622873 replicPy-0.1.0/
--rw-rw-rw-   0        0        0       83 2023-04-13 08:27:23.000000 replicPy-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-04-13 08:32:28.000000 replicPy-0.1.0/LICENCE.txt
--rw-rw-rw-   0        0        0       26 2023-04-13 08:28:44.000000 replicPy-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      648 2023-04-13 09:16:52.621862 replicPy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-13 08:24:39.000000 replicPy-0.1.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 09:16:52.606650 replicPy-0.1.0/replicPy.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-13 09:16:52.000000 replicPy-0.1.0/replicPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-13 09:16:52.000000 replicPy-0.1.0/replicPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:16:52.000000 replicPy-0.1.0/replicPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 09:16:52.000000 replicPy-0.1.0/replicPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 09:16:52.000000 replicPy-0.1.0/replicPy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 09:16:52.609678 replicPy-0.1.0/replicpy/
--rw-rw-rw-   0        0        0        0 2023-04-11 11:53:47.000000 replicPy-0.1.0/replicpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:16:52.619624 replicPy-0.1.0/replicpy/core/
--rw-rw-rw-   0        0        0       65 2023-04-12 10:55:43.000000 replicPy-0.1.0/replicpy/core/__init__.py
--rw-rw-rw-   0        0        0      354 2023-04-12 12:02:20.000000 replicPy-0.1.0/replicpy/core/response.py
--rw-rw-rw-   0        0        0      857 2023-04-12 12:02:50.000000 replicPy-0.1.0/replicpy/core/server.py
--rw-rw-rw-   0        0        0     1127 2023-04-12 12:04:10.000000 replicPy-0.1.0/replicpy/core/setups.py
--rw-rw-rw-   0        0        0       42 2023-04-13 09:16:52.622873 replicPy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-04-13 08:57:39.000000 replicPy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:19:07.750607 replicPy-0.1.1/
+-rw-rw-rw-   0        0        0       83 2023-04-13 08:27:23.000000 replicPy-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-04-13 08:32:28.000000 replicPy-0.1.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-13 08:28:44.000000 replicPy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1426 2023-06-03 08:19:07.749616 replicPy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2023-06-03 08:18:19.000000 replicPy-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 08:19:07.729109 replicPy-0.1.1/replicPy.egg-info/
+-rw-rw-rw-   0        0        0     1426 2023-06-03 08:19:07.000000 replicPy-0.1.1/replicPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-03 08:19:07.000000 replicPy-0.1.1/replicPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 08:19:07.000000 replicPy-0.1.1/replicPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-03 08:19:07.000000 replicPy-0.1.1/replicPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 08:19:07.000000 replicPy-0.1.1/replicPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 08:19:07.732753 replicPy-0.1.1/replicpy/
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:53:47.000000 replicPy-0.1.1/replicpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:19:07.746384 replicPy-0.1.1/replicpy/core/
+-rw-rw-rw-   0        0        0      101 2023-06-03 07:34:12.000000 replicPy-0.1.1/replicpy/core/__init__.py
+-rw-rw-rw-   0        0        0      506 2023-06-03 07:34:14.000000 replicPy-0.1.1/replicpy/core/response.py
+-rw-rw-rw-   0        0        0     1531 2023-06-03 07:34:09.000000 replicPy-0.1.1/replicpy/core/server.py
+-rw-rw-rw-   0        0        0     1127 2023-04-12 12:04:10.000000 replicPy-0.1.1/replicpy/core/setups.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 08:19:07.751604 replicPy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-03 08:15:39.000000 replicPy-0.1.1/setup.py
```

### Comparing `replicPy-0.1.0/LICENCE.txt` & `replicPy-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `replicPy-0.1.0/replicpy/core/setups.py` & `replicPy-0.1.1/replicpy/core/setups.py`

 * *Files identical despite different names*

