# Comparing `tmp/weightipy-0.1.2.tar.gz` & `tmp/weightipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightipy-0.1.2.tar", last modified: Sat Jun  3 20:12:18 2023, max compression
+gzip compressed data, was "weightipy-0.2.0.tar", last modified: Sat Jun  3 20:46:39 2023, max compression
```

## Comparing `weightipy-0.1.2.tar` & `weightipy-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 20:12:10.000000 weightipy-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:10.000000 weightipy-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 20:12:18.702582 weightipy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-03 20:12:10.000000 weightipy-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 20:12:18.702582 weightipy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 20:12:10.000000 weightipy-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/weightipy/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26240 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/rim.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/weight_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/weightipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 20:46:28.000000 weightipy-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:28.000000 weightipy-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-03 20:46:39.924743 weightipy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 20:46:28.000000 weightipy-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 20:46:39.924743 weightipy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 20:46:28.000000 weightipy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/weightipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26240 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/rim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 20:46:28.000000 weightipy-0.2.0/weightipy/weight_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:46:39.924743 weightipy-0.2.0/weightipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 20:46:39.000000 weightipy-0.2.0/weightipy.egg-info/top_level.txt
```

### Comparing `weightipy-0.1.2/LICENSE.txt` & `weightipy-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.2/PKG-INFO` & `weightipy-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.2
+Version: 0.2.0
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
 
@@ -54,27 +54,46 @@
 If your data hasn't been weighted yet, you can use Weightipy's RIM weighting algorithm.
 
 Assuming we have the variables `gender` and `agecat` we can weight the dataset with these two variables:
 
 ```Python
 import weightipy as wp
 
+targets = {
+    "agecat": {"18-24": 5.0, "25-34": 30.0, "35-49": 26.0, "50-64": 19.0, "65+": 20.0},
+    "gender": {"Male": 49, "Female": 51}
+}
+scheme = wp.scheme_from_dict(targets)
+
+df_weighted = wp.weight_dataframe(
+    df=my_df,
+    scheme=scheme,
+    weight_column="weights"
+)
+efficiency = wp.weighting_efficiency(df_weighted["weights"])
+```
+
+Or if we want more control of the raking process, we can use the Rim class directly:
+```Python
+import weightipy as wp
+
 age_targets = {'agecat':{1:5.0, 2:30.0, 3:26.0, 4:19.0, 5:20.0}}
 gender_targets = {'gender':{0:49, 1:51}}
 scheme = wp.Rim('gender_and_age')
 scheme.set_targets(targets=[age_targets, gender_targets])
 
 df_weighted = wp.weight_dataframe(
     df=my_df,
     scheme=scheme,
     weight_column="weights"
 )
 efficiency = wp.weighting_efficiency(df_weighted["weights"])
-
 ```
+
+
 Or by using the underlying functions that will give more access to reports etc:
 ```Python
 ...
 
 my_df["identity"] = range(len(my_df))
 engine = wp.WeightEngine(data=df)
 engine.add_scheme(scheme=scheme, key="identity", verbose=False)
```

### Comparing `weightipy-0.1.2/README.md` & `weightipy-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,27 +46,46 @@
 If your data hasn't been weighted yet, you can use Weightipy's RIM weighting algorithm.
 
 Assuming we have the variables `gender` and `agecat` we can weight the dataset with these two variables:
 
 ```Python
 import weightipy as wp
 
+targets = {
+    "agecat": {"18-24": 5.0, "25-34": 30.0, "35-49": 26.0, "50-64": 19.0, "65+": 20.0},
+    "gender": {"Male": 49, "Female": 51}
+}
+scheme = wp.scheme_from_dict(targets)
+
+df_weighted = wp.weight_dataframe(
+    df=my_df,
+    scheme=scheme,
+    weight_column="weights"
+)
+efficiency = wp.weighting_efficiency(df_weighted["weights"])
+```
+
+Or if we want more control of the raking process, we can use the Rim class directly:
+```Python
+import weightipy as wp
+
 age_targets = {'agecat':{1:5.0, 2:30.0, 3:26.0, 4:19.0, 5:20.0}}
 gender_targets = {'gender':{0:49, 1:51}}
 scheme = wp.Rim('gender_and_age')
 scheme.set_targets(targets=[age_targets, gender_targets])
 
 df_weighted = wp.weight_dataframe(
     df=my_df,
     scheme=scheme,
     weight_column="weights"
 )
 efficiency = wp.weighting_efficiency(df_weighted["weights"])
-
 ```
+
+
 Or by using the underlying functions that will give more access to reports etc:
 ```Python
 ...
 
 my_df["identity"] = range(len(my_df))
 engine = wp.WeightEngine(data=df)
 engine.add_scheme(scheme=scheme, key="identity", verbose=False)
```

### Comparing `weightipy-0.1.2/setup.py` & `weightipy-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             if lib in versions.keys() else lib
             for lib in libs]
 
 
 INSTALL_REQUIRES = version_libs(libs, precisions, versions)
 
 setup(name='weightipy',
-      version='0.1.2',
+      version='0.2.0',
       author='Remi Sebastian Kits',
       author_email='kaitumisuuringute.keskus@gmail.com',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       install_requires=INSTALL_REQUIRES,
       long_description=long_description,
       long_description_content_type='text/markdown'
```

### Comparing `weightipy-0.1.2/weightipy/rim.py` & `weightipy-0.2.0/weightipy/rim.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.2/weightipy/weight_engine.py` & `weightipy-0.2.0/weightipy/weight_engine.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.2/weightipy.egg-info/PKG-INFO` & `weightipy-0.2.0/weightipy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.2
+Version: 0.2.0
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
 
@@ -54,27 +54,46 @@
 If your data hasn't been weighted yet, you can use Weightipy's RIM weighting algorithm.
 
 Assuming we have the variables `gender` and `agecat` we can weight the dataset with these two variables:
 
 ```Python
 import weightipy as wp
 
+targets = {
+    "agecat": {"18-24": 5.0, "25-34": 30.0, "35-49": 26.0, "50-64": 19.0, "65+": 20.0},
+    "gender": {"Male": 49, "Female": 51}
+}
+scheme = wp.scheme_from_dict(targets)
+
+df_weighted = wp.weight_dataframe(
+    df=my_df,
+    scheme=scheme,
+    weight_column="weights"
+)
+efficiency = wp.weighting_efficiency(df_weighted["weights"])
+```
+
+Or if we want more control of the raking process, we can use the Rim class directly:
+```Python
+import weightipy as wp
+
 age_targets = {'agecat':{1:5.0, 2:30.0, 3:26.0, 4:19.0, 5:20.0}}
 gender_targets = {'gender':{0:49, 1:51}}
 scheme = wp.Rim('gender_and_age')
 scheme.set_targets(targets=[age_targets, gender_targets])
 
 df_weighted = wp.weight_dataframe(
     df=my_df,
     scheme=scheme,
     weight_column="weights"
 )
 efficiency = wp.weighting_efficiency(df_weighted["weights"])
-
 ```
+
+
 Or by using the underlying functions that will give more access to reports etc:
 ```Python
 ...
 
 my_df["identity"] = range(len(my_df))
 engine = wp.WeightEngine(data=df)
 engine.add_scheme(scheme=scheme, key="identity", verbose=False)
```

