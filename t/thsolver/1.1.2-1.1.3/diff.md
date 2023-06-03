# Comparing `tmp/thsolver-1.1.2.tar.gz` & `tmp/thsolver-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsolver-1.1.2.tar", last modified: Thu Feb  9 01:24:05 2023, max compression
+gzip compressed data, was "thsolver-1.1.3.tar", last modified: Sat Jun  3 03:40:21 2023, max compression
```

## Comparing `thsolver-1.1.2.tar` & `thsolver-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:24:05.870976 thsolver-1.1.2/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 12:13:18.000000 thsolver-1.1.2/LICENSE
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-02-09 01:24:05.870976 thsolver-1.1.2/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      430 2023-02-09 01:21:20.000000 thsolver-1.1.2/README.md
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-02-09 01:24:05.870976 thsolver-1.1.2/setup.cfg
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1133 2023-02-09 01:21:48.000000 thsolver-1.1.2/setup.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:24:05.870976 thsolver-1.1.2/thsolver/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      782 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     7461 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/config.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2075 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/dataset.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2354 2022-10-25 12:13:18.000000 thsolver-1.1.2/thsolver/lr_scheduler.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      892 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/registry.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1555 2022-10-25 12:13:18.000000 thsolver-1.1.2/thsolver/sampler.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)    13667 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/solver.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2825 2023-02-09 01:19:59.000000 thsolver-1.1.2/thsolver/tracker.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:24:05.870976 thsolver-1.1.2/thsolver.egg-info/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-02-09 01:24:05.000000 thsolver-1.1.2/thsolver.egg-info/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      391 2023-02-09 01:24:05.000000 thsolver-1.1.2/thsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-02-09 01:24:05.000000 thsolver-1.1.2/thsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2022-10-26 01:01:16.000000 thsolver-1.1.2/thsolver.egg-info/not-zip-safe
--rw-rw-r--   0 wangps    (1001) wangps    (1001)       22 2023-02-09 01:24:05.000000 thsolver-1.1.2/thsolver.egg-info/requires.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        9 2023-02-09 01:24:05.000000 thsolver-1.1.2/thsolver.egg-info/top_level.txt
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 12:13:18.000000 thsolver-1.1.3/LICENSE
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-03 03:40:21.684440 thsolver-1.1.3/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      430 2023-06-01 09:42:54.000000 thsolver-1.1.3/README.md
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-06-03 03:40:21.684440 thsolver-1.1.3/setup.cfg
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1133 2023-06-03 03:13:18.000000 thsolver-1.1.3/setup.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/thsolver/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      782 2023-06-01 09:42:51.000000 thsolver-1.1.3/thsolver/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     7026 2023-06-03 03:14:22.000000 thsolver-1.1.3/thsolver/config.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2075 2023-06-01 09:42:51.000000 thsolver-1.1.3/thsolver/dataset.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2354 2022-10-25 12:13:18.000000 thsolver-1.1.3/thsolver/lr_scheduler.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1209 2023-06-01 09:51:14.000000 thsolver-1.1.3/thsolver/registry.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1555 2022-10-25 12:13:18.000000 thsolver-1.1.3/thsolver/sampler.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)    14718 2023-06-01 09:42:54.000000 thsolver-1.1.3/thsolver/solver.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3067 2023-06-01 09:42:54.000000 thsolver-1.1.3/thsolver/tracker.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/thsolver.egg-info/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      391 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2022-10-26 01:01:16.000000 thsolver-1.1.3/thsolver.egg-info/not-zip-safe
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)       22 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/requires.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        9 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/top_level.txt
```

### Comparing `thsolver-1.1.2/LICENSE` & `thsolver-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.2/PKG-INFO` & `thsolver-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsolver
-Version: 1.1.2
+Version: 1.1.3
 Summary: Solver for PyTorch
 Home-page: https://github.com/octree-nn/solver-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `thsolver-1.1.2/setup.py` & `thsolver-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c) 2022 Peng-Shuai Wang <wangps@hotmail.com>
 # Licensed under The MIT License [see LICENSE for details]
 # Written by Peng-Shuai Wang
 # --------------------------------------------------------
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 with open("README.md", "r", encoding="utf-8") as fid:
   long_description = fid.read()
 
 setup(
     name='thsolver',
     version=__version__,
```

### Comparing `thsolver-1.1.2/thsolver/__init__.py` & `thsolver-1.1.3/thsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.2/thsolver/config.py` & `thsolver-1.1.3/thsolver/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _C.SOLVER.max_epoch         = 300        # Maximum training epoch
 _C.SOLVER.warmup_epoch      = 20         # The warmup epoch number
 _C.SOLVER.warmup_init       = 0.001      # The initial ratio of the warmup
 _C.SOLVER.eval_epoch        = 1          # Maximum evaluating epoch
 _C.SOLVER.eval_step         = -1         # Maximum evaluating steps
 _C.SOLVER.test_every_epoch  = 10         # Test model every n training epochs
 _C.SOLVER.log_per_iter      = -1         # Output log every k training iteration
+_C.SOLVER.best_val          = 'min:loss' # The best validation metric
 
 _C.SOLVER.lr_type           = 'step'     # Learning rate type: step or cos
 _C.SOLVER.lr                = 0.1        # Initial learning rate
 _C.SOLVER.lr_min            = 0.0001     # The minimum learning rate
 _C.SOLVER.gamma             = 0.1        # Learning rate step-wise decay
 _C.SOLVER.milestones        = (120,180,) # Learning rate milestones
 _C.SOLVER.lr_power          = 0.9        # Used in poly learning rate
@@ -89,25 +90,16 @@
 _C.DATA.test.num_workers    = 2
 
 # MODEL related parameters
 _C.MODEL = CN(new_allowed=True)
 _C.MODEL.name               = ''          # The name of the model
 _C.MODEL.feature            = 'ND'        # The input features
 _C.MODEL.channel            = 3           # The input feature channel
-_C.MODEL.nout               = 40          # The output feature channel
 _C.MODEL.nempty             = False       # Perform Octree Conv on non-empty octree nodes
 
-# _C.MODEL.stages             = 3
-# _C.MODEL.resblock_num       = 3           # The resblock number
-# _C.MODEL.resblock_type      = 'bottleneck'# Choose from 'bottleneck' and 'basic
-# _C.MODEL.bottleneck         = 4           # The bottleneck factor of one resblock
-
-# _C.MODEL.upsample           = 'nearest'   # The method used for upsampling
-# _C.MODEL.interp             = 'linear'    # The interplation method: linear or nearest
-
 _C.MODEL.sync_bn            = False       # Use sync_bn when training the network
 _C.MODEL.use_checkpoint     = False       # Use checkpoint to save memory
 _C.MODEL.find_unused_parameters = False   # Used in DistributedDataParallel
 
 
 # loss related parameters
 _C.LOSS = CN(new_allowed=True)
```

### Comparing `thsolver-1.1.2/thsolver/dataset.py` & `thsolver-1.1.3/thsolver/dataset.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.2/thsolver/lr_scheduler.py` & `thsolver-1.1.3/thsolver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.2/thsolver/registry.py` & `thsolver-1.1.3/thsolver/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# --------------------------------------------------------
+# Octree-based Sparse Convolutional Neural Networks
+# Copyright (c) 2022 Peng-Shuai Wang <wangps@hotmail.com>
+# Licensed under The MIT License [see LICENSE for details]
+# Written by Peng-Shuai Wang
+# --------------------------------------------------------
+
 _model_entrypoints = {}
 _dataset_entrypoints = {}
 
 
 def register_model(fn):
   name = fn.__module__.split('.')[-1]
   _model_entrypoints[name] = fn
```

### Comparing `thsolver-1.1.2/thsolver/sampler.py` & `thsolver-1.1.3/thsolver/sampler.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.2/thsolver/solver.py` & `thsolver-1.1.3/thsolver/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     self.start_epoch = 1
 
     self.model = None           # torch.nn.Module
     self.optimizer = None       # torch.optim.Optimizer
     self.scheduler = None       # torch.optim.lr_scheduler._LRScheduler
     self.summary_writer = None  # torch.utils.tensorboard.SummaryWriter
     self.log_file = None        # str, used to save training logs
-    self.eval_rst = dict()       # used to save evalation results
+    self.eval_rst = dict()      # used to save evalation results
+    self.best_val = None        # used to save the best validation result
 
   def get_model(self):
     raise NotImplementedError
 
   def get_dataset(self, flags):
     raise NotImplementedError
 
@@ -127,16 +128,15 @@
     self.log_file = os.path.join(self.logdir, 'log.csv')
 
     if self.is_master:
       tqdm.write('Logdir: ' + self.logdir)
 
     if self.is_master and set_writer:
       self.summary_writer = SummaryWriter(self.logdir, flush_secs=20)
-      if not os.path.exists(self.ckpt_dir):
-        os.makedirs(self.ckpt_dir)
+      os.makedirs(self.ckpt_dir, exist_ok=True)
 
   def train_epoch(self, epoch):
     self.model.train()
     if self.world_size > 1:
       self.train_loader.sampler.set_epoch(epoch)
 
     tick = time.time()
@@ -199,43 +199,64 @@
 
       # track the averaged tensors
       test_tracker.update(output)
 
     if self.world_size > 1:
       test_tracker.average_all_gather()
     if self.is_master:
-      test_tracker.log(epoch, self.summary_writer, self.log_file, msg_tag='=>')
       self.result_callback(test_tracker, epoch)
+      self.save_best_checkpoint(test_tracker, epoch)
+      test_tracker.log(epoch, self.summary_writer, self.log_file, msg_tag='=>')
 
   def eval_epoch(self, epoch):
     self.model.eval()
     eval_step = min(self.FLAGS.SOLVER.eval_step, len(self.test_loader))
     if eval_step < 1:
       eval_step = len(self.test_loader)
     for it in tqdm(range(eval_step), ncols=80, leave=False):
       batch = self.test_iter.next()
       batch['iter_num'] = it
       batch['epoch'] = epoch
       with torch.no_grad():
         self.eval_step(batch)
 
+  def save_best_checkpoint(self, tracker: AverageTracker, epoch: int):
+    best_val = self.FLAGS.SOLVER.best_val
+    if not best_val: return  # return if best_val is empty
+
+    compare, key = best_val.split(':')
+    key = 'test/' + key
+    assert compare in ['max', 'min']
+    operator = lambda x, y: x > y if compare == 'max' else x < y
+
+    if key in tracker.value:
+      curr_val = (tracker.value[key] / tracker.num[key]).item()
+      if self.best_val is None or operator(curr_val, self.best_val):
+        self.best_val = curr_val
+        model_dict = (self.model.module.state_dict() if self.world_size > 1
+                      else self.model.state_dict())
+        torch.save(model_dict, os.path.join(self.logdir, 'best_model.pth'))
+        msg = 'epoch: %d, %s: %f' % (epoch, key, curr_val)
+        with open(os.path.join(self.logdir, 'best_model.txt'), 'a') as fid:
+          fid.write(msg + '\n')
+        tqdm.write('=> Best model at ' + msg)
+
   def save_checkpoint(self, epoch):
-    if not self.is_master:
-      return
+    if not self.is_master: return
 
     # clean up
     ckpts = sorted(os.listdir(self.ckpt_dir))
     ckpts = [ck for ck in ckpts if ck.endswith('.pth') or ck.endswith('.tar')]
     if len(ckpts) > self.FLAGS.SOLVER.ckpt_num:
       for ckpt in ckpts[:-self.FLAGS.SOLVER.ckpt_num]:
         os.remove(os.path.join(self.ckpt_dir, ckpt))
 
     # save ckpt
-    model_dict = self.model.module.state_dict() \
-        if self.world_size > 1 else self.model.state_dict()
+    model_dict = (self.model.module.state_dict() if self.world_size > 1
+                  else self.model.state_dict())
     ckpt_name = os.path.join(self.ckpt_dir, '%05d' % epoch)
     torch.save(model_dict, ckpt_name + '.model.pth')
     torch.save({'model_dict': model_dict, 'epoch': epoch,
                 'optimizer_dict': self.optimizer.state_dict(),
                 'scheduler_dict': self.scheduler.state_dict(), },
                ckpt_name + '.solver.tar')
```

### Comparing `thsolver-1.1.2/thsolver/tracker.py` & `thsolver-1.1.3/thsolver/tracker.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,38 +12,43 @@
 from tqdm import tqdm
 from typing import Dict
 
 
 class AverageTracker:
 
   def __init__(self):
-    self.value = None
-    self.num = 0.0
+    self.value = dict()
+    self.num = dict()
     self.max_len = 76
     self.start_time = time.time()
 
   def update(self, value: Dict[str, torch.Tensor]):
+    r'''Update the tracker with the given value, which is called at the end of
+    each iteration.
+    '''
+
     if not value:
       return    # empty input, return
 
-    value = {key: val.detach() for key, val in value.items()}
-    if self.value is None:
-      self.value = value
-    else:
-      for key, val in value.items():
-        self.value[key] += val
-    self.num += 1
+    for key, val in value.items():
+      self.value[key] = self.value.get(key, 0) + val.detach()
+      self.num[key] = self.num.get(key, 0) + 1
 
   def average(self):
-    return {key: val.item() / self.num for key, val in self.value.items()}
+    return {key: val.item() / self.num[key] for key, val in self.value.items()}
 
   @torch.no_grad()
   def average_all_gather(self):
+    r'''Average the tensors on all GPUs using all_gather, which is called at the
+    end of each epoch.
+    '''
+
     for key, tensor in self.value.items():
-      if not tensor.is_cuda: continue
+      if not (isinstance(tensor, torch.Tensor) and tensor.is_cuda):
+        continue  # only gather tensors on GPU
       tensors_gather = [torch.ones_like(tensor)
                         for _ in range(torch.distributed.get_world_size())]
       torch.distributed.all_gather(tensors_gather, tensor, async_op=False)
       tensors = torch.stack(tensors_gather, dim=0)
       self.value[key] = torch.mean(tensors)
 
   def log(self, epoch, summary_writer=None, log_file=None, msg_tag='->',
```

### Comparing `thsolver-1.1.2/thsolver.egg-info/PKG-INFO` & `thsolver-1.1.3/thsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsolver
-Version: 1.1.2
+Version: 1.1.3
 Summary: Solver for PyTorch
 Home-page: https://github.com/octree-nn/solver-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

