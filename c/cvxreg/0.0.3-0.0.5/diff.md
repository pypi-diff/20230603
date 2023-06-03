# Comparing `tmp/cvxreg-0.0.3.tar.gz` & `tmp/cvxreg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.0.3.tar", last modified: Sat Jun  3 19:53:28 2023, max compression
+gzip compressed data, was "cvxreg-0.0.5.tar", last modified: Sat Jun  3 20:58:30 2023, max compression
```

## Comparing `cvxreg-0.0.3.tar` & `cvxreg-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.792292 cvxreg-0.0.3/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1074 2023-05-28 10:01:59.000000 cvxreg-0.0.3/LICENSE
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1701 2023-06-03 19:53:28.792292 cvxreg-0.0.3/PKG-INFO
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1050 2023-06-03 16:12:52.000000 cvxreg-0.0.3/README.md
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      207 2023-06-03 19:37:02.000000 cvxreg-0.0.3/cvxreg/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      995 2023-06-03 15:03:53.000000 cvxreg-0.0.3/cvxreg/base.py
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      292 2023-06-03 10:50:18.000000 cvxreg-0.0.3/cvxreg/constant.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg/models/
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      134 2023-06-03 10:37:47.000000 cvxreg-0.0.3/cvxreg/models/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     3394 2023-06-03 14:55:15.000000 cvxreg-0.0.3/cvxreg/models/_base.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     3352 2023-06-03 19:49:27.000000 cvxreg-0.0.3/cvxreg/models/_penalized.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.792292 cvxreg-0.0.3/cvxreg/utils/
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)       65 2023-06-03 14:51:23.000000 cvxreg-0.0.3/cvxreg/utils/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     2801 2023-06-03 14:40:27.000000 cvxreg-0.0.3/cvxreg/utils/check.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1055 2023-06-03 15:07:38.000000 cvxreg-0.0.3/cvxreg/utils/extmath.py
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)     8052 2023-06-03 11:10:27.000000 cvxreg-0.0.3/cvxreg/utils/tools.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg.egg-info/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1701 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/PKG-INFO
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      427 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/SOURCES.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/dependency_links.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 15:45:50.000000 cvxreg-0.0.3/cvxreg.egg-info/not-zip-safe
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       57 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/requires.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        7 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/top_level.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       38 2023-06-03 19:53:28.792292 cvxreg-0.0.3/setup.cfg
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1119 2023-06-03 19:52:46.000000 cvxreg-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 20:58:20.000000 cvxreg-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-03 20:58:30.744887 cvxreg-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-03 20:58:20.000000 cvxreg-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.740887 cvxreg-0.0.5/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/extmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:58:30.744887 cvxreg-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-03 20:58:20.000000 cvxreg-0.0.5/setup.py
```

### Comparing `cvxreg-0.0.3/LICENSE` & `cvxreg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/PKG-INFO` & `cvxreg-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
+Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
-Download-URL: https://pypi.org/project/cvxreg/
 Keywords: ML,Prediction,Regression
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,9 +29,7 @@
 
 The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/ConvexRegression). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI 
 
     pip install cvxreg
 
-
-
```

### Comparing `cvxreg-0.0.3/README.md` & `cvxreg-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/cvxreg/base.py` & `cvxreg-0.0.5/cvxreg/base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/cvxreg/models/_base.py` & `cvxreg-0.0.5/cvxreg/models/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,17 +54,18 @@
         """
         
         self.shape = shape
         self.fit_intercept = fit_intercept
         self.positive = positive
 
         if self.shape == Convex:
-            CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=CNLS.FUN_COST, rts=CNLS.RTS_VRS)
+            fun_var = CNLS.FUN_COST
         elif self.shape == Concave:
-            CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=CNLS.FUN_PROD, rts=CNLS.RTS_CRS)
+            fun_var = CNLS.FUN_PROD
+        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=CNLS.RTS_CRS)
 
         if self.positive is True:
             self.__model__.beta.setlb(0.0)
         else:
             self.__model__.beta.setlb(None)
```

### Comparing `cvxreg-0.0.3/cvxreg/models/_penalized.py` & `cvxreg-0.0.5/cvxreg/models/_penalized.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,18 @@
         
         self.c = c
         self.shape = shape
         self.fit_intercept = fit_intercept
         self.positive = positive
 
         if self.shape == Convex:
-            CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=CNLS.FUN_COST, rts=CNLS.RTS_VRS)
+            fun_var = CNLS.FUN_COST
         elif self.shape == Concave:
-            CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=CNLS.FUN_PROD, rts=CNLS.RTS_CRS)
+            fun_var = CNLS.FUN_PROD
+        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=CNLS.RTS_CRS)
 
         # new objective function
         self.__model__.objective.deactivate()
         self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
                                                      sense=minimize,
                                                      doc='objective function')
```

### Comparing `cvxreg-0.0.3/cvxreg/utils/check.py` & `cvxreg-0.0.5/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/cvxreg/utils/extmath.py` & `cvxreg-0.0.5/cvxreg/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/cvxreg/utils/tools.py` & `cvxreg-0.0.5/cvxreg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.3/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.0.5/cvxreg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
+Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
-Download-URL: https://pypi.org/project/cvxreg/
 Keywords: ML,Prediction,Regression
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,9 +29,7 @@
 
 The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/ConvexRegression). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI 
 
     pip install cvxreg
 
-
-
```

### Comparing `cvxreg-0.0.3/setup.py` & `cvxreg-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.0.3',
+    version='0.0.5',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
```

