# Comparing `tmp/scoringrules-0.1.1.tar.gz` & `tmp/scoringrules-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoringrules-0.1.1.tar", max compression
+gzip compressed data, was "scoringrules-0.2.0.tar", max compression
```

## Comparing `scoringrules-0.1.1.tar` & `scoringrules-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0    11348 2023-05-10 12:48:41.343565 scoringrules-0.1.1/LICENSE
--rw-r--r--   0        0        0     1633 2023-05-10 12:50:44.962188 scoringrules-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-09 10:34:15.261889 scoringrules-0.1.1/scoringrules/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 10:34:10.218297 scoringrules-0.1.1/scoringrules/brier.py
--rw-r--r--   0        0        0     3817 2023-05-10 10:45:53.522090 scoringrules-0.1.1/scoringrules/crps.py
--rw-r--r--   0        0        0      128 2023-05-10 10:42:11.317264 scoringrules-0.1.1/scoringrules/utils.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 scoringrules-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-10 12:48:41.343565 scoringrules-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2449 2023-06-03 08:01:23.986314 scoringrules-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      509 2023-05-25 06:57:37.688447 scoringrules-0.2.0/scoringrules/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-25 06:57:37.688993 scoringrules-0.2.0/scoringrules/_brier.py
+-rw-r--r--   0        0        0     4106 2023-05-25 06:57:37.689636 scoringrules-0.2.0/scoringrules/_crps.py
+-rw-r--r--   0        0        0     1659 2023-05-25 06:57:37.690273 scoringrules-0.2.0/scoringrules/_energy.py
+-rw-r--r--   0        0        0     1749 2023-05-25 06:57:37.690950 scoringrules-0.2.0/scoringrules/_variogram.py
+-rw-r--r--   0        0        0      379 2023-05-19 15:21:01.887844 scoringrules-0.2.0/scoringrules/backend/__init__.py
+-rw-r--r--   0        0        0     7138 2023-05-25 06:57:37.691656 scoringrules-0.2.0/scoringrules/backend/array.py
+-rw-r--r--   0        0        0      127 2023-05-25 06:57:37.692329 scoringrules-0.2.0/scoringrules/backend/arrayapi/__init__.py
+-rw-r--r--   0        0        0     4261 2023-05-25 06:57:37.692541 scoringrules-0.2.0/scoringrules/backend/arrayapi/array_type.py
+-rw-r--r--   0        0        0     7256 2023-05-25 06:57:37.693234 scoringrules-0.2.0/scoringrules/backend/arrayapi/functions.py
+-rw-r--r--   0        0        0     1485 2023-05-25 06:57:37.693881 scoringrules-0.2.0/scoringrules/backend/base.py
+-rw-r--r--   0        0        0     8623 2023-05-25 06:57:37.694546 scoringrules-0.2.0/scoringrules/backend/gufuncs.py
+-rw-r--r--   0        0        0     3716 2023-05-25 06:57:37.695138 scoringrules-0.2.0/scoringrules/backend/numba.py
+-rw-r--r--   0        0        0     1852 2023-05-25 06:57:37.696125 scoringrules-0.2.0/scoringrules/backend/registry.py
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 scoringrules-0.2.0/PKG-INFO
```

### Comparing `scoringrules-0.1.1/LICENSE` & `scoringrules-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scoringrules-0.1.1/scoringrules/crps.py` & `scoringrules-0.2.0/scoringrules/_crps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,145 @@
-import numpy as np
-from numba import guvectorize
-from numpy.typing import NDArray
-from scipy.stats import norm
+from typing import TypeVar
 
+from scoringrules.backend import backends as srb
+from scoringrules.backend.arrayapi import Array
 
-def ensemble_int(
-    forecasts: NDArray,
-    observation: NDArray,
-    axis: int = -1,
-    sorted_ensemble: bool = False,
-):
-    r"""Compute the Continuous Ranked Probability Score (CRPS).
+ArrayLike = TypeVar("ArrayLike", Array, float)
 
-    $$ \text{CRPS}_{\text{INT}}(M, y) = \int_{\mathbb{R}} \left[ \frac{1}{M}
-    \sum_{i=1}^M \mathbb{1}\{x_i \le x \} - \mathbb{1}(y \le x)  \right] ^2 dx$$
 
+def crps_ensemble(
+    forecasts: Array,
+    observations: ArrayLike,
+    /,
+    *,
+    axis: int = -1,
+    sorted_ensemble: bool = False,
+    estimator: str = "pwm",
+    backend: str = "numba",
+) -> Array:
+    r"""Estimate the Continuous Ranked Probability Score (CRPS) for a finite ensemble.
 
     Parameters
     ----------
-    forecasts: NDArray
+    forecasts: ArrayLike
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the last axis.
-    observation: NDArray
+    observations: ArrayLike
         The observed values.
-    axis: int, optional
-        The axis corresponding to the example. Default is the last axis.
-    sorted_ensemble: bool, optional
+    axis: int
+        The axis corresponding to the ensemble. Default is the last axis.
+    sorted_ensemble: bool
         Boolean indicating whether the ensemble members are already in ascending order.
         Default is False.
+    estimator: str
+        Indicates the CRPS estimator to be used.
+    backend: str
+        The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
     Returns
     -------
-    crps: NDArray
+    crps: ArrayLike
         The CRPS between the forecast ensemble and obs.
 
     Examples
     --------
     >>> from scoringrules import crps
     >>> crps.ensemble(pred, obs)
     """
-    if not sorted_ensemble:
-        forecasts = np.sort(forecasts, axis=axis)
+    return srb[backend].crps_ensemble(
+        forecasts,
+        observations,
+        axis=axis,
+        sorted_ensemble=sorted_ensemble,
+        estimator=estimator,
+    )
+
 
-    return _ensemble_int_gufunc_alt(forecasts, observation)
+def crps_normal(
+    mu: ArrayLike,
+    sigma: ArrayLike,
+    observation: ArrayLike,
+    /,
+    *,
+    backend: str = "numpy",
+) -> ArrayLike:
+    r"""Compute the closed form of the CRPS for the normal distribution.
 
+    It is based on the following formulation from
+    [Geiting et al. (2005)](https://journals.ametsoc.org/view/journals/mwre/133/5/mwr2904.1.xml):
 
-def normal(mu: NDArray, sigma: NDArray, observation: NDArray):
-    """Compute the closed form of the CRPS for the normal distribution.
+    $$ \mathrm{CRPS}(\mathcal{N}(\mu, \sigma), y) = \sigma \Bigl\{ \omega [\Phi(ω) - 1] + 2 \phi(\omega) - \frac{1}{\sqrt{\pi}} \Bigl\},$$
+
+    where $\Phi(ω)$ and $\phi(ω)$ are respectively the CDF and PDF of the standard normal
+    distribution at the normalized prediction error $\omega = \frac{y - \mu}{\sigma}$.
 
     Parameters
     ----------
-    mu: NDArray
+    mu: ArrayLike
         Mean of the forecast normal distribution.
-    sigma: NDArray
+    sigma: ArrayLike
         Standard deviation of the forecast normal distribution.
-    observation: NDArray
+    observation: ArrayLike
         The observed values.
 
     Returns
     -------
     crps: array_like
         The CRPS between Normal(mu, sigma) and obs.
+
+    Examples
+    --------
+    >>> from scoringrules import crps
+    >>> crps.normal(0.1, 0.4, 0.0)
     """
-    sx = (observation - mu) / sigma
-    crps = sigma * (sx * (2 * norm.cdf(sx) - 1) + 2 * norm.pdf(sx) - 1 / np.sqrt(np.pi))
-    return crps
+    return srb[backend].crps_normal(mu, sigma, observation)
+
 
+def crps_lognormal(
+    mulog: ArrayLike,
+    sigmalog: ArrayLike,
+    observation: ArrayLike,
+    backend: str = "numpy",
+) -> ArrayLike:
+    r"""Compute the closed form of the CRPS for the lognormal distribution.
+
+    It is based on the formulation introduced by
+    [Baran and Lerch (2015)](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.2521)
+
+    $$ \mathrm{CRPS}(\mathrm{log}\mathcal{N}(\mu, \sigma), y) =
+    y [2 \Phi(y) - 1] - 2 \mathrm{exp}(\mu + \frac{\sigma^2}{2})
+    \left[ \Phi(\omega - \sigma) + \Phi(\frac{\sigma}{\sqrt{2}}) \right]$$
+
+    where $\Phi$ is the CDF of the standard normal distribution and
+    $\omega = \frac{\mathrm{log}y - \mu}{\sigma}$.
 
-def lognormal(mu, sigma, obs):
-    """Compute the closed form of the CRPS for the lognormal distribution.
 
     Parameters
     ----------
-    mu: array_like
-        Mean of the normal distribution.
-    sigma: array_like
-        Standard deviation of the normal distribution.
+    mulog: ArrayLike
+        Mean of the normal underlying distribution.
+    sigmalog: ArrayLike
+        Standard deviation of the underlying normal distribution.
 
     Returns
     -------
-    crps: array_like
+    crps: ArrayLike
         The CRPS between Lognormal(mu, sigma) and obs.
-    """
-    sx = (np.log(obs) - mu) / sigma
-    ex = 2 * np.exp(mu + sigma**2 / 2)
-    crps = obs * (2 * norm.cdf(sx) - 1) - ex * (
-        norm.cdf(sx - sigma) + norm.cdf(sigma / np.sqrt(2)) - 1
-    )
-    return crps
-
-
-@guvectorize(
-    [
-        "void(float32[:], float32[:], float32[:])",
-        "void(float64[:], float64[:], float64[:])",
-    ],
-    "(n),()->()",
-)
-def _ensemble_int_gufunc_alt(forecasts, observation, result):
-    obs = observation[0]
-    M = forecasts.shape[0]
-
-    if np.isnan(obs):
-        result[0] = np.nan
-        return
-
-    obs_cdf = 0
-    forecast_cdf = 0
-    prev_forecast = 0
-    integral = 0
-
-    for n, forecast in enumerate(forecasts):
-        if np.isnan(forecast):
-            # NumPy sorts NaN to the end
-            if n == 0:
-                integral = np.nan
-            # reset for the sake of the conditional below
-            forecast = prev_forecast
-            break
-
-        # this is evaluated the first time obs < forecast
-        if obs_cdf == 0 and obs < forecast:
-            integral += (obs - prev_forecast) * forecast_cdf**2
-            integral += (forecast - obs) * (forecast_cdf - 1) ** 2
-            obs_cdf = 1
-        # this is the main integral  ∫F(x)-1(y<x)dx
-        else:
-            integral += (forecast_cdf - obs_cdf) ** 2 * (forecast - prev_forecast)
 
-        forecast_cdf += 1 / M
-        prev_forecast = forecast
+    Notes
+    -----
+    The mean and standard deviation are not the values for the distribution itself,
+    but of the underlying normal distribution it is derived from.
 
-    if obs_cdf == 0:
-        integral += obs - forecast
-
-    result[0] = integral
+    Examples
+    --------
+    >>> from scoringrules import crps
+    >>> crps.lognormal(0.1, 0.4, 0.0)
+    """
+    return srb[backend].crps_lognormal(mulog, sigmalog, observation)
 
 
 __all__ = [
-    "ensemble_int",
-    "normal",
-    "lognormal",
+    "crps_ensemble",
+    "crps_normal",
+    "crps_lognormal",
 ]
```

