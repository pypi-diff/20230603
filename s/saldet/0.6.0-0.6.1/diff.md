# Comparing `tmp/saldet-0.6.0.tar.gz` & `tmp/saldet-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.6.0.tar", max compression
+gzip compressed data, was "saldet-0.6.1.tar", max compression
```

## Comparing `saldet-0.6.0.tar` & `saldet-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.6.0/LICENSE
--rw-r--r--   0        0        0     4916 2023-06-02 19:04:58.286355 saldet-0.6.0/README.md
--rw-r--r--   0        0        0      917 2023-06-02 19:12:28.397873 saldet-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-02 18:45:06.967477 saldet-0.6.0/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.6.0/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-26 21:45:23.381327 saldet-0.6.0/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.6.0/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       58 2023-06-02 18:30:19.301072 saldet-0.6.0/saldet/experiment/__init__.py
--rw-r--r--   0        0        0     2920 2023-06-02 18:45:34.745533 saldet-0.6.0/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-06-02 17:51:09.638468 saldet-0.6.0/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.6.0/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.6.0/saldet/io/config.py
--rw-r--r--   0        0        0     1873 2023-05-26 21:46:31.461577 saldet-0.6.0/saldet/io/image.py
--rw-r--r--   0        0        0      147 2023-06-02 18:45:03.905231 saldet-0.6.0/saldet/loss/__init__.py
--rw-r--r--   0        0        0      415 2023-06-02 18:45:03.910327 saldet-0.6.0/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.6.0/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.6.0/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1635 2023-06-02 18:45:03.825497 saldet-0.6.0/saldet/loss/edge_saliency_loss.py
--rw-r--r--   0        0        0     1130 2023-05-17 16:56:43.163212 saldet-0.6.0/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-17 16:57:23.426213 saldet-0.6.0/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.6.0/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.6.0/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       65 2023-05-17 17:43:09.823099 saldet-0.6.0/saldet/models/__init__.py
--rw-r--r--   0        0        0     2457 2023-06-02 18:43:03.889178 saldet-0.6.0/saldet/models/_factory.py
--rw-r--r--   0        0        0       90 2023-06-02 18:43:55.413439 saldet-0.6.0/saldet/models/models/__init__.py
--rw-r--r--   0        0        0     9456 2023-06-02 18:44:33.695473 saldet-0.6.0/saldet/models/models/pfan.py
--rw-r--r--   0        0        0    10194 2023-06-02 18:39:22.910063 saldet-0.6.0/saldet/models/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.6.0/saldet/models/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-26 21:47:34.742688 saldet-0.6.0/saldet/models/models/swin.py
--rw-r--r--   0        0        0     6809 2023-06-02 18:49:54.482272 saldet-0.6.0/saldet/models/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.6.0/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-06-02 19:00:54.443854 saldet-0.6.0/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.6.0/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.6.0/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.6.0/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.6.0/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-06-02 17:51:50.370703 saldet-0.6.0/saldet/pl/model.py
--rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.6.0/saldet/plot/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-26 21:47:47.719210 saldet-0.6.0/saldet/plot/plot.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.6.0/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-26 21:44:58.032894 saldet-0.6.0/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.6.0/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3419 2023-05-27 08:17:01.712509 saldet-0.6.0/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.6.0/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-06-02 17:43:40.303851 saldet-0.6.0/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-26 21:42:57.941431 saldet-0.6.0/saldet/utils/time.py
--rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 saldet-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4916 2023-06-02 19:13:10.122398 saldet-0.6.1/README.md
+-rw-r--r--   0        0        0      917 2023-06-03 06:43:26.009800 saldet-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-03 06:43:16.916703 saldet-0.6.1/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.6.1/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-26 21:45:23.381327 saldet-0.6.1/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.6.1/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-06-02 18:30:19.301072 saldet-0.6.1/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2920 2023-06-02 19:13:10.122939 saldet-0.6.1/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-06-02 17:51:09.638468 saldet-0.6.1/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.6.1/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.6.1/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-26 21:46:31.461577 saldet-0.6.1/saldet/io/image.py
+-rw-r--r--   0        0        0      147 2023-06-02 19:13:10.123107 saldet-0.6.1/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-02 19:13:10.123252 saldet-0.6.1/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.6.1/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.6.1/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1635 2023-06-02 19:13:10.123347 saldet-0.6.1/saldet/loss/edge_saliency_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-17 16:56:43.163212 saldet-0.6.1/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-17 16:57:23.426213 saldet-0.6.1/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.6.1/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.6.1/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       65 2023-06-02 19:13:10.123456 saldet-0.6.1/saldet/models/__init__.py
+-rw-r--r--   0        0        0     2425 2023-06-03 06:45:12.385709 saldet-0.6.1/saldet/models/_factory.py
+-rw-r--r--   0        0        0       90 2023-06-02 19:13:10.123662 saldet-0.6.1/saldet/models/models/__init__.py
+-rw-r--r--   0        0        0     9456 2023-06-02 19:13:10.123781 saldet-0.6.1/saldet/models/models/pfan.py
+-rw-r--r--   0        0        0    10194 2023-06-02 19:13:10.123900 saldet-0.6.1/saldet/models/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-06-02 19:13:10.123991 saldet-0.6.1/saldet/models/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-06-02 19:13:10.124162 saldet-0.6.1/saldet/models/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-06-02 19:13:10.124287 saldet-0.6.1/saldet/models/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.6.1/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-02 19:00:54.443854 saldet-0.6.1/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.6.1/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.6.1/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.6.1/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.6.1/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-06-02 17:51:50.370703 saldet-0.6.1/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.6.1/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-26 21:47:47.719210 saldet-0.6.1/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.6.1/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-26 21:44:58.032894 saldet-0.6.1/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.6.1/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3419 2023-05-27 08:17:01.712509 saldet-0.6.1/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.6.1/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-02 17:43:40.303851 saldet-0.6.1/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-26 21:42:57.941431 saldet-0.6.1/saldet/utils/time.py
+-rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 saldet-0.6.1/PKG-INFO
```

### Comparing `saldet-0.6.0/LICENSE` & `saldet-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/README.md` & `saldet-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/pyproject.toml` & `saldet-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.6.0"
+version = "0.6.1"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
 keywords = ["computer vision", "saliency detection"]
```

### Comparing `saldet-0.6.0/saldet/dataset/inference.py` & `saldet-0.6.1/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/dataset/saliency.py` & `saldet-0.6.1/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/experiment/inference.py` & `saldet-0.6.1/saldet/experiment/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/experiment/train.py` & `saldet-0.6.1/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/io/image.py` & `saldet-0.6.1/saldet/io/image.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/loss/attn_guided.py` & `saldet-0.6.1/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/loss/bce_iou_loss.py` & `saldet-0.6.1/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/loss/edge_saliency_loss.py` & `saldet-0.6.1/saldet/loss/edge_saliency_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/loss/multi_bce.py` & `saldet-0.6.1/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/loss/pg.py` & `saldet-0.6.1/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.6.1/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/models/_factory.py` & `saldet-0.6.1/saldet/models/_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,16 @@
         model_name (str): model name
         checkpoint_path (str, optional): path to model checkpoint. Defaults to None.
 
     Returns:
         nn.Module: saliency model
     """
 
-    if model_name in FACTORY.keys():
-        model = FACTORY[model_name](**kwargs)
-    else:
-        print(f"> [ERROR] Model {model_name} not found.")
-
+    assert model_name in FACTORY.keys(), f"Model {model_name} not supported."
+    model = FACTORY[model_name](**kwargs)
     if checkpoint_path is not None:
         assert os.path.exists(checkpoint_path), f"{checkpoint_path} does not exist."
         try:
             state_dict = torch.load(f=checkpoint_path, map_location=device())
         except Exception as e:
             print(f"Found an exception while loading state dict - {e}")
             print(f"Trying on cpu")
```

### Comparing `saldet-0.6.0/saldet/models/models/pfan.py` & `saldet-0.6.1/saldet/models/models/pfan.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/models/models/pgnet.py` & `saldet-0.6.1/saldet/models/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/models/models/resnet.py` & `saldet-0.6.1/saldet/models/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/models/models/swin.py` & `saldet-0.6.1/saldet/models/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/models/models/u2net.py` & `saldet-0.6.1/saldet/models/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/ops/tensor.py` & `saldet-0.6.1/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/optimizer/optimizer.py` & `saldet-0.6.1/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/pl/data.py` & `saldet-0.6.1/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/pl/model.py` & `saldet-0.6.1/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/plot/plot.py` & `saldet-0.6.1/saldet/plot/plot.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/trainer/callbacks.py` & `saldet-0.6.1/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/saldet/transform/transform.py` & `saldet-0.6.1/saldet/transform/transform.py`

 * *Files identical despite different names*

### Comparing `saldet-0.6.0/PKG-INFO` & `saldet-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saldet
-Version: 0.6.0
+Version: 0.6.1
 Summary: Saliency Detection library (models, loss, utils) with PyTorch
 Home-page: https://github.com/riccardomusmeci/saldet
 License: MIT
 Keywords: computer vision,saliency detection
 Author: Riccardo Musmeci
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

