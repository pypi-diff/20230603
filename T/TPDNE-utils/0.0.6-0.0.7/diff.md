# Comparing `tmp/TPDNE-utils-0.0.6.tar.gz` & `tmp/TPDNE-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPDNE-utils-0.0.6.tar", last modified: Sat Jun  3 16:47:15 2023, max compression
+gzip compressed data, was "TPDNE-utils-0.0.7.tar", last modified: Sat Jun  3 17:00:42 2023, max compression
```

## Comparing `TPDNE-utils-0.0.6.tar` & `TPDNE-utils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:47:15.772574 TPDNE-utils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 16:47:15.772574 TPDNE-utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:47:15.772574 TPDNE-utils-0.0.6/TPDNE_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/TPDNE_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/TPDNE_utils/nginx.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/TPDNE_utils/tpdne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:47:15.772574 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 16:47:15.000000 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-03 16:47:15.000000 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:47:15.000000 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 16:47:15.000000 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 16:47:15.000000 TPDNE-utils-0.0.6/TPDNE_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:47:15.772574 TPDNE-utils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-03 16:47:03.000000 TPDNE-utils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/TPDNE_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/nginx.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/TPDNE_utils/tpdne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 17:00:42.000000 TPDNE-utils-0.0.7/TPDNE_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:00:42.376479 TPDNE-utils-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-03 17:00:31.000000 TPDNE-utils-0.0.7/setup.py
```

### Comparing `TPDNE-utils-0.0.6/LICENSE` & `TPDNE-utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TPDNE-utils-0.0.6/README.md` & `TPDNE-utils-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 # optionally put behind cloudflare
 
 ```
 
 ## Todo
 
 - [x] take care of an nginx template
+- [x] auto-handle various types of tensor outputs. auto-detect channel dimension and move it to last
+- [ ] handle un-normalization of image tensors into 0-256 uint8 by autodetecting range
 - [ ] handle ssl in nginx
-- [ ] auto-handle various types of tensor outputs. auto-detect channel dimension and move it to last
 
 ## Citations
 
 ```bibtex
 @inproceedings{Karras2020ada,
     title     = {Training Generative Adversarial Networks with Limited Data},
     author    = {Tero Karras and Miika Aittala and Janne Hellsten and Samuli Laine and Jaakko Lehtinen and Timo Aila},
```

### Comparing `TPDNE-utils-0.0.6/TPDNE_utils/tpdne.py` & `TPDNE-utils-0.0.7/TPDNE_utils/tpdne.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,51 @@
 from pathlib import Path
 from functools import wraps
 from PIL import Image
 
 from beartype import beartype
 from beartype.typing import Callable, Optional
 
+from einops import rearrange, repeat
+
 # templating
 
 from jinja2 import Environment, FileSystemLoader
 
 current_dir = Path(__file__).parents[0]
 environment = Environment(loader = FileSystemLoader(str(current_dir)))
 nginx_template = environment.get_template('nginx.conf.tmpl')
 
 # helper functions
 
 def exists(val):
     return val is not None
 
+# handle everything that was confusing to me when first encountering image tensors
+
+def auto_handle_image_tensor(t):
+    if t.ndim == 4:
+        # assume batch is first dimension and take first sample
+        t = t[0]
+
+    if t.ndim == 2:
+        # very rare case, but assume greyscale
+        t = rearrange(t, 'h w -> h w 1')
+
+    if t.shape[0] <= 3:
+        # channel first
+        t = rearrange(t, 'c h w -> h w c')
+
+    assert t.shape[-1] <= 3, 'image tensor must be returned in the shape (height, width, channels), where channels is either 3 or 1'
+
+    if t.shape[-1] == 1:
+        t = repeat(t, 'h w 1 -> h w c', c = 3)
+
+    return t
+
 # main function
 
 @beartype
 def sample_image_and_save_repeatedly(
     fn: Callable[..., np.ndarray],         # function that returns a ndarray of shape (3, <width>, <height>)
     output_path: str = './out/random',     # path to the output image, without extension (will be saved as webp)
     *,
@@ -88,14 +112,16 @@
 
     # invoke `fn` in a while loop
 
     while True:
         start = time()
         image_tensor = fn()
 
+        image_tensor = auto_handle_image_tensor(image_tensor)
+
         tmp_image_index = (tmp_image_index + 1) % num_rotated_tmp_images
         tmp_path = str(tmp_dir / f'{tmp_image_index}.{image_format}')
 
         pil_image = Image.fromarray(image_tensor, 'RGB')
 
         if exists(resize_image_to):
             pil_image = pil_image.resize((resize_image_to, resize_image_to))
```

### Comparing `TPDNE-utils-0.0.6/setup.py` & `TPDNE-utils-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'TPDNE-utils',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'TPDNE',
   include_package_data = True,
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/TPDNE',
   keywords = [],
   install_requires = [
     'beartype',
+    'einops>=0.6',
     'jinja2',
     'numpy',
     'pillow'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
```

