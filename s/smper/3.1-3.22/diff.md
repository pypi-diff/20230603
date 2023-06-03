# Comparing `tmp/smper-3.1.tar.gz` & `tmp/smper-3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smper-3.1.tar", last modified: Fri Jun  2 21:03:18 2023, max compression
+gzip compressed data, was "smper-3.22.tar", last modified: Sat Jun  3 14:33:40 2023, max compression
```

## Comparing `smper-3.1.tar` & `smper-3.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.808371 smper-3.1/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-02 21:03:18.808179 smper-3.1/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.1/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-02 21:03:18.808434 smper-3.1/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      420 2023-06-02 21:03:15.000000 smper-3.1/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.806156 smper-3.1/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.806889 smper-3.1/src/smper/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.1/src/smper/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     8705 2023-06-02 21:02:03.000000 smper-3.1/src/smper/smper.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.807937 smper-3.1/src/smper.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.1/src/smper.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.099843 smper-3.22/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-03 14:33:40.099660 smper-3.22/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.22/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-03 14:33:40.099902 smper-3.22/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-03 14:33:37.000000 smper-3.22/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.097731 smper-3.22/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.098488 smper-3.22/src/smper/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.22/src/smper/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     5986 2023-06-03 14:33:20.000000 smper-3.22/src/smper/smper.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.099453 smper-3.22/src/smper.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.22/src/smper.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/top_level.txt
```

