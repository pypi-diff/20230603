# Comparing `tmp/segmenteverygrain-0.0.1.tar.gz` & `tmp/segmenteverygrain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmenteverygrain-0.0.1.tar", last modified: Thu May 25 16:56:53 2023, max compression
+gzip compressed data, was "segmenteverygrain-0.0.2.tar", last modified: Sat Jun  3 00:23:16 2023, max compression
```

## Comparing `segmenteverygrain-0.0.1.tar` & `segmenteverygrain-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-05-25 16:56:53.707072 segmenteverygrain-0.0.1/
--rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.1/LICENSE.txt
--rw-r--r--   0 zoltan     (502) staff       (20)     3277 2023-05-25 16:56:53.706947 segmenteverygrain-0.0.1/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)     2525 2023-05-25 15:55:20.000000 segmenteverygrain-0.0.1/README.md
--rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-05-25 16:56:33.000000 segmenteverygrain-0.0.1/pyproject.toml
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-05-25 16:56:53.706028 segmenteverygrain-0.0.1/segmenteverygrain/
--rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.1/segmenteverygrain/__init__.py
--rw-r--r--   0 zoltan     (502) staff       (20)    32876 2023-05-24 16:45:06.000000 segmenteverygrain-0.0.1/segmenteverygrain/segmenteverygrain.py
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-05-25 16:56:53.706771 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/
--rw-r--r--   0 zoltan     (502) staff       (20)     3277 2023-05-25 16:56:53.000000 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-05-25 16:56:53.000000 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/SOURCES.txt
--rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-05-25 16:56:53.000000 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/dependency_links.txt
--rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-05-25 16:56:53.000000 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/requires.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-05-25 16:56:53.000000 segmenteverygrain-0.0.1/segmenteverygrain.egg-info/top_level.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-05-25 16:56:53.707112 segmenteverygrain-0.0.1/setup.cfg
--rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-05-25 16:56:47.000000 segmenteverygrain-0.0.1/setup.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.407230 segmenteverygrain-0.0.2/
+-rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.2/LICENSE.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)     4022 2023-06-03 00:23:16.407104 segmenteverygrain-0.0.2/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)     3270 2023-05-29 21:10:25.000000 segmenteverygrain-0.0.2/README.md
+-rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-06-03 00:22:58.000000 segmenteverygrain-0.0.2/pyproject.toml
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.405835 segmenteverygrain-0.0.2/segmenteverygrain/
+-rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.2/segmenteverygrain/__init__.py
+-rw-r--r--   0 zoltan     (502) staff       (20)    31747 2023-06-03 00:06:35.000000 segmenteverygrain-0.0.2/segmenteverygrain/segmenteverygrain.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.406921 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/
+-rw-r--r--   0 zoltan     (502) staff       (20)     4022 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/SOURCES.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/dependency_links.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/requires.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/top_level.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-06-03 00:23:16.407269 segmenteverygrain-0.0.2/setup.cfg
+-rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-06-03 00:22:55.000000 segmenteverygrain-0.0.2/setup.py
```

### Comparing `segmenteverygrain-0.0.1/LICENSE.txt` & `segmenteverygrain-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segmenteverygrain-0.0.1/README.md` & `segmenteverygrain-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+# Segment Every Grain
+
+<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.jpg" width="600">
+
 ## Description
 
-'segment_every_grain' is a Python package that aims to detect grains (or grain-like objects) in images. The goal is to develop an ML model that does a reasonably good job at detecting most of the grains in a photo, so that it will be useful for determining grain size and grain shape, a common task in geomorphology and sedimentary geology. 'segment_every_grain' relies on the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything), developed by Meta, for getting high-quality outlines of the grains. However, SAM requires prompts for every object detected and, when used in 'everything' mode, it tends to be slow and results in many overlapping masks and non-grain (background) objects. To deal with these issues, 'segment_every_grain' relies on a Unet-style, patch-based convolutional neural network to create a first-pass segmentation which is then used as a set of prompts for the SAM-based segmentation. Some of the grains will be missed with this approach, but the segmentations that are created tend to be of high quality. 
+'segmenteverygrain' is a Python package that aims to detect grains (or grain-like objects) in images. The goal is to develop an ML model that does a reasonably good job at detecting most of the grains in a photo, so that it will be useful for determining grain size and grain shape, a common task in geomorphology and sedimentary geology. 'segmenteverygrain' relies on the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything), developed by Meta, for getting high-quality outlines of the grains. However, SAM requires prompts for every object detected and, when used in 'everything' mode, it tends to be slow and results in many overlapping masks and non-grain (background) objects. To deal with these issues, 'segmenteverygrain' relies on a Unet-style, patch-based convolutional neural network to create a first-pass segmentation which is then used as a set of prompts for the SAM-based segmentation. Some of the grains will be missed with this approach, but the segmentations that are created tend to be of high quality. 
+
+'segmenteverygrain' also includes a set of functions that make it possible to clean up the segmentation results: delete and merge objects by clicking on them, and adding grains that were not segmented automatically. The QC-d masks can be saved and added to a dataset of grain images (see the 'images' folder). These images then can be used to improve the Unet model. Many of the images used in the dataset are from the [sedinet](https://github.com/DigitalGrainSize/SediNet) project.
 
-'segment_every_grain' also includes a set of functions that make it possible to clean up the segmentation results: delete and merge objects by clicking on them, and adding grains that were not segmented automatically. The QC-d masks can be saved and added to a dataset of grain images (see the 'images' folder). These images then can be used to improve the Unet model. Some of the images used in the dataset are from the [sedinet](https://github.com/DigitalGrainSize/SediNet) project.
+This is *work in progress*.
 
 
 ## Requirements
 
 - numpy
 - matplotlib
 - scipy
+- pandas
 - pillow
 - scikit-image
 - opencv-python
 - networkx
 - rasterio
 - shapely
 - tensorflow
+- pytorch
 - segment-anything
 - tqdm
 
+## Installation
+
+<code>pip install segmenteverygrain</code>
+
 ## Getting started
 
-See the 'Segment_every_grain.ipynb' notebook for an example of how the models can be loaded and used for segmenting an image and QC-ing the result.
+See the [Segment_every_grain.ipynb](https://github.com/zsylvester/segmenteverygrain/blob/main/segmenteverygrain/Segment_every_grain.ipynb) notebook for an example of how the models can be loaded and used for segmenting an image and QC-ing the result.
+
+The [Train_seg_unet_model.ipynb](https://github.com/zsylvester/segmenteverygrain/blob/main/segmenteverygrain/Train_seg_unet_model.ipynb) notebook goes through the steps needed to create, train, and test the Unet model.
 
-The 'Train_seg_unet_model.ipynb' notebook goes through the steps needed to create, train, and test the Unet model.
+The [Segment_every_grain_colab.ipynb](https://github.com/zsylvester/segmenteverygrain/blob/main/segmenteverygrain/Segment_every_grain_colab.ipynb) has been adjusted so that the segmentation can be tested in Google Colab. That said, the interactivity in Colab is not as smooth as in a local notebook.
 
 ## Acknowledgements
 
 Thanks to Danny Stockli, Nick Howes, Jake Covault, Matt Malkowski, Raymond Luong, and Sergey Fomel for discussions and/or helping with generating training data. Funding for this work came from the [Quantitative Clastics Laboratory industrial consortium](http://www.beg.utexas.edu/qcl) at the Bureau of Economic Geology, The University of Texas at Austin.
 
 ## License
 
-segment_every_grain is licensed under the [Apache License 2.0](https://github.com/zsylvester/meanderpy/blob/master/LICENSE.txt).
+segmenteverygrain is licensed under the [Apache License 2.0](https://github.com/zsylvester/segmenteverygrain/blob/master/LICENSE.txt).
```

### Comparing `segmenteverygrain-0.0.1/pyproject.toml` & `segmenteverygrain-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "segmenteverygrain"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Zoltan Sylvester", email="zoltan.sylvester@beg.utexas.edu" },
 ]
 description = "A SAM-based model for segmenting grains in images of grains"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `segmenteverygrain-0.0.1/segmenteverygrain/segmenteverygrain.py` & `segmenteverygrain-0.0.2/segmenteverygrain/segmenteverygrain.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,46 +3,48 @@
 import sys
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import ListedColormap
 from PIL import Image
 from tqdm import tqdm, trange
+from itertools import combinations
 import cv2
 import networkx as nx
 import rasterio
 from rasterio.features import rasterize
 
 from skimage import measure, morphology
 from skimage.measure import regionprops, regionprops_table
 from skimage.morphology import label, binary_dilation, binary_erosion, reconstruction
 from skimage.segmentation import watershed
 from skimage.io import imread, imshow, concatenate_images
 from skimage.transform import resize
+from skimage.feature import peak_local_max
 
-from shapely.geometry import Polygon, LineString, Point
+from shapely.geometry import Polygon, MultiPolygon, LineString, Point
 from shapely.affinity import scale
+from shapely.ops import unary_union
 import scipy.ndimage as ndi
 import scipy.interpolate
+from sklearn.cluster import DBSCAN
 
 import tensorflow as tf
 from tensorflow.keras.models import Model, load_model
 from tensorflow.keras.layers import Input, BatchNormalization, Activation, Dense, Dropout
 from tensorflow.keras.layers import Lambda, RepeatVector, Reshape
 from tensorflow.keras.layers import Conv2D, Conv2DTranspose
 from tensorflow.keras.layers import MaxPooling2D
 from tensorflow.keras.layers import concatenate, add
 from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, ReduceLROnPlateau
 from tensorflow.keras.optimizers import Adam
 from tensorflow.keras.preprocessing.image import load_img
 
 from segment_anything import sam_model_registry, SamAutomaticMaskGenerator, SamPredictor
 
-
-#  functions for assembling big image from prediction tiles:
 def predict_image_tile(im_tile,model):
     if len(np.shape(im_tile)) == 2:
         im_tile = np.expand_dims(im_tile, 2)
     im_tile = model.predict(np.stack((im_tile, im_tile), axis=0), verbose=0)
     im_tile_pred = im_tile[0] 
     return im_tile_pred
 
@@ -101,69 +103,14 @@
         for layer in range(3):
             big_im_pred[(2*r-2)*I2:2*r*I2, i*I+I2:(i+1)*I+I2, layer] += im_tile_pred[:, :, layer] * Wdown
 
     big_im_pred = big_im_pred[:, I2:-I2, :] # crop the left and right side padding
     big_im_pred = big_im_pred[:-pad_rows, :-pad_cols, :] # get rid of padding
     return big_im_pred
 
-def split_grains(im, selem_size):
-    n_elems = 1
-    eroded = im.copy()
-    while (n_elems<2) & (1 in np.unique(eroded)):
-        selem = np.ones((selem_size,selem_size))
-        eroded = binary_erosion(eroded, footprint = selem)
-        temp_labels, n_elems = measure.label(eroded, return_num = True)
-        obj_features = regionprops(temp_labels)
-        for i in range(len(obj_features)):
-            if obj_features[i]['area'] < 10:
-                eroded[temp_labels==i+1] = 0
-        temp_labels, n_elems = measure.label(eroded, return_num = True)
-        selem_size += 1
-    if np.max(eroded)>0:
-        distance = ndi.distance_transform_edt(eroded)
-        rs = []; cs = []
-        # for i in range(n_elems+1):
-        for i in range(n_elems):
-            dist1 = distance.copy()
-            dist1[temp_labels != i+1] = 0
-            r, c = np.unravel_index(np.argmax(dist1), np.shape(im))
-            rs.append(r)
-            cs.append(c)
-        markers = np.zeros(np.shape(im))
-        # for i in range(n_elems+1):
-        for i in range(n_elems):
-            markers[rs[i],cs[i]] = i+1
-        distance = ndi.distance_transform_edt(im)
-        gr_labels = watershed(-distance, markers, mask=im)
-    else:
-        gr_labels = im.copy()
-    return gr_labels, eroded
-
-def split_all_grains(ind, object_features, filled, labels, selem_size):
-    minrow, mincol, maxrow, maxcol = object_features[ind]["bbox"]
-    im = filled[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2].copy()
-    im[labels[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2] != ind+1] = 0
-    if maxcol >= filled.shape[1]:
-        im = np.hstack((im, np.zeros((im.shape[0],2))))
-    result, eroded = split_grains(im, selem_size)
-    im[result==2] = 2
-    start = time.time()
-    while np.max(result)>1:
-        if len(result[result==2]) > len(result[result==1]):
-            result[result==1] = 0
-            result[result==2] = 1
-        else:
-            result[result==1] = 1
-            result[result==2] = 0
-        result, eroded = split_grains(result, selem_size)
-        im[result==2] = np.max(im)+1
-        if time.time() - start > 1.0: # There are objects where this loop gets stuck. We don't want that.
-            break
-    return im
-
 def compute_curvature(x,y):
     """function for computing first derivatives and curvature of a curve (centerline)
     x,y are cartesian coodinates of the curve
     outputs:
     dx - first derivative of x coordinate
     dy - first derivative of y coordinate
     ds - distances between consecutive points along the curve
@@ -187,177 +134,131 @@
         mrb = poly.minimum_rotated_rectangle
     else:
         minor_axis = np.nan
         major_axis = np.nan
         mrb = None
     return minor_axis, major_axis, mrb
 
-def label_and_dilate_grains(big_im, big_im_pred, small_grain_threshold, dilate_size, selem_size, splitting):
-    # separate objects through labeling image regions
-    boundary = (big_im_pred[:,:,2] > 0.5).astype(np.uint8) # set this to 0.95 to minimize false positives
-    boundary[big_im_pred[:,:,0] > 0.5] = 1 # set this to 0.05 to minimize false positives
-
-    labels, n_labels = label(boundary, background=1, return_num=True) # object labeling
-    object_features = regionprops(labels)
-    object_areas = [objf["area"] for objf in object_features]
-    # find the indices of small objects:
-    small_obj_inds = np.where(np.array(object_areas)<small_grain_threshold)[0]+1
-    count = 0
-    for ind in tqdm(small_obj_inds):  # this can take a long time for a large image!
-        labels[labels == ind] = 0
-        count += 1
-
-    # fill holes:
-    labels[labels>0] = 1
-    seed = np.copy(labels)
-    seed[1:-1, 1:-1] = labels.max()
-    filled = reconstruction(seed, labels, method='erosion')
-
-    labels, n_labels = label(filled, return_num = True) # re-label image
-    object_features = regionprops(labels)
-
-    n_grains = n_labels
-    new_labels = labels.copy() # new labels for split grain clusters
-    if splitting == True:
-        for ind in trange(n_labels):
-            minrow, mincol, maxrow, maxcol = object_features[ind]["bbox"]
-            im = filled[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2].copy()
-            im[labels[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2] != ind+1] = 0
-            if maxcol >= filled.shape[1]:
-              im = np.hstack((im, np.zeros((im.shape[0],2))))
-
-            im = split_all_grains(ind, object_features, filled, labels, selem_size)
-            if np.max(im)>1:
-              for i in range(2,int(np.max(im)+1)):
-                if maxcol >= filled.shape[1]:
-                  im = im[:,:-2]
-                new_labels[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2][im == i] = n_grains+1
-                n_grains += 1
-
-    object_features = regionprops(new_labels)
-
-    new_labels_dilated = new_labels.copy()
-    for ind in trange(len(object_features)):
-        minrow, mincol, maxrow, maxcol = object_features[ind]["bbox"]
-        pad = 20
-        im = new_labels[max(0,minrow-pad):maxrow+pad,max(0,mincol-pad):maxcol+pad].copy()
-        im[new_labels[max(0,minrow-pad):maxrow+pad,max(0,mincol-pad):maxcol+pad] != object_features[ind]["label"]] = 0
-        im[im>0] = 1
-        grain_dist = ndi.distance_transform_edt(1 - im)
-        temp = np.ones(np.shape(im))
-        temp[grain_dist > dilate_size] = 0
-        im = temp
-        im[im==1] = ind+1
-        new_labels_dilated[max(0,minrow-pad):maxrow+pad,max(0,mincol-pad):maxcol+pad][im==ind+1] = im[im==ind+1]
-
-    props = regionprops_table(new_labels_dilated, intensity_image = big_im, properties=('label', 'area', 'centroid', 'major_axis_length', 'minor_axis_length', 
-                                                                                        'orientation', 'perimeter', 'max_intensity', 'mean_intensity', 'min_intensity'))
+def label_grains(big_im, big_im_pred, dbs_max_dist=20.0):
+    grains = big_im_pred[:,:,1].copy() # grain prediction
+    grains[grains >= 0.5] = 1
+    grains[grains < 0.5] = 0
+    grains = grains.astype('bool')
+    labels_simple, n_elems = measure.label(grains, return_num = True, connectivity=1)
+    props = regionprops_table(labels_simple, intensity_image = big_im, properties=('label', 'area', 'centroid', 'major_axis_length', 'minor_axis_length', 
+                                                                                    'orientation', 'perimeter', 'max_intensity', 'mean_intensity', 'min_intensity'))
+    grain_data_simple = pd.DataFrame(props)
+    coords_simple = np.vstack((grain_data_simple['centroid-1'], grain_data_simple['centroid-0'])).T # use the centroids of the unet grains as 'simple' prompts'
+    coords_simple = coords_simple.astype('int32')
+    background_probs = big_im_pred[:,:,0][coords_simple[:,1], coords_simple[:,0]]
+    inds = np.where(background_probs < 0.3)[0] # get rid of prompts that are likely to be background
+    coords_simple = coords_simple[inds, :]
+
+    bounds = big_im_pred[:,:,2].copy() # grain boundary prediction
+    bounds[bounds >= 0.5] = 1
+    bounds[bounds < 0.5] = 0
+    bounds = bounds.astype('bool')
+    temp_labels, n_elems = measure.label(bounds, return_num = True, connectivity=1)
+    # Find the object with the largest area:
+    label_counts = np.bincount(temp_labels.ravel())
+    labels = np.where(label_counts > 100)[0][1:]
+    largest_label = np.argmax(label_counts[1:]) + 1
+    for label in labels:
+        temp_labels[temp_labels == label] = largest_label
+    bounds[temp_labels != largest_label] = 0
+    bounds = bounds-1
+    bounds[bounds < 0] = 1
+    bounds = bounds.astype('bool')
+    distance = ndi.distance_transform_edt(bounds)
+    coords = peak_local_max(distance, footprint=np.ones((3, 3)), labels=bounds.astype('bool'))
+    background_probs = big_im_pred[:,:,0][coords[:,0], coords[:,1]]
+    inds = np.where(background_probs < 0.3)[0]
+    coords = coords[inds, :]
+    mask = np.zeros(distance.shape, dtype=bool)
+    mask[tuple(coords.T)] = True
+    markers, _ = ndi.label(mask)
+    labels = watershed(-distance, markers, mask=bounds)
+    props = regionprops_table(labels, intensity_image = big_im, properties=('label', 'area', 'centroid', 'major_axis_length', 'minor_axis_length', 
+                                                                                    'orientation', 'perimeter', 'max_intensity', 'mean_intensity', 'min_intensity'))
     grain_data = pd.DataFrame(props)
+    coords = np.vstack((grain_data['centroid-1'].values, grain_data['centroid-0'].values)).T
+    # Create a DBSCAN clustering object
+    dbscan = DBSCAN(eps=dbs_max_dist, min_samples=2)
+    # Fit the data to the DBSCAN object
+    dbscan.fit(np.vstack((grain_data['centroid-1'], grain_data['centroid-0'])).T)
+    # Get the cluster labels for each point (-1 represents noise/outliers)
+    db_labels = dbscan.labels_
+    coords_ws = coords[np.where(db_labels == -1)[0]]
+    for i in np.unique(db_labels):
+        xy = np.mean(coords[np.where(db_labels == i)[0]], axis=0)
+        coords_ws = np.vstack((coords_ws, xy))
+    coords_ws = coords_ws.astype('int32')
+    background_probs = big_im_pred[:,:,0][coords_ws[:,1], coords_ws[:,0]]
+    inds = np.where(background_probs < 0.05)[0]
+    coords_ws = coords_ws[inds, :]
 
-    # print('plotting...')
-    # create colormap with random colors, first color white (for background)
-    # colors = []
-    # for i in range(n_grains):
-    #     l = list(np.random.random(3))
-    #     l.append(1)
-    #     colors.append(l)
-    # colors[0] = [1,1,1,0]
-    # cmap = ListedColormap(colors)
-
-    # xs, ys = create_grain_outlines(big_im, new_labels_dilated)
-
-    # fig = plt.figure(figsize=(30,20))
-    # plt.imshow(big_im, cmap='gray', interpolation=None)
-    # plt.imshow(new_labels_dilated, cmap=cmap, interpolation=None, alpha=0.4);
-    # for i in range(len(grain_data['label'])):
-    #     plt.plot(xs[i], ys[i],'k', linewidth = 1.0)
-    # plt.xticks([])
-    # plt.yticks([])
-    # plt.xlim([0, np.shape(big_im)[1]])
-    # plt.ylim([np.shape(big_im)[0], 0])
-    # plt.tight_layout()
- 
-    return new_labels_dilated, grain_data
-
-def create_grain_outlines(big_im, new_labels_dilated):
-    object_features = regionprops(new_labels_dilated)
-    filled = new_labels_dilated.copy()
-    filled[filled>0] = 1
-    n_grains = len(object_features)
-    xs = []
-    ys = []
-    for ind in range(n_grains):
-        minrow, mincol, maxrow, maxcol = object_features[ind]["bbox"]
-        im = filled[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2].copy()
-        im[new_labels_dilated[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2] != object_features[ind]["label"]] = 0
-        if maxcol >= filled.shape[1]:
-            im = np.hstack((im, np.zeros((im.shape[0],2))))
-        contours = measure.find_contours(im, 0.5)
-        sx = contours[0][:,1]
-        sy = contours[0][:,0]
-        xs.append(sx + mincol - 2 + 0.5)
-        ys.append(sy + minrow - 2 + 0.5)
-    return xs, ys
-
-def compute_s_coordinates(x, y):
-    dx = np.gradient(x) # first derivatives
-    dy = np.gradient(y)   
-    ds = np.sqrt(dx**2+dy**2)
-    s = np.hstack((0,np.cumsum(ds[1:])))
-    return s
-
-def get_grain_curvature(big_im, labels, regions, ind):
-    filled = labels.copy()
-    filled[filled>0] = 1
-    minrow, mincol, maxrow, maxcol = regions[ind].bbox
-    im = filled[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2].copy()
-    im[labels[max(0,minrow-2):maxrow+2,max(0,mincol-2):maxcol+2] != regions[ind]["label"]] = 0
-    if maxcol >= filled.shape[1]:
-        im = np.hstack((im, np.zeros((im.shape[0],2))))
-    contours = measure.find_contours(im, 0.5)
-    x = contours[0][:,1] + mincol - 2 + 0.5
-    y = contours[0][:,0] + minrow - 2 + 0.5
-    s = compute_s_coordinates(x, y)
-    deltas = 1.0
-    tck, u = scipy.interpolate.splprep([x,y],s=20, per=True) 
-    unew = np.linspace(0,1,1+int(np.round(s[-1]/deltas))) # vector for resampling
-    out = scipy.interpolate.splev(unew,tck) # resampling
-    sx, sy = out[0], out[1]
-    curv = compute_curvature(sx,sy)
-    s = compute_s_coordinates(sx, sy)
-    y0, x0 = regions[ind].centroid
-    orientation = regions[ind].orientation
-    x1 = x0 + np.cos(orientation) * 0.5 * regions[ind].minor_axis_length
-    y1 = y0 - np.sin(orientation) * 0.5 * regions[ind].minor_axis_length
-    x2 = x0 - np.sin(orientation) * 0.5 * regions[ind].major_axis_length
-    y2 = y0 - np.cos(orientation) * 0.5 * regions[ind].major_axis_length
-    fig = plt.figure(figsize = (10, 10))
-    ax = fig.add_subplot(111)
-    ax.imshow(big_im[max(0,minrow-10):maxrow+10, max(0,mincol-10):maxcol+10], cmap='gray', extent = [max(0,mincol-10), maxcol+10, maxrow+10, max(0,minrow-10)])
-    # plt.scatter(sx, sy, s=60, c=curv, cmap='bwr_r', vmin = -0.1, vmax = 0.1)
-    plt.plot(sx, sy, 'r', linewidth=2)
-    ax.plot((x0, x1), (y0, y1), '-r', linewidth=1)
-    ax.plot((x0, x2), (y0, y2), '-r', linewidth=1)
-    ax.plot(x0, y0, '.g', markersize=15)
-    plt.xticks([])
-    plt.yticks([])
-    plt.xlim(max(0,mincol-10), maxcol+10)
-    plt.ylim(maxrow+10, max(0,minrow-10))
-    # plt.colorbar();
-    return curv, sx, sy
+    all_coords = np.vstack((coords_ws, coords_simple))
+    return labels_simple, grains, all_coords
 
 def one_point_prompt(x, y, ax, image, predictor):
     input_point = np.array([[x, y]])
     input_label = np.array([1])
     masks, scores, logits = predictor.predict(
         point_coords=input_point,
         point_labels=input_label,
         multimask_output=True,
     )
     ind = np.argmax(scores)
+    if np.sum(masks[ind])/(image.shape[0]*image.shape[1]) > 0.1: # if mask is very large compared to size of the image
+        scores = np.delete(scores, ind)
+        ind = np.argmax(scores)
+    temp_labels, n_elems = measure.label(masks[ind], return_num = True, connectivity=1)
+    if n_elems > 1: # if the mask has more than one element, find the largest one and delete the rest
+        mask = masks[ind]
+        # Find the object with the largest area
+        label_counts = np.bincount(temp_labels.ravel())
+        largest_label = np.argmax(label_counts[1:]) + 1
+        mask[temp_labels != largest_label] = 0
+    else:
+        mask = masks[ind]
+    contours = measure.find_contours(mask, 0.5)
+    sx = contours[0][:,1]
+    sy = contours[0][:,0]
+    r, c = np.shape(mask)
+    if mask[0,0]: # if the mask contains the upper left corner of the image
+        sx = np.hstack((-0.5, sx, -0.5))
+        sy = np.hstack((-0.5, sy, -0.5))
+    if mask[0,-1]: # if the mask contains the upper right corner of the image
+        sx = np.hstack((c-0.5, sx, c-0.5))
+        sy = np.hstack((-0.5, sy, -0.5))
+    if mask[-1,0]: # if the mask contains the lower left corner of the image
+        sx = np.hstack((-0.5, sx, -0.5))
+        sy = np.hstack((r-0.5, sy, r-0.5))
+    if mask[-1,-1]: # if the mask contains the lower right corner of the image
+        sx = np.hstack((c-0.5, sx, c-0.5))
+        sy = np.hstack((r-0.5, sy, r-0.5))
+    if np.any(mask[0, :]) and np.any(mask[:, -1]) and not mask[0, -1] \
+        or np.any(mask[0, :]) and np.any(mask[:, 0]) and not mask[0, 0] \
+        or np.any(mask[-1, :]) and np.any(mask[:, 0]) and not mask[-1, 0] \
+        or np.any(mask[-1, :]) and np.any(mask[:, -1]) and not mask[-1, -1]:
+        sx = np.hstack((contours[0][:,1], contours[1][:,1]))
+        sy = np.hstack((contours[0][:,0], contours[1][:,0]))
+    color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
+    ax.fill(sx, sy, facecolor=color, edgecolor='k', alpha=0.5)
+    return sx, sy, mask
+
+def multi_point_prompt(x, y, ax, image, predictor):
+    input_point = np.array([[x, y]])
+    input_label = np.array([1])
+    masks, scores, logits = predictor.predict(
+        point_coords=input_point,
+        point_labels=input_label,
+        multimask_output=True,
+    )
+    ind = np.argmax(scores)
     if np.sum(masks[ind])/(image.shape[0]*image.shape[1]) > 0.1:
         scores = np.delete(scores, ind)
         ind = np.argmax(scores)
     contours = measure.find_contours(masks[ind], 0.5)
     sx = contours[0][:,1]
     sy = contours[0][:,0]
     r, c = np.shape(masks[ind])
@@ -369,14 +270,20 @@
         sy = np.hstack((-0.5, sy, -0.5))
     if masks[ind][-1,0]: # if the mask contains the lower left corner of the image
         sx = np.hstack((-0.5, sx, -0.5))
         sy = np.hstack((r-0.5, sy, r-0.5))
     if masks[ind][-1,-1]: # if the mask contains the lower right corner of the image
         sx = np.hstack((c-0.5, sx, c-0.5))
         sy = np.hstack((r-0.5, sy, r-0.5))
+    if np.any(mask[0, :]) and np.any(mask[:, -1]) and not mask[0, -1] \
+        or np.any(mask[0, :]) and np.any(mask[:, 0]) and not mask[0, 0] \
+        or np.any(mask[-1, :]) and np.any(mask[:, 0]) and not mask[-1, 0] \
+        or np.any(mask[-1, :]) and np.any(mask[:, -1]) and not mask[-1, -1]:
+        sx = np.hstack((contours[0][:,1], contours[1][:,1]))
+        sy = np.hstack((contours[0][:,0], contours[1][:,0]))
     color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
     ax.fill(sx, sy, facecolor=color, edgecolor='k', alpha=0.5)
     return sx, sy, masks[ind]
 
 def two_point_prompt(x1, y1, x2, y2, ax, image, predictor):
     input_point = np.array([[x1, y1], [x2, y2]])
     input_label = np.array([1, 0])
@@ -395,30 +302,25 @@
     color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
     ax.fill(sx, sy, facecolor=color, edgecolor='k', alpha=0.5)
     return sx, sy
 
 def find_overlapping_polygons(polygons, min_overlap_area):
     overlapping_polygons = []
     overlap_areas = []
-    polys_to_be_removed = []
+    # polys_to_be_removed = []
     for i, poly1 in tqdm(enumerate(polygons)):
         for j, poly2 in enumerate(polygons):
             if not poly1.is_valid:
                 poly1 = poly1.buffer(0)
             if not poly2.is_valid:
                 poly2 = poly2.buffer(0)
             if i != j and poly1.intersects(poly2) and poly1.intersection(poly2).area > min_overlap_area:
-                if poly1.contains(poly2):
-                    polys_to_be_removed.append(j)
-                elif poly2.contains(poly1):
-                    polys_to_be_removed.append(i)
-                else:
-                    overlapping_polygons.append((i, j))
-                    overlap_areas.append(poly1.intersection(poly2).area)
-    return overlapping_polygons, overlap_areas, polys_to_be_removed
+                overlapping_polygons.append((i, j))
+                overlap_areas.append(poly1.intersection(poly2).area)
+    return overlapping_polygons, overlap_areas #, polys_to_be_removed
 
 def Unet():
     tf.keras.backend.clear_session()
 
     image = tf.keras.Input((256, 256, 3), name='input')
     
     conv1 = Conv2D(16, (3,3), activation='relu', padding = 'same')(image)
@@ -497,91 +399,88 @@
     ax3 = fig.add_subplot(133)
     ax3.imshow(img)
     ax3.imshow(label[:,:,0], alpha=0.3, cmap='Reds')
     ax3.set_title("Blending")
     ax3.set_xticks([])
     ax3.set_yticks([])
 
-def sam_segmentation(sam, big_im, big_im_pred, grain_data):
+def calculate_iou(poly1, poly2):
+    intersection_area = poly1.intersection(poly2).area
+    union_area = poly1.union(poly2).area
+    iou = intersection_area / union_area
+    return iou
+
+def pick_most_similar_polygon(polygons):
+    # Calculate the average IoU for each polygon
+    avg_iou_scores = []
+    for i, poly1 in enumerate(polygons):
+        iou_scores = []
+        for j, poly2 in enumerate(polygons):
+            if i != j:
+                iou_scores.append(calculate_iou(poly1, poly2))
+        avg_iou_scores.append(sum(iou_scores) / len(iou_scores))
+    # Find the polygon with the highest average IoU score
+    most_similar_index = avg_iou_scores.index(max(avg_iou_scores))
+    most_similar_polygon = polygons[most_similar_index]
+    return most_similar_polygon
+
+def sam_segmentation(sam, big_im, big_im_pred, coords, labels, min_area):
     predictor = SamPredictor(sam)
     predictor.set_image(big_im)
     fig, ax = plt.subplots(figsize=(15,10))
     ax.imshow(big_im) #, alpha=0.5)
     all_grains = []
     masks = []
-    for i in trange(len(grain_data['centroid-1'])):
-        x = grain_data['centroid-1'].iloc[i]
-        y = grain_data['centroid-0'].iloc[i]
+    for i in trange(len(coords[:,0])):
+        x = coords[i,0]
+        y = coords[i,1]
         sx, sy, mask = one_point_prompt(x, y, ax, big_im, predictor)
-        if np.mean(big_im_pred[:,:,0][mask]) < 0.3: # skip masks that are mostly background
-        # skip masks that hvae too much background:
-        # if np.sum(big_im_pred[:,:,0][mask])/(np.sum(big_im_pred[:,:,1][mask]) + \
-        #                                      np.sum(big_im_pred[:,:,2][mask])) < 0.3:
-            all_grains.append(Polygon(np.vstack((sx, sy)).T))
+        labels_per_mask = len(np.unique(labels[mask]))
+        if (labels_per_mask < 10) and (np.mean(big_im_pred[:,:,0][mask]) < 0.7): # skip masks that are mostly background
+            poly = Polygon(np.vstack((sx, sy)).T)
+            if not poly.is_valid:
+                poly = poly.buffer(0)
+            all_grains.append(poly)
             masks.append(mask)
     ax.clear()
-    overlap_threshold = 20
-    min_area = 20
     r = big_im.shape[0]
     c = big_im.shape[1]
-    overlapping_polygons, overlap_areas, polys_to_be_removed = find_overlapping_polygons(all_grains, overlap_threshold)
+    overlapping_polygons, overlap_areas = find_overlapping_polygons(all_grains, min_overlap_area=min_area)
     g = nx.Graph(overlapping_polygons)
     comps = list(nx.connected_components(g))
     connected_grains = set()
     for comp in comps:
         connected_grains.update(comp)
-    for j in trange(len(comps)):
-        # j = 0
-        comb_masks_all = np.zeros((big_im.shape[0], big_im.shape[1]))
-        count = 1
+    new_grains = []
+    for i in range(len(all_grains)): # first collect the objects that do not overlap each other
+        if i not in connected_grains and all_grains[i].area > min_area:
+            if not all_grains[i].is_valid:
+                all_grains[i] = all_grains[i].buffer(0)
+            new_grains.append(all_grains[i])
+    for j in trange(len(comps)): # second deal with the overlapping objects, one connected component at a time
+        polygons = [] # polygons in the connected component
         for i in comps[j]:
-            comb_masks_all += masks[i]*count
-            count += 1
-        if len(np.unique(comb_masks_all)) < 100:
-            for i in np.unique(comb_masks_all):
-                if i != 0:
-                    if len(comb_masks_all[comb_masks_all == i]) > overlap_threshold:
-                        new_mask = np.zeros(np.shape(comb_masks_all))
-                        new_mask[comb_masks_all == i] = 1
-                        # Label the objects in the binary image
-                        labeled_image, num_labels = measure.label(new_mask, return_num=True)
-                        # Find the object with the largest area
-                        label_counts = np.bincount(labeled_image.ravel())
-                        largest_label = np.argmax(label_counts[1:]) + 1
-                        new_mask[labeled_image != largest_label] = 0
-                        # Define a disk-shaped structuring element with radius 3
-                        selem = morphology.disk(3)
-                        # Erode the image using the structuring element
-                        new_mask = morphology.binary_erosion(new_mask, selem)
-                        # Dilate the eroded image using the same structuring element
-                        new_mask = morphology.binary_dilation(new_mask, selem)
-                        if np.max(new_mask):
-                            contours = measure.find_contours(new_mask, 0.5)
-                            sx = contours[0][:,1]
-                            sy = contours[0][:,0]
-                            if new_mask[0,0]:
-                                sx = np.hstack((-0.5, sx, -0.5))
-                                sy = np.hstack((-0.5, sy, -0.5))
-                            if new_mask[0,-1]:
-                                sx = np.hstack((c-0.5, sx, c-0.5))
-                                sy = np.hstack((-0.5, sy, -0.5))
-                            if new_mask[-1,0]:
-                                sx = np.hstack((-0.5, sx, -0.5))
-                                sy = np.hstack((r-0.5, sy, r-0.5))
-                            if new_mask[-1,-1]:
-                                sx = np.hstack((c-0.5, sx, c-0.5))
-                                sy = np.hstack((r-0.5, sy, r-0.5))
-                            all_grains.append(Polygon(np.vstack((sx, sy)).T))                       
-    all_grains_new = []
-    for i in range(len(all_grains)):
-        if i not in connected_grains and all_grains[i].area > min_area and i not in polys_to_be_removed:
-            all_grains_new.append(all_grains[i])
-    all_grains = all_grains_new
-    ax.imshow(big_im)
-    # create labeled image
+            polygons.append(all_grains[i])
+        most_similar_polygon = pick_most_similar_polygon(polygons)
+        if most_similar_polygon.area > min_area:
+            new_grains.append(most_similar_polygon)
+        poly_union = unary_union(polygons)
+        remaining_polys = poly_union.difference(most_similar_polygon) # subtract the most similar polygon from the union of all polygons
+        poly_areas = []
+        if type(remaining_polys) == MultiPolygon:
+            for geom in remaining_polys.geoms:
+                poly_areas.append(geom.area)
+            inds = np.where(np.array(poly_areas) > min_area)[0]
+            for ind in inds:
+                new_grains.append(remaining_polys.geoms[ind])
+        if type(remaining_polys) == Polygon:
+            if remaining_polys.area > min_area:
+                new_grains.append(remaining_polys)
+    all_grains = new_grains # replace original list of polygons
+    # create labeled image:
     labels = np.zeros(big_im.shape[:-1])
     mask_all = np.zeros(big_im.shape[:-1])
     for i in trange(len(all_grains)):
         mask = rasterize(
             shapes=[all_grains[i]],
             out_shape=big_im.shape[:-1],
             fill=0,
@@ -602,20 +501,17 @@
             all_touched=False,
             default_value=1,
             dtype=None,
         )
         mask_all[mask == 1] = 1
         mask_all[boundary_mask == 1] = 2
         labels[(mask==1) & (labels==0)] = i+1
-    ax.imshow(mask_all, alpha=0.5)  
-    for i in range(len(all_grains)):
-        color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
-        ax.fill(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], 
-                facecolor=color, edgecolor='none', linewidth=0.5, alpha=0.4)
-        # ax.plot(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], 'k', linewidth=0.5)
+    ax.imshow(big_im)
+    plot_image_w_colorful_grains(big_im, all_grains, ax, cmap='Paired')
+    plot_grain_axes_and_centroids(all_grains, labels, ax, linewidth=1, markersize=10)
     plt.xticks([])
     plt.yticks([])
     plt.xlim([0, np.shape(big_im)[1]])
     plt.ylim([np.shape(big_im)[0], 0])
     plt.tight_layout()
     return all_grains, labels, mask_all, fig, ax
 
@@ -635,14 +531,20 @@
     seed = tf.random.experimental.stateless_split(tf.zeros([2], dtype=tf.int32), num=2)[0]
     image = tf.image.stateless_random_brightness(image, max_delta=0.1, seed=seed)
     image = tf.image.stateless_random_contrast(image, lower=0.9, upper=1.1, seed=seed)
     image = tf.image.stateless_random_flip_left_right(image, seed=seed)
     image = tf.image.stateless_random_flip_up_down(image, seed=seed)
     mask = tf.image.stateless_random_flip_left_right(mask, seed=seed)
     mask = tf.image.stateless_random_flip_up_down(mask, seed=seed)
+    # this doesn't work for some reason (validation loss is too high)
+    # if np.random.random() > 0.5: # only do this half the time 
+    #     image = tf.image.stateless_random_crop(image, (128, 128, 3), seed=seed)
+    #     image = tf.image.resize(image, (256, 256))
+    #     mask = tf.image.stateless_random_crop(mask, (128, 128, 3), seed=seed)
+    #     mask = tf.image.resize(mask, (256, 256), method='nearest')
     return image, mask
 
 def onclick(event, ax, coords, image, predictor):
     x, y = event.xdata, event.ydata
     if event.button == 1: # left mouse button for object
         coords.append((x, y))
         sx, sy, mask = one_point_prompt(coords[-1][0], coords[-1][1], ax, image, predictor)
@@ -664,16 +566,14 @@
         poly = Polygon(path1.vertices).union(Polygon(path2.vertices))
         ax.patches[-1].remove()
         ax.patches[-1].remove()
         color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
         ax.fill(poly.exterior.xy[0], poly.exterior.xy[1], facecolor=color, edgecolor='k', alpha=0.5)
         fig.canvas.draw()
 
-# def on_key(event, arg1, arg2, arg3):
-
 def onclick2(event, all_grains, grain_inds, ax):
     x, y = event.xdata, event.ydata
     point = Point(x, y)
     for i in range(len(all_grains)):
         if all_grains[i].contains(point):
             grain_inds.append(i)
             ax.fill(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], color='r', alpha=0.5)
@@ -705,14 +605,28 @@
             all_grains.remove(all_grains[grain_inds[-2]-1])
         all_grains.append(poly)  # add merged polygon to 'all_grains'
         color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
         ax.fill(poly.exterior.xy[0], poly.exterior.xy[1], 
                 facecolor=color, edgecolor='k', linewidth=2, alpha=0.5)
         fig.canvas.draw()
 
+def click_for_scale(event, ax):
+    global x1, x2, y1, y2, dist
+    if event.button == 1: # left mouse button for start point of scale
+        x1, y1 = event.xdata, event.ydata
+        ax.plot(x1, y1, 'ro')
+        ax.figure.canvas.draw()
+    if event.button == 3: # right mouse button for end point of scale
+        x2, y2 = event.xdata, event.ydata
+        ax.plot(x2, y2, 'ro')
+        ax.plot([x1, x2], [y1, y2], 'r')
+        ax.figure.canvas.draw()
+        dist = ((x2 - x1)**2 + (y2 - y1)**2)**0.5
+        print('number of pixels: ' + str(np.round(dist, 2)))
+
 def get_grains_from_patches(ax, image):
     all_grains = []
     for i in range(len(ax.patches)):
         x = ax.patches[i].get_path().vertices[:,0]
         y = ax.patches[i].get_path().vertices[:,1]
         all_grains.append(Polygon(np.vstack((x, y)).T))
         
@@ -743,11 +657,50 @@
             dtype=None,
         )
         mask_all[mask == 1] = 1
         mask_all[boundary_mask == 1] = 2
         labels[(mask==1) & (labels==0)] = i+1
     plt.figure()
     plt.imshow(labels)
-    plt.figure()
-    plt.imshow(image)
-    plt.imshow(mask_all, alpha=0.5)
-    return all_grains, labels, mask_all
+    fig = plt.figure()
+    ax = fig.add_subplot(111)
+    ax.imshow(image)
+    ax.imshow(mask_all, alpha=0.5)
+    for i in range(len(all_grains)):
+        ax.fill(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], 
+                facecolor=(0,0,1), edgecolor='none', linewidth=0.5, alpha=0.4)
+    return all_grains, labels, mask_all, fig, ax
+
+def plot_image_w_colorful_grains(image, all_grains, ax, cmap='viridis'):
+    # Choose a colormap
+    colormap = cmap
+    # Get the colormap object
+    cmap = plt.cm.get_cmap(colormap)
+    # Generate random indices for colors
+    num_colors = len(all_grains)  # Number of colors to choose
+    color_indices = np.random.randint(0, cmap.N, num_colors)
+    # Get the individual colors
+    colors = [cmap(i) for i in color_indices]
+    # fig = plt.figure(figsize=(10,10))
+    # ax = fig.add_subplot(111)
+    ax.imshow(image)
+    for i in range(len(all_grains)):
+        color = colors[i]
+        ax.fill(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], 
+                facecolor=color, edgecolor='none', linewidth=1, alpha=0.4)
+        ax.plot(all_grains[i].exterior.xy[0], all_grains[i].exterior.xy[1], 
+                color='k', linewidth=1)
+    ax.set_xticks([])
+    ax.set_yticks([])
+
+def plot_grain_axes_and_centroids(all_grains, labels, ax, linewidth=1, markersize=10):
+    regions = regionprops(labels.astype('int'))
+    for ind in range(len(all_grains)):
+        y0, x0 = regions[ind].centroid
+        orientation = regions[ind].orientation
+        x1 = x0 + np.cos(orientation) * 0.5 * regions[ind].minor_axis_length
+        y1 = y0 - np.sin(orientation) * 0.5 * regions[ind].minor_axis_length
+        x2 = x0 - np.sin(orientation) * 0.5 * regions[ind].major_axis_length
+        y2 = y0 - np.cos(orientation) * 0.5 * regions[ind].major_axis_length
+        ax.plot((x0, x1), (y0, y1), '-k', linewidth=linewidth)
+        ax.plot((x0, x2), (y0, y2), '-k', linewidth=linewidth)
+        ax.plot(x0, y0, '.k', markersize=markersize)
```

### Comparing `segmenteverygrain-0.0.1/setup.py` & `segmenteverygrain-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """\
 
 """
 
 setuptools.setup(
     name="segmenteverygrain",
-    version="0.0.1",
+    version="0.0.2",
     author="Zoltan Sylvester",
     author_email="zoltan.sylvester@beg.utexas.edu",
     description="a SAM-based model for segmenting grains in images of grains",
     keywords = 'sedimentology, geomorphology, grain size, segment anything model',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zsylvester/segmenteverygrain",
```

