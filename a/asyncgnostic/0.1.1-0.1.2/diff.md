# Comparing `tmp/asyncgnostic-0.1.1.tar.gz` & `tmp/asyncgnostic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncgnostic-0.1.1.tar", max compression
+gzip compressed data, was "asyncgnostic-0.1.2.tar", max compression
```

## Comparing `asyncgnostic-0.1.1.tar` & `asyncgnostic-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/LICENSE
--rw-r--r--   0        0        0     1232 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/README.md
--rw-r--r--   0        0        0      484 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3074 2023-06-03 11:08:53.574695 asyncgnostic-0.1.1/src/asyncgnostic/__init__.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 asyncgnostic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-03 13:18:33.679801 asyncgnostic-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2204 2023-06-03 13:18:33.679801 asyncgnostic-0.1.2/README.md
+-rw-r--r--   0        0        0      484 2023-06-03 13:18:33.679801 asyncgnostic-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3074 2023-06-03 13:18:33.679801 asyncgnostic-0.1.2/src/asyncgnostic/__init__.py
+-rw-r--r--   0        0        0     2730 1970-01-01 00:00:00.000000 asyncgnostic-0.1.2/PKG-INFO
```

### Comparing `asyncgnostic-0.1.1/LICENSE` & `asyncgnostic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgnostic-0.1.1/src/asyncgnostic/__init__.py` & `asyncgnostic-0.1.2/src/asyncgnostic/__init__.py`

 * *Files identical despite different names*

