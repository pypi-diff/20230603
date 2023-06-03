# Comparing `tmp/kube-tests-0.0.5.tar.gz` & `tmp/kube-tests-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube-tests-0.0.5.tar", last modified: Sat Jun  3 14:28:30 2023, max compression
+gzip compressed data, was "kube-tests-0.0.6.tar", last modified: Sat Jun  3 14:35:41 2023, max compression
```

## Comparing `kube-tests-0.0.5.tar` & `kube-tests-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:28:30.767935 kube-tests-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:28:30.767935 kube-tests-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 14:28:02.000000 kube-tests-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:28:30.767935 kube-tests-0.0.5/kube_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/iloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/iparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/job_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/template_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-03 14:28:02.000000 kube-tests-0.0.5/kube_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:28:30.767935 kube-tests-0.0.5/kube_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:28:30.000000 kube-tests-0.0.5/kube_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-03 14:28:30.000000 kube-tests-0.0.5/kube_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:28:30.000000 kube-tests-0.0.5/kube_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:28:30.000000 kube-tests-0.0.5/kube_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 14:28:30.000000 kube-tests-0.0.5/kube_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-03 14:28:02.000000 kube-tests-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:28:30.767935 kube-tests-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 14:28:02.000000 kube-tests-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:41.006928 kube-tests-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:35:41.006928 kube-tests-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 14:35:13.000000 kube-tests-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:41.002927 kube-tests-0.0.6/kube_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/iloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/iparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/job_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:41.002927 kube-tests-0.0.6/kube_tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/loaders/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/loaders/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:41.006928 kube-tests-0.0.6/kube_tests/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/parsers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/parsers/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/template_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-03 14:35:13.000000 kube-tests-0.0.6/kube_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:35:41.002927 kube-tests-0.0.6/kube_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 14:35:40.000000 kube-tests-0.0.6/kube_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-03 14:35:40.000000 kube-tests-0.0.6/kube_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:35:40.000000 kube-tests-0.0.6/kube_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:35:40.000000 kube-tests-0.0.6/kube_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 14:35:40.000000 kube-tests-0.0.6/kube_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-03 14:35:13.000000 kube-tests-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:35:41.006928 kube-tests-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-03 14:35:13.000000 kube-tests-0.0.6/setup.py
```

### Comparing `kube-tests-0.0.5/kube_tests/adapter.py` & `kube-tests-0.0.6/kube_tests/adapter.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.5/kube_tests/client.py` & `kube-tests-0.0.6/kube_tests/client.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.5/kube_tests/job_builder.py` & `kube-tests-0.0.6/kube_tests/job_builder.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.5/kube_tests/template_compiler.py` & `kube-tests-0.0.6/kube_tests/template_compiler.py`

 * *Files identical despite different names*

### Comparing `kube-tests-0.0.5/kube_tests/utils.py` & `kube-tests-0.0.6/kube_tests/utils.py`

 * *Files identical despite different names*

