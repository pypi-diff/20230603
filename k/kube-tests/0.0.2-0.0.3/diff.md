# Comparing `tmp/kube-tests-0.0.2.tar.gz` & `tmp/kube-tests-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube-tests-0.0.2.tar", last modified: Sat Jun  3 14:10:22 2023, max compression
+gzip compressed data, was "kube-tests-0.0.3.tar", last modified: Sat Jun  3 14:12:02 2023, max compression
```

## Comparing `kube-tests-0.0.2.tar` & `kube-tests-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:10:22.757142 kube-tests-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:10:22.757142 kube-tests-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 14:09:49.000000 kube-tests-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:10:22.753142 kube-tests-0.0.2/kube_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/iloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/iparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/job_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/template_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-03 14:09:49.000000 kube-tests-0.0.2/kube_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:10:22.757142 kube-tests-0.0.2/kube_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:10:22.000000 kube-tests-0.0.2/kube_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-03 14:10:22.000000 kube-tests-0.0.2/kube_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:10:22.000000 kube-tests-0.0.2/kube_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:10:22.000000 kube-tests-0.0.2/kube_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 14:10:22.000000 kube-tests-0.0.2/kube_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-03 14:09:49.000000 kube-tests-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:10:22.757142 kube-tests-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 14:09:49.000000 kube-tests-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:12:02.180372 kube-tests-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:12:02.180372 kube-tests-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 14:11:31.000000 kube-tests-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:12:02.180372 kube-tests-0.0.3/kube_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/iloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/iparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/job_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/template_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-03 14:11:31.000000 kube-tests-0.0.3/kube_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:12:02.180372 kube-tests-0.0.3/kube_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:12:02.000000 kube-tests-0.0.3/kube_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-03 14:12:02.000000 kube-tests-0.0.3/kube_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:12:02.000000 kube-tests-0.0.3/kube_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:12:02.000000 kube-tests-0.0.3/kube_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 14:12:02.000000 kube-tests-0.0.3/kube_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-03 14:11:31.000000 kube-tests-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:12:02.180372 kube-tests-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 14:11:31.000000 kube-tests-0.0.3/setup.py
```

### Comparing `kube-tests-0.0.2/kube_tests/adapter.py` & `kube-tests-0.0.3/kube_tests/adapter.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.2/kube_tests/client.py` & `kube-tests-0.0.3/kube_tests/client.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.2/kube_tests/job_builder.py` & `kube-tests-0.0.3/kube_tests/job_builder.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.2/kube_tests/template_compiler.py` & `kube-tests-0.0.3/kube_tests/template_compiler.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.2/kube_tests/utils.py` & `kube-tests-0.0.3/kube_tests/utils.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.2/setup.py` & `kube-tests-0.0.3/setup.py`

 * *Files identical despite different names*

