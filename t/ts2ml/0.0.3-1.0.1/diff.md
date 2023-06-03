# Comparing `tmp/ts2ml-0.0.3.tar.gz` & `tmp/ts2ml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts2ml-0.0.3.tar", last modified: Wed May 31 00:08:03 2023, max compression
+gzip compressed data, was "ts2ml-1.0.1.tar", last modified: Sat Jun  3 14:11:18 2023, max compression
```

## Comparing `ts2ml-0.0.3.tar` & `ts2ml-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 00:08:03.887681 ts2ml-0.0.3/
--rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ts2ml-0.0.3/LICENSE
--rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ts2ml-0.0.3/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     9414 2023-05-31 00:08:03.887460 ts2ml-0.0.3/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     8565 2023-05-31 00:02:42.000000 ts2ml-0.0.3/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)      917 2023-05-31 00:07:03.000000 ts2ml-0.0.3/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-31 00:08:03.887742 ts2ml-0.0.3/setup.cfg
--rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ts2ml-0.0.3/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 00:08:03.886124 ts2ml-0.0.3/ts2ml/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-05-31 00:07:03.000000 ts2ml-0.0.3/ts2ml/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      387 2023-05-31 00:07:03.000000 ts2ml-0.0.3/ts2ml/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2207 2023-05-31 00:07:03.000000 ts2ml-0.0.3/ts2ml/core.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 00:08:03.887097 ts2ml-0.0.3/ts2ml.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     9414 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      304 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       53 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:56:32.000000 ts2ml-0.0.3/ts2ml.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       42 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-05-31 00:08:03.000000 ts2ml-0.0.3/ts2ml.egg-info/top_level.txt
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-03 14:11:18.400604 ts2ml-1.0.1/
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ts2ml-1.0.1/LICENSE
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ts2ml-1.0.1/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    26063 2023-06-03 14:11:18.400449 ts2ml-1.0.1/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    25214 2023-06-03 14:05:13.000000 ts2ml-1.0.1/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      930 2023-06-03 14:07:33.000000 ts2ml-1.0.1/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-03 14:11:18.400727 ts2ml-1.0.1/setup.cfg
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ts2ml-1.0.1/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-03 14:11:18.398882 ts2ml-1.0.1/ts2ml/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-06-03 14:05:49.000000 ts2ml-1.0.1/ts2ml/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      873 2023-06-03 14:05:49.000000 ts2ml-1.0.1/ts2ml/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     8685 2023-06-03 14:05:49.000000 ts2ml-1.0.1/ts2ml/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-03 14:11:18.400218 ts2ml-1.0.1/ts2ml.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    26063 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      304 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       53 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:56:32.000000 ts2ml-1.0.1/ts2ml.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       55 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-03 14:11:18.000000 ts2ml-1.0.1/ts2ml.egg-info/top_level.txt
```

### Comparing `ts2ml-0.0.3/LICENSE` & `ts2ml-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ts2ml-0.0.3/settings.ini` & `ts2ml-1.0.1/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ts2ml
 lib_name = ts2ml
-version = 0.0.3
+version = 1.0.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ts2ml
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = joaopcnogueira@gmail.com
 copyright = 2023 onwards, João Nogueira
 description = Tools to Transform a Time Series into Features and Target a.k.a Supervised Learning
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = joaopcnogueira
-requirements = fastcore pandas numpy tqdm
+requirements = fastcore pandas numpy tqdm scikit-learn
 dev_requirements = jupyter
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `ts2ml-0.0.3/setup.py` & `ts2ml-1.0.1/setup.py`

 * *Files identical despite different names*

