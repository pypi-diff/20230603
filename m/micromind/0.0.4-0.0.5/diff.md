# Comparing `tmp/micromind-0.0.4.tar.gz` & `tmp/micromind-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micromind-0.0.4.tar", last modified: Fri Mar  3 12:24:08 2023, max compression
+gzip compressed data, was "micromind-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `micromind-0.0.4.tar` & `micromind-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-03-03 12:24:00.693664 micromind-0.0.4/LICENSE
--rw-r--r--   0        0        0     1858 2023-03-03 12:24:00.693664 micromind-0.0.4/README.md
--rw-r--r--   0        0        0      726 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/__init__.py
--rw-r--r--   0        0        0       77 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/conversion/__init__.py
--rw-r--r--   0        0        0     3643 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/conversion/convert.py
--rw-r--r--   0        0        0       27 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/networks/__init__.py
--rw-r--r--   0        0        0    24515 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/networks/phinet.py
--rw-r--r--   0        0        0        0 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/utils/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-03 12:24:00.693664 micromind-0.0.4/micromind/utils/configlib.py
--rw-r--r--   0        0        0     1536 2023-03-03 12:24:00.693664 micromind-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 micromind-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-03 15:31:23.025485 micromind-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1981 2023-06-03 15:31:23.025485 micromind-0.0.5/README.md
+-rw-r--r--   0        0        0      726 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/conversion/__init__.py
+-rw-r--r--   0        0        0     4016 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/conversion/convert.py
+-rw-r--r--   0        0        0       27 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/networks/__init__.py
+-rw-r--r--   0        0        0    25507 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/networks/phinet.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2023-06-03 15:31:23.025485 micromind-0.0.5/micromind/utils/configlib.py
+-rw-r--r--   0        0        0     1587 2023-06-03 15:31:23.025485 micromind-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 micromind-0.0.5/PKG-INFO
```

### Comparing `micromind-0.0.4/micromind/__init__.py` & `micromind-0.0.5/micromind/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .networks.phinet import PhiNet
 from .utils import configlib
 
 
 # Package version
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 """datasets_info is a dictionary that contains information about the attributes
 of the datasets.
 This dictionary is used in networks.py inside the from_pretrained class method
 in order to examine the inputs and initialize the PhiNet or, in case of
 mismatching between dataset and Nclasses, raise an AssertionError."""
 datasets_info = {
```

### Comparing `micromind-0.0.4/micromind/conversion/convert.py` & `micromind-0.0.5/micromind/conversion/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,37 +2,43 @@
 Conversion from pytorch to different standard formats
 for inference (ONNX, OpenVINO, tflite).
 
 Authors:
     - Francesco Paissan, 2023
     - Alberto Ancilotto, 2023
 """
-import os
-import shutil
-import sys
-from pathlib import Path
-
-import numpy as np
-import onnx
-import onnxsim
-import tensorflow as tf
-import torch
-import torch.nn as nn
-from onnx_tf.backend import prepare
-from openvino.tools.mo import main as mo_main
+try:
+    import os
+    import shutil
+    import sys
+    from pathlib import Path
+
+    import numpy as np
+    import onnx
+    import onnxsim
+    import tensorflow as tf
+    import torch
+    import torch.nn as nn
+    from onnx_tf.backend import prepare
+    from openvino.tools.mo import main as mo_main
+except Exception as e:
+    print(str(e))
+    print("Did you install micromind with conversion capabilities?")
+    print("Please try again after pip install micromind[conversion].")
+    quit()
 
 
 @torch.no_grad()
 def convert_to_onnx(net: nn.Module, save_path: Path, simplify: bool = True):
     """Converts nn.Module to onnx and saves it to save_path.
     Optionally simplifies it."""
-    x = torch.zeros([1] + net.input_shape)
+    x = torch.zeros([1] + list(net.input_shape))
 
     torch.onnx.export(
-        net,
+        net.cpu(),
         x,
         save_path,
         verbose=False,
         input_names=["input"],
         output_names=["output"],
         opset_version=11,
     )
@@ -84,21 +90,26 @@
 def convert_to_tflite(
     net: nn.Module, save_path: Path, batch_quant: torch.Tensor = None
 ) -> None:
     """Converts nn.Module to tf_lite, optionally quantizes it."""
     if not isinstance(save_path, Path):
         save_path = Path(save_path)
 
+    if not (batch_quant is None):
+        batch_quant = batch_quant.cpu()
+
     vino_sub = save_path.joinpath("vino")
     os.makedirs(vino_sub, exist_ok=True)
     vino_path = convert_to_openvino(net, vino_sub)
     if os.name == "nt":
         openvino2tensorflow_exe_cmd = [
             sys.executable,
-            os.path.join(os.path.dirname(sys.executable), "openvino2tensorflow"),
+            os.path.join(
+                os.path.dirname(sys.executable), "Scripts", "openvino2tensorflow"
+            ),
         ]
     else:
         openvino2tensorflow_exe_cmd = ["openvino2tensorflow"]
 
     cmd = openvino2tensorflow_exe_cmd + [
         "--model_path",
         str(vino_path),
```

### Comparing `micromind-0.0.4/micromind/networks/phinet.py` & `micromind-0.0.5/micromind/networks/phinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
 from torchinfo import summary
+import os
 
 import micromind
 
 
 def correct_pad(input_shape, kernel_size):
     """Returns a tuple for zero-padding for 2D convolution with downsampling
 
@@ -415,21 +416,23 @@
         cls,
         dataset,
         alpha,
         beta,
         t_zero,
         num_layers,
         resolution,
+        path=None,
         num_classes=None,
         classifier=True,
         device=None,
     ):
-        """Loads parameters from checkpoint through Hugging Face Hub.
-        This function constructs two strings, "repo_dir" to find the model on Hugging
-        Face Hub and "file_to_choose" to select the correct file inside the repo, and
+        """Loads parameters from checkpoint through Hugging Face Hub or through local
+        file system.
+        This function constructs two strings, `repo_dir` to find the model on Hugging
+        Face Hub and `file_to_choose` to select the correct file inside the repo, and
         use them to download the pretrained model and initialize the PhiNet.
 
         Arguments
         ---------
         dataset : string
             The dataset on which the model has been trained with.
         alpha : float
@@ -438,14 +441,17 @@
             The beta hyperparameter.
         t_zero : float
             The t_zero hyperparameter.
         num_layers : int
             The number of layers.
         resolution : int
             The resolution of the images used during training.
+        path : string
+            The directory path or file path pointing to the checkpoint.
+            If None, the checkpoint is searched on HuggingFace.
         num_classes : int
             The number of classes that the model has been trained for.
             If None, it gets the specific value determined by the dataset used.
         classifier : bool
             If True, the model returend includes the classifier.
         device : string
             The device that loads all the tensors.
@@ -457,14 +463,15 @@
 
         Example
         -------
         .. doctest::
 
             >>> from micromind import PhiNet
             >>> model = PhiNet.from_pretrained("CIFAR-10", 3.0, 0.75, 6.0, 7, 160)
+            Checkpoint taken from HuggingHace hub.
             Checkpoint loaded successfully.
         """
         if num_classes is None:
             num_classes = micromind.datasets_info[dataset]["Nclasses"]
 
         repo_dir = f"micromind/{dataset}"
         file_to_choose = f"\
@@ -480,33 +487,49 @@
 
         if device is None:
             if torch.cuda.is_available():
                 device = "cuda"
             else:
                 device = "cpu"
 
-        try:
-            downloaded_file_path = hf_hub_download(
-                repo_id=repo_dir, filename=file_to_choose
-            )
-            state_dict = torch.load(str(downloaded_file_path), map_location=device)
-            model_found = True
-
-        except EntryNotFoundError:
-            state_dict = {
-                "args": SimpleNamespace(
-                    alpha=alpha,
-                    beta=beta,
-                    t_zero=t_zero,
-                    num_layers=num_layers,
-                    num_classes=num_classes,
+        if path is not None:
+            path_to_search = os.path.join(path, file_to_choose)
+            if os.path.isfile(path):
+                path_to_search = path
+            if os.path.isfile(path_to_search):
+                state_dict = torch.load(str(path_to_search), map_location=device)
+                model_found = True
+                print("Checkpoint taken from local file system.")
+            else:
+                model_found = False
+                print(
+                    "Checkpoint not taken from local file system."
+                    + f"{path_to_search} is not a valid checkpoint."
+                )
+        if (path is None) or not model_found:
+            try:
+                downloaded_file_path = hf_hub_download(
+                    repo_id=repo_dir, filename=file_to_choose
                 )
-            }
-            model_found = False
-            logging.warning("Model initialized without loading checkpoint.")
+                state_dict = torch.load(str(downloaded_file_path), map_location=device)
+                print("Checkpoint taken from HuggingHace hub.")
+                model_found = True
+
+            except EntryNotFoundError:
+                state_dict = {
+                    "args": SimpleNamespace(
+                        alpha=alpha,
+                        beta=beta,
+                        t_zero=t_zero,
+                        num_layers=num_layers,
+                        num_classes=num_classes,
+                    )
+                }
+                model_found = False
+                logging.warning("Model initialized without loading checkpoint.")
 
         # model initialized
         model = cls(
             (micromind.datasets_info[dataset]["NChannels"], resolution, resolution),
             alpha=state_dict["args"].alpha,
             beta=state_dict["args"].beta,
             t_zero=state_dict["args"].t_zero,
@@ -825,18 +848,18 @@
             spatial_res = (
                 spatial_res / 2 if block_id in downsampling_layers else spatial_res
             )
             block_id += 1
 
         if include_top:
             # Includes classification head if required
-            self.glob_pooling = lambda x: nn.functional.avg_pool2d(x, x.size()[2:])
-
-            self.new_convolution = nn.Conv2d(
-                int(block_filters * alpha), num_classes, kernel_size=1, bias=True
+            self.classifier = nn.Sequential(
+                nn.AdaptiveAvgPool2d((1, 1)),
+                nn.Flatten(),
+                nn.Linear(int(block_filters * alpha), num_classes, bias=True),
             )
 
     def forward(self, x):
         """Executes PhiNet network
 
         Arguments
         -------
@@ -847,12 +870,10 @@
         ------
             Logits if `include_top=True`, otherwise embeddings : torch.Tensor
         """
         for layers in self._layers:
             x = layers(x)
 
         if self.classify:
-            x = self.glob_pooling(x)
-            x = self.new_convolution(x)
-            x = x.view(-1, x.shape[1])
+            x = self.classifier(x)
 
         return x
```

### Comparing `micromind-0.0.4/micromind/utils/configlib.py` & `micromind-0.0.5/micromind/utils/configlib.py`

 * *Files identical despite different names*

### Comparing `micromind-0.0.4/pyproject.toml` & `micromind-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,52 +10,54 @@
 name = "micromind"
 dynamic=["version"]
 description = "MicroMind"
 readme = "README.md"
 authors = [{ name = "Francesco Paissan & others", email = "francescopaissan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
     "torch",
     "torchinfo",
     "huggingface_hub",
+]
+requires-python = ">=3.8"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "flake8", "isort", "pip-tools", "pytest", "pre-commit"]
+conversion = [
     "onnx",
     "onnx_tf==1.10.0",
     "onnx-simplifier==0.4.13",
     "onnxruntime==1.13.1",
     "openvino-dev==2022.3.0",
     "openvino2tensorflow==1.34.0",
     "tensorflow_datasets==4.8.1",
     "tensorflow==2.11.0",
-    "tensorflow_probability"
+    "tensorflow_probability==0.19.0"
 ]
-requires-python = ">=3.9"
-
-[project.optional-dependencies]
-dev = ["black", "bumpver", "flake8", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/fpaissan/micromind"
 
 [project.scripts]
 phinet = "__main__:main"
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 py-modules = []
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `micromind-0.0.4/PKG-INFO` & `micromind-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 Metadata-Version: 2.1
 Name: micromind
-Version: 0.0.4
+Version: 0.0.5
 Summary: MicroMind
 Keywords: feed,reader,tutorial
 Author-email: Francesco Paissan & others <francescopaissan@gmail.com>
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: torch
 Requires-Dist: torchinfo
 Requires-Dist: huggingface_hub
-Requires-Dist: onnx
-Requires-Dist: onnx_tf==1.10.0
-Requires-Dist: onnx-simplifier==0.4.13
-Requires-Dist: onnxruntime==1.13.1
-Requires-Dist: openvino-dev==2022.3.0
-Requires-Dist: openvino2tensorflow==1.34.0
-Requires-Dist: tensorflow_datasets==4.8.1
-Requires-Dist: tensorflow==2.11.0
-Requires-Dist: tensorflow_probability
+Requires-Dist: onnx ; extra == "conversion"
+Requires-Dist: onnx_tf==1.10.0 ; extra == "conversion"
+Requires-Dist: onnx-simplifier==0.4.13 ; extra == "conversion"
+Requires-Dist: onnxruntime==1.13.1 ; extra == "conversion"
+Requires-Dist: openvino-dev==2022.3.0 ; extra == "conversion"
+Requires-Dist: openvino2tensorflow==1.34.0 ; extra == "conversion"
+Requires-Dist: tensorflow_datasets==4.8.1 ; extra == "conversion"
+Requires-Dist: tensorflow==2.11.0 ; extra == "conversion"
+Requires-Dist: tensorflow_probability==0.19.0 ; extra == "conversion"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
 Project-URL: Homepage, https://github.com/fpaissan/micromind
+Provides-Extra: conversion
 Provides-Extra: dev
 
-<div align="center">    
- 
-[![Paper](http://img.shields.io/badge/paper-arxiv.1001.2234-B31B1B.svg)](https://arxiv.org/abs/2110.00337)
+[![Python version: 3.8 | 3.9 | 3.10](https://img.shields.io/badge/python-3.9%20|%203.10-blue)](https://www.python.org/downloads/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/fpaissan/micromind/blob/main/LICENSE)
+![PyPI version](https://img.shields.io/pypi/v/micromind)
 
-</div>
+This is the official repo of `micromind`, a toolkit that aims at bridging two communities: artificial intelligence and embedded systems. `micromind` is based on [PyTorch](https://pytorch.org) and provides exportability for the supported models in ONNX, Intel OpenVINO, and TFLite.
 
-This repository is a collection of our efforts towards the design, implementation and evaluation of ML techniques in the field of tinyML. 
+---------------------------------------------------------------------------------------------------------
 
-Here is a list of things you can do with the `phinet` package:
- - [image classification](recipes/image_classification)
+## 💡 Key features
 
-## To install the package 
+- Smooth flow from research to deployment;
+- Support for multimedia analytics recipes (image classification, sound event detection, etc);
+- Detailed API documentation;
+- Tutorials for embedded deployment;
 
-```setup
-pip install git+https://github.com/fpaissan/phinet
-```
+---------------------------------------------------------------------------------------------------------
+
+## 🛠️️ Installation
+
+### Using Pip
+
+First of all, install [Python 3.8 or later](https://www.python.org). Open a terminal and run:
 
-## Cite us
 ```
-@article{10.1145/3510832,
-	author = {Paissan, Francesco and Ancilotto, Alberto and Farella, Elisabetta},
-	title = {PhiNets: A Scalable Backbone for Low-Power AI at the Edge},
-	year = {2022},
-	publisher = {Association for Computing Machinery},
-	address = {New York, NY, USA},
-	url = {https://doi.org/10.1145/3510832},
-	doi = {10.1145/3510832},
-	journal = {ACM Trans. Embed. Comput. Syst.},
-}
+pip install micromind
 ```
-<!---
-
-## Pre-trained Models
+for the basic install. To install `micromind` with the full exportability features, run
 
-You can download pretrained models here:
+```
+pip install micromind[conversion]
+```
 
-- [My awesome model](https://drive.google.com/mymodel.pth) trained on ImageNet using parameters x,y,z. 
+### From source
 
->📋  Give a link to where/how the pretrained models can be downloaded and how they were trained (if applicable).  Alternatively you can have an additional column in your results table with a link to the models.
+First of all, install [Python 3.9 or later](https://www.python.org).
+Clone or download and extract the repository, navigate to `<path-to-repository>`, open a
+terminal and run:
 
-## Results
+```
+pip install -e .
+```
+for the basic install. To install `micromind` with the full exportability features, run
 
-Our model achieves the following performance on :
+```
+pip install -e .[conversion]
+```
 
-### [Image Classification on ImageNet](https://paperswithcode.com/sota/image-classification-on-imagenet)
+---------------------------------------------------------------------------------------------------------
 
-| Model name         | Top 1 Accuracy  | Top 5 Accuracy |
-| ------------------ |---------------- | -------------- |
-| My awesome model   |     85%         |      95%       |
+## 📧 Contact
 
-> Include a table of results from your paper, and link back to the leaderboard for clarity and context. If your main result is a figure, include that figure and link to the command or notebook to reproduce it. 
+[francescopaissan@gmail.com](mailto:francescopaissan@gmail.com)
 
---->
+---------------------------------------------------------------------------------------------------------
```

