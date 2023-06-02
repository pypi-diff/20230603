# Comparing `tmp/mesmerize-core-0.2.0.tar.gz` & `tmp/mesmerize-core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesmerize-core-0.2.0.tar", last modified: Wed Mar  1 10:30:48 2023, max compression
+gzip compressed data, was "mesmerize-core-0.2.2.tar", last modified: Fri Jun  2 22:11:09 2023, max compression
```

## Comparing `mesmerize-core-0.2.0.tar` & `mesmerize-core-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.295172 mesmerize-core-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-03-01 10:30:48.295172 mesmerize-core-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.291172 mesmerize-core-0.2.0/mesmerize_core/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.291172 mesmerize-core-0.2.0/mesmerize_core/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/algorithms/cnmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/algorithms/cnmfe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/algorithms/mcorr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.291172 mesmerize-core-0.2.0/mesmerize_core/arrays/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/arrays/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/arrays/_cnmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/arrays/_tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/arrays/_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/batch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.291172 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/_batch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/cnmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/mcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/movie_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/mesmerize_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.291172 mesmerize-core-0.2.0/mesmerize_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-03-01 10:30:48.000000 mesmerize-core-0.2.0/mesmerize_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-01 10:30:48.000000 mesmerize-core-0.2.0/mesmerize_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 10:30:48.000000 mesmerize-core-0.2.0/mesmerize_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-01 10:30:48.000000 mesmerize-core-0.2.0/mesmerize_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 10:30:48.000000 mesmerize-core-0.2.0/mesmerize_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 10:30:48.295172 mesmerize-core-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:48.295172 mesmerize-core-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/tests/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    49954 2023-03-01 10:30:36.000000 mesmerize-core-0.2.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.951843 mesmerize-core-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-02 22:11:09.951843 mesmerize-core-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.947843 mesmerize-core-0.2.2/mesmerize_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.947843 mesmerize-core-0.2.2/mesmerize_core/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/algorithms/cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/algorithms/cnmfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/algorithms/mcorr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.947843 mesmerize-core-0.2.2/mesmerize_core/arrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/arrays/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/arrays/_cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/arrays/_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/arrays/_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/batch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.947843 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/_batch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25508 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20213 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/mcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/movie_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/mesmerize_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.947843 mesmerize-core-0.2.2/mesmerize_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-02 22:11:09.000000 mesmerize-core-0.2.2/mesmerize_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-02 22:11:09.000000 mesmerize-core-0.2.2/mesmerize_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:11:09.000000 mesmerize-core-0.2.2/mesmerize_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 22:11:09.000000 mesmerize-core-0.2.2/mesmerize_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 22:11:09.000000 mesmerize-core-0.2.2/mesmerize_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:11:09.951843 mesmerize-core-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:11:09.951843 mesmerize-core-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/tests/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46638 2023-06-02 22:10:58.000000 mesmerize-core-0.2.2/tests/test_core.py
```

### Comparing `mesmerize-core-0.2.0/LICENSE` & `mesmerize-core-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/PKG-INFO` & `mesmerize-core-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesmerize-core
-Version: 0.2.0
+Version: 0.2.2
 Summary: High level pandas-based API for batch analysis of Calcium Imaging data using CaImAn
 Home-page: https://github.com/nel-lab/mesmerize-core
 Author: Kushal Kolar, Caitlin Lewis, Arjun Putcha
 Author-email: 
 License: Apache-Software-License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mesmerize-core-0.2.0/README.md` & `mesmerize-core-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/__init__.py` & `mesmerize-core-0.2.2/mesmerize_core/__init__.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/algorithms/cnmf.py` & `mesmerize-core-0.2.2/mesmerize_core/algorithms/cnmf.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/algorithms/cnmfe.py` & `mesmerize-core-0.2.2/mesmerize_core/algorithms/cnmfe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import click
 import numpy as np
 import caiman as cm
 from caiman.source_extraction.cnmf import cnmf as cnmf
 from caiman.source_extraction.cnmf.params import CNMFParams
 import psutil
-import pandas as pd
 import traceback
 from pathlib import Path
 from shutil import move as move_file
 import os
 import time
 from datetime import datetime
 
@@ -52,85 +51,70 @@
 
     try:
         fname_new = cm.save_memmap(
             [input_movie_path], base_name=f"{uuid}_cnmf-memmap_", order="C", dview=dview
         )
 
         print("making memmap")
-        gSig = params["main"]["gSig"][0]
-
         Yr, dims, T = cm.load_memmap(fname_new)
         images = np.reshape(Yr.T, [T] + list(dims), order="F")
 
+        # TODO: if projections already exist from mcorr we don't
+        #  need to waste compute time re-computing them here
         proj_paths = dict()
         for proj_type in ["mean", "std", "max"]:
             p_img = getattr(np, f"nan{proj_type}")(images, axis=0)
             proj_paths[proj_type] = output_dir.joinpath(
                 f"{uuid}_{proj_type}_projection.npy"
             )
             np.save(str(proj_paths[proj_type]), p_img)
 
-        downsample_ratio = params["downsample_ratio"]
-        # in fname new load in memmap order C
-
-        cn_filter, pnr = cm.summary_images.correlation_pnr(
-            images[::downsample_ratio], swap_dim=False, gSig=gSig
-        )
-
-        pnr_output_path = output_dir.joinpath(f"{uuid}_pn.npy").resolve()
-        cn_output_path = output_dir.joinpath(f"{uuid}_cn.npy").resolve()
-
-        np.save(str(pnr_output_path), pnr, allow_pickle=False)
-        np.save(str(cn_output_path), cn_filter, allow_pickle=False)
-
         d = dict()  # for output
 
-        if params["do_cnmfe"]:
-            cnmfe_params_dict = {
-                "method_init": "corr_pnr",
-                "n_processes": n_processes,
-                "only_init": True,  # for 1p
-                "center_psf": True,  # for 1p
-                "normalize_init": False,  # for 1p
-            }
-            tot = {**cnmfe_params_dict, **params["main"]}
-            cnmfe_params_dict = CNMFParams(params_dict=tot)
-            cnm = cnmf.CNMF(
-                n_processes=n_processes, dview=dview, params=cnmfe_params_dict
+        # force the CNMFE params
+        cnmfe_params_dict = {
+            "method_init": "corr_pnr",
+            "n_processes": n_processes,
+            "only_init": True,  # for 1p
+            "center_psf": True,  # for 1p
+            "normalize_init": False,  # for 1p
+        }
+
+        params_dict = {**cnmfe_params_dict, **params["main"]}
+
+        cnmfe_params_dict = CNMFParams(params_dict=params_dict)
+        cnm = cnmf.CNMF(
+            n_processes=n_processes, dview=dview, params=cnmfe_params_dict
+        )
+        print("Performing CNMFE")
+        cnm = cnm.fit(images)
+        print("evaluating components")
+        cnm.estimates.evaluate_components(images, cnm.params, dview=dview)
+
+        cnmf_hdf5_path = output_dir.joinpath(f"{uuid}.hdf5").resolve()
+        cnm.save(str(cnmf_hdf5_path))
+
+        # save output paths to outputs dict
+        d["cnmf-hdf5-path"] = cnmf_hdf5_path.relative_to(output_dir.parent)
+
+        for proj_type in proj_paths.keys():
+            d[f"{proj_type}-projection-path"] = proj_paths[proj_type].relative_to(
+                output_dir.parent
             )
-            print("Performing CNMFE")
-            cnm = cnm.fit(images)
-            print("evaluating components")
-            cnm.estimates.evaluate_components(images, cnm.params, dview=dview)
-
-            cnmf_hdf5_path = output_dir.joinpath(f"{uuid}.hdf5").resolve()
-            cnm.save(str(cnmf_hdf5_path))
-
-            # save output paths to outputs dict
-            d["cnmf-hdf5-path"] = cnmf_hdf5_path.relative_to(output_dir.parent)
-
-            for proj_type in proj_paths.keys():
-                d[f"{proj_type}-projection-path"] = proj_paths[proj_type].relative_to(
-                    output_dir.parent
-                )
 
         cnmf_memmap_path = output_dir.joinpath(Path(fname_new).name)
         if IS_WINDOWS:
             Yr._mmap.close()  # accessing private attr but windows is annoying otherwise
         move_file(fname_new, cnmf_memmap_path)
 
         cnmfe_memmap_path = cnmf_memmap_path.relative_to(output_dir.parent)
-        cn_output_path = cn_output_path.relative_to(output_dir.parent)
-        pnr_output_path = pnr_output_path.relative_to(output_dir.parent)
 
         d.update(
             {
                 "cnmf-memmap-path": cnmfe_memmap_path,
-                "corr-img-path": cn_output_path,
-                "pnr-image-path": pnr_output_path,
                 "success": True,
                 "traceback": None,
             }
         )
 
     except:
         d = {"success": False, "traceback": traceback.format_exc()}
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/algorithms/mcorr.py` & `mesmerize-core-0.2.2/mesmerize_core/algorithms/mcorr.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/arrays/_base.py` & `mesmerize-core-0.2.2/mesmerize_core/arrays/_base.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/arrays/_cnmf.py` & `mesmerize-core-0.2.2/mesmerize_core/arrays/_cnmf.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/arrays/_tiff.py` & `mesmerize-core-0.2.2/mesmerize_core/arrays/_tiff.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,42 @@
 import numpy as np
 import tifffile
 
 from ._base import LazyArray
 
 
 class LazyTiff(LazyArray):
-    def __init__(self, path: Union[Path, str]):
+    def __init__(self, path: Union[Path, str], shape: Tuple[int] = None):
+        """
+        Lazy reader for tiff files. WIP, works for some tiff files.
+        Try ``tifffile.memmap`` first before trying ``LazyTiff``
+
+        Parameters
+        ----------
+        path: str or Path
+            path to tiff file
+
+        shape: Tuple[int]
+            manually set shape
+        """
+
         self._tif = tifffile.TiffFile(path)
         tiffseries = self._tif.series[0].levels[0]
 
-        # TODO: someone who's better with tiff can help on this
-        if len(self._tif.pages) == 1:
-            n_frames = len(self._tif.series)
+        if shape is None:
+            # TODO: someone who's better with tiff can help on this
+            if len(self._tif.pages) == 1:
+                n_frames = len(self._tif.series)
+            else:
+                n_frames = len(self._tif.pages)
+
+            self._shape = (n_frames, *tiffseries.shape)
         else:
-            n_frames = len(self._tif.pages)
+            self._shape = shape
 
-        self._shape = (n_frames, *tiffseries.shape)
         self._dtype = tiffseries.dtype.name
 
     @property
     def dtype(self) -> str:
         return self._dtype
 
     @property
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/arrays/_video.py` & `mesmerize-core-0.2.2/mesmerize_core/arrays/_video.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             as_grayscale: bool = False,
             rgb_weights: Tuple[float, float, float] = (0.299, 0.587, 0.114)
     ):
         """
         LazyVideo reader, basically just a wrapper for ``decord.VideoReader``.
         Should support opening anything that decord can open.
 
-        **Requires ``decord`` to be installed**
+        **Requires ``decord`` to be installed**: https://github.com/dmlc/decord
 
         Parameters
         ----------
         path: Path or str
             path to video file
 
         min_max: Tuple[int, int], optional
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/batch_utils.py` & `mesmerize-core-0.2.2/mesmerize_core/batch_utils.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/_utils.py` & `mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         def wrapper(self, *args, **kwargs):
             if self._series["outputs"] is None:
                 raise BatchItemNotRunError("Item has not been run")
 
             if algo is not None:
                 if algo not in self._series["algo"]:
                     raise WrongAlgorithmExtensionError(
-                        f"<{algo} extension called for a <{self._series}> item"
+                        f"<{algo}> extension called for a <{self._series.algo}> item"
                     )
 
             if not self._series["outputs"]["success"]:
                 tb = self._series["outputs"]["traceback"]
                 raise BatchItemUnsuccessfulError(f"Batch item was unsuccessful, traceback from subprocess:\n{tb}")
             return func(self, *args, **kwargs)
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/cache.py` & `mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/cache.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/cnmf.py` & `mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/cnmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,59 +289,14 @@
         Returns
         -------
         Tuple[List[np.ndarray], List[np.ndarray]]
             | (List[coordinates array], List[centers of masses array])
             | each array of coordinates is 2D, [xs, ys]
             | each center of mass is [x, y]
 
-        Examples
-        --------
-
-        This example loads the input movie and contours, and plots them with fastplotlib
-
-        .. code-block:: python
-
-            from mesmerize_core import load_batch
-
-            # needs fastplotlib and must be run in a notebook
-            from fastplotlib import Plot
-            from ipywidgets import IntSlider, VBox
-
-            df = load_batch("/path/to/batch_dataframe_file.pickle")
-
-            # assuming the 0th index is a cnmf item
-            movie = df.iloc[0].caiman.get_input_movie()
-            contours, coms = df.iloc[0].cnmf.get_contours()
-
-            # the following requires fastplotlib and must be run in a new notebook cell
-            slider = IntSlider(value=0, min=0, max=movie.shape[0] - 1, step=1)
-            plot = Plot()
-
-            image_graphic = plot.image(movie[0].T, cmap="gnuplot2")
-            # note the movie frame is transposed, this is sometimes requires to get the contours to align
-
-            for coor in contours:
-                # line data has to be 3D
-                zs = np.ones(coor.shape[0])  # this will place it above the image graphic
-                c3d = [coor[:, 0], coor[:, 1], zs]
-                coors_3d = np.dstack(c3d)[0]
-
-                # make all the lines red, [R, G, B, A] array
-                colors = np.vstack([[1., 0., 0., 0.7]] * coors_3d.shape[0])
-                plot.line(data=coors_3d, colors=colors)
-
-            previous_slider_value = 0
-            def update_frame():  # runs on each rendering cycle
-                if slider.value == previous_slider_value:
-                    return
-                image_graphic.update_data(data=movie[slider.value].T)
-
-            plot.add_animations([update_frame])
-
-            VBox([plot.show(), slider])
         """
 
         cnmf_obj = self.get_output()
         contours = self._get_spatial_contours(cnmf_obj, component_indices, swap_dim)
 
         coordinates = list()
         coms = list()
@@ -391,22 +346,26 @@
         --------
 
         Plot the temporal components as a heatmap
 
         .. code-block:: python
 
             from mesmerize_core import load_batch
-            from seaborn import heatmap
+            from fastplotlib import Plot
 
             df = load_batch("/path/to/batch_dataframe_file.pickle")
 
             # assumes 0th index is a cnmf batch item
             temporal = df.iloc[0].cnmf.get_temporal()
 
-            heatmap(temporal)
+            plot = Plot()
+
+            plot.add_line_collection(temporal)
+
+            plot.show()
         """
 
         cnmf_obj = self.get_output()
 
         C = cnmf_obj.estimates.C[component_indices]
         f = cnmf_obj.estimates.f
 
@@ -419,15 +378,15 @@
     @_component_indices_parser
     @cnmf_cache.use_cache
     def get_rcm(
             self,
             component_indices: Union[np.ndarray, str] = None,
             temporal_components: np.ndarray = None,
             return_copy=False
-    ) -> LazyArray:
+    ) -> LazyArrayRCM:
         """
         Return the reconstructed movie with no background, i.e. ``A ⊗ C``, as a ``LazyArray``.
         This is an array that performs lazy computation of the reconstructed movie only upon indexing.
 
         Parameters
         ----------
         component_indices: optional, Union[np.ndarray, str]
@@ -446,15 +405,15 @@
         return_copy: bool, default ``False``
             | if ``True`` returns a copy of the cached value in memory.
             | if ``False`` returns the same object as the cached value in memory
             | ``False`` is used by default when returning ``LazyArrays`` for technical reasons
 
         Returns
         -------
-        LazyArray
+        LazyArrayRCM
             shape is [n_frames, x_dims, y_dims]
 
         Examples
         --------
 
         This example uses fastplotlib to display the reconstructed movie from a CNMF item that has already been run.
 
@@ -503,21 +462,21 @@
         spatial = cnmf_obj.estimates.A[:, component_indices]
         temporal = temporal_components[component_indices, :]
 
         return LazyArrayRCM(spatial=spatial, temporal=temporal, frame_dims=dims)
 
     @validate("cnmf")
     @cnmf_cache.use_cache
-    def get_rcb(self,) -> LazyArray:
+    def get_rcb(self,) -> LazyArrayRCB:
         """
         Return the reconstructed background, ``(b ⊗ f)``
 
         Returns
         -------
-        LazyArray
+        LazyArrayRCB
             shape is [n_frames, x_dims, y_dims]
 
         Examples
         --------
 
         This example uses fastplotlib to display the reconstructed movie from a CNMF item that has already been run.
 
@@ -555,21 +514,21 @@
         spatial = cnmf_obj.estimates.b
         temporal = cnmf_obj.estimates.f
 
         return LazyArrayRCB(spatial=spatial, temporal=temporal, frame_dims=dims)
 
     @validate("cnmf")
     @cnmf_cache.use_cache
-    def get_residuals(self) -> np.ndarray:
+    def get_residuals(self) -> LazyArrayResiduals:
         """
         Return residuals, ``Y - (A ⊗ C) - (b ⊗ f)``
 
         Returns
         -------
-        LazyArray
+        LazyArrayResiduals
             shape is [n_frames, x_dims, y_dims]
 
         Examples
         --------
 
         This example uses fastplotlib to display the reconstructed movie from a CNMF item that has already been run.
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/common.py` & `mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from subprocess import Popen
 from typing import *
 from uuid import UUID, uuid4
 from shutil import rmtree
 from itertools import chain
 from collections import Counter
 from datetime import datetime
+import time
 
 import numpy as np
 import pandas as pd
 
 from ._batch_exceptions import BatchItemNotRunError, BatchItemUnsuccessfulError, DependencyError
 from ._utils import validate, _index_parser
 from ..batch_utils import (
@@ -145,15 +146,15 @@
                 f"is set to <{max_index_diff}>. This is to prevent overwriting "
                 f"the full DataFrame with a sub-DataFrame. If you still wish "
                 f"to save the smaller DataFrame, use `caiman.save_to_disk()` "
                 f"with `max_index_diff` set to the highest allowable difference "
                 f"in row number."
             )
 
-        bak = path.with_suffix(path.suffix + f"bak.{time()}")
+        bak = path.with_suffix(path.suffix + f"bak.{time.time()}")
 
         shutil.copyfile(path, bak)
         try:
             self._df.to_pickle(path)
             os.remove(bak)
         except:
             shutil.copyfile(bak, path)
@@ -199,16 +200,26 @@
 
             | if ``False``, this batch item is removed even if its output is the input to another batch item
 
         Returns
         -------
 
         """
+        if self._df.iloc[index]["outputs"] is not None:
+            if self._df.iloc[index]["outputs"]["success"] is True:
+                # if success, don't skip checks
+                skip_checks = False
+            else:
+                # if failed item, skip checks, allow removal since it cannot have children
+                skip_checks = True
+        else:
+            # if not run, skip checks, it cannot have children
+            skip_checks = True
 
-        if self._df.iloc[index]["algo"] == "mcorr":
+        if self._df.iloc[index]["algo"] == "mcorr" and not skip_checks:
             if safe_removal:
                 children = self.get_children(index)
                 if len(children) > 0:
                     raise DependencyError(
                         f"This batch item's output is used as the input for batch items with the following UUIDs:\n"
                         f"{children}\n"
                         f"If you still want to force removal of this batch item use `safe_removal=False`"
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core/caiman_extensions/mcorr.py` & `mesmerize-core-0.2.2/mesmerize_core/caiman_extensions/mcorr.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/movie_readers.py` & `mesmerize-core-0.2.2/mesmerize_core/movie_readers.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core/utils.py` & `mesmerize-core-0.2.2/mesmerize_core/utils.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/mesmerize_core.egg-info/PKG-INFO` & `mesmerize-core-0.2.2/mesmerize_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesmerize-core
-Version: 0.2.0
+Version: 0.2.2
 Summary: High level pandas-based API for batch analysis of Calcium Imaging data using CaImAn
 Home-page: https://github.com/nel-lab/mesmerize-core
 Author: Kushal Kolar, Caitlin Lewis, Arjun Putcha
 Author-email: 
 License: Apache-Software-License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mesmerize-core-0.2.0/mesmerize_core.egg-info/SOURCES.txt` & `mesmerize-core-0.2.2/mesmerize_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/setup.py` & `mesmerize-core-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.2.0/tests/params.py` & `mesmerize-core-0.2.2/tests/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,14 @@
             "min_cnn_thr": 0.8,
             "cnn_lowest": 0.1,
             "decay_time": 1,
         },
         "refit": True,
     },
     "cnmfe_full": {
-        "do_cnmfe": True,
-        "keep_memmap": True,
         "main": {
             "gSig": (10, 10),
             "gSiz": (41, 41),
             "p": 1,
             "min_corr": 0.89,
             "min_pnr": 4,
             "rf": 50,
@@ -51,18 +49,9 @@
             "ring_size_factor": 1.5,
             "merge_thresh": 0.7,
             "low_rank_background": False,
             "method_deconvolution": "oasis",
             "update_background_components": True,
             "del_duplicates": True,
         },
-        "downsample_ratio": 1,
-    },
-    "cnmfe_partial": {
-        "do_cnmfe": False,
-        "keep_memmap": True,
-        "main": {
-            "gSig": (10, 10),
-        },
-        "downsample_ratio": 1,
-    },
+    }
 }
```

### Comparing `mesmerize-core-0.2.0/tests/test_core.py` & `mesmerize-core-0.2.2/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -676,93 +676,16 @@
         params=test_params["mcorr"],
     )
     process = df.iloc[-1].caiman.run()
     # process.wait()
 
     df = load_batch(batch_path)
 
-    # Test if pnr and cn alone work
-    algo = "cnmfe"
-    param_name = "cnmfe_partial"
-    print(f"testing cnmfe - partial")
-    input_movie_path = df.iloc[0].mcorr.get_output_path()
-    print(input_movie_path)
-    df.caiman.add_item(
-        algo=algo,
-        item_name=f"test-{algo}",
-        input_movie_path=input_movie_path,
-        params=test_params[param_name],
-    )
-
-    assert df.iloc[-1]["algo"] == algo
-    assert df.iloc[-1]["item_name"] == f"test-{algo}"
-    assert df.iloc[-1]["params"] == test_params[param_name]
-    assert df.iloc[-1]["outputs"] is None
-    try:
-        UUID(df.iloc[-1]["uuid"])
-    except:
-        pytest.fail("Something wrong with setting UUID for batch items")
-
-    assert (
-            batch_dir.joinpath(df.iloc[-1]["input_movie_path"])
-            == batch_dir.joinpath(df.iloc[0].mcorr.get_output_path())
-            == df.paths.resolve(df.iloc[-1]["input_movie_path"])
-    )
-
-    process = df.iloc[-1].caiman.run()
-    # process.wait()
-
-    df = load_batch(batch_path)
-
-    with pd.option_context("display.max_rows", None, "display.max_columns", None):
-        print(df)
-
-    pprint(df.iloc[-1]["outputs"], width=-1)
-    print(df.iloc[-1]["outputs"]["traceback"])
-
-    # Confirm output path is as expected
-    assert df.iloc[-1]["outputs"]["success"] is True
-    assert df.iloc[-1]["outputs"]["traceback"] is None
-
-    assert (
-            input_movie_path
-            == df.iloc[-1].caiman.get_input_movie_path()
-            == df.paths.resolve(df.iloc[-1]["input_movie_path"])
-    )
-
-    assert batch_dir.joinpath(
-        str(df.iloc[-1]["uuid"]),
-        f'{df.iloc[-1]["uuid"]}_cnmf-memmap_d1_128_d2_128_d3_1_order_C_frames_1000.mmap',
-    ) == df.paths.resolve(df.iloc[-1]["outputs"]["cnmf-memmap-path"])
-
-    assert batch_dir.joinpath(
-        str(df.iloc[-1]["uuid"]), f'{df.iloc[-1]["uuid"]}_pn.npy'
-    ) == df.paths.resolve(df.iloc[-1]["outputs"]["pnr-image-path"])
-
-    assert batch_dir.joinpath(
-        str(df.iloc[-1]["uuid"]), f'{df.iloc[-1]["uuid"]}_cn.npy'
-    ) == df.paths.resolve(df.iloc[-1]["outputs"]["corr-img-path"])
-
-    # extension tests - partial
-
-    # test to check caiman get_corr_image()
-    corr_img = df.iloc[-1].caiman.get_corr_image()
-    corr_img_actual = numpy.load(
-        ground_truths_dir.joinpath("cnmfe_partial", "cnmfe_partial_correlation_img.npy")
-    )
-    numpy.testing.assert_allclose(corr_img, corr_img_actual, rtol=1e-1, atol=1e-10)
-
-    # test to check caiman get_pnr_image()
-    pnr_image = df.iloc[-1].caiman.get_pnr_image()
-    pnr_image_actual = numpy.load(
-        ground_truths_dir.joinpath("cnmfe_partial", "cnmfe_partial_pnr_img.npy")
-    )
-    numpy.testing.assert_allclose(pnr_image, pnr_image_actual, rtol=1e2, atol=1e-10)
-
     # Test if running full cnmfe works
+    print("testing cnmfe")
     algo = "cnmfe"
     param_name = "cnmfe_full"
     input_movie_path = df.iloc[0].mcorr.get_output_path()
     print(input_movie_path)
 
     df.caiman.add_item(
         algo=algo,
@@ -844,28 +767,14 @@
             batch_dir.joinpath(df.iloc[-1]["outputs"]["max-projection-path"])
             == df.paths.resolve(df.iloc[-1]["outputs"]["max-projection-path"])
             == batch_dir.joinpath(
         str(df.iloc[-1]["uuid"]), f'{df.iloc[-1]["uuid"]}_max_projection.npy'
     )
     )
 
-    # test to check correlation image output path
-    assert (
-            batch_dir.joinpath(df.iloc[-1]["outputs"]["corr-img-path"])
-            == df.paths.resolve(df.iloc[-1]["outputs"]["corr-img-path"])
-            == batch_dir.joinpath(str(df.iloc[-1]["uuid"]), f'{df.iloc[-1]["uuid"]}_cn.npy')
-    )
-
-    # test to check pnr image output path
-    assert (
-            batch_dir.joinpath(df.iloc[-1]["outputs"]["pnr-image-path"])
-            == df.paths.resolve(df.iloc[-1]["outputs"]["pnr-image-path"])
-            == batch_dir.joinpath(str(df.iloc[-1]["uuid"]), f'{df.iloc[-1]["uuid"]}_pn.npy')
-    )
-
     # extension tests - full
 
     # test to check cnmf get_cnmf_memmap()
     cnmfe_mmap_output = df.iloc[-1].cnmf.get_cnmf_memmap()
     cnmfe_mmap_output_actual = numpy.load(
         ground_truths_dir.joinpath("cnmfe_full", "cnmfe_full_output_mmap.npy")
     )
```

