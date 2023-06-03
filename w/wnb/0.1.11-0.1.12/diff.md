# Comparing `tmp/wnb-0.1.11.tar.gz` & `tmp/wnb-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnb-0.1.11.tar", last modified: Sat Jun  3 04:24:02 2023, max compression
+gzip compressed data, was "wnb-0.1.12.tar", last modified: Sat Jun  3 05:00:13 2023, max compression
```

## Comparing `wnb-0.1.11.tar` & `wnb-0.1.12.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:24:02.494122 wnb-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-03 04:24:02.494122 wnb-0.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-03 04:23:52.000000 wnb-0.1.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:24:02.494122 wnb-0.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-03 04:23:52.000000 wnb-0.1.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:24:02.494122 wnb-0.1.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-03 04:23:52.000000 wnb-0.1.11/tests/test_gnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:24:02.494122 wnb-0.1.11/wnb/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-06-03 04:23:52.000000 wnb-0.1.11/wnb/gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:24:02.494122 wnb-0.1.11/wnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-03 04:24:02.000000 wnb-0.1.11/wnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-03 04:24:02.000000 wnb-0.1.11/wnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:24:02.000000 wnb-0.1.11/wnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 04:24:02.000000 wnb-0.1.11/wnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 04:24:02.000000 wnb-0.1.11/wnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-03 05:00:12.998049 wnb-0.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 05:00:03.000000 wnb-0.1.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:00:12.998049 wnb-0.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-03 05:00:03.000000 wnb-0.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.994049 wnb-0.1.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-03 05:00:03.000000 wnb-0.1.12/tests/test_gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-03 05:00:03.000000 wnb-0.1.12/tests/test_gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/wnb/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/wnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/top_level.txt
```

### Comparing `wnb-0.1.11/PKG-INFO` & `wnb-0.1.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.11
+Version: 0.1.12
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,20 +17,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.11-green)
+![](https://img.shields.io/badge/version-v0.1.12-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
-<img src="logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
@@ -49,15 +50,15 @@
 Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
 rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
 of gaussian MLD-WNB.
 
 ## Install
 The easiest way to install the wnb library is by using `pip`:
 ```commandline
-pip install git+https://github.com/msamsami/weighted-naive-bayes
+pip install wnb
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
 Furthermore, it is fully compatible with Scikit-learn API.
 
 ## Getting started
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers.
```

### Comparing `wnb-0.1.11/README.md` & `wnb-0.1.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.11-green)
+![](https://img.shields.io/badge/version-v0.1.12-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
-<img src="logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
@@ -28,15 +29,15 @@
 Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
 rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
 of gaussian MLD-WNB.
 
 ## Install
 The easiest way to install the wnb library is by using `pip`:
 ```commandline
-pip install git+https://github.com/msamsami/weighted-naive-bayes
+pip install wnb
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
 Furthermore, it is fully compatible with Scikit-learn API.
 
 ## Getting started
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers.
```

### Comparing `wnb-0.1.11/setup.py` & `wnb-0.1.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 from os import path
 from setuptools import setup
 
 
 setup(
     name='wnb',
-    version='0.1.11',
+    version='0.1.12',
     description='Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.',
     keywords=['python', 'bayes', 'naivebayes', 'classifier', 'probabilistic'],
     author='Mehdi Samsami',
     author_email='mehdisamsami@live.com',
     url='https://github.com/msamsami/weighted-naive-bayes',
     long_description=codecs.open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

### Comparing `wnb-0.1.11/tests/test_gnb.py` & `wnb-0.1.12/tests/test_gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.11/wnb/_base.py` & `wnb-0.1.12/wnb/_base.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.11/wnb/dist.py` & `wnb-0.1.12/wnb/dist.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.11/wnb/gnb.py` & `wnb-0.1.12/wnb/gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.11/wnb/gwnb.py` & `wnb-0.1.12/wnb/gwnb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from abc import ABCMeta
 import numbers
-from typing import Union, Optional
+from typing import Union, Optional, Sequence
 import warnings
 
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
 from scipy.special import logsumexp
 
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.exceptions import DataConversionWarning
-from sklearn.utils import check_array, as_float_array
+from sklearn.utils import as_float_array, check_array, deprecated
 from sklearn.utils.validation import check_is_fitted
 from sklearn.utils.multiclass import type_of_target
 
 
 class GaussianWNB(ClassifierMixin, BaseEstimator, metaclass=ABCMeta):
     """
     Binary Gaussian Minimum Log-likelihood Difference Weighted Naive Bayes (MLD-WNB) Classifier
     """
 
-    def __init__(self, priors: Optional[Union[list, np.ndarray]] = None, error_weights: Optional[np.ndarray] = None,
+    def __init__(self, *,
+                 priors: Optional[Union[Sequence[float], np.ndarray]] = None,
+                 error_weights: Optional[np.ndarray] = None,
                  max_iter: int = 25, step_size: float = 1e-4, penalty: str = 'l2', C: float = 1.0) -> None:
         """Initializes an object of the class.
 
         Args:
-            priors (Optional[Union[list, np.ndarray]]): Prior probabilities. Defaults to None.
+            priors (Optional[Union[Sequence[float], np.ndarray]]): Prior probabilities. Defaults to None.
             error_weights (Optional[np.ndarray]): Matrix of error weights (n_classes * n_classes). Defaults to None.
             max_iter (int): Maximum number of gradient descent iterations. Defaults to 25.
             step_size (float): Step size of weight update (i.e., learning rate). Defaults to 1e-4.
             penalty (str): Regularization term; must be either 'l1' or 'l2'. Defaults to 'l2'.
             C (float): Regularization strength; must be a positive float. Defaults to 1.0.
 
         Returns:
@@ -44,15 +46,15 @@
 
     def _more_tags(self):
         return {
             'binary_only': True,
             'requires_y': True
         }
 
-    def __check_inputs(self, X, y):
+    def _check_inputs(self, X, y):
         # Check that the dataset has only two unique labels
         if type_of_target(y) != 'binary':
             warnings.warn('This version of MLD-WNB only supports binary classification.')
             raise ValueError('Unknown label type: non-binary')
 
         # Check if only one class is present in label vector
         if self.n_classes_ == 1:
@@ -113,15 +115,18 @@
         # Check that the maximum number of iterations is a positive integer
         if not isinstance(self.max_iter, numbers.Number) or self.max_iter < 0:
             raise ValueError(
                 "Maximum number of iteration must be a positive integer; got (max_iter=%r)"
                 % self.max_iter
             )
 
-    def __prepare_X_y(self, X=None, y=None):
+    def _prepare_X_y(self, X=None, y=None, from_fit=False):
+        if from_fit and y is None:
+            raise ValueError("requires y to be passed, but the target y is None")
+
         if X is not None:
             # Convert to NumPy array if X is Pandas DataFrame
             if isinstance(X, pd.DataFrame):
                 X = X.values
             X = as_float_array(X)
 
         if y is not None:
@@ -137,15 +142,15 @@
 
             y = y.flatten()
 
         output = tuple(item for item in [X, y] if item is not None)
         output = output[0] if len(output) == 1 else output
         return output
 
-    def __prepare_parameters(self, X, y):
+    def _prepare_parameters(self, X, y):
         # Calculate mean and standard deviation of features for each class
         for c in range(self.n_classes_):
             self.mu_[:, c] = np.mean(X[y == c, :], axis=0)  # Calculate mean of features for class c
             self.std_[:, c] = np.std(X[y == c, :], axis=0)  # Calculate std of features for class c
 
         # Update if no priors is provided
         if self.priors is None:
@@ -175,83 +180,84 @@
             y (Union[np.ndarray, pd.DataFrame, pd.Series]): Array-like of shape (n_samples,). Target values.
             learning_hist (bool): Whether to keep the learning history (i.e., the value of cost function in each
                                   learning iteration)
 
         Returns:
             self: The instance itself.
         """
-        X, y = self.__prepare_X_y(X, y)
+        X, y = self._prepare_X_y(X, y, from_fit=True)
 
         self.classes_, y_ = np.unique(y, return_inverse=True)  # Unique class labels and their indices
         self.n_classes_ = len(self.classes_)  # Number of classes
         self.__n_samples, self.n_features_in_ = X.shape  # Number of samples and features
 
-        self.__check_inputs(X, y)
+        self._check_inputs(X, y)
         y = y_
 
         self.mu_ = np.zeros((self.n_features_in_, self.n_classes_))  # Mean of features (n_features x 1)
         self.std_ = np.zeros((self.n_features_in_, self.n_classes_))  # Standard deviation of features (n_features x 1)
         self.coef_ = np.ones((self.n_features_in_,))  # WNB coefficients (n_features x 1)
         self.cost_hist_ = np.array([np.nan for _ in range(self.max_iter)])  # To store cost value in each iteration
 
-        self.__prepare_parameters(X, y)
+        self._prepare_parameters(X, y)
 
         # Learn the weights using gradient descent
         self.n_iter_ = 0
         for self.n_iter_ in range(self.max_iter):
             # Predict on X
             y_hat = self.__predict(X)
 
             # Calculate cost
-            self.cost_hist_[self.n_iter_], _lambda = self.__calculate_cost(X, y, y_hat, learning_hist)
+            self.cost_hist_[self.n_iter_], _lambda = self._calculate_cost(X, y, y_hat, learning_hist)
 
             # Calculate gradients (most time-consuming)
-            _grad = self.__calculate_grad(X, _lambda)
+            _grad = self._calculate_grad(X, _lambda)
 
             # Add regularization
             if self.penalty == 'l1':
                 _grad += self.C * np.sign(self.coef_)
             elif self.penalty == 'l2':
                 _grad += 2 * self.C * self.coef_
 
             # Update weights
             self.coef_ = self.coef_ - self.step_size * _grad
 
         return self
 
-    def __calculate_cost(self, X, y, y_hat, learning_hist):
+    def _calculate_cost(self, X, y, y_hat, learning_hist):
         _lambda = [self.error_weights_[y[i], y_hat[i]] for i in range(self.__n_samples)]
 
         if learning_hist:
             # Calculate cost
             _cost = 0
             for i in range(self.__n_samples):
                 _sum = np.log(self.class_prior_[1] / self.class_prior_[0])
                 x = X[i, :]
                 for j in range(self.n_features_in_):
                     _sum += self.coef_[j] * (np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 1], self.std_[j, 1]))
-                                                - np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 0], self.std_[j, 0])))
+                                             - np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 0], self.std_[j, 0])))
                 _cost += _lambda[i] * _sum
         else:
             _cost = None
 
         return _cost, _lambda
 
-    def __calculate_grad(self, X, _lambda):
+    def _calculate_grad(self, X, _lambda):
         _grad = np.repeat(np.log(self.std_[:, 0] / self.std_[:, 1]).reshape(1, -1), self.__n_samples, axis=0)
         _grad += 0.5 * ((X - np.repeat(self.mu_[:, 0].reshape(1, -1), self.__n_samples, axis=0)) /
                         (np.repeat(self.std_[:, 0].reshape(1, -1), self.__n_samples, axis=0))) ** 2
         _grad -= 0.5 * ((X - np.repeat(self.mu_[:, 1].reshape(1, -1), self.__n_samples, axis=0)) /
                         (np.repeat(self.std_[:, 1].reshape(1, -1), self.__n_samples, axis=0))) ** 2
         _grad *= np.transpose(np.repeat(np.array(_lambda).reshape(1, -1), self.n_features_in_, axis=0))
         _grad = np.sum(_grad, axis=0)
 
         return _grad
 
-    def __calculate_grad_slow(self, X, _lambda):
+    @deprecated()
+    def _calculate_grad_slow(self, X, _lambda):
         _grad = np.zeros((self.n_features_in_,))
         for i in range(self.__n_samples):
             x = X[i, :]
             _log_p = np.array(
                 [
                     np.log(self.std_[j, 0] / self.std_[j, 1]) +
                     0.5*((x[j] - self.mu_[j, 0]) / self.std_[j, 0])**2 -
@@ -300,15 +306,15 @@
         if not X.shape[1] == self.n_features_in_:
             raise ValueError(
                 "Expected input with %d features, got %d instead." % (self.n_features_in_, X.shape[1])
             )
 
         n_samples = X.shape[0]
 
-        X = self.__prepare_X_y(X=X)
+        X = self._prepare_X_y(X=X)
 
         log_priors = np.tile(np.log(self.class_prior_), (n_samples, 1))
         w_reshaped = np.tile(self.coef_.reshape(-1, 1), (1, self.n_classes_))
         term1 = np.sum(np.multiply(w_reshaped, -np.log(np.sqrt(2 * np.pi) * self.std_)))
         var_inv = np.multiply(w_reshaped, 1/np.multiply(self.std_, self.std_))
         mu_by_var = np.multiply(self.mu_, var_inv)
         term2 = -0.5*(np.matmul(np.multiply(X, X), var_inv) - 2*np.matmul(X, mu_by_var)
```

### Comparing `wnb-0.1.11/wnb.egg-info/PKG-INFO` & `wnb-0.1.12/wnb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.11
+Version: 0.1.12
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,20 +17,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.11-green)
+![](https://img.shields.io/badge/version-v0.1.12-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
-<img src="logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
@@ -49,15 +50,15 @@
 Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
 rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
 of gaussian MLD-WNB.
 
 ## Install
 The easiest way to install the wnb library is by using `pip`:
 ```commandline
-pip install git+https://github.com/msamsami/weighted-naive-bayes
+pip install wnb
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
 Furthermore, it is fully compatible with Scikit-learn API.
 
 ## Getting started
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers.
```

