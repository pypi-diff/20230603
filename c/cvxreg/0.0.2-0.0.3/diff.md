# Comparing `tmp/cvxreg-0.0.2.tar.gz` & `tmp/cvxreg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.0.2.tar", last modified: Sat Jun  3 15:45:50 2023, max compression
+gzip compressed data, was "cvxreg-0.0.3.tar", last modified: Sat Jun  3 19:53:28 2023, max compression
```

## Comparing `cvxreg-0.0.2.tar` & `cvxreg-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 15:45:50.147557 cvxreg-0.0.2/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1074 2023-05-28 10:01:59.000000 cvxreg-0.0.2/LICENSE
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1691 2023-06-03 15:45:50.147557 cvxreg-0.0.2/PKG-INFO
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1041 2023-06-03 15:42:00.000000 cvxreg-0.0.2/README.md
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 15:45:50.143557 cvxreg-0.0.2/cvxreg/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      217 2023-05-27 09:28:51.000000 cvxreg-0.0.2/cvxreg/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      995 2023-06-03 15:03:53.000000 cvxreg-0.0.2/cvxreg/base.py
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      292 2023-06-03 10:50:18.000000 cvxreg-0.0.2/cvxreg/constant.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 15:45:50.147557 cvxreg-0.0.2/cvxreg/cr_model/
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      134 2023-06-03 10:37:47.000000 cvxreg-0.0.2/cvxreg/cr_model/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     3394 2023-06-03 14:55:15.000000 cvxreg-0.0.2/cvxreg/cr_model/_base.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     6481 2023-06-03 10:53:59.000000 cvxreg-0.0.2/cvxreg/cr_model/_penalized.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 15:45:50.147557 cvxreg-0.0.2/cvxreg/utils/
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)       65 2023-06-03 14:51:23.000000 cvxreg-0.0.2/cvxreg/utils/__init__.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     2801 2023-06-03 14:40:27.000000 cvxreg-0.0.2/cvxreg/utils/check.py
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1055 2023-06-03 15:07:38.000000 cvxreg-0.0.2/cvxreg/utils/extmath.py
--rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)     8052 2023-06-03 11:10:27.000000 cvxreg-0.0.2/cvxreg/utils/tools.py
-drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 15:45:50.143557 cvxreg-0.0.2/cvxreg.egg-info/
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1691 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/PKG-INFO
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      433 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/SOURCES.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/dependency_links.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/not-zip-safe
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       57 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/requires.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        7 2023-06-03 15:45:50.000000 cvxreg-0.0.2/cvxreg.egg-info/top_level.txt
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       38 2023-06-03 15:45:50.147557 cvxreg-0.0.2/setup.cfg
--rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1118 2023-06-03 15:44:19.000000 cvxreg-0.0.2/setup.py
+drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.792292 cvxreg-0.0.3/
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1074 2023-05-28 10:01:59.000000 cvxreg-0.0.3/LICENSE
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1701 2023-06-03 19:53:28.792292 cvxreg-0.0.3/PKG-INFO
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1050 2023-06-03 16:12:52.000000 cvxreg-0.0.3/README.md
+drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg/
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      207 2023-06-03 19:37:02.000000 cvxreg-0.0.3/cvxreg/__init__.py
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      995 2023-06-03 15:03:53.000000 cvxreg-0.0.3/cvxreg/base.py
+-rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      292 2023-06-03 10:50:18.000000 cvxreg-0.0.3/cvxreg/constant.py
+drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg/models/
+-rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)      134 2023-06-03 10:37:47.000000 cvxreg-0.0.3/cvxreg/models/__init__.py
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     3394 2023-06-03 14:55:15.000000 cvxreg-0.0.3/cvxreg/models/_base.py
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     3352 2023-06-03 19:49:27.000000 cvxreg-0.0.3/cvxreg/models/_penalized.py
+drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.792292 cvxreg-0.0.3/cvxreg/utils/
+-rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)       65 2023-06-03 14:51:23.000000 cvxreg-0.0.3/cvxreg/utils/__init__.py
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     2801 2023-06-03 14:40:27.000000 cvxreg-0.0.3/cvxreg/utils/check.py
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1055 2023-06-03 15:07:38.000000 cvxreg-0.0.3/cvxreg/utils/extmath.py
+-rw-r--r--   0 zhiqiang  (1000) zhiqiang  (1000)     8052 2023-06-03 11:10:27.000000 cvxreg-0.0.3/cvxreg/utils/tools.py
+drwxrwxr-x   0 zhiqiang  (1000) zhiqiang  (1000)        0 2023-06-03 19:53:28.788292 cvxreg-0.0.3/cvxreg.egg-info/
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1701 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/PKG-INFO
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)      427 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        1 2023-06-03 15:45:50.000000 cvxreg-0.0.3/cvxreg.egg-info/not-zip-safe
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       57 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/requires.txt
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)        7 2023-06-03 19:53:28.000000 cvxreg-0.0.3/cvxreg.egg-info/top_level.txt
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)       38 2023-06-03 19:53:28.792292 cvxreg-0.0.3/setup.cfg
+-rw-rw-r--   0 zhiqiang  (1000) zhiqiang  (1000)     1119 2023-06-03 19:52:46.000000 cvxreg-0.0.3/setup.py
```

### Comparing `cvxreg-0.0.2/LICENSE` & `cvxreg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/PKG-INFO` & `cvxreg-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
-Download-URL: https://pypi.org/project/pysfa/
+Download-URL: https://pypi.org/project/cvxreg/
 Keywords: ML,Prediction,Regression
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/pysfa/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/pysfa)
+[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.2/README.md` & `cvxreg-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/pysfa/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/pysfa)
+[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.2/cvxreg/base.py` & `cvxreg-0.0.3/cvxreg/base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/cvxreg/cr_model/_base.py` & `cvxreg-0.0.3/cvxreg/models/_base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/cvxreg/utils/check.py` & `cvxreg-0.0.3/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/cvxreg/utils/extmath.py` & `cvxreg-0.0.3/cvxreg/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/cvxreg/utils/tools.py` & `cvxreg-0.0.3/cvxreg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.2/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.0.3/cvxreg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
-Download-URL: https://pypi.org/project/pysfa/
+Download-URL: https://pypi.org/project/cvxreg/
 Keywords: ML,Prediction,Regression
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/pysfa/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/pysfa)
+[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.2/setup.py` & `cvxreg-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.0.2',
+    version='0.0.3',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
     keywords=['ML', 'Prediction', 'Regression'],
     url='https://github.com/ConvexRegression/ConvexRegression',
-    download_url='https://pypi.org/project/pysfa/',
+    download_url='https://pypi.org/project/cvxreg/',
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

