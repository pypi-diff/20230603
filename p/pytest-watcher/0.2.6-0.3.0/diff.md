# Comparing `tmp/pytest-watcher-0.2.6.tar.gz` & `tmp/pytest-watcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-watcher-0.2.6.tar", max compression
+gzip compressed data, was "pytest-watcher-0.3.0.tar", max compression
```

## Comparing `pytest-watcher-0.2.6.tar` & `pytest-watcher-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-10-19 14:45:40.729543 pytest-watcher-0.2.6/LICENSE
--rw-r--r--   0        0        0     1376 2022-12-11 17:00:09.959069 pytest-watcher-0.2.6/README.md
--rw-r--r--   0        0        0     1561 2022-12-11 17:01:00.299554 pytest-watcher-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       67 2022-12-11 16:52:21.734228 pytest-watcher-0.2.6/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2022-10-19 14:45:40.730627 pytest-watcher-0.2.6/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     3330 2022-12-11 16:54:47.747033 pytest-watcher-0.2.6/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     2283 2022-12-11 17:06:17.560494 pytest-watcher-0.2.6/setup.py
--rw-r--r--   0        0        0     2422 2022-12-11 17:06:17.560647 pytest-watcher-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-19 14:45:40.729543 pytest-watcher-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3318 2023-06-02 23:06:45.106513 pytest-watcher-0.3.0/README.md
+-rw-r--r--   0        0        0     1563 2023-06-02 23:17:38.128731 pytest-watcher-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-06-02 23:15:11.891180 pytest-watcher-0.3.0/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2022-10-19 14:45:40.730627 pytest-watcher-0.3.0/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     4655 2023-06-02 23:07:08.404121 pytest-watcher-0.3.0/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     4300 2023-06-02 23:21:11.185308 pytest-watcher-0.3.0/setup.py
+-rw-r--r--   0        0        0     4366 2023-06-02 23:21:11.185496 pytest-watcher-0.3.0/PKG-INFO
```

### Comparing `pytest-watcher-0.2.6/LICENSE` & `pytest-watcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-watcher-0.2.6/pyproject.toml` & `pytest-watcher-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pytest-watcher"
-version = "0.2.6"
-description = "Continiously runs pytest on changes in *.py files"
+version = "0.3.0"
+description = "Automatically rerun your tests on file modifications"
 authors = ["Olzhas Arystanov <o.arystanov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/olzhasar/pytest-watcher"
 repository = "https://github.com/olzhasar/pytest-watcher"
 keywords = ["pytest", "watch", "watcher"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
```

