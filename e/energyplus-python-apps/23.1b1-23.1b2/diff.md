# Comparing `tmp/energyplus_python_apps-23.1b1.tar.gz` & `tmp/energyplus_python_apps-23.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_python_apps-23.1b1.tar", last modified: Fri Jun  2 21:39:29 2023, max compression
+gzip compressed data, was "energyplus_python_apps-23.1b2.tar", last modified: Fri Jun  2 22:12:23 2023, max compression
```

## Comparing `energyplus_python_apps-23.1b1.tar` & `energyplus_python_apps-23.1b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/energyplus_python_apps/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/energyplus_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      763 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/energyplus_python_apps/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.786191 energyplus_python_apps-23.1b2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/energyplus_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/energyplus_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/energyplus_python_apps/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 22:12:23.786191 energyplus_python_apps-23.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/setup.py
```

### Comparing `energyplus_python_apps-23.1b1/LICENSE.txt` & `energyplus_python_apps-23.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_python_apps-23.1b1/PKG-INFO` & `energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus_python_apps
-Version: 23.1b1
+Name: energyplus-python-apps
+Version: 23.1b2
 Summary: Meta-package collecting all official EnergyPlus Python utilities
 Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus Python Apps
         
         This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
```

### Comparing `energyplus_python_apps-23.1b1/README.md` & `energyplus_python_apps-23.1b2/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_python_apps-23.1b1/energyplus_python_apps/configure.py` & `energyplus_python_apps-23.1b2/energyplus_python_apps/configure.py`

 * *Files identical despite different names*

### Comparing `energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/PKG-INFO` & `energyplus_python_apps-23.1b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus-python-apps
-Version: 23.1b1
+Name: energyplus_python_apps
+Version: 23.1b2
 Summary: Meta-package collecting all official EnergyPlus Python utilities
 Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus Python Apps
         
         This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
```

### Comparing `energyplus_python_apps-23.1b1/setup.py` & `energyplus_python_apps-23.1b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Edwin Lee, for NREL, for United States Department of Energy',
     url='https://github.com/Myoldmopar/EnergyPlusPythonApps',
     license='ModifiedBSD',
     install_requires=[
         'energyplus-launch==3.6.9',
         'energyplus-ruleset-model==0.5',
         'energyplus-transition-tools==2.0.8',
-        'energyplus-pet==0.49',
+        'energyplus-pet==0.50',
         'energyplus-idd-idf-utilities==0.88',
         'energyplus-regressions==2.0.3',
         'energyplus-api-helpers==0.4',
         'energyplus-diff-analysis==0.2',
         # 'energyplus-expand-objects==blah',
         # 'energyplus-epjson-editor==blah',
     ],
```

