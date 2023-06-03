# Comparing `tmp/envutil-0.2.0.tar.gz` & `tmp/envutil-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envutil-0.2.0.tar", max compression
+gzip compressed data, was "envutil-0.2.1.tar", max compression
```

## Comparing `envutil-0.2.0.tar` & `envutil-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-03 17:17:31.415430 envutil-0.2.0/README.md
--rw-r--r--   0        0        0     1826 2023-06-03 17:27:15.960244 envutil-0.2.0/envutil/__init__.py
--rw-r--r--   0        0        0      346 2023-06-03 17:27:22.798729 envutil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 envutil-0.2.0/setup.py
--rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 envutil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1881 2023-06-03 20:11:41.633075 envutil-0.2.1/README.md
+-rw-r--r--   0        0        0     1826 2023-06-03 17:31:11.833293 envutil-0.2.1/envutil/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-03 20:25:46.606889 envutil-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 envutil-0.2.1/setup.py
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 envutil-0.2.1/PKG-INFO
```

### Comparing `envutil-0.2.0/envutil/__init__.py` & `envutil-0.2.1/envutil/__init__.py`

 * *Files identical despite different names*

