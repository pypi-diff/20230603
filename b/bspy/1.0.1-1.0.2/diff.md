# Comparing `tmp/bspy-1.0.1.tar.gz` & `tmp/bspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspy-1.0.1.tar", last modified: Wed May 31 23:45:55 2023, max compression
+gzip compressed data, was "bspy-1.0.2.tar", last modified: Sat Jun  3 18:01:57 2023, max compression
```

## Comparing `bspy-1.0.1.tar` & `bspy-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.997211 bspy-1.0.1/
--rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3624 2023-05-31 23:45:54.998208 bspy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2509 2023-05-31 22:33:10.000000 bspy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.947148 bspy-1.0.1/bspy/
--rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.0.1/bspy/__init__.py
--rw-rw-rw-   0        0        0    26824 2023-05-27 22:15:48.000000 bspy-1.0.1/bspy/_spline_domain.py
--rw-rw-rw-   0        0        0     5094 2023-05-27 22:11:33.000000 bspy-1.0.1/bspy/_spline_evaluation.py
--rw-rw-rw-   0        0        0     6951 2023-05-30 15:31:32.000000 bspy-1.0.1/bspy/_spline_fitting.py
--rw-rw-rw-   0        0        0     3394 2023-05-27 22:15:35.000000 bspy-1.0.1/bspy/_spline_intersection.py
--rw-rw-rw-   0        0        0    30613 2023-05-27 22:16:57.000000 bspy-1.0.1/bspy/_spline_operations.py
--rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.0.1/bspy/bspyApp.py
--rw-rw-rw-   0        0        0    16737 2022-03-07 01:45:17.000000 bspy-1.0.1/bspy/drawableSpline.py
--rw-rw-rw-   0        0        0    45950 2023-05-31 22:01:34.000000 bspy-1.0.1/bspy/spline.py
--rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.0.1/bspy/splineOpenGLFrame.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.975733 bspy-1.0.1/bspy.egg-info/
--rw-rw-rw-   0        0        0     3624 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1111 2023-05-31 23:45:55.001214 bspy-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.994212 bspy-1.0.1/tests/
--rw-rw-rw-   0        0        0    66440 2023-05-30 15:34:50.000000 bspy-1.0.1/tests/test_bspy.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3624 2023-06-03 18:01:57.675293 bspy-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2023-05-31 22:33:10.000000 bspy-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.650320 bspy-1.0.2/bspy/
+-rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.0.2/bspy/__init__.py
+-rw-rw-rw-   0        0        0    26824 2023-05-27 22:15:48.000000 bspy-1.0.2/bspy/_spline_domain.py
+-rw-rw-rw-   0        0        0     5094 2023-05-27 22:11:33.000000 bspy-1.0.2/bspy/_spline_evaluation.py
+-rw-rw-rw-   0        0        0     6951 2023-05-30 15:31:32.000000 bspy-1.0.2/bspy/_spline_fitting.py
+-rw-rw-rw-   0        0        0     3394 2023-05-27 22:15:35.000000 bspy-1.0.2/bspy/_spline_intersection.py
+-rw-rw-rw-   0        0        0    30613 2023-05-27 22:16:57.000000 bspy-1.0.2/bspy/_spline_operations.py
+-rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.0.2/bspy/bspyApp.py
+-rw-rw-rw-   0        0        0    16737 2022-03-07 01:45:17.000000 bspy-1.0.2/bspy/drawableSpline.py
+-rw-rw-rw-   0        0        0    47566 2023-06-03 17:57:12.000000 bspy-1.0.2/bspy/spline.py
+-rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.0.2/bspy/splineOpenGLFrame.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/bspy.egg-info/
+-rw-rw-rw-   0        0        0     3624 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1111 2023-06-03 18:01:57.690966 bspy-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/tests/
+-rw-rw-rw-   0        0        0    66430 2023-06-03 17:50:05.000000 bspy-1.0.2/tests/test_bspy.py
```

### Comparing `bspy-1.0.1/LICENSE` & `bspy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/PKG-INFO` & `bspy-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.0.1/README.md` & `bspy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/__init__.py` & `bspy-1.0.2/bspy/__init__.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/_spline_domain.py` & `bspy-1.0.2/bspy/_spline_domain.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/_spline_evaluation.py` & `bspy-1.0.2/bspy/_spline_evaluation.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/_spline_fitting.py` & `bspy-1.0.2/bspy/_spline_fitting.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/_spline_intersection.py` & `bspy-1.0.2/bspy/_spline_intersection.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/_spline_operations.py` & `bspy-1.0.2/bspy/_spline_operations.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/bspyApp.py` & `bspy-1.0.2/bspy/bspyApp.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/drawableSpline.py` & `bspy-1.0.2/bspy/drawableSpline.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy/spline.py` & `bspy-1.0.2/bspy/spline.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,40 +163,44 @@
 
         Parameters
         ----------
         other : `Spline`
             The spline to add to self. The number of dependent variables must match self.
 
         indMap : `iterable` or `None`, optional
-            An iterable of pairs of indices. 
-            Each pair (n, m) maps the nth independent variable of self to the mth independent variable of other. 
-            The domains of the nth and mth independent variables must match. 
-            An independent variable can map to no more than one other independent variable.
+            An iterable of indices or pairs of indices. Each index refers to an independent variable.
+            Within the iterable, a single index, `n`, maps the nth independent variable of self to the same independent variable of other.
+            A pair `(n, m)` maps the nth independent variable of self to the mth independent variable of other. 
+            For example, if you wanted to compute `self(u, v, w) + other(u, w)`, you'd pass `[0, (2, 1)]` for `indMap`. 
             Unmapped independent variables remain independent (the default).
+            The domains of mapped independent variables must match. 
+            An independent variable can map to no more than one other independent variable.
 
         Returns
         -------
         spline : `Spline`
-            The result of adding other to self.
+            The result of adding self and other.
 
         See Also
         --------
         `subtract` : Subtract two splines.
         `multiply` : Multiply two splines.
-        `common_basis : Align a collection of splines to a common basis, elevating the order and adding knots as needed.
+        `common_basis` : Align a collection of splines to a common basis, elevating the order and adding knots as needed.
 
         Notes
         -----
         Uses `common_basis` to ensure mapped variables share the same order and knots. 
         """
+        if indMap is not None:
+            indMap = [mapping if _isIterable(mapping) else (mapping, mapping) for mapping in indMap]
         return bspy._spline_operations.add(self, other, indMap)
 
     def blossom(self, uvw):
         """
-        Compute the blossom of the spline at a given parameter values.
+        Compute the blossom of the spline at given parameter values.
 
         Parameters
         ----------
         uvwValues : `iterable`
             An iterable of length `nInd` that specifies the degree-sized vectors of blossom parameters for each independent variable.
 
         Returns
@@ -319,15 +323,15 @@
         """
         Contract a spline by assigning a fixed value to one or more of its independent variables.
 
         Parameters
         ----------
         uvw : `iterable`
             An iterable of length `nInd` that specifies the values of each independent variable to contract.
-            A value of `None` for an independent variables indicates that variable should remain unchanged.
+            A value of `None` for an independent variable indicates that variable should remain unchanged.
 
         Returns
         -------
         spline : `Spline`
             The contracted spline.
 
         See Also
@@ -342,42 +346,44 @@
 
         Parameters
         ----------
         other : `Spline`
             The spline to convolve with self.
 
         indMap : `iterable` or `None`, optional
-            An iterable of pairs of indices. 
-            Each pair (n, m) maps the nth independent variable of self to the mth independent variable of other. 
-            An independent variable can map to no more than one other independent variable.
+            An iterable of indices or pairs of indices. Each index refers to an independent variable.
+            Within the iterable, a single index, `n`, maps the nth independent variable of self to the same independent variable of other.
+            A pair `(n, m)` maps the nth independent variable of self to the mth independent variable of other. 
+            For example, if you wanted to convolve `self(u, v, w)` with `other(u, w)`, you'd pass `[0, (2, 1)]` for `indMap`. 
             Unmapped independent variables remain independent (the default).
+            An independent variable can map to no more than one other independent variable.
 
         productType : {'C', 'D', 'S'}, optional
             The type of product to perform on the dependent variables (default is 'S').
                 'C' is for a cross product, self x other (nDep must be 2 or 3).
                 'D' is for a dot product (nDep must match).
                 'S' is for a scalar product (nDep must be 1 for one of the splines).
         
         Returns
         -------
         spline : `Spline`
-            The result of convolving other with self.
+            The result of convolving self with other.
 
         See Also
         --------
         `multiply` : Multiply two splines (cross, dot, or scalar product).
         `integrate` : Integrate a spline with respect to one of its independent variables, returning the resulting spline.
 
         Notes
         -----
         Taken in part from Lee, E. T. Y. "Computing a chain of blossoms, with application to products of splines." 
         Computer Aided Geometric Design 11, no. 6 (1994): 597-620.
         """
         if indMap is not None:
-            indMap = [(*mapping, True) for mapping in indMap]
+            indMap = [(*(mapping if _isIterable(mapping) else (mapping, mapping)), True) for mapping in indMap]
         return bspy._spline_operations.multiplyAndConvolve(self, other, indMap, productType)
 
     def cross(self, vector):
         """
         Cross product a spline with `nDep` of 2 or 3 by the given vector.
 
         Parameters
@@ -800,44 +806,46 @@
 
         Parameters
         ----------
         other : `Spline`
             The spline to multiply by self.
 
         indMap : `iterable` or `None`, optional
-            An iterable of pairs of indices. 
-            Each pair (n, m) maps the nth independent variable of self to the mth independent variable of other. 
-            The domains of the nth and mth independent variables must match. 
-            An independent variable can map to no more than one other independent variable.
+            An iterable of indices or pairs of indices. Each index refers to an independent variable.
+            Within the iterable, a single index, `n`, maps the nth independent variable of self to the same independent variable of other.
+            A pair `(n, m)` maps the nth independent variable of self to the mth independent variable of other. 
+            For example, if you wanted to compute `self(u, v, w) * other(u, w)`, you'd pass `[0, (2, 1)]` for `indMap`. 
             Unmapped independent variables remain independent (the default).
+            The domains of mapped independent variables must match. 
+            An independent variable can map to no more than one other independent variable.
 
         productType : {'C', 'D', 'S'}, optional
             The type of product to perform on the dependent variables (default is 'S').
                 'C' is for a cross product, self x other (nDep must be 2 or 3).
                 'D' is for a dot product (nDep must match).
                 'S' is for a scalar product (nDep must be 1 for one of the splines).
         
         Returns
         -------
         spline : `Spline`
-            The result of multiplying other to self.
+            The result of multiplying self and other.
 
         See Also
         --------
         `add` : Add two splines.
         `subtract` : Subtract two splines.
         `convolve` : Convolve two splines (cross, dot, or scalar product).
 
         Notes
         -----
         Taken in part from Lee, E. T. Y. "Computing a chain of blossoms, with application to products of splines." 
         Computer Aided Geometric Design 11, no. 6 (1994): 597-620.
         """
         if indMap is not None:
-            indMap = [(*mapping, False) for mapping in indMap]
+            indMap = [(*(mapping if _isIterable(mapping) else (mapping, mapping)), False) for mapping in indMap]
         return bspy._spline_operations.multiplyAndConvolve(self, other, indMap, productType)
 
     def range_bounds(self):
         """
         Return the range of a spline as upper and lower bounds on each of the
         dependent variables
         """
@@ -943,35 +951,39 @@
 
         Parameters
         ----------
         other : `Spline`
             The spline to subtract from self. The number of dependent variables must match self.
 
         indMap : `iterable` or `None`, optional
-            An iterable of pairs of indices. 
-            Each pair (n, m) maps the nth independent variable of self to the mth independent variable of other. 
-            The domains of the nth and mth independent variables must match. 
-            An independent variable can map to no more than one other independent variable.
+            An iterable of indices or pairs of indices. Each index refers to an independent variable.
+            Within the iterable, a single index, `n`, maps the nth independent variable of self to the same independent variable of other.
+            A pair `(n, m)` maps the nth independent variable of self to the mth independent variable of other. 
+            For example, if you wanted to compute `self(u, v, w) - other(u, w)`, you'd pass `[0, (2, 1)]` for `indMap`. 
             Unmapped independent variables remain independent (the default).
+            The domains of mapped independent variables must match. 
+            An independent variable can map to no more than one other independent variable.
 
         Returns
         -------
         spline : `Spline`
             The result of subtracting other from self.
 
         See Also
         --------
         `add` : Add two splines.
         `multiply` : Multiply two splines.
-        `common_basis : Align a collection of splines to a common basis, elevating the order and adding knots as needed.
+        `common_basis` : Align a collection of splines to a common basis, elevating the order and adding knots as needed.
 
         Notes
         -----
         Uses `common_basis` to ensure mapped variables share the same order and knots. 
         """
+        if indMap is not None:
+            indMap = [mapping if _isIterable(mapping) else (mapping, mapping) for mapping in indMap]
         return self.add(other.scale(-1.0), indMap)
 
     def transform(self, matrix, maxSingularValue=None):
         """
         Transform a spline by the given matrix.
 
         Parameters
```

### Comparing `bspy-1.0.1/bspy/splineOpenGLFrame.py` & `bspy-1.0.2/bspy/splineOpenGLFrame.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.1/bspy.egg-info/PKG-INFO` & `bspy-1.0.2/bspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.0.1/setup.cfg` & `bspy-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7370 790d 0a76 6572 7369 6f6e   = bspy..version
-00000020: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
+00000020: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
 00000030: 203d 2045 7269 6320 4272 6563 686e 6572   = Eric Brechner
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2065 7269 6362 7265 6340 6d73 6e2e 636f   ericbrec@msn.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 204c 6962 7261 7279 2066 6f72 206d 616e   Library for man
 00000080: 6970 756c 6174 696e 6720 616e 6420 7265  ipulating and re
 00000090: 6e64 6572 696e 6720 6e6f 6e2d 756e 6966  ndering non-unif
```

### Comparing `bspy-1.0.1/tests/test_bspy.py` & `bspy-1.0.2/tests/test_bspy.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     maxerror = 0.0
     spline1 = bspy.Spline(1, 2, (5,), (5,), [np.array([0, 0, 0, 0, 0.2, 0.5, 0.5, 1, 1, 1], float)], 
         np.array(((100, 260), (260, 100), (580, 260), (260, 420), (420, 100)), float))
     spline2 = bspy.Spline(1, 2, (4,), (6,), [np.array([0, 0, 0, 0.2, 0.3, 0.4, 0.5, 0.5, 1, 1], float)], 
         np.array(((260, 100), (100, 260), (260, 420), (420, 420), (580, 260), (420, 100)), float))
     
     # Add with shared independent variable.
-    added = spline1.add(spline2, [[0, 0]])
+    added = spline1.add(spline2, [0])
     maxerror = 0.0
     for u in np.linspace(spline1.knots[0][spline1.order[0]-1], spline1.knots[0][spline1.nCoef[0]], 100):
         [x, y] = spline1.evaluate([u]) + spline2.evaluate([u])
         [xTest, yTest] = added.evaluate([u])
         maxerror = max(maxerror, (xTest - x) ** 2 + (yTest - y) ** 2)
     assert maxerror <= np.finfo(float).eps
 
@@ -797,15 +797,15 @@
     maxerror = 0.0
     spline1 = bspy.Spline(1, 2, (5,), (5,), [np.array([0, 0, 0, 0, 0.2, 0.5, 0.5, 1, 1, 1], float)], 
         np.array(((100, 260), (260, 100), (580, 260), (260, 420), (420, 100)), float))
     spline2 = bspy.Spline(1, 2, (4,), (6,), [np.array([0, 0, 0, 0.2, 0.3, 0.4, 0.5, 0.5, 1, 1], float)], 
         np.array(((260, 100), (100, 260), (260, 420), (420, 420), (580, 260), (420, 100)), float))
     
     # Multiply with shared independent variable.
-    multiplied = spline1.multiply(spline2, [[0, 0]], 'D')
+    multiplied = spline1.multiply(spline2, [0], 'D')
     maxerror = 0.0
     for u in np.linspace(spline1.knots[0][spline1.order[0]-1], spline1.knots[0][spline1.nCoef[0]], 100):
         x = np.dot(spline1.evaluate([u]), spline2.evaluate([u]))
         xTest = multiplied.evaluate([u])
         maxerror = max(maxerror, (xTest - x) ** 2)
     assert maxerror <= np.finfo(float).eps
```

