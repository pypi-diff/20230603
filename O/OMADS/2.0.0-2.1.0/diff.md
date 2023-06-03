# Comparing `tmp/OMADS-2.0.0.tar.gz` & `tmp/OMADS-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMADS-2.0.0.tar", last modified: Sat Jun  3 03:55:10 2023, max compression
+gzip compressed data, was "OMADS-2.1.0.tar", last modified: Sat Jun  3 04:21:42 2023, max compression
```

## Comparing `OMADS-2.0.0.tar` & `OMADS-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 03:55:10.361292 OMADS-2.0.0/
--rw-rw-rw-   0        0        0    35823 2023-01-13 00:51:14.000000 OMADS-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     9183 2023-06-03 03:55:10.361792 OMADS-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8344 2023-06-03 01:09:06.000000 OMADS-2.0.0/README.md
--rw-rw-rw-   0        0        0      533 2023-01-13 00:51:14.000000 OMADS-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      999 2023-06-03 03:55:10.363294 OMADS-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-06-02 04:53:44.000000 OMADS-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:55:10.331293 OMADS-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 03:55:10.348793 OMADS-2.0.0/src/OMADS/
--rw-rw-rw-   0        0        0    18576 2023-06-03 01:05:08.000000 OMADS-2.0.0/src/OMADS/MADS.py
--rw-rw-rw-   0        0        0    80405 2023-06-02 23:43:07.000000 OMADS-2.0.0/src/OMADS/POLL.py
--rw-rw-rw-   0        0        0    51087 2023-06-03 01:04:59.000000 OMADS-2.0.0/src/OMADS/SEARCH.py
--rw-rw-rw-   0        0        0      386 2023-06-02 04:52:36.000000 OMADS-2.0.0/src/OMADS/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-02 04:48:08.000000 OMADS-2.0.0/src/OMADS/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-03 03:55:10.357792 OMADS-2.0.0/src/OMADS.egg-info/
--rw-rw-rw-   0        0        0     9183 2023-06-03 03:55:10.000000 OMADS-2.0.0/src/OMADS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-03 03:55:10.000000 OMADS-2.0.0/src/OMADS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 03:55:10.000000 OMADS-2.0.0/src/OMADS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2023-06-03 03:55:10.000000 OMADS-2.0.0/src/OMADS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 03:55:10.000000 OMADS-2.0.0/src/OMADS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 03:55:10.359793 OMADS-2.0.0/tests/
--rw-rw-rw-   0        0        0     4113 2023-06-03 02:41:49.000000 OMADS-2.0.0/tests/test_OMADS_BASIC.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:21:42.930942 OMADS-2.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-13 00:51:14.000000 OMADS-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9783 2023-06-03 04:21:42.931442 OMADS-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8944 2023-06-03 04:20:46.000000 OMADS-2.1.0/README.md
+-rw-rw-rw-   0        0        0      533 2023-01-13 00:51:14.000000 OMADS-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      999 2023-06-03 04:21:42.932949 OMADS-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-06-03 04:21:01.000000 OMADS-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:21:42.910443 OMADS-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 04:21:42.921943 OMADS-2.1.0/src/OMADS/
+-rw-rw-rw-   0        0        0    18576 2023-06-03 01:05:08.000000 OMADS-2.1.0/src/OMADS/MADS.py
+-rw-rw-rw-   0        0        0    80405 2023-06-02 23:43:07.000000 OMADS-2.1.0/src/OMADS/POLL.py
+-rw-rw-rw-   0        0        0    51087 2023-06-03 01:04:59.000000 OMADS-2.1.0/src/OMADS/SEARCH.py
+-rw-rw-rw-   0        0        0      386 2023-06-02 04:52:36.000000 OMADS-2.1.0/src/OMADS/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 04:48:08.000000 OMADS-2.1.0/src/OMADS/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-03 04:21:42.927941 OMADS-2.1.0/src/OMADS.egg-info/
+-rw-rw-rw-   0        0        0     9783 2023-06-03 04:21:42.000000 OMADS-2.1.0/src/OMADS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-03 04:21:42.000000 OMADS-2.1.0/src/OMADS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 04:21:42.000000 OMADS-2.1.0/src/OMADS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2023-06-03 04:21:42.000000 OMADS-2.1.0/src/OMADS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 04:21:42.000000 OMADS-2.1.0/src/OMADS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 04:21:42.929443 OMADS-2.1.0/tests/
+-rw-rw-rw-   0        0        0     4113 2023-06-03 02:41:49.000000 OMADS-2.1.0/tests/test_OMADS_BASIC.py
```

### Comparing `OMADS-2.0.0/LICENSE` & `OMADS-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OMADS-2.0.0/PKG-INFO` & `OMADS-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMADS
-Version: 2.0.0
+Version: 2.1.0
 Summary: Statistical Learning Models Library
 Home-page: https://github.com/Ahmed-Bayoumy/OMADS
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/OMADS/issues
 Platform: UNKNOWN
@@ -17,22 +17,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
 License-File: LICENSE
 
 [![pages-build-deployment](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment/badge.svg?branch=DEV)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment)
+[![lx-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml)
+[![win-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml)
+[![macos-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml)
+
 # OMADS
 MADS: A python implementation for the mesh adaptive direct search (MADS) method; ORTHO-MADS algorithm.
 
 For technical and code documentation, please visit [OMADS Webpage](https://ahmed-bayoumy.github.io/OMADS/).
 
 ---
 
-**Version 1.5.0**
+**Version 2.1.0**
 
 ---
 
 ## License & copyright
 
 © Ahmed H. Bayoumy 
 ---
@@ -43,15 +47,15 @@
 
 ```pycon
    @software{OMADS_AB,
    author       = {Bayoumy, A.},
    title        = {OMADS},
    year         = 2022,
    publisher    = {Github},
-   version      = {1.5.0},
+   version      = {2.1.0},
    url          = {https://github.com/Ahmed-Bayoumy/OMADS}
    }
 ```
 
 ## How to use OMADS package
 
 After installing the `OMADS` package from [PYPI](https://pypi.org/) website, the functions and classes of `OMADS` basic 
@@ -195,13 +199,12 @@
  #iteration = 46
  nb_success = 4
  psize = 9.094947017729282e-13
  psize_success = 1.0
  psize_max = 2.0
 ```
 
-
-https://user-images.githubusercontent.com/22842095/204689951-a3d7ff9d-58f1-4af4-a200-7108c1a3250f.mp4
+https://github.com/Ahmed-Bayoumy/OMADS/assets/22842095/5dc72c34-4722-4d93-8c84-d17f5595556d
```

### Comparing `OMADS-2.0.0/README.md` & `OMADS-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [![pages-build-deployment](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment/badge.svg?branch=DEV)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment)
+[![lx-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml)
+[![win-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml)
+[![macos-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml)
+
 # OMADS
 MADS: A python implementation for the mesh adaptive direct search (MADS) method; ORTHO-MADS algorithm.
 
 For technical and code documentation, please visit [OMADS Webpage](https://ahmed-bayoumy.github.io/OMADS/).
 
 ---
 
-**Version 1.5.0**
+**Version 2.1.0**
 
 ---
 
 ## License & copyright
 
 © Ahmed H. Bayoumy 
 ---
@@ -21,15 +25,15 @@
 
 ```pycon
    @software{OMADS_AB,
    author       = {Bayoumy, A.},
    title        = {OMADS},
    year         = 2022,
    publisher    = {Github},
-   version      = {1.5.0},
+   version      = {2.1.0},
    url          = {https://github.com/Ahmed-Bayoumy/OMADS}
    }
 ```
 
 ## How to use OMADS package
 
 After installing the `OMADS` package from [PYPI](https://pypi.org/) website, the functions and classes of `OMADS` basic 
@@ -173,11 +177,10 @@
  #iteration = 46
  nb_success = 4
  psize = 9.094947017729282e-13
  psize_success = 1.0
  psize_max = 2.0
 ```
 
-
-https://user-images.githubusercontent.com/22842095/204689951-a3d7ff9d-58f1-4af4-a200-7108c1a3250f.mp4
+https://github.com/Ahmed-Bayoumy/OMADS/assets/22842095/5dc72c34-4722-4d93-8c84-d17f5595556d
```

### Comparing `OMADS-2.0.0/pyproject.toml` & `OMADS-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OMADS-2.0.0/setup.cfg` & `OMADS-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204f 4d41 4453 0d0a 7665 7273 696f   = OMADS..versio
-00000020: 6e20 3d20 322e 302e 300d 0a61 7574 686f  n = 2.0.0..autho
+00000020: 6e20 3d20 322e 312e 300d 0a61 7574 686f  n = 2.1.0..autho
 00000030: 7220 3d20 4168 6d65 6420 482e 2042 6179  r = Ahmed H. Bay
 00000040: 6f75 6d79 0d0a 6175 7468 6f72 5f65 6d61  oumy..author_ema
 00000050: 696c 203d 2061 686d 6564 2e62 6179 6f75  il = ahmed.bayou
 00000060: 6d79 406d 6169 6c2e 6d63 6769 6c6c 2e63  my@mail.mcgill.c
 00000070: 610d 0a64 6573 6372 6970 7469 6f6e 203d  a..description =
 00000080: 2022 5079 7468 6f6e 2070 6163 6b61 6765   "Python package
 00000090: 2066 6f72 2044 464f 3b20 616e 2069 6d70   for DFO; an imp
```

### Comparing `OMADS-2.0.0/setup.py` & `OMADS-2.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 if __name__ == "__main__":
   setup(
     name="OMADS",
     author="Ahmed H. Bayoumy",
     author_email="ahmed.bayoumy@mail.mcgill.ca",
-    version='2.0.0',
+    version='2.1.0',
     packages=find_packages(include=['SLML', 'SLML.*']),
     description="Statistical Learning Models Library",
     install_requires=[
       'cocopp==2.6.3',
       'NOBM>=1.0.1',
       'numpy>=1.22.4',
       'pandas>=1.5.2',
```

### Comparing `OMADS-2.0.0/src/OMADS/MADS.py` & `OMADS-2.1.0/src/OMADS/MADS.py`

 * *Files identical despite different names*

### Comparing `OMADS-2.0.0/src/OMADS/POLL.py` & `OMADS-2.1.0/src/OMADS/POLL.py`

 * *Files identical despite different names*

### Comparing `OMADS-2.0.0/src/OMADS/SEARCH.py` & `OMADS-2.1.0/src/OMADS/SEARCH.py`

 * *Files identical despite different names*

### Comparing `OMADS-2.0.0/src/OMADS.egg-info/PKG-INFO` & `OMADS-2.1.0/src/OMADS.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMADS
-Version: 2.0.0
+Version: 2.1.0
 Summary: Statistical Learning Models Library
 Home-page: https://github.com/Ahmed-Bayoumy/OMADS
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/OMADS/issues
 Platform: UNKNOWN
@@ -17,22 +17,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
 License-File: LICENSE
 
 [![pages-build-deployment](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment/badge.svg?branch=DEV)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment)
+[![lx-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml)
+[![win-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml)
+[![macos-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml)
+
 # OMADS
 MADS: A python implementation for the mesh adaptive direct search (MADS) method; ORTHO-MADS algorithm.
 
 For technical and code documentation, please visit [OMADS Webpage](https://ahmed-bayoumy.github.io/OMADS/).
 
 ---
 
-**Version 1.5.0**
+**Version 2.1.0**
 
 ---
 
 ## License & copyright
 
 © Ahmed H. Bayoumy 
 ---
@@ -43,15 +47,15 @@
 
 ```pycon
    @software{OMADS_AB,
    author       = {Bayoumy, A.},
    title        = {OMADS},
    year         = 2022,
    publisher    = {Github},
-   version      = {1.5.0},
+   version      = {2.1.0},
    url          = {https://github.com/Ahmed-Bayoumy/OMADS}
    }
 ```
 
 ## How to use OMADS package
 
 After installing the `OMADS` package from [PYPI](https://pypi.org/) website, the functions and classes of `OMADS` basic 
@@ -195,13 +199,12 @@
  #iteration = 46
  nb_success = 4
  psize = 9.094947017729282e-13
  psize_success = 1.0
  psize_max = 2.0
 ```
 
-
-https://user-images.githubusercontent.com/22842095/204689951-a3d7ff9d-58f1-4af4-a200-7108c1a3250f.mp4
+https://github.com/Ahmed-Bayoumy/OMADS/assets/22842095/5dc72c34-4722-4d93-8c84-d17f5595556d
```

### Comparing `OMADS-2.0.0/tests/test_OMADS_BASIC.py` & `OMADS-2.1.0/tests/test_OMADS_BASIC.py`

 * *Files identical despite different names*

