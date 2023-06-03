# Comparing `tmp/sphecerix-0.2.0-py3-none-any.whl.zip` & `tmp/sphecerix-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5536 bytes, number of entries: 9
--rw-r--r--  2.0 unx      219 b- defN 23-May-28 19:49 sphecerix/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-May-28 19:49 sphecerix/_version.py
--rw-r--r--  2.0 unx     3394 b- defN 23-May-28 19:49 sphecerix/atomic_wave_functions.py
--rw-r--r--  2.0 unx     1220 b- defN 23-May-28 19:49 sphecerix/tesseral.py
--rw-r--r--  2.0 unx     2314 b- defN 23-May-28 19:49 sphecerix/wignerd.py
--rw-r--r--  2.0 unx     2873 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/RECORD
-9 files, 10848 bytes uncompressed, 4324 bytes compressed:  60.1%
+Zip file size: 6275 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-03 12:02 sphecerix/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-03 12:02 sphecerix/_version.py
+-rw-r--r--  2.0 unx     3394 b- defN 23-Jun-03 12:02 sphecerix/atomic_wave_functions.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-03 12:02 sphecerix/tesseral.py
+-rw-r--r--  2.0 unx     5712 b- defN 23-Jun-03 12:02 sphecerix/wignerd.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/RECORD
+9 files, 14246 bytes uncompressed, 5063 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sphecerix/tesseral.py
 Comment: 
 
 Filename: sphecerix/wignerd.py
 Comment: 
 
-Filename: sphecerix-0.2.0.dist-info/METADATA
+Filename: sphecerix-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: sphecerix-0.2.0.dist-info/WHEEL
+Filename: sphecerix-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: sphecerix-0.2.0.dist-info/top_level.txt
+Filename: sphecerix-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sphecerix-0.2.0.dist-info/RECORD
+Filename: sphecerix-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphecerix/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

## sphecerix/wignerd.py

```diff
@@ -4,29 +4,125 @@
 from scipy.special import factorial
 from scipy.spatial.transform import Rotation as R
 from .tesseral import tesseral_transformation
 
 def tesseral_wigner_D(l, Robj):
     """
     Produce the Wigner D-matrix for tesseral spherical harmonics
+
+    Parameters
+    ----------
+    l : int
+        Order of the spherical harmonics
+    Robj : scipy.spatial.transform.Rotation
+        Rotation in :math:`\mathbb{R}^{3}`
+
+    Returns
+    -------
+    D : numpy.ndarray
+        Real-valued Wigner-D matrix with dimensions :math:`(2l+1) \\times (2l+1)`
+
+    Raises
+    ------
+    TypeError
+        If the Robj object is not of type scipy.spatial.transform.R.
+
+    Examples
+    --------
+    >>> from sphecerix import tesseral_wigner_D
+    >>> from scipy.spatial.transform import Rotation as R
+    >>> import numpy as np
+    >>> 
+    >>> # build rotation axis and set angle
+    >>> axis = np.ones(3) / np.sqrt(3)
+    >>> angle = np.pi
+    >>> Robj = R.from_rotvec(axis * angle)
+    >>> 
+    >>> # construct tesseral Wigner D matrix
+    >>> D = tesseral_wigner_D(2, Robj)
+    >>> print(D)
+    [[ 5.55555556e-01  2.22222222e-01  7.69800359e-01  2.22222222e-01
+       1.89744731e-16]
+     [ 2.22222222e-01  5.55555556e-01 -3.84900179e-01  2.22222222e-01
+       6.66666667e-01]
+     [ 7.69800359e-01 -3.84900179e-01 -3.33333333e-01 -3.84900179e-01
+       5.42310034e-16]
+     [ 2.22222222e-01  2.22222222e-01 -3.84900179e-01  5.55555556e-01
+      -6.66666667e-01]
+     [-1.01229242e-16  6.66666667e-01 -4.65653372e-16 -6.66666667e-01
+      -3.33333333e-01]]
+
+    Construct the Wigner-D matrix for the tesseral p-orbitals for a rotation around
+    the :math:`\\frac{1}{\\sqrt{3}}(1,1,1)` axis by an angle :math:`\\pi`.
+
     """
     # verify that Robj is a rotation object
     if not isinstance(Robj, R):
         raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
     
     T = tesseral_transformation(l)
     alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
     D = wigner_D(l, Robj)
     
     return np.real(T @ D @ T.conjugate().transpose())
 
 def wigner_D(l, Robj):
     """
-    Produce Wigner D-matrix for order l of spherical harmonics and
-    given axis angle rotation
+    Produce Wigner D-matrix for canonical spherical harmonics
+
+    Parameters
+    ----------
+    l : int
+        Order of the spherical harmonics
+    Robj : scipy.spatial.transform.Rotation
+        Rotation in :math:`\mathbb{R}^{3}`
+
+    Returns
+    -------
+    D : numpy.ndarray
+        Complex-valued Wigner-D matrix with dimensions :math:`(2l+1) \\times (2l+1)`
+
+    Raises
+    ------
+    TypeError
+        If the Robj object is not of type scipy.spatial.transform.R. 
+
+    Examples
+    --------
+    >>> from sphecerix import wigner_D
+    >>> from scipy.spatial.transform import Rotation as R
+    >>> import numpy as np
+    >>> 
+    >>> # build rotation axis and set angle
+    >>> axis = np.ones(3) / np.sqrt(3)
+    >>> angle = np.pi
+    >>> Robj = R.from_rotvec(axis * angle)
+    >>> 
+    >>> # construct tesseral Wigner D matrix
+    >>> D = wigner_D(2, Robj)
+    >>> print(D)
+    [[ 1.11111111e-01-1.45486986e-16j -2.22222222e-01+2.22222222e-01j
+      -3.29266657e-16-5.44331054e-01j  4.44444444e-01+4.44444444e-01j
+      -4.44444444e-01-4.42577444e-17j]
+     [-2.22222222e-01-2.22222222e-01j  5.55555556e-01-3.33066907e-16j
+      -2.72165527e-01+2.72165527e-01j -5.55111512e-17+2.22222222e-01j
+      -4.44444444e-01-4.44444444e-01j]
+     [ 3.83471103e-16+5.44331054e-01j -2.72165527e-01-2.72165527e-01j
+      -3.33333333e-01+0.00000000e+00j  2.72165527e-01-2.72165527e-01j
+       3.83471103e-16-5.44331054e-01j]
+     [ 4.44444444e-01-4.44444444e-01j -5.55111512e-17-2.22222222e-01j
+       2.72165527e-01+2.72165527e-01j  5.55555556e-01+3.33066907e-16j
+       2.22222222e-01-2.22222222e-01j]
+     [-4.44444444e-01+4.42577444e-17j -4.44444444e-01+4.44444444e-01j
+      -3.29266657e-16+5.44331054e-01j  2.22222222e-01+2.22222222e-01j
+       1.11111111e-01+1.45486986e-16j]]
+
+    Construct the Wigner-D matrix for the canonical p-orbitals for a rotation around
+    the :math:`\\frac{1}{\\sqrt{3}}(1,1,1)` axis by an angle :math:`\\pi`.
+
     """
     # verify that Robj is a rotation object
     if not isinstance(Robj, R):
         raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
 
     alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
     d = wigner_d(l, beta)
```

## Comparing `sphecerix-0.2.0.dist-info/METADATA` & `sphecerix-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphecerix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/sphecerix
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

## Comparing `sphecerix-0.2.0.dist-info/RECORD` & `sphecerix-0.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sphecerix/__init__.py,sha256=Qq3BOzEm_wsbEA4Shsh5qz7nDqIl82OxlUtcVCMU078,219
-sphecerix/_version.py,sha256=1KhrBItVjTCR-Sumh0o09b_aKrjTTcJrpTBh5GBw6Lk,21
+sphecerix/_version.py,sha256=tC9CwL4Nm8brVXJnZNGk_eoZaJj6eOtLKtOrdJMrpoI,21
 sphecerix/atomic_wave_functions.py,sha256=VO9_8spYmPvTbRncdG9aPMzjkA3qFTj6jUTJIsOyER0,3394
 sphecerix/tesseral.py,sha256=7ak1E_tsT5IMavEVyNqaNtY64jUdfuecl8IZr2M9Rfc,1220
-sphecerix/wignerd.py,sha256=EqU1rwTH93AwEqBHH4f03VplOVqY1F6Q_XccVsd8DyY,2314
-sphecerix-0.2.0.dist-info/METADATA,sha256=Ew6Q7mwcz0VEg2TW9UDXsQlwXP1ZK0uGXkd6jr9WVVc,2873
-sphecerix-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sphecerix-0.2.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
-sphecerix-0.2.0.dist-info/RECORD,,
+sphecerix/wignerd.py,sha256=MXUOTd1cLyc17I522eaLO75plalRGauIzkRFCI-FmNk,5712
+sphecerix-0.2.1.dist-info/METADATA,sha256=IM2bIOfyc913ibBmQGfho022xodFIkGBn4Iu-XKIL-k,2873
+sphecerix-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sphecerix-0.2.1.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
+sphecerix-0.2.1.dist-info/RECORD,,
```

