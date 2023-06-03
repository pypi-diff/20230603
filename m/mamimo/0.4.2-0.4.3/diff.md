# Comparing `tmp/mamimo-0.4.2.tar.gz` & `tmp/mamimo-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamimo-0.4.2.tar", max compression
+gzip compressed data, was "mamimo-0.4.3.tar", max compression
```

## Comparing `mamimo-0.4.2.tar` & `mamimo-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       76 2022-11-22 17:35:12.322624 mamimo-0.4.2/mamimo/__init__.py
--rw-r--r--   0        0        0     2007 2022-09-29 20:59:31.951368 mamimo-0.4.2/mamimo/analysis.py
--rw-r--r--   0        0        0     9173 2022-11-22 17:53:23.233723 mamimo-0.4.2/mamimo/carryover.py
--rw-r--r--   0        0        0      129 2022-05-15 14:33:03.709480 mamimo-0.4.2/mamimo/datasets/__init__.py
--rw-r--r--   0        0        0     2229 2022-05-15 16:52:39.446790 mamimo-0.4.2/mamimo/datasets/_load_fake_mmm.py
--rw-r--r--   0        0        0    23763 2022-05-15 15:07:18.155555 mamimo-0.4.2/mamimo/linear_model.py
--rw-r--r--   0        0        0     6187 2022-11-22 17:53:23.241729 mamimo-0.4.2/mamimo/saturation.py
--rw-r--r--   0        0        0     8596 2022-05-15 22:22:49.150301 mamimo-0.4.2/mamimo/time_utils.py
--rw-r--r--   0        0        0      661 2022-11-22 17:35:00.919749 mamimo-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6667 2022-09-29 20:17:27.684761 mamimo-0.4.2/README.md
--rw-r--r--   0        0        0     7467 2022-11-22 17:54:37.343492 mamimo-0.4.2/setup.py
--rw-r--r--   0        0        0     7079 2022-11-22 17:54:37.343492 mamimo-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-06-03 08:21:27.249868 mamimo-0.4.3/mamimo/__init__.py
+-rw-r--r--   0        0        0     2007 2023-06-03 08:16:14.772551 mamimo-0.4.3/mamimo/analysis.py
+-rw-r--r--   0        0        0     9172 2023-06-03 08:16:14.773548 mamimo-0.4.3/mamimo/carryover.py
+-rw-r--r--   0        0        0      129 2023-06-03 08:16:14.775551 mamimo-0.4.3/mamimo/datasets/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-03 08:16:14.776551 mamimo-0.4.3/mamimo/datasets/_load_fake_mmm.py
+-rw-r--r--   0        0        0    23764 2023-06-03 08:16:14.790555 mamimo-0.4.3/mamimo/linear_model.py
+-rw-r--r--   0        0        0     6185 2023-06-03 08:16:14.792150 mamimo-0.4.3/mamimo/saturation.py
+-rw-r--r--   0        0        0     8596 2023-06-03 08:16:14.794162 mamimo-0.4.3/mamimo/time_utils.py
+-rw-r--r--   0        0        0      685 2023-06-03 08:22:33.453027 mamimo-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6667 2023-06-03 08:16:14.768526 mamimo-0.4.3/README.md
+-rw-r--r--   0        0        0     7467 2023-06-03 08:26:08.846767 mamimo-0.4.3/setup.py
+-rw-r--r--   0        0        0     7079 2023-06-03 08:26:08.846767 mamimo-0.4.3/PKG-INFO
```

### Comparing `mamimo-0.4.2/mamimo/analysis.py` & `mamimo-0.4.3/mamimo/analysis.py`

 * *Files identical despite different names*

### Comparing `mamimo-0.4.2/mamimo/carryover.py` & `mamimo-0.4.3/mamimo/carryover.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 import numpy as np
 from scipy.signal import convolve2d
-from sklearn.base import BaseEstimator, TransformerMixin, _OneToOneFeatureMixin
+from sklearn.base import BaseEstimator, TransformerMixin, OneToOneFeatureMixin
 from sklearn.utils import check_array
 from sklearn.utils.validation import (
     FLOAT_DTYPES,
     _check_feature_names_in,
     check_is_fitted,
 )
 
 
-class Carryover(_OneToOneFeatureMixin, BaseEstimator, TransformerMixin, ABC):
+class Carryover(OneToOneFeatureMixin, BaseEstimator, TransformerMixin, ABC):
     """
     Smooth the columns of an array by applying a convolution.
 
     Parameters
     ----------
     window : int
         Size of the sliding window. The effect of a holiday will reach from
@@ -74,15 +74,15 @@
 
         Returns
         -------
         Carryover
             Fitted transformer.
 
         """
-        X = self._validate_data(X, dtype=FLOAT_DTYPES)
+        _ = self._validate_data(X, dtype=FLOAT_DTYPES)
 
         self.sliding_window_ = self._get_sliding_window()
         self.sliding_window_ = (
             self.sliding_window_.reshape(-1, 1) / self.sliding_window_.sum()
         )
 
         return self
@@ -237,15 +237,15 @@
         return sliding_window
 
 
 class ExponentialCarryover(Carryover):
     """
     Smoothes time series data with an exponential window.
 
-    Smooth the columns of an array by applying a convolution with a exponentially
+    Smooth the columns of an array by applying a convolution with an exponentially
     decaying curve. This class can be used for modelling carry over effects in
     marketing mix models.
 
     Parameters
     ----------
     window : int, default=1
         Size of the sliding window. The effect of a holiday will reach from
```

### Comparing `mamimo-0.4.2/mamimo/datasets/_load_fake_mmm.py` & `mamimo-0.4.3/mamimo/datasets/_load_fake_mmm.py`

 * *Files identical despite different names*

### Comparing `mamimo-0.4.2/mamimo/linear_model.py` & `mamimo-0.4.3/mamimo/linear_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     check_is_fitted,
     check_X_y,
 )
 
 
 class BaseScipyMinimizeRegressor(BaseEstimator, RegressorMixin, ABC):
     """
-    Base class for regressors relying on scipy's minimze method.
+    Base class for regressors relying on scipy's minimize method.
 
     Derive a class from this one and give it the function to be minimized.
 
     Parameters
     ----------
     alpha : float, default=0.0
         Constant that multiplies the penalty terms. Defaults to 1.0.
```

### Comparing `mamimo-0.4.2/mamimo/saturation.py` & `mamimo-0.4.3/mamimo/saturation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 import numpy as np
-from sklearn.base import BaseEstimator, TransformerMixin, _OneToOneFeatureMixin
+from sklearn.base import BaseEstimator, TransformerMixin, OneToOneFeatureMixin
 from sklearn.utils.validation import (
     FLOAT_DTYPES,
     _check_feature_names_in,
     check_array,
     check_is_fitted,
 )
 
 
-class Saturation(_OneToOneFeatureMixin, BaseEstimator, TransformerMixin, ABC):
+class Saturation(OneToOneFeatureMixin, BaseEstimator, TransformerMixin, ABC):
     """Base class for all saturations, such as Box-Cox, Adbudg, ..."""
 
     def fit(self, X: np.ndarray, y: None = None) -> Saturation:
         """
         Fit the transformer.
 
         In this special case, nothing is done.
```

### Comparing `mamimo-0.4.2/mamimo/time_utils.py` & `mamimo-0.4.3/mamimo/time_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import (
+    FLOAT_DTYPES,
     _check_feature_names_in,
     check_array,
     check_is_fitted,
 )
 
 
 def add_date_indicators(df: pd.DataFrame, **kwargs) -> pd.DataFrame:
@@ -227,16 +228,15 @@
 
         Returns
         -------
         PowerTrend
             Fitted transformer.
 
         """
-        X = check_array(X)
-        self._check_n_features(X, reset=True)
+        _ = self._validate_data(X, dtype=FLOAT_DTYPES)
 
         return self
 
     def transform(self, X: np.ndarray) -> np.ndarray:
         """
         Apply the power function.
```

### Comparing `mamimo-0.4.2/pyproject.toml` & `mamimo-0.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mamimo"
-version = "0.4.2"
+version = "0.4.3"
 description = "A package to create marketing mix models."
 authors = ["Robert Kübler <xgarve@gmail.com>"]
 repository = "https://github.com/Garve/mamimo"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,14 +17,15 @@
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 mypy = "^0.950"
 pre-commit = "^2.18.1"
 pydocstyle = "^6.1.1"
 pytest = "^7.1.2"
 Sphinx = "^5.2.2"
+hypothesis = "^6.59.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `mamimo-0.4.2/README.md` & `mamimo-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mamimo-0.4.2/setup.py` & `mamimo-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.22.3,<2.0.0', 'pandas>=1.4.2,<2.0.0', 'scikit-learn>=1.0.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'mamimo',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'A package to create marketing mix models.',
     'long_description': '# MaMiMo\nThis is a small library that helps you with your everyday **Ma**rketing **Mi**x **Mo**delling. It contains a few saturation functions, carryovers and some utilities for creating with time features. You can also read my article about it here: [>>>Click<<<](https://towardsdatascience.com/a-small-python-library-for-marketing-mix-modeling-mamimo-100f31666e18).\n\nGive it a try via `pip install mamimo`!\n\n# Small Example\nYou can create a marketing mix model using different components from MaMiMo as well as [scikit-learn](https://scikit-learn.org/stable/). First, we can create a dataset via\n```python\nfrom mamimo.datasets import load_fake_mmm\n\ndata = load_fake_mmm()\n\nX = data.drop(columns=[\'Sales\'])\ny = data[\'Sales\']\n```\n\n`X` contains media spends only now, but you can enrich it with more information.\n\n## Feature Engineering\n\nMaMiMo lets you add time features, for example, via\n\n```python\nfrom mamimo.time_utils import add_time_features, add_date_indicators\n\n\nX = (X\n     .pipe(add_time_features, month=True)\n     .pipe(add_date_indicators, special_date=["2020-01-05"])\n     .assign(trend=range(200))\n)\n```\n\nThis adds\n\n- a month column (integers between 1 and 12),\n- a binary column named special_date that is 1 on the 5h of January 2020 and 0 everywhere else, and\n- a (so far linear) trend which is only counting up from 0 to 199.\n\n`X` looks like this now:\n\n![1_iPkUH70amWOZijv6LVhM3A](https://user-images.githubusercontent.com/932327/169354994-624c5608-8dcf-49ae-94e2-5195f019d596.png)\n\n## Building a Model\n\nWe can now build a final model like this:\n```python\nfrom mamimo.time_utils import PowerTrend\nfrom mamimo.carryover import ExponentialCarryover\nfrom mamimo.saturation import ExponentialSaturation\nfrom sklearn.linear_model import LinearRegression\nfrom sklearn.preprocessing import OneHotEncoder\nfrom sklearn.compose import ColumnTransformer\nfrom sklearn.pipeline import Pipeline\n\ncats =  [list(range(1, 13))] # different months, known beforehand\n\npreprocess = ColumnTransformer(\n    [\n     (\'tv_pipe\', Pipeline([\n            (\'carryover\', ExponentialCarryover()),\n            (\'saturation\', ExponentialSaturation())\n     ]), [\'TV\']),\n     (\'radio_pipe\', Pipeline([\n            (\'carryover\', ExponentialCarryover()),\n            (\'saturation\', ExponentialSaturation())\n     ]), [\'Radio\']),\n     (\'banners_pipe\', Pipeline([\n            (\'carryover\', ExponentialCarryover()),\n            (\'saturation\', ExponentialSaturation())\n     ]), [\'Banners\']),\n    (\'month\', OneHotEncoder(sparse=False, categories=cats), [\'month\']),\n    (\'trend\', PowerTrend(), [\'trend\']),\n    (\'special_date\', ExponentialCarryover(), [\'special_date\'])\n    ]\n)\n\nmodel = Pipeline([\n    (\'preprocess\', preprocess),\n    (\'regression\', LinearRegression(\n        positive=True,\n        fit_intercept=False # no intercept because of the months\n        ) \n    )\n])\n```\n\nThis builds a model that does the following:\n- the media channels are preprocessed using the [adstock transformation](https://en.wikipedia.org/wiki/Advertising_adstock), i.e. a carryover effect and a saturation is added\n- the month is one-hot (dummy) encoded\n- the trend is changed from linear to something like t^a, with some exponent a to be optimized\n- the special_date 2020-01-05 gets a carryover effect as well, meaning that not only on this special week there was some special effect on the sales, but also the weeks after it\n\n## Training The Model\nWe can then hyperparameter tune the model via\n```python\nfrom scipy.stats import randint, uniform\nfrom sklearn.model_selection import RandomizedSearchCV, TimeSeriesSplit\n\ntuned_model = RandomizedSearchCV(\n    model,\n    param_distributions={\n        \'preprocess__tv_pipe__carryover__window\': randint(1, 10),\n        \'preprocess__tv_pipe__carryover__strength\': uniform(0, 1),\n        \'preprocess__tv_pipe__saturation__exponent\': uniform(0, 1),\n        \'preprocess__radio_pipe__carryover__window\': randint(1, 10),\n        \'preprocess__radio_pipe__carryover__strength\': uniform(0, 1),\n        \'preprocess__radio_pipe__saturation__exponent\': uniform(0, 1),\n        \'preprocess__banners_pipe__carryover__window\': randint(1, 10),\n        \'preprocess__banners_pipe__carryover__strength\': uniform(0, 1),\n        \'preprocess__banners_pipe__saturation__exponent\': uniform(0, 1),\n        \'preprocess__trend__power\': uniform(0, 2),           \n        \'preprocess__special_date__window\': randint(1, 10),  \n        \'preprocess__special_date__strength\': uniform(0, 1), \n    },\n    cv=TimeSeriesSplit(),\n    random_state=0,\n    n_iter=1000, # can take some time, lower number for faster results\n)\n\ntuned_model.fit(X, y)\n```\n\nYou can also use `GridSearch`, Optuna, or other hyperparameter tune methods and packages here, as long as it is compatible to scikit-learn.\n\n## Analyzing\nWith `tuned_model.predict(X)` and some plotting, we get\n\n![1_Bf4NKiUPNVVH87-7PNNZGw](https://user-images.githubusercontent.com/932327/169356818-158a322e-c18c-4404-a32f-ee69778c4d22.png)\n\nYou can get the best found hyperparameters using `print(tuned_model.best_params_)`.\n\n### Plotting\nYou can compute the channel contributions via \n```python\nfrom mamimo.analysis import breakdown\n\ncontributions = breakdown(tuned_model.best_estimator_, X, y)\n```\n\nThis returns a dataframe with the contributions of each channel fo each time step, summing to the historical values present in `y`. You can get a nice plot via\n```python\nax = contributions.plot.area(\n    figsize=(16, 10),\n    linewidth=1,\n    title="Predicted Sales and Breakdown",\n    ylabel="Sales",\n    xlabel="Date",\n)\nhandles, labels = ax.get_legend_handles_labels()\nax.legend(\n    handles[::-1],\n    labels[::-1],\n    title="Channels",\n    loc="center left",\n    bbox_to_anchor=(1.01, 0.5),\n)\n```\n\n![1_SIlnsYXxRjhSZf-1jE4aDQ](https://user-images.githubusercontent.com/932327/169357525-c4f79fa0-a2fd-46b2-8331-47e534737d81.png)\n\nWow, that\'s a lot of channels. Let us group some of them together.\n\n```python\ngroup_channels = {\'Baseline\': [f\'month__month_{i}\' for i in range(1, 13)] + [\'Base\', \'trend__trend\']} \n# read: \'Baseline consists of the months, base and trend.\'\n# You can add more groups!\n\ncontributions = breakdown(\n    tuned_model.best_estimator_,\n    X,\n    y,\n    group_channels\n)\n```\n\nIf we plot again, we get\n\n![1_xHzrUMMTKGxo7dvKpebjNg](https://user-images.githubusercontent.com/932327/169357648-13ae9097-d45b-4690-b3dd-63139da020b7.png)\n\nYay!\n\n-----------------\n[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/G2G7EBKVH)\n\n',
     'author': 'Robert Kübler',
     'author_email': 'xgarve@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Garve/mamimo',
```

### Comparing `mamimo-0.4.2/PKG-INFO` & `mamimo-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamimo
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package to create marketing mix models.
 Home-page: https://github.com/Garve/mamimo
 Author: Robert Kübler
 Author-email: xgarve@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

