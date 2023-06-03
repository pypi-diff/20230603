# Comparing `tmp/jianglab-0.3.2.tar.gz` & `tmp/jianglab-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.2.tar", last modified: Fri Jun  2 14:35:51 2023, max compression
+gzip compressed data, was "jianglab-0.3.3.tar", last modified: Fri Jun  2 15:30:04 2023, max compression
```

## Comparing `jianglab-0.3.2.tar` & `jianglab-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 14:35:51.014932 jianglab-0.3.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-02 14:35:51.014515 jianglab-0.3.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 14:35:51.010974 jianglab-0.3.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    13436 2023-06-02 14:35:46.000000 jianglab-0.3.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 14:35:51.013651 jianglab-0.3.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-02 14:35:50.000000 jianglab-0.3.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-02 14:35:50.000000 jianglab-0.3.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-02 14:35:50.000000 jianglab-0.3.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-02 14:35:50.000000 jianglab-0.3.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-02 14:35:50.000000 jianglab-0.3.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-02 14:35:51.015076 jianglab-0.3.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-02 14:35:44.000000 jianglab-0.3.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 15:30:04.573621 jianglab-0.3.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-02 15:30:04.573207 jianglab-0.3.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 15:30:04.569867 jianglab-0.3.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    17216 2023-06-02 15:29:13.000000 jianglab-0.3.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-02 15:30:04.572325 jianglab-0.3.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-02 15:30:04.000000 jianglab-0.3.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-02 15:30:04.000000 jianglab-0.3.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-02 15:30:04.000000 jianglab-0.3.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-02 15:30:04.000000 jianglab-0.3.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-02 15:30:04.000000 jianglab-0.3.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-02 15:30:04.573839 jianglab-0.3.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-02 15:29:38.000000 jianglab-0.3.3/setup.py
```

### Comparing `jianglab-0.3.2/PKG-INFO` & `jianglab-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `jianglab-0.3.2/README.md` & `jianglab-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.2/jianglab/common_functions.py` & `jianglab-0.3.3/jianglab/common_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -259,43 +259,120 @@
 def save_instance(filename, instance):
     with open(filename, "wb") as file_:
         pickle.dump(instance, file_, -1)
 
 def load_instance(filename):
     return pickle.load(open(filename, "rb", -1))
 
-def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
-    if arr.shape[0] != 0:
-        counter = 0
-        neighbor_size = np.array(neighbor_size)
-        pad =  (neighbor_size/2).astype(np.int32)
-        arr_pad = np.pad(arr, ((pad[0],pad[0]), (pad[1],pad[1]), (pad[2],pad[2])), 'constant', constant_values = arr.max())
-        arr_pad = arr_pad.astype(np.int32)
-        center_list = []
-        i_range, j_range, k_range = (arr_pad.shape[0]-pad[0]),(arr_pad.shape[1]-pad[1]),(arr_pad.shape[2]-pad[2])
-        #surround_varience = []
-        for i in tqdm(range(0, i_range,1), desc="Roughly find 3d local minimal"):
-            for j in range(j_range):
-                for k in range(k_range):
-                    m,n,p = neighbor_size
+def get_bad_lanes(cmcr_file_path):
+    gsheet = import_gsheet()
+    bad_lanes = cmcr_file_path.split("\\")[-1].replace("-",".").split(".")[:6]
+    bad_lanes = ",".join(bad_lanes)
+    bad_lanes = gsheet[gsheet.File_name.str.contains(bad_lanes)]["Bad_lanes"]
+    bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
+    return bad_lanes
+
+def clean_centers_all_process(arr, neighbour_size = (6,6,6)):
+    def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
+        if arr.shape[0] != 0:
+            counter = 0
+            neighbor_size = np.array(neighbor_size)
+            pad =  (neighbor_size/2).astype(np.int32)
+            arr_pad = np.pad(arr, ((pad[0],pad[0]), (pad[1],pad[1]), (pad[2],pad[2])), 'constant', constant_values = arr.max())
+            arr_pad = arr_pad.astype(np.int32)
+            center_list = []
+            i_range, j_range, k_range = (arr_pad.shape[0]-pad[0]),(arr_pad.shape[1]-pad[1]),(arr_pad.shape[2]-pad[2])
+            #surround_varience = []
+            for i in tqdm(range(0, i_range,1), desc="Roughly find 3d local minimal"):
+                for j in range(j_range):
+                    for k in range(k_range):
+                        m,n,p = neighbor_size
+                        try:
+                            if i >= pad[0] and j >= pad[1] and k >= pad[2]:
+                                surround = arr_pad[i+pad[0]-m:i+pad[0]+m,j+pad[1]-n:j+pad[1]+n,k+pad[2]-p:k+pad[2]+p]
+                                surround[m, n, p] = surround[m, n, p]+1
+                                if np.all(arr_pad[i,j,k] <= surround):
+                                    center_list.append([i-pad[0],j-pad[1],k-pad[2]])
+                                    counter+=1
+                                    # if counter % 100 ==0:
+                                    #     print(i-pad[0],j-pad[1],k-pad[2])
+                                    #     print(counter)
+                                else:
+                                    pass
+                        except OSError as e:
+                            print(e)
+            return np.array(center_list)
+        else:
+            print("Empty input. Detection failed.")
+            return np.array([0,0,0])
+        
+    def remove_close_centers(center_list):
+            new_centers = []
+            for center in tqdm(center_list, desc="Remove close centers "):
+                center_check = True
+                for new_center in new_centers[-1000:]:
                     try:
-                        if i >= pad[0] and j >= pad[1] and k >= pad[2]:
-                            surround = arr_pad[i+pad[0]-m:i+pad[0]+m,j+pad[1]-n:j+pad[1]+n,k+pad[2]-p:k+pad[2]+p]
-                            surround[m, n, p] = surround[m, n, p]+1
-                            if np.all(arr_pad[i,j,k] <= surround):
-                                center_list.append([i-pad[0],j-pad[1],k-pad[2]])
-                                counter+=1
-                                # if counter % 100 ==0:
-                                #     print(i-pad[0],j-pad[1],k-pad[2])
-                                #     print(counter)
+                        if np.abs(new_center[0]-center[0]) <50:
+                            distance = np.linalg.norm(center - new_center)
+                            if distance > np.sqrt(12) and distance != 0:
+                                center_check = center_check and True
                             else:
-                                pass
-                    except OSError as e:
-                        print(e)
-        return np.array(center_list)
-    else:
-        print("Empty input. Detection failed.")
-        return np.array([0,0,0])
+                                center_check = False
+                    except:
+                        print("Fail to reduce center counts")
+                    
+                if center_check == True:
+                    new_centers.append(center)
+            return np.array(new_centers)
+
+    def remove_centers_close_to_edges(center_list):
+        clean_centers = []
+        for center in center_list:
+            if center.shape != ():
+                if center[1] > 2 and center[1] <63 and center [2]>2 and center[2]<63:
+                    clean_centers.append(center)
+        return np.array(clean_centers)
+
+    def remove_isolated_centers(center_list, lp_data):
+            all_check = []
+            clean_centers_2 = []
+            data_mean, data_std = lp_data.mean(), lp_data.std()
+            for center in tqdm(center_list, desc="Remove isolated events "):
+                if center[0] > 12:
+                    surround = lp_data[center[0]-2:center[0]+3,center[1]-1:center[1]+2, center[2]-1:center[2]+2].copy()
+                    surround[:,1,1] = 0
+                    presurround = lp_data[center[0]-12:center[0]-7,center[1]-1:center[1]+2, center[2]-1:center[2]+2].copy()
+                    presurround[:,1,1] = 0
+                    check_surround = (surround.sum()-presurround.sum())/40
+                    all_check.append(check_surround)
+                    if check_surround < data_mean - 2*data_std: #this is an arbitrary number
+                        clean_centers_2.append(center)
+            return np.array(clean_centers_2)
+
+    center_list = find_3d_local_min_general(arr, neighbor_size = neighbour_size)
+    center_list = remove_close_centers(center_list)
+    center_list = remove_centers_close_to_edges(center_list)
+    center_list = remove_isolated_centers(center_list, arr)
+    return center_list
+
+def clean_cmcr_data(cmcr_file_path,
+                    kernel_size = 51,
+                    pre_resample_rate = 100,
+                    post_resample_rate = 10, neighbour_size = (6,6,6)):
+    raw_cmcr_data = load_raw_data(cmcr_file_path)
+    lowpass_data = get_lowpass_data(raw_cmcr_data, 
+                                    pre_resample_rate=pre_resample_rate, 
+                                    post_resample_rate=post_resample_rate, 
+                                    kernel_size=kernel_size
+                                    )
+    bad_lanes = get_bad_lanes(cmcr_file_path)
+    clean_data = remove_bad_lanes(lowpass_data, bad_lanes)
+    clean_centers = clean_centers_all_process(clean_data, 
+                                              neighbour_size = neighbour_size)
+
+    return clean_centers, clean_data
+
+
     
 
 def func3():
     pass
```

### Comparing `jianglab-0.3.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.3.3/jianglab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `jianglab-0.3.2/setup.py` & `jianglab-0.3.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
@@ -25,10 +25,11 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

