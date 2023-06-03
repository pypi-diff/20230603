# Comparing `tmp/sleeptimer-1.0.0.tar.gz` & `tmp/sleeptimer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleeptimer-1.0.0.tar", last modified: Sat Jun  3 17:16:27 2023, max compression
+gzip compressed data, was "sleeptimer-1.0.1.tar", last modified: Sat Jun  3 17:47:19 2023, max compression
```

## Comparing `sleeptimer-1.0.0.tar` & `sleeptimer-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:16:27.298083 sleeptimer-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)      193 2023-06-03 17:16:27.297810 sleeptimer-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-03 17:16:27.298304 sleeptimer-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      344 2023-06-03 17:09:51.000000 sleeptimer-1.0.0/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:16:27.295679 sleeptimer-1.0.0/sleeptimer/
--rw-r--r--   0 mac        (501) staff       (20)     2204 2023-06-03 17:05:53.000000 sleeptimer-1.0.0/sleeptimer/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:16:27.297474 sleeptimer-1.0.0/sleeptimer.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      193 2023-06-03 17:16:27.000000 sleeptimer-1.0.0/sleeptimer.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      200 2023-06-03 17:16:27.000000 sleeptimer-1.0.0/sleeptimer.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-03 17:16:27.000000 sleeptimer-1.0.0/sleeptimer.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-06-03 17:16:27.000000 sleeptimer-1.0.0/sleeptimer.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-03 17:16:27.000000 sleeptimer-1.0.0/sleeptimer.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:47:19.419101 sleeptimer-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)     1065 2023-06-03 17:35:12.000000 sleeptimer-1.0.1/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      215 2023-06-03 17:47:19.418800 sleeptimer-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1703 2023-06-03 17:44:38.000000 sleeptimer-1.0.1/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-03 17:47:19.419183 sleeptimer-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      294 2023-06-03 17:44:30.000000 sleeptimer-1.0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:47:19.415770 sleeptimer-1.0.1/sleeptimer/
+-rw-r--r--   0 mac        (501) staff       (20)     2204 2023-06-03 17:05:53.000000 sleeptimer-1.0.1/sleeptimer/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-03 17:47:19.418442 sleeptimer-1.0.1/sleeptimer.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      215 2023-06-03 17:47:19.000000 sleeptimer-1.0.1/sleeptimer.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      185 2023-06-03 17:47:19.000000 sleeptimer-1.0.1/sleeptimer.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-03 17:47:19.000000 sleeptimer-1.0.1/sleeptimer.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-03 17:47:19.000000 sleeptimer-1.0.1/sleeptimer.egg-info/top_level.txt
```

### Comparing `sleeptimer-1.0.0/sleeptimer/__init__.py` & `sleeptimer-1.0.1/sleeptimer/__init__.py`

 * *Files identical despite different names*

