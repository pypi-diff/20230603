# Comparing `tmp/torch_adapters-0.0.4.tar.gz` & `tmp/torch_adapters-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_adapters-0.0.4.tar", max compression
+gzip compressed data, was "torch_adapters-0.0.5.tar", max compression
```

## Comparing `torch_adapters-0.0.4.tar` & `torch_adapters-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.4/LICENSE
--rw-r--r--   0        0        0      223 2023-05-30 00:02:18.733760 torch_adapters-0.0.4/README.md
--rw-r--r--   0        0        0      576 2023-06-01 21:32:25.317945 torch_adapters-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.4/src/torch_adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.4/src/torch_adapters/adapters/__init__.py
--rw-r--r--   0        0        0     1146 2023-05-30 14:37:46.194482 torch_adapters-0.0.4/src/torch_adapters/adapters/lora.py
--rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.4/src/torch_adapters/adapters/mixin.py
--rw-r--r--   0        0        0     3161 2023-06-01 19:54:15.021807 torch_adapters-0.0.4/src/torch_adapters/adapters/prompt_tuning.py
--rw-r--r--   0        0        0     2970 2023-06-01 21:11:08.412133 torch_adapters-0.0.4/src/torch_adapters/utils.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 torch_adapters-0.0.4/setup.py
--rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 torch_adapters-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.5/LICENSE
+-rw-r--r--   0        0        0      365 2023-06-03 17:10:11.157420 torch_adapters-0.0.5/README.md
+-rw-r--r--   0        0        0      576 2023-06-03 17:10:11.125420 torch_adapters-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.5/src/torch_adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.5/src/torch_adapters/adapters/__init__.py
+-rw-r--r--   0        0        0     1112 2023-06-03 16:58:19.487497 torch_adapters-0.0.5/src/torch_adapters/adapters/adapter.py
+-rw-r--r--   0        0        0     1731 2023-06-03 16:44:50.108688 torch_adapters-0.0.5/src/torch_adapters/adapters/lora.py
+-rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.5/src/torch_adapters/adapters/mixin.py
+-rw-r--r--   0        0        0     3161 2023-06-01 19:54:15.021807 torch_adapters-0.0.5/src/torch_adapters/adapters/prompt_tuning.py
+-rw-r--r--   0        0        0     4038 2023-06-03 17:04:27.528683 torch_adapters-0.0.5/src/torch_adapters/utils.py
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 torch_adapters-0.0.5/setup.py
+-rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 torch_adapters-0.0.5/PKG-INFO
```

### Comparing `torch_adapters-0.0.4/LICENSE` & `torch_adapters-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.4/pyproject.toml` & `torch_adapters-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-adapters"
-version = "0.0.4"
+version = "0.0.5"
 description = "Small Library of Torch Adaptation modules"
 authors = ["ma2za <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "torch_adapters", from = "src" }]
 
 repository = "https://github.com/ma2za/torch-adapters"
```

### Comparing `torch_adapters-0.0.4/src/torch_adapters/adapters/lora.py` & `torch_adapters-0.0.5/src/torch_adapters/adapters/lora.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections import OrderedDict
 
-import torch
 from torch import nn, Tensor
-from torch.nn import init
 
 from torch_adapters.adapters.mixin import AdapterMixin
 
 
 class LoRA(nn.Linear, AdapterMixin):
     """
 
+    Layers to train at finetuning: adapter, layer-norm, classifier.
+
     LoRA: Low-Rank Adaptation of Large Language Models
     by Edward J. Hu, Yelong Shen, Phillip Wallis, Zeyuan Allen-Zhu,
     Yuanzhi Li, Shean Wang, Lu Wang, Weizhu Chen
     https://arxiv.org/abs/2106.09685
 
     """
 
@@ -21,20 +21,30 @@
                  src: nn.Linear,
                  alpha: int = 8,
                  r: int = 8):
         super().__init__(src.in_features, src.out_features)
 
         self.copy_attributes_from_source(src)
 
-        self.lora_weight = torch.nn.Sequential(OrderedDict([
+        self.lora_weight = nn.Sequential(OrderedDict([
             ("A", nn.Linear(self.in_features, r, bias=False)),
             ("B", nn.Linear(r, self.out_features, bias=False))
         ]))
 
         self.alpha = alpha
         self.r = r
 
-        init.zeros_(self.lora_weight.B.weight)
-        init.normal_(self.lora_weight.A.weight)
+        nn.init.zeros_(self.lora_weight.B.weight)
+        nn.init.normal_(self.lora_weight.A.weight)
+
+    def merge(self) -> nn.Linear:
+        # TODO add copy of other attributes
+        # TODO check if matrix transpose is required
+        merged_layer = nn.Linear(self.in_features, self.out_features)
+        merged_weight = self.weight.data + (self.alpha / self.r) * (
+                self.lora_weight.B.weight.data @ self.lora_weight.A.weight.data)
+        merged_layer.weight.data = merged_weight.detach().clone().to(self.weight.device)
+        merged_layer.bias.data = self.bias.data.detach().clone().to(self.bias.device)
+        return merged_layer
 
     def forward(self, input_ids: Tensor) -> Tensor:
         return super().forward(input_ids) + self.lora_weight(input_ids) * (self.alpha / self.r)
```

### Comparing `torch_adapters-0.0.4/src/torch_adapters/adapters/prompt_tuning.py` & `torch_adapters-0.0.5/src/torch_adapters/adapters/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.4/src/torch_adapters/utils.py` & `torch_adapters-0.0.5/src/torch_adapters/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 from operator import attrgetter
 from typing import List, Dict
 
 import torch
 from torch import nn
 
+from .adapters.adapter import Adapter
 from .adapters.lora import LoRA
 from .adapters.prompt_tuning import PromptTuningEmbedding, PromptTokenTypeEmbedding, \
     PromptAbsolutePositionalEmbedding
 
 
-# TODO group in una utility class
+# TODO group in a utility class
 
 # TODO consider if unify in one add method with configuration
 
 
+def add_adapter(model: nn.Module, layers_names: List[str], config: Dict) -> torch.nn.Module:
+    """
+
+    :param model:
+    :param layers_names:
+    :param config:
+    :return:
+    """
+    for name, module in model.named_modules():
+        if any([i in name for i in layers_names]):
+            module_name, attr_name = name.rsplit(".", 1)
+            module: nn.Module = attrgetter(module_name)(model)
+            attr: nn.Module = attrgetter(name)(model)
+
+            # TODO specialize exception
+            if not isinstance(attr, nn.Linear):
+                raise Exception
+
+            module.__setattr__(attr_name, Adapter(attr, adapter_size=config.get("adapter_size", 64)))
+    return model
+
+
 def add_lora(model: nn.Module, layers_names: List[str], config: Dict) -> torch.nn.Module:
     """
 
     Replace in-place the linear layers named in layers_names with a LoRA layer
     having the same weight and bias parameters.
 
     :param model:
@@ -41,14 +64,23 @@
                 attr,
                 alpha=config.get("alpha", 8),
                 r=config.get("r", 8)
             ))
     return model
 
 
+def merge_lora(model, layers_names):
+    for name, module in model.named_modules():
+        if isinstance(module, LoRA):
+            module_name, attr_name = name.rsplit(".", 1)
+            parent_module: nn.Module = attrgetter(module_name)(model)
+            parent_module.__setattr__(attr_name, module.merge())
+    return model
+
+
 def add_prompt_tuning(model: nn.Module, embeddings: Dict, config: Dict) -> nn.Module:
     for name, module in model.named_modules():
         if any([i in name for i in embeddings.keys()]):
             module_name, attr_name = name.rsplit(".", 1)
             if attr_name not in embeddings.keys():
                 continue
             module: nn.Module = attrgetter(module_name)(model)
```

### Comparing `torch_adapters-0.0.4/setup.py` & `torch_adapters-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-adapters',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Small Library of Torch Adaptation modules',
-    'long_description': '# Torch Adapters\n\n> <em>"During a gold rush, sell shovels."</em>\n\n# Introduction\n\nSmall Library of Torch Adaptation modules\n\n# Installation\n\nYou can install torch-adapters using:\n\n    $ pip install torch-adapters\n\n# Usage\n\n',
+    'long_description': '# Torch Adapters\n\n> <em>"During a gold rush, sell shovels."</em>\n\n# Introduction\n\nSmall Library of Torch Adaptation modules\n\n### Supported Methods\n\n- [X] LoRA\n- [X] Prompt Tuning\n- [X] Bottleneck Adapter\n\n# Installation\n\nYou can install torch-adapters using:\n\n    $ pip install torch-adapters\n\n# Usage\n\n    $ add_lora(model, ["key", "value"], {"alpha": 8, "r": 8})\n',
     'author': 'ma2za',
     'author_email': 'mazzapaolo2019@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ma2za/torch-adapters',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `torch_adapters-0.0.4/PKG-INFO` & `torch_adapters-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adapters
-Version: 0.0.4
+Version: 0.0.5
 Summary: Small Library of Torch Adaptation modules
 Home-page: https://github.com/ma2za/torch-adapters
 License: MIT
 Keywords: lora,adapters,llm,transformers,bert
 Author: ma2za
 Author-email: mazzapaolo2019@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -22,16 +22,23 @@
 
 > <em>"During a gold rush, sell shovels."</em>
 
 # Introduction
 
 Small Library of Torch Adaptation modules
 
+### Supported Methods
+
+- [X] LoRA
+- [X] Prompt Tuning
+- [X] Bottleneck Adapter
+
 # Installation
 
 You can install torch-adapters using:
 
     $ pip install torch-adapters
 
 # Usage
 
+    $ add_lora(model, ["key", "value"], {"alpha": 8, "r": 8})
```

