# Comparing `tmp/packages-0.1.0.tar.gz` & `tmp/packages-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packages-0.1.0.tar", last modified: Sun Dec 15 20:43:59 2019, max compression
+gzip compressed data, was "packages-0.1.1.tar", max compression
```

## Comparing `packages-0.1.0.tar` & `packages-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,18 @@
--rw-r--r--   0        0        0       22 2019-12-15 20:43:33.898736 packages-0.1.0/packages/__init__.py
--rw-r--r--   0        0        0      286 2019-12-15 20:43:33.902736 packages-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      493 2019-12-15 20:43:59.145302 packages-0.1.0/setup.py
--rw-r--r--   0        0        0      240 2019-12-15 20:43:59.145565 packages-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-03 12:53:03.171976 packages-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0       22 2023-06-03 12:50:38.766960 packages-0.1.1/packages/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-03 12:50:38.766960 packages-0.1.1/packages/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:50:38.766960 packages-0.1.1/packages/aggs/__init__.py
+-rw-r--r--   0        0        0     1509 2023-06-03 12:50:38.766960 packages-0.1.1/packages/aggs/contains_wheel_metadata.json
+-rw-r--r--   0        0        0     1352 2023-06-03 12:50:38.766960 packages-0.1.1/packages/aggs/has_multiple_dist_info.json
+-rw-r--r--   0        0        0      276 2023-06-03 12:50:38.766960 packages-0.1.1/packages/cli.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/_options.py
+-rw-r--r--   0        0        0      672 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/agg.py
+-rw-r--r--   0        0        0      416 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/list_wheel_files.py
+-rw-r--r--   0        0        0     3649 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/update_db.py
+-rw-r--r--   0        0        0     2254 2023-06-03 12:50:38.766960 packages-0.1.1/packages/commands/update_wheel_info.py
+-rw-r--r--   0        0        0      802 2023-06-03 12:50:38.766960 packages-0.1.1/packages/data.py
+-rw-r--r--   0        0        0     2406 2023-06-03 12:50:38.766960 packages-0.1.1/packages/network.py
+-rw-r--r--   0        0        0      515 2023-06-03 13:03:34.868434 packages-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      914 2023-06-03 13:03:58.236295 packages-0.1.1/setup.py
+-rw-r--r--   0        0        0      731 2023-06-03 13:03:58.236446 packages-0.1.1/PKG-INFO
```

