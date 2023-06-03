# Comparing `tmp/weightipy-0.1.0.tar.gz` & `tmp/weightipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightipy-0.1.0.tar", last modified: Sun Mar 27 15:59:09 2022, max compression
+gzip compressed data, was "weightipy-0.1.1.tar", last modified: Sat Jun  3 15:20:35 2023, max compression
```

## Comparing `weightipy-0.1.0.tar` & `weightipy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 15:59:09.665205 weightipy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-03-27 15:58:47.000000 weightipy-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-27 15:58:47.000000 weightipy-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2022-03-27 15:59:09.665205 weightipy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-03-27 15:58:47.000000 weightipy-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-27 15:59:09.665205 weightipy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-03-27 15:58:47.000000 weightipy-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 15:59:09.665205 weightipy-0.1.0/weightipy/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-03-27 15:58:47.000000 weightipy-0.1.0/weightipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26127 2022-03-27 15:58:47.000000 weightipy-0.1.0/weightipy/rim.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-27 15:58:47.000000 weightipy-0.1.0/weightipy/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8993 2022-03-27 15:58:47.000000 weightipy-0.1.0/weightipy/weight_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 15:59:09.665205 weightipy-0.1.0/weightipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2022-03-27 15:59:09.000000 weightipy-0.1.0/weightipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-27 15:59:09.000000 weightipy-0.1.0/weightipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 15:59:09.000000 weightipy-0.1.0/weightipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-27 15:59:09.000000 weightipy-0.1.0/weightipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-27 15:59:09.000000 weightipy-0.1.0/weightipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.081215 weightipy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-03 15:20:26.000000 weightipy-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:26.000000 weightipy-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 15:20:35.081215 weightipy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-03 15:20:26.000000 weightipy-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 15:20:35.081215 weightipy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-03 15:20:26.000000 weightipy-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.077215 weightipy-0.1.1/weightipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/rim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-03 15:20:26.000000 weightipy-0.1.1/weightipy/weight_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:20:35.081215 weightipy-0.1.1/weightipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 15:20:35.000000 weightipy-0.1.1/weightipy.egg-info/top_level.txt
```

### Comparing `weightipy-0.1.0/LICENSE.txt` & `weightipy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.0/PKG-INFO` & `weightipy-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.1.1
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
 
-Weightipy is a cut down version of Quantipy for weighting people data using the RIM (raking) algorithm.
+Weightipy is a cut down version of [Quantipy3](https://github.com/Quantipy/quantipy3) for weighting people data using the RIM (iterative raking) algorithm.
 
-### Weightipy for Python 3
-This repository is a modified version of [Quantipy3](https://github.com/Quantipy/quantipy3), that only contains the RIM weighting algorithm of Quantipy3.
+### Planned features
+- Support for multithreaded weighting
+- Support for more weighting algorithms
+- Rewrite of the API to be less oriented towards how Quantipy worked and more in line with simple weighting needs
 
 #### Origins
 - Quantipy was concieved of and instigated by Gary Nelson: http://www.datasmoothie.com
 
 #### Contributors
 - Alexander Buchhammer, Alasdair Eaglestone, James Griffiths, Kerstin Müller : https://yougov.co.uk
 - Datasmoothie’s Birgir Hrafn Sigurðsson and [Geir Freysson](http://www.twitter.com/@geirfreysson): http://www.datasmoothie.com
@@ -110,9 +108,7 @@
 But when developing a specific aspect of Weightipy, it might be quicker to run (e.g. for the DataSet)
 
 `python3 -m unittest tests.test_rim`
 
 Tests for unsupported features are skipped, [see here for what tests are supported](SupportedFeaturesPython3.md).
 
 We welcome volunteers and supporters. Please include a test case with any pull request, especially those that run calculations.
-
-
```

### Comparing `weightipy-0.1.0/README.md` & `weightipy-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Weightipy
 
-Weightipy is a cut down version of Quantipy for weighting people data using the RIM (raking) algorithm.
+Weightipy is a cut down version of [Quantipy3](https://github.com/Quantipy/quantipy3) for weighting people data using the RIM (iterative raking) algorithm.
 
-### Weightipy for Python 3
-This repository is a modified version of [Quantipy3](https://github.com/Quantipy/quantipy3), that only contains the RIM weighting algorithm of Quantipy3.
+### Planned features
+- Support for multithreaded weighting
+- Support for more weighting algorithms
+- Rewrite of the API to be less oriented towards how Quantipy worked and more in line with simple weighting needs
 
 #### Origins
 - Quantipy was concieved of and instigated by Gary Nelson: http://www.datasmoothie.com
 
 #### Contributors
 - Alexander Buchhammer, Alasdair Eaglestone, James Griffiths, Kerstin Müller : https://yougov.co.uk
 - Datasmoothie’s Birgir Hrafn Sigurðsson and [Geir Freysson](http://www.twitter.com/@geirfreysson): http://www.datasmoothie.com
```

### Comparing `weightipy-0.1.0/setup.py` & `weightipy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             if lib in versions.keys() else lib
             for lib in libs]
 
 
 INSTALL_REQUIRES = version_libs(libs, precisions, versions)
 
 setup(name='weightipy',
-      version='0.1.0',
+      version='0.1.1',
       author='Remi Sebastian Kits',
       author_email='kaitumisuuringute.keskus@gmail.com',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       install_requires=INSTALL_REQUIRES,
       long_description=long_description,
       long_description_content_type='text/markdown'
```

### Comparing `weightipy-0.1.0/weightipy/__init__.py` & `weightipy-0.1.1/weightipy/__init__.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.0/weightipy/rim.py` & `weightipy-0.1.1/weightipy/rim.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,9 +617,9 @@
             if diff_error > 0.001:
                 print("Raking achieved only partial convergence, please check the results to ensure that sufficient convergence was achieved.")
                 print("No improvement was apparent after %s iterations" % iteration)
             else:
                 if self.verbose:
                     print('Raking converged in %s iterations' % iteration)
                     print('Generating report')
-        self.generate_report()
+                    self.generate_report()
         return self.iteration_counter
```

### Comparing `weightipy-0.1.0/weightipy/weight_engine.py` & `weightipy-0.1.1/weightipy/weight_engine.py`

 * *Files identical despite different names*

### Comparing `weightipy-0.1.0/weightipy.egg-info/PKG-INFO` & `weightipy-0.1.1/weightipy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: weightipy
-Version: 0.1.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.1.1
 Author: Remi Sebastian Kits
 Author-email: kaitumisuuringute.keskus@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Weightipy
 
-Weightipy is a cut down version of Quantipy for weighting people data using the RIM (raking) algorithm.
+Weightipy is a cut down version of [Quantipy3](https://github.com/Quantipy/quantipy3) for weighting people data using the RIM (iterative raking) algorithm.
 
-### Weightipy for Python 3
-This repository is a modified version of [Quantipy3](https://github.com/Quantipy/quantipy3), that only contains the RIM weighting algorithm of Quantipy3.
+### Planned features
+- Support for multithreaded weighting
+- Support for more weighting algorithms
+- Rewrite of the API to be less oriented towards how Quantipy worked and more in line with simple weighting needs
 
 #### Origins
 - Quantipy was concieved of and instigated by Gary Nelson: http://www.datasmoothie.com
 
 #### Contributors
 - Alexander Buchhammer, Alasdair Eaglestone, James Griffiths, Kerstin Müller : https://yougov.co.uk
 - Datasmoothie’s Birgir Hrafn Sigurðsson and [Geir Freysson](http://www.twitter.com/@geirfreysson): http://www.datasmoothie.com
@@ -110,9 +108,7 @@
 But when developing a specific aspect of Weightipy, it might be quicker to run (e.g. for the DataSet)
 
 `python3 -m unittest tests.test_rim`
 
 Tests for unsupported features are skipped, [see here for what tests are supported](SupportedFeaturesPython3.md).
 
 We welcome volunteers and supporters. Please include a test case with any pull request, especially those that run calculations.
-
-
```

