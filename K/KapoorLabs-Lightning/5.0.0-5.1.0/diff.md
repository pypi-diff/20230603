# Comparing `tmp/KapoorLabs-Lightning-5.0.0.tar.gz` & `tmp/KapoorLabs-Lightning-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-ppk3dq1b/KapoorLabs-Lightning-5.0.0.tar", last modified: Fri Jun  2 20:35:22 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-w8gquhdx/KapoorLabs-Lightning-5.1.0.tar", last modified: Sat Jun  3 13:57:46 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.0.0.tar` & `KapoorLabs-Lightning-5.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:22.483291 KapoorLabs-Lightning-5.0.0/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:20.952504 KapoorLabs-Lightning-5.0.0/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:21.195708 KapoorLabs-Lightning-5.0.0/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.0.0/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.0.0/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-02 20:35:22.485890 KapoorLabs-Lightning-5.0.0/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:21.438649 KapoorLabs-Lightning-5.0.0/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-02 20:35:22.495407 KapoorLabs-Lightning-5.0.0/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:20.975080 KapoorLabs-Lightning-5.0.0/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:21.674197 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-02 20:35:20.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:22.313098 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 20:35:22.435033 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-02 20:35:19.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    34976 2023-06-02 19:04:40.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15630 2023-05-27 20:24:35.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1534 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.0.0/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.361976 KapoorLabs-Lightning-5.1.0/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:44.984099 KapoorLabs-Lightning-5.1.0/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.231732 KapoorLabs-Lightning-5.1.0/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.1.0/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.1.0/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-03 13:57:46.363329 KapoorLabs-Lightning-5.1.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.405348 KapoorLabs-Lightning-5.1.0/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-03 13:57:46.372376 KapoorLabs-Lightning-5.1.0/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.008059 KapoorLabs-Lightning-5.1.0/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.637494 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-03 13:57:44.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.202700 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.311787 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    34411 2023-06-03 13:55:57.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15630 2023-05-27 20:24:35.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.0.0/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.1.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/.gitignore` & `KapoorLabs-Lightning-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/LICENSE` & `KapoorLabs-Lightning-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/PKG-INFO` & `KapoorLabs-Lightning-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.0.0
+Version: 5.1.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.0.0/README.md` & `KapoorLabs-Lightning-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/Apache-2` & `KapoorLabs-Lightning-5.1.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/BSD-3` & `KapoorLabs-Lightning-5.1.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/GPL-3` & `KapoorLabs-Lightning-5.1.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/LGPL-3` & `KapoorLabs-Lightning-5.1.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/MIT` & `KapoorLabs-Lightning-5.1.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/licenses/MPL-2` & `KapoorLabs-Lightning-5.1.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/setup.cfg` & `KapoorLabs-Lightning-5.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.0.0
+Version: 5.1.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.0.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,70 +15,65 @@
 from .pytorch_models import CloudAutoEncoder, DeepEmbeddedClustering
 
 
 class LightningData(LightningDataModule):
     def __init__(
         self,
         hparams,
+        num_workers=4,
     ):
         super().__init__()
         self.save_hyperparameters()
-
+        self.num_workers = num_workers
         self.train_val_test_split: float = hparams["train_val_test_split"]
-        self._batch_size: int = hparams["batch_size"]
+        self.batch_size: int = hparams["batch_size"]
         self.dataset: Dataset = hparams["dataset"]
 
-    @property
-    def batch_size(self):
-        return self._batch_size
-
-    @batch_size.setter
-    def batch_size(self, value):
-        self._batch_size = value
-
     def setup(self, stage: str):
         self.train_val_test_split = [
             int(self.train_val_test_split[i] * len(self.dataset) / 100)
             for i in range(len(self.train_val_test_split) - 1)
         ]
         self.train_val_test_split.append(
             len(self.dataset) - sum(self.train_val_test_split)
         )
         print(
-            f"LightningData.setup() called with stage={stage} on dataset of length {len(self.dataset)} with {self.train_val_test_split} split."
+            f"LightningData.setup() called with stage={stage} on dataset of length {len(self.dataset)} with {self.train_val_test_split} split and batch size {self.batch_size}"
         )
         self.data_train, self.data_val, self.data_test = random_split(
             dataset=self.dataset,
             lengths=self.train_val_test_split,
             generator=torch.Generator().manual_seed(42),
         )
 
     def train_dataloader(self):
         return DataLoader(
             self.data_train,
-            batch_size=self._batch_size,
-            num_workers=os.cpu_count() // 3,
+            batch_size=self.batch_size,
+            num_workers=self.num_workers,
         )
 
     def val_dataloader(self):
         return DataLoader(
             self.data_val,
-            batch_size=self._batch_size,
-            num_workers=os.cpu_count() // 3,
+            batch_size=self.batch_size,
+            num_workers=self.num_workers,
         )
 
     def test_dataloader(self):
         return DataLoader(
             self.data_test,
-            batch_size=self._batch_size,
-            num_workers=os.cpu_count() // 3,
+            batch_size=self.batch_size,
+            num_workers=self.num_workers,
         )
 
     def predict_dataloader(self):
-        return DataLoader(self.dataset, batch_size=1)
+        return DataLoader(
+            self.dataset, batch_size=1, num_workers=self.num_workers
+        )
 
     def teardown(self, stage: str):
         # Used to clean-up when the run is finished
         pass
 
 
 class LightningModel(LightningModule):
@@ -406,15 +401,15 @@
     def forward(self, z):
         return self.network(z)
 
     def encoder_loss(self, y_hat, y):
         return self.loss_func(y_hat, y)
 
     def cluster_loss(self, clusters, tar_dist):
-        return self.cluster_loss_func(clusters, tar_dist)
+        return self.cluster_loss_func(torch.log(clusters), tar_dist)
 
     def training_step(self, batch, batch_idx):
         self.compute_device = batch.device
         self.to(self.compute_device)
         self.target_distribution = self._get_target_distribution(
             self.cluster_distribution
         )
@@ -687,14 +682,15 @@
         batch_size: int = 64,
         min_epochs: int = 1,
         epochs: int = 10,
         precision: int = 16,
         accelerator: str = "gpu",
         devices: int = -1,
         strategy: str = "auto",
+        num_workers: int = 4,
         enable_checkpointing: bool = True,
         callbacks: List[Callback] = None,
         scheduler: schedulers = None,
         logger: Logger = None,
         **kwargs,
     ):
         self.dataset = dataset
@@ -729,14 +725,16 @@
 
         self.strategy = strategy
 
         self.min_epochs = min_epochs
 
         self.precision = precision
 
+        self.num_workers = num_workers
+
         self.hparams = {
             "loss_func": self.loss_func,
             "model_func": self.model_func,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
@@ -747,15 +745,17 @@
         self.hparams.update(kwargs=kwargs)
 
     def _train_model(self):
         self.model = LightningModel(
             self.model_func, self.loss_func, self.optim_func, self.scheduler
         )
 
-        self.datas = LightningData(hparams=self.hparams)
+        self.datas = LightningData(
+            hparams=self.hparams, num_workers=self.num_workers
+        )
         self.datas.setup("fit")
         self.default_root_dir = (
             Path(self.model_save_file).absolute().parent.as_posix()
         )
         self.default_root_dir = os.path.join(
             self.default_root_dir, Path(self.model_save_file).stem
         )
@@ -778,33 +778,21 @@
             self.trainer.fit(
                 self.model,
                 train_dataloaders=self.datas.train_dataloader(),
                 val_dataloaders=self.datas.val_dataloader(),
                 ckpt_path=self.ckpt_file,
             )
 
-            self.trainer.validate(
-                model=self.model,
-                dataloaders=self.datas.val_dataloader(),
-                ckpt_path=self.ckpt_file,
-                verbose=True,
-            )
         else:
             self.trainer.fit(
                 self.model,
                 train_dataloaders=self.datas.train_dataloader(),
                 val_dataloaders=self.datas.val_dataloader(),
             )
 
-            self.trainer.validate(
-                model=self.model,
-                dataloaders=self.datas.val_dataloader(),
-                verbose=True,
-            )
-
     def callback_metrics(self):
         return self.trainer.callback_metrics
 
 
 class AutoLightningTrain:
     def __init__(
         self,
@@ -818,14 +806,15 @@
         batch_size: int = 64,
         min_epochs: int = 1,
         epochs: int = 10,
         accelerator: str = "gpu",
         devices: int = -1,
         strategy: str = "auto",
         num_nodes: int = 1,
+        num_workers: int = 4,
         enable_checkpointing: bool = True,
         callbacks: List[Callback] = None,
         scheduler: schedulers = None,
         logger: Logger = None,
         **kwargs,
     ):
         self.dataset = dataset
@@ -860,14 +849,16 @@
 
         self.strategy = strategy
 
         self.min_epochs = min_epochs
 
         self.num_nodes = num_nodes
 
+        self.num_workers = num_workers
+
         self.hparams = {
             "loss_func": self.loss_func,
             "model_func": self.model_func,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
@@ -878,15 +869,17 @@
         self.hparams.update(kwargs=kwargs)
 
     def _train_model(self):
         self.model = AutoLightningModel(
             self.model_func, self.loss_func, self.optim_func, self.scheduler
         )
 
-        self.datas = LightningData(hparams=self.hparams)
+        self.datas = LightningData(
+            hparams=self.hparams, num_workers=self.num_workers
+        )
         self.datas.setup("fit")
         self.default_root_dir = (
             Path(self.model_save_file).absolute().parent.as_posix()
         )
         self.default_root_dir = os.path.join(
             self.default_root_dir, Path(self.model_save_file).stem
         )
@@ -944,14 +937,15 @@
         cluster_loss_func: torch.nn.Module,
         network: DeepEmbeddedClustering,
         optim_func: optimizers._Optimizer,
         model_save_file: str,
         ckpt_file: str = None,
         train_val_test_split: List = [95, 2.5, 2.5],
         gamma: int = 1,
+        num_workers: int = 4,
         batch_size: int = 64,
         min_epochs: int = 1,
         epochs: int = 10,
         accelerator: str = "gpu",
         devices: int = -1,
         strategy: str = "auto",
         num_nodes: int = 1,
@@ -1000,14 +994,16 @@
 
         self.min_epochs = min_epochs
 
         self.num_nodes = num_nodes
 
         self.mem_percent = mem_percent
 
+        self.num_workers = num_workers
+
         self.hparams = {
             "loss_func": self.loss_func,
             "network": self.network,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
@@ -1034,80 +1030,66 @@
             min_epochs=self.min_epochs,
             max_epochs=self.epochs,
             default_root_dir=self.default_root_dir,
             enable_checkpointing=self.enable_checkpointing,
             num_nodes=self.num_nodes,
         )
 
-        self.datas = LightningData(hparams=self.hparams)
+        self.datas = LightningData(
+            hparams=self.hparams, num_workers=self.num_workers
+        )
         self.datas.setup("fit")
         train_dataloaders = self.datas.train_dataloader()
-        val_dataloaders = self.datas.val_dataloader()
-
-        self.datas.batch_size = 1
-        train_dataloaders_inf = self.datas.train_dataloader()
+        predict_loader = self.datas.predict_dataloader()
 
         if self.ckpt_file is None:
             get_kmeans = True
         else:
             get_kmeans = False
         net, cluster_distribution = initialize_repeat_function(
             self.network,
             self.loss_func,
             self.cluster_loss_func,
-            train_dataloaders_inf,
+            predict_loader,
             self.optim_func,
             self.gamma,
             self.mem_percent,
             self.accelerator,
             self.devices,
             kmeans=get_kmeans,
         )
 
         self.model = ClusterLightningModel(
             net,
             self.loss_func,
             self.cluster_loss_func,
             self.optim_func,
-            train_dataloaders_inf,
+            predict_loader,
             cluster_distribution,
             self.accelerator,
             self.devices,
             self.scheduler,
             gamma=self.gamma,
             mem_percent=self.mem_percent,
         )
 
         if self.ckpt_file is not None:
             self.trainer.fit(
                 self.model,
                 train_dataloaders=train_dataloaders,
-                val_dataloaders=val_dataloaders,
                 ckpt_path=self.ckpt_file,
             )
 
-            self.trainer.validate(
-                model=self.model,
-                dataloaders=val_dataloaders,
-                ckpt_path=self.ckpt_file,
-                verbose=True,
-            )
         else:
             self.trainer.fit(
                 self.model,
                 train_dataloaders=self.datas.train_dataloader(),
                 val_dataloaders=self.datas.val_dataloader(),
             )
 
-            self.trainer.validate(
-                model=self.model,
-                dataloaders=self.datas.val_dataloader(),
-                verbose=True,
-            )
-
     def callback_metrics(self):
         return self.trainer.callback_metrics
 
 
 def initialize_repeat_function(
     network,
     loss_func,
```

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,14 +36,20 @@
             transform_list.append(transforms.RandAugment())
 
         if "normalize" in self.aug_str:
             transform_list.append(transforms.ConvertImageDtype(torch.float))
             transform_list.append(
                 transforms.Normalize(mean=self.mean, std=self.std)
             )
+        if "resnet" in self.aug_str:
+            transform_list.append(transforms.Resize((224, 224)))
+            transform_list.append(transforms.ToTensor())
+            transform_list.append(
+                transforms.Normalize(mean=self.mean, std=self.std)
+            )
 
         self.transform = transforms.Compose(transform_list)
 
     def get_transform(self):
         """
         Returns the composed transform.
         """
```

### Comparing `KapoorLabs-Lightning-5.0.0/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.0.0/tox.ini` & `KapoorLabs-Lightning-5.1.0/tox.ini`

 * *Files identical despite different names*

