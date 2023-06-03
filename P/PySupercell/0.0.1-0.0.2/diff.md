# Comparing `tmp/PySupercell-0.0.1.tar.gz` & `tmp/PySupercell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.1.tar", last modified: Sat Jun  3 11:39:40 2023, max compression
+gzip compressed data, was "PySupercell-0.0.2.tar", last modified: Sat Jun  3 11:43:53 2023, max compression
```

## Comparing `PySupercell-0.0.1.tar` & `PySupercell-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.180456 PySupercell-0.0.1/
--rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.1/LICENSE.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.1/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:39:40.180456 PySupercell-0.0.1/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.176456 PySupercell-0.0.1/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:39:39.000000 PySupercell-0.0.1/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      547 2023-06-03 11:39:40.000000 PySupercell-0.0.1/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 11:39:39.000000 PySupercell-0.0.1/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 11:39:39.000000 PySupercell-0.0.1/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 11:39:39.000000 PySupercell-0.0.1/PySupercell.egg-info/top_level.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 10:06:26.000000 PySupercell-0.0.1/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.176456 PySupercell-0.0.1/bin/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9840 2023-06-03 10:18:05.000000 PySupercell-0.0.1/bin/pysc.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.176456 PySupercell-0.0.1/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       53 2023-06-03 11:23:33.000000 PySupercell-0.0.1/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.176456 PySupercell-0.0.1/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.1/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.1/examples/example1/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-06-03 11:35:47.000000 PySupercell-0.0.1/examples/example1/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.176456 PySupercell-0.0.1/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 11:15:37.000000 PySupercell-0.0.1/examples/example3/POSCAR_redefine
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 11:37:17.000000 PySupercell-0.0.1/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.180456 PySupercell-0.0.1/pysupercell/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8621 2023-06-03 10:12:44.000000 PySupercell-0.0.1/pysupercell/QE_ibrav_lib.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 11:39:27.000000 PySupercell-0.0.1/pysupercell/__init__.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4587 2023-06-03 10:16:44.000000 PySupercell-0.0.1/pysupercell/arguments.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44205 2023-06-03 11:30:54.000000 PySupercell-0.0.1/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 11:39:40.180456 PySupercell-0.0.1/setup.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3609 2023-06-03 11:11:06.000000 PySupercell-0.0.1/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:39:40.180456 PySupercell-0.0.1/tests_basic/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.1/tests_basic/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.1/tests_basic/test_1.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/
+-rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.2/LICENSE.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.2/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:43:53.111161 PySupercell-0.0.2/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      547 2023-06-03 11:43:53.000000 PySupercell-0.0.2/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/top_level.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 10:06:26.000000 PySupercell-0.0.2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/bin/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9840 2023-06-03 10:18:05.000000 PySupercell-0.0.2/bin/pysc.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       53 2023-06-03 11:23:33.000000 PySupercell-0.0.2/examples/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.2/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.2/examples/example1/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-06-03 11:35:47.000000 PySupercell-0.0.2/examples/example1/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 11:15:37.000000 PySupercell-0.0.2/examples/example3/POSCAR_redefine
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 11:37:17.000000 PySupercell-0.0.2/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/pysupercell/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8621 2023-06-03 10:12:44.000000 PySupercell-0.0.2/pysupercell/QE_ibrav_lib.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 11:39:40.000000 PySupercell-0.0.2/pysupercell/__init__.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4587 2023-06-03 10:16:44.000000 PySupercell-0.0.2/pysupercell/arguments.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44205 2023-06-03 11:30:54.000000 PySupercell-0.0.2/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 11:43:53.111161 PySupercell-0.0.2/setup.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3609 2023-06-03 11:43:48.000000 PySupercell-0.0.2/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/tests_basic/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.2/tests_basic/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.2/tests_basic/test_1.py
```

### Comparing `PySupercell-0.0.1/LICENSE.txt` & `PySupercell-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.2/PySupercell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/README.md` & `PySupercell-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/bin/pysc.py` & `PySupercell-0.0.2/bin/pysc.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/examples/example1/POSCAR_redefine` & `PySupercell-0.0.2/examples/example1/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/examples/example3/POSCAR_redefine` & `PySupercell-0.0.2/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.2/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.2/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/pysupercell/arguments.py` & `PySupercell-0.0.2/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/pysupercell/pysupercell.py` & `PySupercell-0.0.2/pysupercell/pysupercell.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.1/setup.py` & `PySupercell-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
 
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.1',
+version='0.0.2',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure'],
 py_modules=core_modules,
 license="MIT License",
```

