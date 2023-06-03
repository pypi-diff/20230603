# Comparing `tmp/rhubarb_py-1.8.4.tar.gz` & `tmp/rhubarb_py-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhubarb_py-1.8.4.tar", max compression
+gzip compressed data, was "rhubarb_py-1.8.5.tar", max compression
```

## Comparing `rhubarb_py-1.8.4.tar` & `rhubarb_py-1.8.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-06-02 10:39:01.423738 rhubarb_py-1.8.4/LICENSE
--rw-r--r--   0        0        0     7567 2023-06-02 10:39:01.423738 rhubarb_py-1.8.4/README.md
--rw-r--r--   0        0        0     3669 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      570 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/__init__.py
--rw-r--r--   0        0        0    16069 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/_core.py
--rw-r--r--   0        0        0     3131 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/base.py
--rw-r--r--   0        0        0       40 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/exceptions.py
--rw-r--r--   0        0        0     7555 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/kafka.py
--rw-r--r--   0        0        0     2483 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/memory.py
--rw-r--r--   0        0        0     3094 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/postgres.py
--rw-r--r--   0        0        0     4360 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/rabbitmq.py
--rw-r--r--   0        0        0    13779 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/backends/redis.py
--rw-r--r--   0        0        0      210 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/event.py
--rw-r--r--   0        0        0        0 2023-06-02 10:39:01.427738 rhubarb_py-1.8.4/rhubarb/py.typed
--rw-r--r--   0        0        0     8816 1970-01-01 00:00:00.000000 rhubarb_py-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-03 15:42:33.536909 rhubarb_py-1.8.5/LICENSE
+-rw-r--r--   0        0        0     7567 2023-06-03 15:42:33.536909 rhubarb_py-1.8.5/README.md
+-rw-r--r--   0        0        0     3665 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0      570 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/__init__.py
+-rw-r--r--   0        0        0    16069 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/_core.py
+-rw-r--r--   0        0        0     3131 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/base.py
+-rw-r--r--   0        0        0       40 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/exceptions.py
+-rw-r--r--   0        0        0     7555 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/kafka.py
+-rw-r--r--   0        0        0     2483 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/memory.py
+-rw-r--r--   0        0        0     3094 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/postgres.py
+-rw-r--r--   0        0        0     4360 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/rabbitmq.py
+-rw-r--r--   0        0        0    13779 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/backends/redis.py
+-rw-r--r--   0        0        0      210 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/event.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:42:33.540909 rhubarb_py-1.8.5/rhubarb/py.typed
+-rw-r--r--   0        0        0     8816 1970-01-01 00:00:00.000000 rhubarb_py-1.8.5/PKG-INFO
```

### Comparing `rhubarb_py-1.8.4/LICENSE` & `rhubarb_py-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/README.md` & `rhubarb_py-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/pyproject.toml` & `rhubarb_py-1.8.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rhubarb-py"
 packages = [{ include = "rhubarb" }]
-version = "1.8.4"
+version = "1.8.5"
 description = "Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API"
 readme = "README.md"
 authors = ["mopeyjellyfish <dev@davidhall.tech>"]
 license = "MIT"
 repository = "https://github.com/mopeyjellyfish/rhubarb"
 homepage = "https://github.com/mopeyjellyfish/rhubarb"
 
@@ -44,24 +44,24 @@
 rabbitmq = ["aio-pika"]
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
 black = { version = "^23.3", allow-prereleases = true }
 darglint = "^1.8.0"
 isort = { extras = ["colors"], version = "^5.9.3" }
-mypy = "^0.971"
-mypy-extensions = "^0.4.3"
-pre-commit = "^2.20.0"
+mypy = "^1.0"
+mypy-extensions = "^1.0.0"
+pre-commit = "^3.3.2"
 pydocstyle = "^6.1.1"
 pylint = "^2.14.5"
 pytest = "^7.3.1"
-pyupgrade = "^2.37.3"
+pyupgrade = "^3.4.0"
 safety = "^2.1.1"
 pytest-asyncio = "^0.21.0"
-Sphinx = "^5.1.1"
+Sphinx = "^6.2.1"
 sphinx-rtd-theme = "^1.0.0"
 pytest-cov = "^4.1.0"
 asyncpg = ">=0.24,<0.28"
 aiokafka = ">=0.7.2,<0.9.0"
 aio-pika = ">=6.8,<10.0"
 hypothesis = "^6.53.0"
```

### Comparing `rhubarb_py-1.8.4/rhubarb/__init__.py` & `rhubarb_py-1.8.5/rhubarb/__init__.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/_core.py` & `rhubarb_py-1.8.5/rhubarb/_core.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/base.py` & `rhubarb_py-1.8.5/rhubarb/backends/base.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/kafka.py` & `rhubarb_py-1.8.5/rhubarb/backends/kafka.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/memory.py` & `rhubarb_py-1.8.5/rhubarb/backends/memory.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/postgres.py` & `rhubarb_py-1.8.5/rhubarb/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/rabbitmq.py` & `rhubarb_py-1.8.5/rhubarb/backends/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/rhubarb/backends/redis.py` & `rhubarb_py-1.8.5/rhubarb/backends/redis.py`

 * *Files identical despite different names*

### Comparing `rhubarb_py-1.8.4/PKG-INFO` & `rhubarb_py-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhubarb-py
-Version: 1.8.4
+Version: 1.8.5
 Summary: Rhubarb is a library that simplifies realtime streaming for a number of backends into a single API
 Home-page: https://github.com/mopeyjellyfish/rhubarb
 License: MIT
 Author: mopeyjellyfish
 Author-email: dev@davidhall.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

