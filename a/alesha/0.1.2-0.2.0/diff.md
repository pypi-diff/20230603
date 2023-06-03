# Comparing `tmp/alesha-0.1.2.tar.gz` & `tmp/alesha-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alesha-0.1.2.tar", max compression
+gzip compressed data, was "alesha-0.2.0.tar", max compression
```

## Comparing `alesha-0.1.2.tar` & `alesha-0.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      919 2023-06-03 06:58:23.651458 alesha-0.1.2/alesha.py
--rw-r--r--   0        0        0      248 2023-06-03 07:56:28.880857 alesha-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 alesha-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6869 2023-06-03 08:45:30.666515 alesha-0.2.0/alesha.py
+-rw-r--r--   0        0        0      248 2023-06-03 08:45:48.517009 alesha-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 alesha-0.2.0/PKG-INFO
```

