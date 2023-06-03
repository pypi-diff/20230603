# Comparing `tmp/prefab-0.2.5.tar.gz` & `tmp/prefab-0.2.6.tar.gz`

## Comparing `prefab-0.2.5.tar` & `prefab-0.2.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.2.5/.gitattributes
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.2.5/.pylintrc
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.2.5/requirements.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.2.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/logo.png
--rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/promo_c.png
--rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/promo_p.png
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/circles-inverse_512x512.png
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/circles_512x512.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_16x128_256x256.png
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_32x128_256x256.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_64x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_16x128_256x256.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_32x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_64x128_256x256.png
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/devices.gds
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_16_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_32_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_64_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_16_512x512.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_32_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_64_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_16_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_32_512x512.png
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_64_512x512.png
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/pie_128x128_256x256.png
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/rectangle_128x128_256x256.png
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/ring_64x128_256x256.png
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/star_128x128_256x256.png
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 prefab-0.2.5/docs/models.md
--rw-r--r--   0        0        0   281939 2020-02-02 00:00:00.000000 prefab-0.2.5/examples/example_prediction.ipynb
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/__init__.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/io.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/predictor.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/processor.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.2.5/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.2.5/LICENSE
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 prefab-0.2.5/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    35376 2020-02-02 00:00:00.000000 prefab-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.2.6/.gitattributes
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.2.6/.pylintrc
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.2.6/requirements.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.2.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/logo.png
+-rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/promo_c.png
+-rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/promo_p.png
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/circles-inverse_512x512.png
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/circles_512x512.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_16x128_256x256.png
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_32x128_256x256.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_64x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_16x128_256x256.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_32x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_64x128_256x256.png
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/devices.gds
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_16_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_32_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_64_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_16_512x512.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_32_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_64_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_16_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_32_512x512.png
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_64_512x512.png
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/pie_128x128_256x256.png
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/rectangle_128x128_256x256.png
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/ring_64x128_256x256.png
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/star_128x128_256x256.png
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 prefab-0.2.6/docs/models.md
+-rw-r--r--   0        0        0   232507 2020-02-02 00:00:00.000000 prefab-0.2.6/examples/example_prediction.ipynb
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/__init__.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/io.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/predictor.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/processor.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.2.6/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 prefab-0.2.6/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    35500 2020-02-02 00:00:00.000000 prefab-0.2.6/PKG-INFO
```

### Comparing `prefab-0.2.5/.github/workflows/python-publish.yml` & `prefab-0.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/assets/logo.png` & `prefab-0.2.6/assets/logo.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/assets/promo_c.png` & `prefab-0.2.6/assets/promo_c.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/assets/promo_p.png` & `prefab-0.2.6/assets/promo_p.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/circles-inverse_512x512.png` & `prefab-0.2.6/devices/circles-inverse_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/circles_512x512.png` & `prefab-0.2.6/devices/circles_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross-inverse_16x128_256x256.png` & `prefab-0.2.6/devices/cross-inverse_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross-inverse_32x128_256x256.png` & `prefab-0.2.6/devices/cross-inverse_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross-inverse_64x128_256x256.png` & `prefab-0.2.6/devices/cross-inverse_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross_16x128_256x256.png` & `prefab-0.2.6/devices/cross_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross_32x128_256x256.png` & `prefab-0.2.6/devices/cross_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/cross_64x128_256x256.png` & `prefab-0.2.6/devices/cross_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/devices.gds` & `prefab-0.2.6/devices/devices.gds`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_16x256_16_512x512.png` & `prefab-0.2.6/devices/grating_16x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_16x256_32_512x512.png` & `prefab-0.2.6/devices/grating_16x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_16x256_64_512x512.png` & `prefab-0.2.6/devices/grating_16x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_32x256_16_512x512.png` & `prefab-0.2.6/devices/grating_32x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_32x256_32_512x512.png` & `prefab-0.2.6/devices/grating_32x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_32x256_64_512x512.png` & `prefab-0.2.6/devices/grating_32x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_64x256_16_512x512.png` & `prefab-0.2.6/devices/grating_64x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_64x256_32_512x512.png` & `prefab-0.2.6/devices/grating_64x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/grating_64x256_64_512x512.png` & `prefab-0.2.6/devices/grating_64x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/pie_128x128_256x256.png` & `prefab-0.2.6/devices/pie_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/rectangle_128x128_256x256.png` & `prefab-0.2.6/devices/rectangle_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/ring_64x128_256x256.png` & `prefab-0.2.6/devices/ring_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/devices/star_128x128_256x256.png` & `prefab-0.2.6/devices/star_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/prefab/__init__.py` & `prefab-0.2.6/prefab/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Import PreFab as pf.
 """
 
 from prefab.predictor import predict
 
 from prefab.io import load_device_img
 from prefab.io import load_device_gds
+from prefab.io import device_to_cell
 
 from prefab.processor import binarize
 from prefab.processor import binarize_hard
 from prefab.processor import trim
 from prefab.processor import clip
 from prefab.processor import pad
 from prefab.processor import get_contour
@@ -21,8 +22,9 @@
     "binarize",
     "binarize_hard",
     "trim",
     "clip",
     "pad",
     "get_contour",
     "get_uncertainty",
+    "device_to_cell"
 )
```

### Comparing `prefab-0.2.5/prefab/io.py` & `prefab-0.2.6/prefab/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loading and exporting functions for device images/matrices.
 """
 
 import matplotlib.image as img
 import numpy as np
 import gdspy
 import cv2
-from prefab.processor import pad, trim, binarize_hard
+from prefab.processor import pad, binarize_hard
 
 
 def load_device_img(path: str, device_length: int) -> np.ndarray:
     """Loads a device in from an image file.
 
     A device is loaded from an image file and processed to prepare for
     prediction. Processing includes scaling, binarization, and padding.
@@ -20,19 +20,17 @@
             be predicted.
 
     Returns:
         A numpy matrix representing the shape of a loaded device prepared for
         prediction.
     """
     device = img.imread(path)[:, :, 1]
-    device = trim(device)
     scale = device_length/device.shape[1]
     device = cv2.resize(device, (0, 0), fx=scale, fy=scale)
     device = binarize_hard(device)
-    device = pad(device, slice_length=128, padding=2)
     return device
 
 
 def load_device_gds(path: str, cell_name: str,
                     coords: list[list[int]] = None) -> np.ndarray:
     """Loads a device in from a GDSII layout file.
 
@@ -73,7 +71,43 @@
                         int(coords[1][1] - bounds[0][1]),
                         int(coords[0][0] - bounds[0][0]):
                         int(coords[1][0] - bounds[0][0])]
 
     device = np.flipud(device)
     device = pad(device, slice_length=128, padding=2)
     return device
+
+def device_to_cell(device: np.ndarray, cell_name: str,
+                   library: gdspy.GdsLibrary, res: float, layer: int = 1) \
+                    -> gdspy.Cell:
+    """Converts a device to a gdspy cell (for GDSII export).
+
+    Args:
+        device: A numpy matrix representing the shape of a device.
+        cell_name: A str indicating the name of the cell to be created.
+        library: A gdspy library for the cell to be added to.
+        res: A float indicating the resolution (in pixels/nm) of the device.
+        layer: An int indicating the GDSII layer to be used.
+
+    Returns:
+        A gdspy cell representing the GDSII layout of a device.
+    """
+    device = np.flipud(device)
+    contours = cv2.findContours(device.astype(np.uint8), 2, 1)
+
+    outers = []
+    inners = []
+    for idx, contour in enumerate(contours[0]):
+        if len(contour) > 2:
+            contour = contour/1000  # μm to nm
+            points = contour.squeeze().tolist()
+            points = list(tuple(sub) for sub in points)
+            if contours[1][0][idx][3] == -1:
+                outers.append(points)
+            else:
+                inners.append(points)
+
+    poly = gdspy.boolean(outers, inners, 'xor', layer=layer)
+    poly = poly.scale(res, res)
+    cell = library.new_cell(cell_name)
+    cell.add(poly)
+    return cell
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prefab-0.2.5/prefab/predictor.py` & `prefab-0.2.6/prefab/predictor.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 import base64
 import numpy as np
 import requests
 import cv2
 from prefab.processor import binarize
 
 
-def predict(device: np.ndarray, model_name: str, step_length: int = 64,
+def predict(device: np.ndarray, model_name: str, model_num: str,
             binary: bool = False) -> np.ndarray:
     """Makes a complete prediction of a device.
 
     A prediction is made by sending an image of a device to a cloud
     function that inferences the model. If the model is a corrector (i.e.,
     self.model_type = 'c'), the result can be interpreted as a correction
     instead.
 
     Args:
         device: A binary numpy matrix representing the shape of a device.
-        model_type: A string indicating the name of the model. See
+        model_name: A string indicating the name of the model. See
+            documentation for names of available models.
+        model_num: A string indicating the number of the model. See
             documentation for names of available models.
-        step_length: An integer indicating the step length (in pixels) for
-            slicing. A smaller step length results in a more accurate
-            prediction, as feature is predicted from multiple perspectives.
         binary: A bool indicating if the prediction will be binarized.
 
     Returns:
         A numpy matrix representing the shape of a predicted device. Pixel
         values closer to 1 indicate high core material likeliness, while
         pixel values closer to 0 indicate high cladding material
         likeliness. Inbetween pixel values indicate uncertainty in the
@@ -36,16 +35,15 @@
     """
     function_url = 'https://prefab-photonics--predict.modal.run'
 
     device_img = cv2.imencode('.png', 255*device)[1].tobytes()
     device_img_base64 = base64.b64encode(device_img).decode('utf-8')
     predict_data = {'device': device_img_base64,
                     'model_name': model_name,
-                    'step_length': step_length,
-                    'model_num': 0}
+                    'model_num': model_num}
 
     prediction_img_base64 = requests.post(function_url, json=predict_data,
                                           timeout=200)
 
     prediction_img_data = base64.b64decode(prediction_img_base64.json())
     prediction_img = np.frombuffer(prediction_img_data, np.uint8)
     prediction = cv2.imdecode(prediction_img, 0)/255
```

### Comparing `prefab-0.2.5/prefab/processor.py` & `prefab-0.2.6/prefab/processor.py`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/LICENSE` & `prefab-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefab-0.2.5/README.md` & `prefab-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 `PreFab` also makes automatic corrections to device designs so that the fabricated outcome is closer to the nominal design. Less structural variation generally means less performance degradation from simulation to experiment.
 
 ![Example of PreFab correction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_c.png?raw=true) *Corrected fabrication of a star structure on a silicon-on-insulator e-beam lithography process.*
 
 ## Models
 
-Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available:
+Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available (see full list on [`docs/models.md`](docs/models.md)):
 
-| Foundry | Process | Latest Version (Date) | Type | Status | Name | Usage|
-| --- | ------- | --------------- | --------- | ----- | ---------------- | ---|
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Predictor | Beta | p_ANT_NanoSOI_v4 | Open |
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Corrector | Beta | c_ANT_NanoSOI_v4 | Open |
+| Foundry | Process | Latest Version | Latest Dataset | Type | Full Name | Status | Usage |
+| ------- | ------- | -------------- | -------------- | ---- | --------- |------- | ----- |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Predictor | p_ANT_NanoSOI_v5_d4 | Beta | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Corrector | c_ANT_NanoSOI_v5_d4 | Beta | Open |
 
 *This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
 
 ## Installation
 
 ### Local
```

### Comparing `prefab-0.2.5/pyproject.toml` & `prefab-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "prefab"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     {name = "Dusan Gostimirovic", email="dusan@prefabphotonics.com"},
 ]
 keywords = ["photonics", "nanofabrication", "machine learning", "layout"]
 description = "Machine learning based prediction of photonic device fabrication"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `prefab-0.2.5/PKG-INFO` & `prefab-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab
-Version: 0.2.5
+Version: 0.2.6
 Summary: Machine learning based prediction of photonic device fabrication
 Project-URL: Homepage, https://github.com/PreFab-Photonics/PreFab
 Author-email: Dusan Gostimirovic <dusan@prefabphotonics.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -537,20 +537,20 @@
 
 `PreFab` also makes automatic corrections to device designs so that the fabricated outcome is closer to the nominal design. Less structural variation generally means less performance degradation from simulation to experiment.
 
 ![Example of PreFab correction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_c.png?raw=true) *Corrected fabrication of a star structure on a silicon-on-insulator e-beam lithography process.*
 
 ## Models
 
-Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available:
+Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available (see full list on [`docs/models.md`](docs/models.md)):
 
-| Foundry | Process | Latest Version (Date) | Type | Status | Name | Usage|
-| --- | ------- | --------------- | --------- | ----- | ---------------- | ---|
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Predictor | Beta | p_ANT_NanoSOI_v4 | Open |
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Corrector | Beta | c_ANT_NanoSOI_v4 | Open |
+| Foundry | Process | Latest Version | Latest Dataset | Type | Full Name | Status | Usage |
+| ------- | ------- | -------------- | -------------- | ---- | --------- |------- | ----- |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Predictor | p_ANT_NanoSOI_v5_d4 | Beta | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Corrector | c_ANT_NanoSOI_v5_d4 | Beta | Open |
 
 *This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
 
 ## Installation
 
 ### Local
```

