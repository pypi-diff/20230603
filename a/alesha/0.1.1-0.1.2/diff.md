# Comparing `tmp/alesha-0.1.1.tar.gz` & `tmp/alesha-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alesha-0.1.1.tar", max compression
+gzip compressed data, was "alesha-0.1.2.tar", max compression
```

## Comparing `alesha-0.1.1.tar` & `alesha-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,3 @@
--rw-r--r--   0        0        0     6148 2023-06-03 07:48:13.931202 alesha-0.1.1/alesha/.DS_Store
--rw-r--r--   0        0        0      919 2023-06-03 06:58:23.651458 alesha-0.1.1/alesha/alesha.py
--rw-r--r--   0        0        0      282 2023-06-03 07:49:42.163284 alesha-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 alesha-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      919 2023-06-03 06:58:23.651458 alesha-0.1.2/alesha.py
+-rw-r--r--   0        0        0      248 2023-06-03 07:56:28.880857 alesha-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 alesha-0.1.2/PKG-INFO
```

### Comparing `alesha-0.1.1/alesha/alesha.py` & `alesha-0.1.2/alesha.py`

 * *Files identical despite different names*

