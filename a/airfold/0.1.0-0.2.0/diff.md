# Comparing `tmp/airfold-0.1.0.tar.gz` & `tmp/airfold-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airfold-0.1.0.tar", last modified: Sat Jun  3 15:57:10 2023, max compression
+gzip compressed data, was "airfold-0.2.0.tar", last modified: Sat Jun  3 18:46:17 2023, max compression
```

## Comparing `airfold-0.1.0.tar` & `airfold-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,47 @@
-drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 15:57:10.885913 airfold-0.1.0/
--rw-rw-r--   0 kit       (1000) kit       (1000)    11357 2023-06-03 15:19:50.000000 airfold-0.1.0/LICENSE
--rw-rw-r--   0 kit       (1000) kit       (1000)      421 2023-06-03 15:57:10.885913 airfold-0.1.0/PKG-INFO
--rw-rw-r--   0 kit       (1000) kit       (1000)      103 2023-04-21 00:48:16.000000 airfold-0.1.0/README.md
-drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 15:57:10.885913 airfold-0.1.0/airfold.egg-info/
--rw-rw-r--   0 kit       (1000) kit       (1000)      421 2023-06-03 15:57:10.000000 airfold-0.1.0/airfold.egg-info/PKG-INFO
--rw-rw-r--   0 kit       (1000) kit       (1000)      317 2023-06-03 15:57:10.000000 airfold-0.1.0/airfold.egg-info/SOURCES.txt
--rw-rw-r--   0 kit       (1000) kit       (1000)        1 2023-06-03 15:57:10.000000 airfold-0.1.0/airfold.egg-info/dependency_links.txt
--rw-rw-r--   0 kit       (1000) kit       (1000)      294 2023-06-03 15:57:10.000000 airfold-0.1.0/airfold.egg-info/requires.txt
--rw-rw-r--   0 kit       (1000) kit       (1000)        1 2023-06-03 15:57:10.000000 airfold-0.1.0/airfold.egg-info/top_level.txt
--rw-rw-r--   0 kit       (1000) kit       (1000)     1379 2023-06-03 15:56:59.000000 airfold-0.1.0/pyproject.toml
--rw-rw-r--   0 kit       (1000) kit       (1000)       38 2023-06-03 15:57:10.885913 airfold-0.1.0/setup.cfg
--rw-rw-r--   0 kit       (1000) kit       (1000)       82 2023-06-03 15:13:44.000000 airfold-0.1.0/setup.py
-drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 15:57:10.885913 airfold-0.1.0/test/
--rw-rw-r--   0 kit       (1000) kit       (1000)     4186 2023-06-02 21:47:19.000000 airfold-0.1.0/test/test_config.py
--rw-rw-r--   0 kit       (1000) kit       (1000)     1792 2023-05-03 22:10:34.000000 airfold-0.1.0/test/test_locks.py
--rw-rw-r--   0 kit       (1000) kit       (1000)     5301 2023-06-02 13:31:33.000000 airfold-0.1.0/test/test_parse.py
--rw-rw-r--   0 kit       (1000) kit       (1000)     2983 2023-05-28 00:18:50.000000 airfold-0.1.0/test/test_runtime_ch.py
--rw-rw-r--   0 kit       (1000) kit       (1000)    11504 2023-06-02 13:31:33.000000 airfold-0.1.0/test/test_storage.py
--rw-rw-r--   0 kit       (1000) kit       (1000)     1616 2023-05-03 22:10:34.000000 airfold-0.1.0/test/test_utils.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/
+-rw-rw-r--   0 kit       (1000) kit       (1000)    11357 2023-06-03 15:19:50.000000 airfold-0.2.0/LICENSE
+-rw-rw-r--   0 kit       (1000) kit       (1000)      421 2023-06-03 18:46:17.339433 airfold-0.2.0/PKG-INFO
+-rw-rw-r--   0 kit       (1000) kit       (1000)      103 2023-04-21 00:48:16.000000 airfold-0.2.0/README.md
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/airfold/
+-rw-rw-r--   0 kit       (1000) kit       (1000)        0 2023-04-10 17:51:01.000000 airfold-0.2.0/airfold/__init__.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/airfold/cli/
+-rwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-04-10 17:51:01.000000 airfold-0.2.0/airfold/cli/__init__.py
+-rwxrwxr-x   0 kit       (1000) kit       (1000)      217 2023-06-03 17:47:05.000000 airfold-0.2.0/airfold/cli/cli.py
+-rwxrwxr-x   0 kit       (1000) kit       (1000)     1266 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/cli/pipe.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     2284 2023-06-02 21:46:51.000000 airfold-0.2.0/airfold/config.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)    14838 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/context.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     1580 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/format.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)      258 2023-05-28 00:18:50.000000 airfold-0.2.0/airfold/log.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     5942 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/models.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     4350 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/parse.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/airfold/runtime/
+-rw-rw-r--   0 kit       (1000) kit       (1000)        0 2023-04-21 00:48:16.000000 airfold-0.2.0/airfold/runtime/__init__.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)    10245 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/runtime/ch.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     6261 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/runtime/ch_cluster.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     3297 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/runtime/runtime.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)      287 2023-05-28 00:18:50.000000 airfold-0.2.0/airfold/runtime/type.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/airfold/storage/
+-rw-rw-r--   0 kit       (1000) kit       (1000)        0 2023-04-10 17:51:01.000000 airfold-0.2.0/airfold/storage/__init__.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)    29321 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/storage/ch.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)    18735 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/storage/sqlite.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     8830 2023-06-01 23:45:55.000000 airfold-0.2.0/airfold/storage/storage.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)      313 2023-05-28 00:18:50.000000 airfold-0.2.0/airfold/storage/type.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)       48 2023-05-01 18:12:58.000000 airfold-0.2.0/airfold/type.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     2578 2023-06-02 13:31:33.000000 airfold-0.2.0/airfold/utils.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/airfold.egg-info/
+-rw-rw-r--   0 kit       (1000) kit       (1000)      421 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/PKG-INFO
+-rw-rw-r--   0 kit       (1000) kit       (1000)      830 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/SOURCES.txt
+-rw-rw-r--   0 kit       (1000) kit       (1000)        1 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/dependency_links.txt
+-rw-rw-r--   0 kit       (1000) kit       (1000)       48 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/entry_points.txt
+-rw-rw-r--   0 kit       (1000) kit       (1000)      294 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/requires.txt
+-rw-rw-r--   0 kit       (1000) kit       (1000)        8 2023-06-03 18:46:17.000000 airfold-0.2.0/airfold.egg-info/top_level.txt
+-rw-rw-r--   0 kit       (1000) kit       (1000)     1430 2023-06-03 18:46:09.000000 airfold-0.2.0/pyproject.toml
+-rw-rw-r--   0 kit       (1000) kit       (1000)       38 2023-06-03 18:46:17.339433 airfold-0.2.0/setup.cfg
+-rw-rw-r--   0 kit       (1000) kit       (1000)      108 2023-06-03 17:31:35.000000 airfold-0.2.0/setup.py
+drwxrwxr-x   0 kit       (1000) kit       (1000)        0 2023-06-03 18:46:17.339433 airfold-0.2.0/test/
+-rw-rw-r--   0 kit       (1000) kit       (1000)     4186 2023-06-02 21:47:19.000000 airfold-0.2.0/test/test_config.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     1792 2023-05-03 22:10:34.000000 airfold-0.2.0/test/test_locks.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     5301 2023-06-02 13:31:33.000000 airfold-0.2.0/test/test_parse.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     2983 2023-05-28 00:18:50.000000 airfold-0.2.0/test/test_runtime_ch.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)    11504 2023-06-02 13:31:33.000000 airfold-0.2.0/test/test_storage.py
+-rw-rw-r--   0 kit       (1000) kit       (1000)     1616 2023-05-03 22:10:34.000000 airfold-0.2.0/test/test_utils.py
```

### Comparing `airfold-0.1.0/LICENSE` & `airfold-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/pyproject.toml` & `airfold-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "airfold"
-version = "0.1.0"
+version = "0.2.0"
 description = "Pioneering real-time data"
 authors = [
     {name = "Julian Gilyadov", email = "israelg99@gmail.com"},
     {name = "Constantine Peresypkin", email = "pconstantine@gmail.com"},
 ]
 dependencies = [
     "clickhouse-connect>=0.5.25",
@@ -16,14 +16,17 @@
     "sqlglot>=15.0.0",
     "typer",
 ]
 requires-python = ">=3.10, <4"
 readme = "README.md"
 license = {text = "Apache-2.0"}
 
+[project.scripts]
+airfold = "airfold.cli.cli:app"
+
 [project.optional-dependencies]
 test = [
     "bandit",
     "black",
     "coverage",
     "ipykernel",
     "ipython",
```

### Comparing `airfold-0.1.0/test/test_config.py` & `airfold-0.2.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/test/test_locks.py` & `airfold-0.2.0/test/test_locks.py`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/test/test_parse.py` & `airfold-0.2.0/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/test/test_runtime_ch.py` & `airfold-0.2.0/test/test_runtime_ch.py`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/test/test_storage.py` & `airfold-0.2.0/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `airfold-0.1.0/test/test_utils.py` & `airfold-0.2.0/test/test_utils.py`

 * *Files identical despite different names*

