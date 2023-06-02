# Comparing `tmp/aipose-2.1.0.tar.gz` & `tmp/aipose-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipose-2.1.0.tar", max compression
+gzip compressed data, was "aipose-2.1.1.tar", max compression
```

## Comparing `aipose-2.1.0.tar` & `aipose-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1327 2023-06-02 22:32:01.100757 aipose-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6531 2023-06-02 22:32:01.100757 aipose-2.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/__init__.py
--rw-r--r--   0        0        0      348 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/__main__.py
--rw-r--r--   0        0        0      218 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/frame/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/frame/frame_manager_base.py
--rw-r--r--   0        0        0     2241 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/frame/frame_plot.py
--rw-r--r--   0        0        0     2791 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/frame/frame_yolo_v7.py
--rw-r--r--   0        0        0        0 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/models/yolov7/__init__.py
--rw-r--r--   0        0        0    10481 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/models/yolov7/domain.py
--rw-r--r--   0        0        0     3809 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/models/yolov7/types.py
--rw-r--r--   0        0        0     3330 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/plot.py
--rw-r--r--   0        0        0     2789 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/stream/__init__.py
--rw-r--r--   0        0        0     8244 2023-06-02 22:32:01.100757 aipose-2.1.0/aipose/utils.py
--rw-r--r--   0        0        0     2505 2023-06-02 22:32:01.356762 aipose-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     8013 1970-01-01 00:00:00.000000 aipose-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1327 2023-06-02 22:38:12.403816 aipose-2.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     6531 2023-06-02 22:38:12.403816 aipose-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/__main__.py
+-rw-r--r--   0        0        0      218 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/frame/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/frame/frame_manager_base.py
+-rw-r--r--   0        0        0     2241 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/frame/frame_plot.py
+-rw-r--r--   0        0        0     2791 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/frame/frame_yolo_v7.py
+-rw-r--r--   0        0        0        0 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/models/yolov7/__init__.py
+-rw-r--r--   0        0        0    10526 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/models/yolov7/domain.py
+-rw-r--r--   0        0        0     3809 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/models/yolov7/types.py
+-rw-r--r--   0        0        0     3330 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/plot.py
+-rw-r--r--   0        0        0     2789 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/stream/__init__.py
+-rw-r--r--   0        0        0     8244 2023-06-02 22:38:12.403816 aipose-2.1.1/aipose/utils.py
+-rw-r--r--   0        0        0     2505 2023-06-02 22:38:12.671819 aipose-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8013 1970-01-01 00:00:00.000000 aipose-2.1.1/PKG-INFO
```

### Comparing `aipose-2.1.0/LICENSE.txt` & `aipose-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/README.md` & `aipose-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/frame/frame_manager_base.py` & `aipose-2.1.1/aipose/frame/frame_manager_base.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/frame/frame_plot.py` & `aipose-2.1.1/aipose/frame/frame_plot.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/frame/frame_yolo_v7.py` & `aipose-2.1.1/aipose/frame/frame_yolo_v7.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/models/yolov7/domain.py` & `aipose-2.1.1/aipose/models/yolov7/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,29 +270,29 @@
         # Apply transforms
         image = transforms.ToTensor()(image)  # torch.Size([3, 567, 960])
         if torch.cuda.is_available():
             image = image.half().to(self.device)
         # Turn image into batch
         image = image.unsqueeze(0)  # torch.Size([1, 3, 567, 960])
         with torch.no_grad():
-            output, _ = self.model(image)
+            original_output, _ = self.model(image)
 
-        output = non_max_suppression_kpt(
-            output,
+        original_output = non_max_suppression_kpt(
+            original_output,
             0.25,
             0.65,
             nc=self.model.yaml["nc"],
             nkpt=self.model.yaml["nkpt"],
             kpt_label=True,
         )
 
         with torch.no_grad():
-            output = output_to_keypoint(output)
+            output = output_to_keypoint(original_output)
 
         return (
             [
                 YoloV7PoseKeypoints(prediction, image.shape[2], image.shape[3])
                 for prediction in output
             ],
             image,
-            output,
+            original_output,
         )
```

### Comparing `aipose-2.1.0/aipose/models/yolov7/types.py` & `aipose-2.1.1/aipose/models/yolov7/types.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/plot.py` & `aipose-2.1.1/aipose/plot.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/stream/__init__.py` & `aipose-2.1.1/aipose/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/aipose/utils.py` & `aipose-2.1.1/aipose/utils.py`

 * *Files identical despite different names*

### Comparing `aipose-2.1.0/pyproject.toml` & `aipose-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aipose"
-version = "2.1.0"
+version = "2.1.1"
 description = "Library to use pose estimation in your projects easily"
 license = "https://github.com/Tlaloc-Es/aipose/blob/master/LICENSE.txt"
 homepage = "https://github.com/Tlaloc-Es/aipose"
 repository = "https://github.com/Tlaloc-Es/aipose"
 documentation = "https://aipose.readthedocs.io/en/latest/"
 keywords = ["pose-estimator", "yolo", "yolov7"]
 authors = ["Tlaloc-Es <dev@tlaloc-es.com>"]
@@ -61,15 +61,15 @@
 ipykernel = "^6.21.2"
 notebook = "^6.5.2"
 seaborn = "^0.12.2"
 ipywidgets = "^8.0.4"
 vulture = "^2.7"
 
 [tool.commitizen]
-version = "2.1.0"
+version = "2.1.1"
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "$version"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `aipose-2.1.0/PKG-INFO` & `aipose-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipose
-Version: 2.1.0
+Version: 2.1.1
 Summary: Library to use pose estimation in your projects easily
 Home-page: https://github.com/Tlaloc-Es/aipose
 License: https://github.com/Tlaloc-Es/aipose/blob/master/LICENSE.txt
 Keywords: pose-estimator,yolo,yolov7
 Author: Tlaloc-Es
 Author-email: dev@tlaloc-es.com
 Requires-Python: >=3.10,<4.0
```

