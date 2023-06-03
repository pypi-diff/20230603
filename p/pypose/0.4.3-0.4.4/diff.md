# Comparing `tmp/pypose-0.4.3.tar.gz` & `tmp/pypose-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.4.3.tar", last modified: Thu May  4 17:45:27 2023, max compression
+gzip compressed data, was "pypose-0.4.4.tar", last modified: Sat Jun  3 19:15:29 2023, max compression
```

## Comparing `pypose-0.4.3.tar` & `pypose-0.4.4.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-04 17:45:11.000000 pypose-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-04 17:45:27.624483 pypose-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-04 17:45:11.000000 pypose-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/function/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/pnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 17:45:11.000000 pypose-0.4.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 17:45:11.000000 pypose-0.4.3/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:45:27.624483 pypose-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-04 17:45:11.000000 pypose-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.754408 pypose-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-03 19:15:13.000000 pypose-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-03 19:15:29.754408 pypose-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-03 19:15:13.000000 pypose-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43346 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-03 19:15:13.000000 pypose-0.4.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 19:15:13.000000 pypose-0.4.4/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:15:29.754408 pypose-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-03 19:15:13.000000 pypose-0.4.4/setup.py
```

### Comparing `pypose-0.4.3/LICENSE` & `pypose-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/PKG-INFO` & `pypose-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.3
+Version: 0.4.4
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
-Author: Chen Wang
-Author-email: chenwang@dr.com
+Author: Chen Wang and PyPose Team
+Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
 Project-URL: Documentation, https://pypose.org/docs
 Project-URL: Source Code, https://github.com/pypose/pypose
 Keywords: robotics,deep learning,pytorch
 Classifier: Environment :: GPU
 Classifier: Environment :: Console
```

### Comparing `pypose-0.4.3/README.md` & `pypose-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/__init__.py` & `pypose-0.4.4/pypose/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/basics/ops.py` & `pypose-0.4.4/pypose/basics/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/function/geometry.py` & `pypose-0.4.4/pypose/function/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,11 @@
-import math
 import torch
 from .. import mat2SE3
 from ..basics import pm
-from .. import lietensor
-from .. import LieTensor
-
-
-def is_lietensor(obj):
-    r'''
-    Check whether an instance or object is a LieTensor or not.
-
-    Args:
-        obj (``obj``): a Python object or instantance.
-
-    Return:
-        ``bool``: ``True`` if obj is a LieTensor object otherwise ``False``.
-    '''
-    return True if isinstance(obj, LieTensor) else False
-
-def is_SE3(obj):
-    r'''
-    Check whether an instance or object is an SE3 Type LieTensor or not.
-
-    Args:
-        obj (``obj``): a Python object or instantance.
-
-    Return:
-        ``bool``: ``True`` if obj is a SE3 Type LieTensor object otherwise ``False``.
-    '''
-    return True if isinstance(obj.ltype, lietensor.lietensor.SE3Type) else False
+from .checking import is_lietensor
 
 
 def cart2homo(coordinates:torch.Tensor):
     r'''
     Converts batched Cartesian coordinates to Homogeneous coordinates
     by adding ones to last dimension.
```

### Comparing `pypose-0.4.3/pypose/function/linalg.py` & `pypose-0.4.4/pypose/function/linalg.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/lietensor/__init__.py` & `pypose-0.4.4/pypose/lietensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/lietensor/basics.py` & `pypose-0.4.4/pypose/lietensor/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,18 @@
         \alpha * \bm{a}_i + \bm{x}_i & \text{if}~\bm{x}_i~\text{is a Lie Algebra} \\
         \mathrm{Exp}(\alpha * \bm{a}_i) \times \bm{x}_i & \text{if}~\bm{x}_i~\text{is a Lie Group}
         \end{cases}
 
     where :math:`\bm{x}` is the ``input`` LieTensor, :math:`\bm{a}` is the ``other`` Tensor to add,
     and :math:`\bm{y}` is the output LieTensor.
 
+    Warning:
+        For better readability, we suggest calling ``a + b`` instead of ``a.add(b)`` or
+        ``pypose.add(a, b)``, which have the same behaviors.
+
     Note:
         A Lie Group normally requires a larger space than its corresponding Lie Algebra, thus
         the elements in the last dimension of the ``other`` Tensor (treated as a Lie Algebra
         in this function) beyond the expected shape of the Lie Algebra are ignored. This is
         because the gradient of a Lie Group is computed as a left perturbation (a Lie Algebra)
         in its tangent space and is stored in the LieGroup's :obj:`LieTensor.grad`, which has
         the same storage space with the LieGroup.
@@ -141,15 +145,15 @@
 
         other (:obj:`Number`, :obj:`Tensor`, or :obj:`LieTensor`): the value for input to be
             multiplied by.
 
     Return:
         :obj:`Tensor`/:obj:`LieTensor`: the product of ``input`` and ``other``.
 
-    .. list-table:: List of :obj:`pypose.mul` cases 
+    .. list-table:: List of :obj:`pypose.mul` cases
         :widths: 25 30 25
         :header-rows: 1
 
         * - input :obj:`LieTensor`
           - other
           - output
         * - Lie Algebra
@@ -158,85 +162,89 @@
         * - Lie Group
           - :obj:`Tensor` :math:`\in \mathbb{R^{*\times3}}`
           - :obj:`Tensor`
         * - Lie Group
           - :obj:`Tensor` :math:`\in \mathbb{R^{*\times4}}`
           - :obj:`Tensor`
         * - Lie Group
-          - :obj:`Lie Group` 
+          - :obj:`Lie Group`
           - :obj:`Lie Group`
 
-    When multiplying a Lie Group by another Lie Group, they must have the 
+    When multiplying a Lie Group by another Lie Group, they must have the
     same Lie type.
 
+    Warning:
+        For better readability, we suggest calling ``a * b`` or ``a @ b`` instead of
+        ``a.mul(b)`` or ``pypose.mul(a, b)``, which have the same behaviors.
+
     Note:
         - When ``other`` is a Tensor, this operator is equivalent to :meth:`Act`.
         - When ``other`` is a number and ``input`` is a Lie Algebra, this operator performs
           simple element-wise multiplication.
         - When ``input`` is a Lie Group, more details are shown below.
-   
+
     * Input :math:`\bm{x}`'s :obj:`ltype` is :obj:`SO3_type`
       (input :math:`\bm{x}` is an instance of :meth:`SO3`):
 
       .. math::
         {\displaystyle \bm{y}_i={\begin{bmatrix}
               q_i^wq_i^{w'} - q_i^xq_i^{x'} -q_i^yq_i^{y'} - q_i^zq_i^{z'}\\
               q_i^wq_i^{x'} + q_i^xq_i^{w'} +q_i^yq_i^{z'} - q_i^zq_i^{y'}\\
               q_i^wq_i^{y'} - q_i^xq_i^{z'} +q_i^yq_i^{w'} + q_i^zq_i^{x'}\\
               q_i^wq_i^{z'} + q_i^xq_i^{y'} -q_i^yq_i^{x'} + q_i^zq_i^{w'}
               \end{bmatrix}
         }^T},
-    
+
       where :math:`\bm{x}_i = [q_i^x, q_i^y, q_i^z, q_i^w]` and
       :math:`\bm{a}_i = [q_i^{x'}, q_i^{y'}, q_i^{z'}, q_i^{w'}]` are the ``input``
       and ``other`` LieTensor, respectively.
-        
+
     Note:
         :math:`\mathbf{y}_i` can be simply derived by taking the complex number multiplication.
 
-        .. math:: 
-            \bm{y}_i = 
-            (q_i^x\mathbf{i} + q_i^y\mathbf{j} + q_i^z\mathbf{k} + q_i^w) \ast 
+        .. math::
+            \bm{y}_i =
+            (q_i^x\mathbf{i} + q_i^y\mathbf{j} + q_i^z\mathbf{k} + q_i^w) \ast
             (q_i^{x'}\mathbf{i} + q_i^{y'}\mathbf{j} + q_i^{z'}\mathbf{k} + q_i^{w'}),
 
         where and :math:`\mathbf{i}` :math:`\mathbf{j}`, and :math:`\mathbf{k}` are the imaginary
         units.
 
         .. math::
             \mathbf{i}^2 = \mathbf{j}^2 = \mathbf{k}^2 = \mathbf{ijk} = -1
 
     * Input :math:`\bm{x}`'s :obj:`ltype` is :obj:`SE3_type`
       (input :math:`\bm{x}` is an instance of :meth:`SE3`):
 
         .. math::
             \bm{y}_i = [\mathbf{q}_i * \mathbf{t}_i' + \mathbf{t}_i,
                         \mathbf{q}_i * \mathbf{q}_i']
-        
+
         where :math:`\bm{x}_i = [\mathbf{t}_i, \mathbf{q}_i]` and
         :math:`\bm{a}_i = [\mathbf{t}_i', \mathbf{q}_i']` are the ``input`` and ``other``
         LieTensor, respectively; :math:`\mathbf{t}_i`, :math:`\mathbf{t}_i'` and
         :math:`\mathbf{q}_i`, :math:`\mathbf{q}_i'` are their translation and :obj:`SO3`
         parts, respectively; the operator :math:`\ast` denotes the obj:`SO3_type`
         multiplication introduced above.
-            
+
     * Input :math:`\bm{x}`'s :obj:`ltype` is :obj:`RxSO3_type`
       (input :math:`\bm{x}` is an instance of :meth:`RxSO3`)
 
         .. math::
             \bm{y}_i = [\mathbf{q}_i * \mathbf{q}_i', s_is_i']
 
         where :math:`s_i` and :math:`s_i'` are the scale parts of the ``input`` and
         ``other`` LieTensor, respectively.
 
     * Input :math:`\bm{x}`'s :obj:`ltype` is :obj:`Sim3_type`
       (input :math:`\bm{x}` is an instance of :meth:`Sim3`):
 
         .. math::
             \bm{y}_i = [\mathbf{q}_i * \mathbf{t}_i' + \mathbf{t}_i,
-                            \mathbf{q}_i * \mathbf{q}_i', s_is_i'] 
+                            \mathbf{q}_i * \mathbf{q}_i', s_is_i']
 
         where :math:`\bm{x}_i = [\mathbf{t}_i, \mathbf{q}_i, s_i]` and
         :math:`\bm{a}_i = [\mathbf{t}_i', \mathbf{q}_i', s_i']` are the ``input`` and
         ``other`` LieTensor, respectively.
 
     Examples:
         * :obj:`Lie Algebra` :math:`*` :obj:`Number` :math:`\mapsto` :obj:`Lie Algebra`
@@ -261,15 +269,15 @@
             >>> x, a
             (SO3Type LieTensor:
             LieTensor([ 0.6047, -0.2129, -0.1781,  0.7465]),
             tensor([-0.1811, -0.2278, -1.9956]))
             >>> x * a
             tensor([ 0.9089,  1.6984, -0.5969])
             >>> a = torch.randn(4)
-            >>> a 
+            >>> a
             tensor([ 1.5236, -1.2757, -0.7140,  0.2467])
             >>> x * a
             tensor([ 1.6588, -0.4687, -1.2196,  0.2467]
 
         * :obj:`SO3_type` :math:`*` :obj:`SO3_type` :math:`\mapsto` :obj:`SO3_type`
 
             >>> a = pp.randn_SO3()
```

### Comparing `pypose-0.4.3/pypose/lietensor/convert.py` & `pypose-0.4.4/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/lietensor/lietensor.py` & `pypose-0.4.4/pypose/lietensor/lietensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def Exp(self, x):
         if not self.on_manifold:
             raise AttributeError("Lie Group has no Exp attribute")
         raise NotImplementedError("Instance has no Exp attribute.")
 
     def Inv(self, x):
         if self.on_manifold:
-            return - x
+            return LieTensor(-x, ltype=x.ltype)
         raise NotImplementedError("Instance has no Inv attribute.")
 
     def Act(self, X, p):
         """ action on a points tensor(*, 3[4]) (homogeneous)"""
         if not self.on_manifold:
             raise AttributeError("Lie Group has no Act attribute")
         raise NotImplementedError("Instance has no Act attribute.")
@@ -179,15 +179,15 @@
     def __init__(self):
         super().__init__(4, 4, 3)
 
     def Log(self, X):
         X = X.tensor() if hasattr(X, 'ltype') else X
         x = SO3_Log.apply(X)
         return LieTensor(x, ltype=so3_type)
-    
+
     def Act(self, X, p):
         assert not self.on_manifold and isinstance(p, torch.Tensor)
         assert p.shape[-1]==3 or p.shape[-1]==4, "Invalid Tensor Dimension"
         X = X.tensor() if hasattr(X, 'ltype') else X
         input, out_shape = broadcast_inputs(X, p)
         if p.shape[-1]==3:
             out = SO3_Act.apply(*input)
@@ -209,20 +209,20 @@
         # Transform on points
         if not self.on_manifold and isinstance(Y, torch.Tensor):
             return self.Act(X, Y)
         # (scalar or tensor) * manifold
         if self.on_manifold:
             return LieTensor(torch.mul(X, Y), ltype=SO3_type)
         raise NotImplementedError('Invalid __mul__ operation')
-    
+
     def Inv(self, X):
         X = X.tensor() if hasattr(X, 'ltype') else X
         out = SO3_Inv.apply(X)
         return LieTensor(out, ltype=SO3_type)
-    
+
     def Adj(self, X, a):
         X = X.tensor() if hasattr(X, 'ltype') else X
         a = a.tensor() if hasattr(a, 'ltype') else a
         input, out_shape = broadcast_inputs(X, a)
         out = SO3_AdjXa.apply(*input)
         dim = -1 if out.nelement() != 0 else X.shape[-1]
         out = out.view(out_shape + (dim,))
@@ -1014,14 +1014,20 @@
 
     def __mul__(self, other):
         r'''
         See :meth:`pypose.mul`
         '''
         return self.ltype.Mul(self, other)
 
+    def mul(self, other):
+        r'''
+        See :meth:`pypose.mul`
+        '''
+        return self.ltype.Mul(self, other)
+
     def __matmul__(self, other):
         r'''
         See :meth:`pypose.matmul`
         '''
         if isinstance(other, LieTensor):
             return self.ltype.Mul(self, other)
         else: # Same with: self.ltype.matrix(self) @ other
@@ -1104,15 +1110,15 @@
 
         # sigularity when pitch angle ~ +/-pi/2
         roll1 = torch.atan2(t0, t1)
         roll2 = torch.zeros_like(t0)
         flag = t2.abs() < 1. - eps
         yaw1 = torch.atan2(t3, t4)
         yaw2 = -2 * pm(t2) * torch.atan2(x, w)
-        
+
         roll = torch.where(flag, roll1, roll2)
         pitch = torch.asin(t2.clamp(-1, 1))
         yaw = torch.where(flag, yaw1, yaw2)
 
         return torch.stack([roll, pitch, yaw], dim=-1)
 
     def identity_(self):
```

### Comparing `pypose-0.4.3/pypose/lietensor/operation.py` & `pypose-0.4.4/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/lietensor/utils.py` & `pypose-0.4.4/pypose/lietensor/utils.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/dynamics.py` & `pypose-0.4.4/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/ekf.py` & `pypose-0.4.4/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/icp.py` & `pypose-0.4.4/pypose/module/icp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/imu_preintegrator.py` & `pypose-0.4.4/pypose/module/imu_preintegrator.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/lqr.py` & `pypose-0.4.4/pypose/module/lqr.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/pf.py` & `pypose-0.4.4/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/pnp.py` & `pypose-0.4.4/pypose/module/pnp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/module/ukf.py` & `pypose-0.4.4/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/optim/corrector.py` & `pypose-0.4.4/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/optim/functional.py` & `pypose-0.4.4/pypose/optim/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import torch
+from .. import hasnan
 from functools import partial
 from torch.autograd.functional import jacobian
 from torch.func import jacrev, jacfwd, functional_call
 
 
 def modjac(model, input=None, create_graph=False, strict=False, vectorize=False, \
                     strategy='reverse-mode', flatten=False):
     r'''
     Compute the model Jacobian with respect to the model parameters.
 
-    For a parametric model :math:`\bm{f}(\bm{\theta}, \bm{x})`, where :math:`\bm{\theta}` is
-    the learnable parameter and :math:`\bm{x}` is the input, it computes the
+    For a parametric model :math:`\bm{f}(\bm{\theta}, \bm{x})`, where :math:`\bm{\theta}`
+    is the learnable parameter and :math:`\bm{x}` is the input, it computes the
     Jacobian of the :math:`i`-th output and :math:`j`-th parameter as
 
     .. math::
         {\displaystyle \mathbf{J}_{i,j} =
         {\begin{bmatrix}
             {\dfrac {\partial \bm{f}_{i,1}}{\partial \bm{\theta}_{j,1}}} &amp;
             \cdots&amp;{\dfrac {\partial \bm{f}_{i,1}}{\partial \bm{\theta}_{j,n}}}\\
@@ -134,27 +135,23 @@
     def func_param(*new_params_values):
         new_params_dict = dict(zip(params_names, new_params_values))
         return functional_call(model, (new_params_dict, buffers), input)
 
     J = jacobian(func_param, params_values, create_graph=create_graph, strict=strict, \
                     vectorize=vectorize, strategy=strategy)
 
+    assert not hasnan(J), 'Jacobian contains Nan! Check your model and input!'
+
     if flatten and isinstance(J, tuple):
         if any(isinstance(j, tuple) for j in J):
             J = torch.cat([torch.cat([j.view(-1, p.numel()) \
                     for j, p in zip(Jr, params_values)], dim=1) for Jr in J])
         else:
-            J = torch.cat([j.view(-1, p.numel()) for j, p in zip(J, params_values)], dim=1)
-
-    if isinstance(J, tuple):
-        assert not torch.any(torch.stack([torch.any(torch.isnan(j)) for j in J])), \
-            'Jacobian contains Nan! Check your model and input!'
-    else:
-        assert not torch.any(torch.isnan(J)), \
-            'Jacobian contains Nan! Check your model and input!'
+            J = torch.cat([j.view(-1, p.numel()) \
+                           for j, p in zip(J, params_values)], dim=1)
 
     return J
 
 
 def modjacrev(model, input, argnums=0, *, has_aux=False):
     params = dict(model.named_parameters())
     func = partial(functional_call, model)
```

### Comparing `pypose-0.4.3/pypose/optim/kernel.py` & `pypose-0.4.4/pypose/optim/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch
+import torch, math
 from torch import nn, Tensor
 
 
 class Huber(nn.Module):
     r"""The robust Huber kernel cost function.
 
     .. math::
@@ -241,26 +241,25 @@
     .. figure:: /_static/img/optim/kernel/tolerant.png
                         :width: 600
     """
     def __init__(self, a: float = 1.0, b: float = -1.0) -> None:
         super().__init__()
         assert a > 0, ValueError("a has to be positive: {}".format(a))
         assert b < 0, ValueError("b has to be negative: {}".format(b))
-        self.a = a
-        self.b = b
+        self.a, self.b = a, b
 
     def forward(self, input: Tensor) -> Tensor:
         '''
         Args:
             input (torch.Tensor): the input tensor (non-negative).
         '''
         assert torch.all(input >= 0), 'input has to be non-negative'
-        part1 = (1 + ((input-self.a) / self.b).exp()).log()
-        part2 = (1 + (-self.a / self.b).exp())
-        return self.b * part1 - self.b * part2
+        result = self.b * (1 + ((input-self.a) / self.b).exp()).log()
+        offset = self.b * math.log((1 + math.exp(-self.a / self.b))) # constant, no grad.
+        return result - offset
 
 
 class Scale(nn.Module):
     r"""The robust Scale kernel cost function.
 
     .. math::
         \bm{y}_i=\delta*\bm{x}_i
@@ -292,8 +291,7 @@
 
     def forward(self, input):
         '''
         Args:
             input (torch.Tensor): the input tensor (non-negative).
         '''
         return self.delta * input
-
```

### Comparing `pypose-0.4.3/pypose/optim/optimizer.py` & `pypose-0.4.4/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/optim/scheduler.py` & `pypose-0.4.4/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/optim/solver.py` & `pypose-0.4.4/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/optim/strategy.py` & `pypose-0.4.4/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/utils/collect_env.py` & `pypose-0.4.4/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose/utils/stepper.py` & `pypose-0.4.4/pypose/utils/stepper.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.3/pypose.egg-info/PKG-INFO` & `pypose-0.4.4/pypose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.3
+Version: 0.4.4
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
-Author: Chen Wang
-Author-email: chenwang@dr.com
+Author: Chen Wang and PyPose Team
+Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
 Project-URL: Documentation, https://pypose.org/docs
 Project-URL: Source Code, https://github.com/pypose/pypose
 Keywords: robotics,deep learning,pytorch
 Classifier: Environment :: GPU
 Classifier: Environment :: Console
```

### Comparing `pypose-0.4.3/pypose.egg-info/SOURCES.txt` & `pypose-0.4.4/pypose.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pypose.egg-info/dependency_links.txt
 pypose.egg-info/requires.txt
 pypose.egg-info/top_level.txt
 pypose.egg-info/zip-safe
 pypose/basics/__init__.py
 pypose/basics/ops.py
 pypose/function/__init__.py
+pypose/function/checking.py
 pypose/function/geometry.py
 pypose/function/linalg.py
 pypose/lietensor/__init__.py
 pypose/lietensor/basics.py
 pypose/lietensor/convert.py
 pypose/lietensor/lietensor.py
 pypose/lietensor/operation.py
```

### Comparing `pypose-0.4.3/setup.py` & `pypose-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
 def load_requirements(filename: str):
     with open(filename) as f:
         return [x.strip() for x in f.readlines() if "-r" != x[0:2]]
 
 
 requirements_extras = {
-    "runtime": load_requirements("requirements/runtime.txt"), 
+    "runtime": load_requirements("requirements/runtime.txt"),
     "docs": load_requirements("requirements/docs.txt"),}
 
 requirements_extras["all"] = list(set(sum(requirements_extras.values(), [])))
 
 if __name__ == '__main__':
     setup(
         name = 'pypose',
-        author = 'Chen Wang',
+        author = 'Chen Wang and PyPose Team',
         version = VERSION,
-        author_email = 'chenwang@dr.com',
+        author_email = 'admin@pypose.org',
         url = 'https://pypose.org',
         download_url = 'https://github.com/pypose/pypose',
         license = 'Apache License 2.0',
         license_files = ('LICENSE',),
         description = 'To connect classic robotics with modern learning methods.',
         long_description=long_description,
         long_description_content_type='text/markdown',
```

