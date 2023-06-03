# Comparing `tmp/TPDNE-utils-0.0.7.tar.gz` & `tmp/TPDNE-utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPDNE-utils-0.0.7.tar", last modified: Sat Jun  3 17:00:42 2023, max compression
+gzip compressed data, was "TPDNE-utils-0.0.8.tar", last modified: Sat Jun  3 17:16:17 2023, max compression
```

## Comparing `TPDNE-utils-0.0.7.tar` & `TPDNE-utils-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/TPDNE_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/nginx.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/tpdne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:16:17.991914 TPDNE-utils-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:16:17.991914 TPDNE-utils-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:16:17.991914 TPDNE-utils-0.0.8/TPDNE_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/TPDNE_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/TPDNE_utils/nginx.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/TPDNE_utils/tpdne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:16:17.991914 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:16:17.000000 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-03 17:16:17.000000 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:16:17.000000 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-03 17:16:17.000000 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 17:16:17.000000 TPDNE-utils-0.0.8/TPDNE_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:16:17.991914 TPDNE-utils-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-03 17:16:06.000000 TPDNE-utils-0.0.8/setup.py
```

### Comparing `TPDNE-utils-0.0.7/LICENSE` & `TPDNE-utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TPDNE-utils-0.0.7/README.md` & `TPDNE-utils-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 ```
 
 ## Todo
 
 - [x] take care of an nginx template
 - [x] auto-handle various types of tensor outputs. auto-detect channel dimension and move it to last
-- [ ] handle un-normalization of image tensors into 0-256 uint8 by autodetecting range
+- [x] handle un-normalization of image tensors into 0-255 uint8 by autodetecting range
 - [ ] handle ssl in nginx
 
 ## Citations
 
 ```bibtex
 @inproceedings{Karras2020ada,
     title     = {Training Generative Adversarial Networks with Limited Data},
```

### Comparing `TPDNE-utils-0.0.7/TPDNE_utils/tpdne.py` & `TPDNE-utils-0.0.8/TPDNE_utils/tpdne.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,27 @@
         t = rearrange(t, 'c h w -> h w c')
 
     assert t.shape[-1] <= 3, 'image tensor must be returned in the shape (height, width, channels), where channels is either 3 or 1'
 
     if t.shape[-1] == 1:
         t = repeat(t, 'h w 1 -> h w c', c = 3)
 
-    return t
+    # handle scale
+
+    if t.dtype == np.float:
+        has_negatives = np.any(t < 0)
+
+        if has_negatives:
+            t = t * 127.5 + 128
+        else:
+            t = t * 255
+
+        t = t.astype(np.uint8)
+
+    return t.clip(0, 255)
 
 # main function
 
 @beartype
 def sample_image_and_save_repeatedly(
     fn: Callable[..., np.ndarray],         # function that returns a ndarray of shape (3, <width>, <height>)
     output_path: str = './out/random',     # path to the output image, without extension (will be saved as webp)
```

### Comparing `TPDNE-utils-0.0.7/setup.py` & `TPDNE-utils-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'TPDNE-utils',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'TPDNE',
   include_package_data = True,
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/TPDNE',
```

