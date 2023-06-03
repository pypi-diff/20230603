# Comparing `tmp/weightipy-0.1.1.tar.gz` & `tmp/weightipy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightipy-0.1.1.tar", last modified: Sat Jun  3 15:20:35 2023, max compression
+gzip compressed data, was "weightipy-0.1.2.tar", last modified: Sat Jun  3 20:12:18 2023, max compression
```

## Comparing `weightipy-0.1.1.tar` & `weightipy-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.081215 weightipy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 15:20:26.000000 weightipy-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:26.000000 weightipy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 15:20:35.081215 weightipy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-03 15:20:26.000000 weightipy-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 15:20:35.081215 weightipy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 15:20:26.000000 weightipy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.077215 weightipy-0.1.1/weightipy/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/rim.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/weight_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.081215 weightipy-0.1.1/weightipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 20:12:10.000000 weightipy-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:10.000000 weightipy-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 20:12:18.702582 weightipy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-03 20:12:10.000000 weightipy-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 20:12:18.702582 weightipy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 20:12:10.000000 weightipy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/weightipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26240 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/rim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 20:12:10.000000 weightipy-0.1.2/weightipy/weight_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:12:18.702582 weightipy-0.1.2/weightipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 20:12:18.000000 weightipy-0.1.2/weightipy.egg-info/top_level.txt
```

### Comparing `weightipy-0.1.1/LICENSE.txt` & `weightipy-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.1/PKG-INFO` & `weightipy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.1
+Version: 0.1.2
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
```

### Comparing `weightipy-0.1.1/README.md` & `weightipy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.1/setup.py` & `weightipy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             if lib in versions.keys() else lib
             for lib in libs]
 
 
 INSTALL_REQUIRES = version_libs(libs, precisions, versions)
 
 setup(name='weightipy',
-      version='0.1.1',
+      version='0.1.2',
       author='Remi Sebastian Kits',
       author_email='kaitumisuuringute.keskus@gmail.com',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       install_requires=INSTALL_REQUIRES,
       long_description=long_description,
       long_description_content_type='text/markdown'
```

### Comparing `weightipy-0.1.1/weightipy/__init__.py` & `weightipy-0.1.2/weightipy/__init__.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.1/weightipy/rim.py` & `weightipy-0.1.2/weightipy/rim.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,16 @@
         self._df[self._weight_name()].replace(-1.00, np.NaN, inplace=True)
         if list(self._group_targets.keys()):
             self._adjust_groups()
         if self.total > 0 and not list(self._group_targets.keys()):
             self._scale_total()
         for group in self.groups:
             filter_def = self.groups[group][self._FILTER_DEF]
+            if "summary" not in self.groups[group]['report']:
+                break
             try:
                 if filter_def is not None:
                     self.groups[group]['report']['summary']['Total: weighted'] = \
                     self._df.query(filter_def)[self._weight_name()].sum()
                     self.groups[group]['report']['summary']['Total: unweighted'] = \
                     self._df.query(filter_def)[self._weight_name()].count()
                 else:
@@ -617,9 +619,10 @@
             if diff_error > 0.001:
                 print("Raking achieved only partial convergence, please check the results to ensure that sufficient convergence was achieved.")
                 print("No improvement was apparent after %s iterations" % iteration)
             else:
                 if self.verbose:
                     print('Raking converged in %s iterations' % iteration)
                     print('Generating report')
-                    self.generate_report()
+        if self.verbose:
+            self.generate_report()
         return self.iteration_counter
```

### Comparing `weightipy-0.1.1/weightipy/weight_engine.py` & `weightipy-0.1.2/weightipy/weight_engine.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.1/weightipy.egg-info/PKG-INFO` & `weightipy-0.1.2/weightipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.1
+Version: 0.1.2
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
```

