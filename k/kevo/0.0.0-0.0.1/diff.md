# Comparing `tmp/kevo-0.0.0.tar.gz` & `tmp/kevo-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kevo-0.0.0.tar", last modified: Sat Jun  3 11:11:25 2023, max compression
+gzip compressed data, was "kevo-0.0.1.tar", last modified: Sat Jun  3 11:30:17 2023, max compression
```

## Comparing `kevo-0.0.0.tar` & `kevo-0.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      216 2023-06-03 11:11:25.638918 kevo-0.0.0/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1783 2023-05-26 19:42:25.000000 kevo-0.0.0/README.md
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/kevo/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      112 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/__init__.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/kevo/common/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      146 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/common/__init__.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     2422 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/common/bloomfilter.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1880 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/common/fencepointers.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     6198 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/common/hashindex.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1652 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/common/ringbuffer.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/kevo/engines/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      202 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/__init__.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     8539 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/appendlog.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)    10484 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/hybridlog.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     2692 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/kvstore.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)    12586 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/lsmtree.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     2767 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/engines/memonly.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     7334 2023-05-26 18:35:29.000000 kevo-0.0.0/kevo/remote.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/kevo.egg-info/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      216 2023-06-03 11:11:25.000000 kevo-0.0.0/kevo.egg-info/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      664 2023-06-03 11:11:25.000000 kevo-0.0.0/kevo.egg-info/SOURCES.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-03 11:11:25.000000 kevo-0.0.0/kevo.egg-info/dependency_links.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       78 2023-06-03 11:11:25.000000 kevo-0.0.0/kevo.egg-info/requires.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        5 2023-06-03 11:11:25.000000 kevo-0.0.0/kevo.egg-info/top_level.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-03 11:11:25.638918 kevo-0.0.0/setup.cfg
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      528 2023-06-03 11:10:29.000000 kevo-0.0.0/setup.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:11:25.638918 kevo-0.0.0/tests/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     4564 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_appendlog.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1079 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_bloomfilter.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      537 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_fencepointers.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      881 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_hashindex.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     4657 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_hybridlog.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     4287 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_lsmtree.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1914 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_memonly.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     2034 2023-05-26 18:35:55.000000 kevo-0.0.0/tests/test_ringbuffer.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.731072 kevo-0.0.1/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      216 2023-06-03 11:30:17.727072 kevo-0.0.1/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1783 2023-05-26 19:42:25.000000 kevo-0.0.1/README.md
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.727072 kevo-0.0.1/kevo/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      112 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/__init__.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.727072 kevo-0.0.1/kevo/common/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      146 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/common/__init__.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     2422 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/common/bloomfilter.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1880 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/common/fencepointers.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     6198 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/common/hashindex.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1652 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/common/ringbuffer.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.727072 kevo-0.0.1/kevo/engines/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      202 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/__init__.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     8539 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/appendlog.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)    10484 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/hybridlog.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     2692 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/kvstore.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)    12586 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/lsmtree.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     2767 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/engines/memonly.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     7334 2023-05-26 18:35:29.000000 kevo-0.0.1/kevo/remote.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.727072 kevo-0.0.1/kevo.egg-info/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      216 2023-06-03 11:30:17.000000 kevo-0.0.1/kevo.egg-info/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      664 2023-06-03 11:30:17.000000 kevo-0.0.1/kevo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-03 11:30:17.000000 kevo-0.0.1/kevo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       78 2023-06-03 11:30:17.000000 kevo-0.0.1/kevo.egg-info/requires.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        5 2023-06-03 11:30:17.000000 kevo-0.0.1/kevo.egg-info/top_level.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-03 11:30:17.731072 kevo-0.0.1/setup.cfg
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      528 2023-06-03 11:21:03.000000 kevo-0.0.1/setup.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-03 11:30:17.727072 kevo-0.0.1/tests/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     4564 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_appendlog.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1079 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_bloomfilter.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      537 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_fencepointers.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      881 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_hashindex.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     4657 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_hybridlog.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     4287 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_lsmtree.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1914 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_memonly.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     2034 2023-05-26 18:35:55.000000 kevo-0.0.1/tests/test_ringbuffer.py
```

### Comparing `kevo-0.0.0/README.md` & `kevo-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/common/bloomfilter.py` & `kevo-0.0.1/kevo/common/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/common/fencepointers.py` & `kevo-0.0.1/kevo/common/fencepointers.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/common/hashindex.py` & `kevo-0.0.1/kevo/common/hashindex.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/common/ringbuffer.py` & `kevo-0.0.1/kevo/common/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/engines/appendlog.py` & `kevo-0.0.1/kevo/engines/appendlog.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/engines/hybridlog.py` & `kevo-0.0.1/kevo/engines/hybridlog.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/engines/kvstore.py` & `kevo-0.0.1/kevo/engines/kvstore.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/engines/lsmtree.py` & `kevo-0.0.1/kevo/engines/lsmtree.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/engines/memonly.py` & `kevo-0.0.1/kevo/engines/memonly.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo/remote.py` & `kevo-0.0.1/kevo/remote.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/kevo.egg-info/SOURCES.txt` & `kevo-0.0.1/kevo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/setup.py` & `kevo-0.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 setuptools.setup(
     name="kevo",
-    version="0.0.0",
+    version="0.0.1",
     author="Nikos Gavalas",
     description="Key-value store with 3 backend engines",
     classifiers=classifiers,
     keywords=["key-value", "store"],
     packages=setuptools.find_packages(),
     install_requires=[
         'sortedcontainers >= 2.4.0, < 3',
```

### Comparing `kevo-0.0.0/tests/test_appendlog.py` & `kevo-0.0.1/tests/test_appendlog.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_bloomfilter.py` & `kevo-0.0.1/tests/test_bloomfilter.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_fencepointers.py` & `kevo-0.0.1/tests/test_fencepointers.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_hashindex.py` & `kevo-0.0.1/tests/test_hashindex.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_hybridlog.py` & `kevo-0.0.1/tests/test_hybridlog.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_lsmtree.py` & `kevo-0.0.1/tests/test_lsmtree.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_memonly.py` & `kevo-0.0.1/tests/test_memonly.py`

 * *Files identical despite different names*

### Comparing `kevo-0.0.0/tests/test_ringbuffer.py` & `kevo-0.0.1/tests/test_ringbuffer.py`

 * *Files identical despite different names*

