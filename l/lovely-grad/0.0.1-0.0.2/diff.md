# Comparing `tmp/lovely-grad-0.0.1.tar.gz` & `tmp/lovely-grad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovely-grad-0.0.1.tar", last modified: Fri Jun  2 10:48:18 2023, max compression
+gzip compressed data, was "lovely-grad-0.0.2.tar", last modified: Sat Jun  3 08:30:46 2023, max compression
```

## Comparing `lovely-grad-0.0.1.tar` & `lovely-grad-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-02 10:48:18.721427 lovely-grad-0.0.1/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    11337 2023-04-27 10:12:58.000000 lovely-grad-0.0.1/LICENSE
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2023-04-27 10:12:58.000000 lovely-grad-0.0.1/MANIFEST.in
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1063 2023-06-02 10:48:18.721427 lovely-grad-0.0.1/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      307 2023-05-31 08:37:42.000000 lovely-grad-0.0.1/README.md
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-02 10:48:18.719427 lovely-grad-0.0.1/lovely_grad/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       67 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3679 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/_modidx.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     7120 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/repr_str.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-02 10:48:18.721427 lovely-grad-0.0.1/lovely_grad/utils/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       21 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/utils/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3755 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/utils/config.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      767 2023-05-31 10:42:00.000000 lovely-grad-0.0.1/lovely_grad/utils/misc.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-02 10:48:18.720427 lovely-grad-0.0.1/lovely_grad.egg-info/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1063 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      452 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/SOURCES.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/dependency_links.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       44 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/entry_points.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-05-31 09:23:20.000000 lovely-grad-0.0.1/lovely_grad.egg-info/not-zip-safe
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       29 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/requires.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       12 2023-06-02 10:48:18.000000 lovely-grad-0.0.1/lovely_grad.egg-info/top_level.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2023-06-02 10:48:14.000000 lovely-grad-0.0.1/settings.ini
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-06-02 10:48:18.721427 lovely-grad-0.0.1/setup.cfg
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2596 2023-05-31 09:25:11.000000 lovely-grad-0.0.1/setup.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-03 08:30:46.594885 lovely-grad-0.0.2/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    11337 2023-04-27 10:12:58.000000 lovely-grad-0.0.2/LICENSE
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2023-04-27 10:12:58.000000 lovely-grad-0.0.2/MANIFEST.in
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    13086 2023-06-03 08:30:46.594885 lovely-grad-0.0.2/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    12329 2023-06-03 07:57:22.000000 lovely-grad-0.0.2/README.md
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-03 08:30:46.592886 lovely-grad-0.0.2/lovely_grad/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      162 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     7404 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/_modidx.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1544 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/patch.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3271 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/repr_chans.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2905 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/repr_plt.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3184 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/repr_rgb.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     6938 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/repr_str.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-03 08:30:46.593886 lovely-grad-0.0.2/lovely_grad/utils/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       21 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/utils/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3753 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/utils/config.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      767 2023-06-03 08:26:45.000000 lovely-grad-0.0.2/lovely_grad/utils/misc.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-06-03 08:30:46.593886 lovely-grad-0.0.2/lovely_grad.egg-info/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    13086 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      547 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/SOURCES.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/dependency_links.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       44 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/entry_points.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-06-03 08:30:15.000000 lovely-grad-0.0.2/lovely_grad.egg-info/not-zip-safe
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       29 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/requires.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       12 2023-06-03 08:30:46.000000 lovely-grad-0.0.2/lovely_grad.egg-info/top_level.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2023-06-03 08:22:57.000000 lovely-grad-0.0.2/settings.ini
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-06-03 08:30:46.594885 lovely-grad-0.0.2/setup.cfg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2596 2023-05-31 09:25:11.000000 lovely-grad-0.0.2/setup.py
```

### Comparing `lovely-grad-0.0.1/LICENSE` & `lovely-grad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lovely-grad-0.0.1/lovely_grad/repr_str.py` & `lovely-grad-0.0.2/lovely_grad/repr_str.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,14 @@
 
 # %% ../nbs/00_repr_str.ipynb 9
 def plain_repr(x: Tensor):
     "Pick the right function to get a plain repr"
     # assert isinstance(x, np.ndarray), f"expected np.ndarray but got {type(x)}" # Could be a sub-class.
     return x._plain_repr() if hasattr(x, "_plain_repr") else repr(x)
 
-# def plain_str(x: torch.Tensor):
-#     "Pick the right function to get a plain str."
-#     # assert isinstance(x, np.ndarray), f"expected np.ndarray but got {type(x)}"
-#     return x._plain_str() if hasattr(type(x), "_plain_str") else str(x)
 
 # %% ../nbs/00_repr_str.ipynb 10
 def is_nasty(x: Tensor):
     """Return true of any `x` values are inf or nan"""
     if x.shape == (): return False # min/max don't like zero-lenght arrays
     
     x_min = x.min().numpy().squeeze()
@@ -72,15 +68,15 @@
         meanstd = f"μ={pretty_str(x_mean)} σ={pretty_str(x_std)}" if x.numel() >= 2 else None
 
         return sparse_join([minmax, meanstd])
 
 # %% ../nbs/00_repr_str.ipynb 13
 def to_str(x: Tensor,  # Input
             verbose:        bool    =False,
-            auto_realize:    O[bool] =None,
+            auto_realize:   O[bool] =None,
             depth:          int     =0,
             lvl:            int     =0,
             color:          O[bool] =None
         ) -> str:
 
     # if plain:
     #     return plain_repr(x)
@@ -101,27 +97,29 @@
 
     grad = "grad" if x.requires_grad else None          # grad
     if x.grad is not None: grad = grad + ansi_color("+", "green", color)
 
 
     numel = None
     if x.shape and max(x.shape) != x.numel():
-        numel = f"n={x.ndim}"
+        numel = f"n={x.numel()}"
         # if get_config().show_mem_above <= x.nbytes:
         #     numel = sparse_join([numel, f"({bytes_to_human(x.nbytes)})"])
     # elif get_config().show_mem_above <= x.nbytes:
         # numel = bytes_to_human(x.nbytes)
 
+    res  = ""
+    if verbose: # Put this on top before the tensor is possibly realized.
+        res += plain_repr(x) + "\n"
 
     just_realized = None
     if auto_realize and not x.lazydata.realized:
         just_realized = ansi_color("Realized "+ str(x.lazydata.op.op).split(".")[-1], "grey", color)
         x.realize()
 
-    res  = ""
     if x.lazydata.realized:
         # `lovely-numpy` is used to calculate stats when doing so on GPU would require
         # memory allocation (no-float tensors, tensors with bad numbers),
         #
         # Temporarily set the numpy config to match our config for consistency.
         with lnp_config(precision=conf.precision,
                         threshold_min=conf.threshold_min,
@@ -130,23 +128,21 @@
 
             if is_nasty(x) or not x.is_floating_point():
                 common = np_to_str_common(x.numpy(), color=color)
             else:
                 common = tensor_to_str_common(x, color=color)
 
             vals = pretty_str(x.numpy()) if 0 < x.numel() <= 10 else None
-            res = sparse_join([type_str, dtype, numel, common, grad, dev,  vals, just_realized])
+            res += sparse_join([type_str, dtype, numel, common, grad, dev, just_realized, vals])
     else:
         op = "Lazy " + str(x.lazydata.op.op).split(".")[-1]
-        res = sparse_join([type_str, dtype, numel, grad, dev, op])
+        res += sparse_join([type_str, dtype, numel, grad, dev, op])
     # else:
     #     res = plain_repr(x)
 
-    if verbose:
-        res += "\n" + plain_repr(x)
 
     if depth and x.ndim > 1:
         with config(show_mem_above=np.inf):
             deep_width = min((x.shape[0]), conf.deeper_width) # Print at most this many lines
             deep_lines = [ " "*conf.indent*(lvl+1) + to_str(x[i,:].realize(), depth=depth-1, lvl=lvl+1)
                                 for i in range(deep_width)]
```

### Comparing `lovely-grad-0.0.1/lovely_grad/utils/config.py` & `lovely-grad-0.0.2/lovely_grad/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/03a_utils.config.ipynb.
 
 # %% auto 0
 __all__ = ['set_config', 'get_config', 'config']
 
-# %% ../../nbs/03a_utils.config.ipynb 6
+# %% ../../nbs/03a_utils.config.ipynb 5
 from copy import copy
 from types import SimpleNamespace
 from typing import Optional as O, Union as U, Callable, TypeVar
 from contextlib import contextmanager
 from lovely_numpy import config as np_config
 
-# %% ../../nbs/03a_utils.config.ipynb 7
+# %% ../../nbs/03a_utils.config.ipynb 6
 class Config(SimpleNamespace):
     "Config"
     def __init__(self,
             precision     = 3,    # Digits after `.`
             threshold_max = 3,    # .abs() larger than 1e3 -> Sci mode
             threshold_min = -4,   # .abs() smaller that 1e-4 -> Sci mode
             sci_mode      = None, # Sci mode (2.3e4). None=auto
-            auto_realize   = True, # Realize Tensors before printing
+            auto_realize   = True,# Realize Tensors before printing
             show_mem_above= 1024, # Show memory footprint above this size
             indent        = 2,    # Indent for .deeper()
             color         = True, # ANSI colors in text
             deeper_width  = 9,    # For .deeper, width per level
             plt_seed      = 42,   # Sampling seed for `plot`
             fig_close     = True, # Close matplotlib Figure
             fig_show      = False,# Call `plt.show()` for `.plt`, `.chans` and `.rgb`
 
     ):
         super().__init__(**{k:v for k,v in locals().items() if k not in ["self", "__class__"]})
 
 _defaults = Config()
 _config = copy(_defaults)
 
-# %% ../../nbs/03a_utils.config.ipynb 10
+# %% ../../nbs/03a_utils.config.ipynb 9
 # Allows passing None as an argument to reset the 
 class _Default():
     def __repr__(self):
         return "Ignore"
 D = _Default()
 Default = TypeVar("Default")
 
-# %% ../../nbs/03a_utils.config.ipynb 11
+# %% ../../nbs/03a_utils.config.ipynb 10
 def set_config( precision:      U[Default,int,None]  =D,
                 threshold_min:  U[Default,int,None]  =D,
                 threshold_max:  U[Default,int,None]  =D,
                 sci_mode:       U[Default,bool,None] =D,
                 auto_realize:    U[Default,bool,None] =D,
                 show_mem_above: U[Default,int,None]  =D,
                 indent:         U[Default,bool,None] =D,
@@ -61,20 +61,20 @@
     for k,v in args.items():
         if v != D:
             if v is None:
                 setattr(_config, k, getattr(_defaults, k))
             else:
                 setattr(_config, k, v)
 
-# %% ../../nbs/03a_utils.config.ipynb 12
+# %% ../../nbs/03a_utils.config.ipynb 11
 def get_config():
     "Get a copy of config variables"
     return copy(_config)
 
-# %% ../../nbs/03a_utils.config.ipynb 13
+# %% ../../nbs/03a_utils.config.ipynb 12
 @contextmanager
 def config( precision:      U[Default,int,None]  =D,
             threshold_min:  U[Default,int,None]  =D,
             threshold_max:  U[Default,int,None]  =D,
             sci_mode:       U[Default,bool,None] =D,
             auto_realize:    U[Default,bool,None] =D,
             show_mem_above: U[Default,int,None]  =D,
```

### Comparing `lovely-grad-0.0.1/lovely_grad/utils/misc.py` & `lovely-grad-0.0.2/lovely_grad/utils/misc.py`

 * *Files identical despite different names*

### Comparing `lovely-grad-0.0.1/settings.ini` & `lovely-grad-0.0.2/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lovely-grad
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = mit
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lovely_grad
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 
 ### Docs ###
 branch = master
-custom_sidebar = False
+custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
 author = Alexey
 author_email = alexey.zaytsev@gmail.com
 copyright = 2023 onwards, %(author)s
-description = 😘 Lovely Grad - tiny tensors need love too
+description = 🫀 Lovely Grad - tiny tensors need some love
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = xl0
 
 ### Optional ###
 requirements = lovely-numpy tinygrad
```

### Comparing `lovely-grad-0.0.1/setup.py` & `lovely-grad-0.0.2/setup.py`

 * *Files identical despite different names*

