# Comparing `tmp/nemo_library-1.0.2.tar.gz` & `tmp/nemo_library-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.2.tar", last modified: Sat Jun  3 18:54:41 2023, max compression
+gzip compressed data, was "nemo_library-1.0.3.tar", last modified: Sat Jun  3 19:00:22 2023, max compression
```

## Comparing `nemo_library-1.0.2.tar` & `nemo_library-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 18:54:41.527514 nemo_library-1.0.2/
--rw-r--r--   0 schuglocal   (503) staff       (20)      256 2023-06-03 18:54:41.527246 nemo_library-1.0.2/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     1793 2023-06-03 06:16:17.000000 nemo_library-1.0.2/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     1875 2023-06-03 18:52:03.000000 nemo_library-1.0.2/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 18:54:41.524850 nemo_library-1.0.2/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.2/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    10969 2023-06-03 18:44:16.000000 nemo_library-1.0.2/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.2/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 18:54:41.526826 nemo_library-1.0.2/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)      256 2023-06-03 18:54:41.000000 nemo_library-1.0.2/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 18:54:41.000000 nemo_library-1.0.2/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 18:54:41.000000 nemo_library-1.0.2/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 18:54:41.000000 nemo_library-1.0.2/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 18:54:41.000000 nemo_library-1.0.2/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 18:54:41.527573 nemo_library-1.0.2/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      434 2023-06-03 18:52:49.000000 nemo_library-1.0.2/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:00:22.646924 nemo_library-1.0.3/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2169 2023-06-03 19:00:22.646742 nemo_library-1.0.3/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1793 2023-06-03 06:16:17.000000 nemo_library-1.0.3/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1875 2023-06-03 18:52:03.000000 nemo_library-1.0.3/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:00:22.644185 nemo_library-1.0.3/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.3/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    10969 2023-06-03 18:44:16.000000 nemo_library-1.0.3/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.3/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:00:22.646304 nemo_library-1.0.3/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2169 2023-06-03 19:00:22.000000 nemo_library-1.0.3/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:00:22.000000 nemo_library-1.0.3/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:00:22.000000 nemo_library-1.0.3/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:00:22.000000 nemo_library-1.0.3/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:00:22.000000 nemo_library-1.0.3/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:00:22.646972 nemo_library-1.0.3/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 18:59:58.000000 nemo_library-1.0.3/setup.py
```

### Comparing `nemo_library-1.0.2/README.md` & `nemo_library-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.2/README.rst` & `nemo_library-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.2/nemo_library/nemo_library.py` & `nemo_library-1.0.3/nemo_library/nemo_library.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.2/nemo_library/symbols.py` & `nemo_library-1.0.3/nemo_library/symbols.py`

 * *Files identical despite different names*

