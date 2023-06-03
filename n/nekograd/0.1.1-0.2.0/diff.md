# Comparing `tmp/nekograd-0.1.1.tar.gz` & `tmp/nekograd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nekograd-0.1.1.tar", last modified: Sun Apr 23 12:27:41 2023, max compression
+gzip compressed data, was "nekograd-0.2.0.tar", last modified: Sat Jun  3 08:19:33 2023, max compression
```

## Comparing `nekograd-0.1.1.tar` & `nekograd-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 12:27:31.000000 nekograd-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 12:27:31.000000 nekograd-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-23 12:27:41.879311 nekograd-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-23 12:27:31.000000 nekograd-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/data/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/data/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/model/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-23 12:27:31.000000 nekograd-0.1.1/nekograd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:27:41.879311 nekograd-0.1.1/nekograd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:27:41.000000 nekograd-0.1.1/nekograd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 12:27:31.000000 nekograd-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:27:41.879311 nekograd-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-23 12:27:31.000000 nekograd-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 08:19:24.000000 nekograd-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 08:19:24.000000 nekograd-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-03 08:19:33.955092 nekograd-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-03 08:19:24.000000 nekograd-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.951092 nekograd-0.2.0/nekograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/nekograd/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/data/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/nekograd/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/metrics/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/metrics/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/nekograd/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/nekograd/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/torch/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-03 08:19:24.000000 nekograd-0.2.0/nekograd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:19:33.955092 nekograd-0.2.0/nekograd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-03 08:19:33.000000 nekograd-0.2.0/nekograd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-03 08:19:33.000000 nekograd-0.2.0/nekograd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:19:33.000000 nekograd-0.2.0/nekograd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 08:19:33.000000 nekograd-0.2.0/nekograd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 08:19:33.000000 nekograd-0.2.0/nekograd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 08:19:24.000000 nekograd-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:19:33.955092 nekograd-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-03 08:19:24.000000 nekograd-0.2.0/setup.py
```

### Comparing `nekograd-0.1.1/LICENSE` & `nekograd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/PKG-INFO` & `nekograd-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: nekograd
-Version: 0.1.1
-Home-page: https://github.com/arseniybelkov/nekograd
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![codecov](https://codecov.io/gh/arseniybelkov/nekograd/branch/master/graph/badge.svg?token=J49UF83POB)](https://codecov.io/gh/arseniybelkov/nekograd)
 # nekograd
 _Fast & Flexible_ ~~(just like a catgirl)~~ deep learning framework.
   
-All frameworks require vast manuscripts of code written in order to
+All frameworks require vast manuscripts of code to be written in order to
 create the simplest trainable model configuration.
-We propose `nekograd` as a convinient way of creating such pipelines
+We propose `nekograd` as a convenient way of creating such pipelines
 with the least amount of code needed to be written.
+## Installation
 ```bash
 pip install nekograd
 ```
+or
+```bash
+git clone https://github.com/arseniybelkov/nekograd.git
+cd nekograd && pip install -e .
+```
 
 ## Example
 
+`CoreModel` inherits everything from [__LightningModule__](https://lightning.ai/docs/pytorch/stable/common/lightning_module.html#)  
+and just implements it basic methods so you don't have to. 
+
 ```python
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
 from nekograd.model import CoreModel
 from nekograd.model.policy import Multiply
 from sklearn.metrics import accuracy_score
@@ -47,8 +47,8 @@
 
 device = "gpu" if torch.cuda.is_available() else "cpu"
 
 trainer = pl.Trainer(max_epochs=20, accelerator=device)
 
 trainer.fit(model, datamodule=...)
 trainer.test(model, datamodule=...)
-```
+```
```

### Comparing `nekograd-0.1.1/README.md` & `nekograd-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,39 @@
+Metadata-Version: 2.1
+Name: nekograd
+Version: 0.2.0
+Home-page: https://github.com/arseniybelkov/nekograd
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![codecov](https://codecov.io/gh/arseniybelkov/nekograd/branch/master/graph/badge.svg?token=J49UF83POB)](https://codecov.io/gh/arseniybelkov/nekograd)
 # nekograd
 _Fast & Flexible_ ~~(just like a catgirl)~~ deep learning framework.
   
-All frameworks require vast manuscripts of code written in order to
+All frameworks require vast manuscripts of code to be written in order to
 create the simplest trainable model configuration.
-We propose `nekograd` as a convinient way of creating such pipelines
+We propose `nekograd` as a convenient way of creating such pipelines
 with the least amount of code needed to be written.
+## Installation
 ```bash
 pip install nekograd
 ```
+or
+```bash
+git clone https://github.com/arseniybelkov/nekograd.git
+cd nekograd && pip install -e .
+```
 
 ## Example
 
+`CoreModel` inherits everything from [__LightningModule__](https://lightning.ai/docs/pytorch/stable/common/lightning_module.html#)  
+and just implements it basic methods so you don't have to. 
+
 ```python
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
 from nekograd.model import CoreModel
 from nekograd.model.policy import Multiply
 from sklearn.metrics import accuracy_score
@@ -38,8 +56,8 @@
 
 device = "gpu" if torch.cuda.is_available() else "cpu"
 
 trainer = pl.Trainer(max_epochs=20, accelerator=device)
 
 trainer.fit(model, datamodule=...)
 trainer.test(model, datamodule=...)
-```
+```
```

### Comparing `nekograd-0.1.1/nekograd/data/split.py` & `nekograd-0.2.0/nekograd/data/split.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Hashable, Sequence, Tuple, Union
 
-from cytoolz import get
 from sklearn.model_selection import KFold, StratifiedKFold, train_test_split
+from toolz import get
 
 __all__ = ["train_val_test_split", "k_fold", "k_fold_single_test"]
 
 
 def train_val_test_split(
     ids: Sequence,
     val_size: Union[int, float],
```

### Comparing `nekograd-0.1.1/nekograd/metrics/binary.py` & `nekograd-0.2.0/nekograd/metrics/binary.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/metrics/checks.py` & `nekograd-0.2.0/nekograd/metrics/checks.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/metrics/utils.py` & `nekograd-0.2.0/nekograd/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/model/base.py` & `nekograd-0.2.0/nekograd/model/base.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/model/commands.py` & `nekograd-0.2.0/nekograd/model/commands.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/model/model.py` & `nekograd-0.2.0/nekograd/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
-from cytoolz import compose, keymap
 from more_itertools import collapse, unzip
+from toolz import compose, keymap
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
 from ..torch.utils import to_np
 from .base import EPOCH_OUTPUT, STEP_OUTPUT, BaseModel
 from .commands import compute_metrics
 from .utils import criterion_wrapper
@@ -41,20 +41,20 @@
     def configure_optimizers(self) -> Tuple[List[Optimizer], List[_LRScheduler]]:
         if self.optimizer is None or self.lr_scheduler is None:
             raise NotImplementedError(
                 "If you do not pass optimizer and lr_scheduler to __init__ method, "
                 "you must specify "
                 "configure_optimizers method"
             )
-        self.lr_scheduler = {
+        lr_scheduler = {
             "scheduler": self.lr_scheduler,
             "name": "lr_scheduler",
             "interval": "epoch",
         }
-        return [self.optimizer], [self.lr_scheduler]
+        return [self.optimizer], [lr_scheduler]
 
     def forward(self, *xs: torch.Tensor) -> torch.Tensor:
         return self.architecture(*xs)
 
     def training_step(
         self, batch: Tuple[torch.Tensor, ...], batch_idx: int
     ) -> Dict[str, torch.Tensor]:
```

### Comparing `nekograd-0.1.1/nekograd/model/policy.py` & `nekograd-0.2.0/nekograd/model/policy.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/model/utils.py` & `nekograd-0.2.0/nekograd/model/utils.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd/torch/criterion.py` & `nekograd-0.2.0/nekograd/torch/criterion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from inspect import isfunction
 from typing import Callable, Dict, List, Union
 
 import torch
-from cytoolz.functoolz import juxt
 from more_itertools import zip_equal
+from toolz.functoolz import juxt
 
 
 class CriterionDict(torch.nn.Module):
     """
     Parameters
     ----------
     criterions: Callable
```

### Comparing `nekograd-0.1.1/nekograd/torch/utils.py` & `nekograd-0.2.0/nekograd/torch/utils.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.1.1/nekograd.egg-info/PKG-INFO` & `nekograd-0.2.0/nekograd.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: nekograd
-Version: 0.1.1
+Version: 0.2.0
 Home-page: https://github.com/arseniybelkov/nekograd
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![codecov](https://codecov.io/gh/arseniybelkov/nekograd/branch/master/graph/badge.svg?token=J49UF83POB)](https://codecov.io/gh/arseniybelkov/nekograd)
 # nekograd
 _Fast & Flexible_ ~~(just like a catgirl)~~ deep learning framework.
   
-All frameworks require vast manuscripts of code written in order to
+All frameworks require vast manuscripts of code to be written in order to
 create the simplest trainable model configuration.
-We propose `nekograd` as a convinient way of creating such pipelines
+We propose `nekograd` as a convenient way of creating such pipelines
 with the least amount of code needed to be written.
+## Installation
 ```bash
 pip install nekograd
 ```
+or
+```bash
+git clone https://github.com/arseniybelkov/nekograd.git
+cd nekograd && pip install -e .
+```
 
 ## Example
 
+`CoreModel` inherits everything from [__LightningModule__](https://lightning.ai/docs/pytorch/stable/common/lightning_module.html#)  
+and just implements it basic methods so you don't have to. 
+
 ```python
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
 from nekograd.model import CoreModel
 from nekograd.model.policy import Multiply
 from sklearn.metrics import accuracy_score
```

### Comparing `nekograd-0.1.1/nekograd.egg-info/SOURCES.txt` & `nekograd-0.2.0/nekograd.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 nekograd/data/split.py
 nekograd/metrics/__init__.py
 nekograd/metrics/binary.py
 nekograd/metrics/checks.py
 nekograd/metrics/utils.py
 nekograd/model/__init__.py
 nekograd/model/base.py
+nekograd/model/callbacks.py
 nekograd/model/commands.py
 nekograd/model/model.py
 nekograd/model/policy.py
 nekograd/model/utils.py
 nekograd/torch/__init__.py
 nekograd/torch/criterion.py
 nekograd/torch/utils.py
```

