# Comparing `tmp/CDynamics-2.0.2.tar.gz` & `tmp/CDynamics-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDynamics-2.0.2.tar", last modified: Sat Mar  4 13:07:25 2023, max compression
+gzip compressed data, was "CDynamics-2.0.3.tar", last modified: Sat Jun  3 05:38:20 2023, max compression
```

## Comparing `CDynamics-2.0.2.tar` & `CDynamics-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-03-04 13:07:25.729337 CDynamics-2.0.2/
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-03-04 13:07:25.729337 CDynamics-2.0.2/CDynamics/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     4218 2023-03-04 13:05:28.000000 CDynamics-2.0.2/CDynamics/__init__.py
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-03-04 13:07:25.729337 CDynamics-2.0.2/CDynamics.egg-info/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-03-04 13:07:24.000000 CDynamics-2.0.2/CDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      194 2023-03-04 13:07:25.000000 CDynamics-2.0.2/CDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2023-03-04 13:07:25.000000 CDynamics-2.0.2/CDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       17 2023-03-04 13:07:25.000000 CDynamics-2.0.2/CDynamics.egg-info/requires.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       10 2023-03-04 13:07:25.000000 CDynamics-2.0.2/CDynamics.egg-info/top_level.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-03-04 13:07:25.729337 CDynamics-2.0.2/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2023-03-04 13:07:25.729337 CDynamics-2.0.2/setup.cfg
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      744 2023-03-04 13:07:14.000000 CDynamics-2.0.2/setup.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/CDynamics/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     4258 2023-06-03 05:32:24.000000 CDynamics-2.0.3/CDynamics/__init__.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/CDynamics.egg-info/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 05:38:19.000000 CDynamics-2.0.3/CDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      194 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2023-06-03 05:38:19.000000 CDynamics-2.0.3/CDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       23 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/requires.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       10 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 05:38:20.313935 CDynamics-2.0.3/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2023-06-03 05:38:20.313935 CDynamics-2.0.3/setup.cfg
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      760 2023-06-03 05:35:31.000000 CDynamics-2.0.3/setup.py
```

### Comparing `CDynamics-2.0.2/CDynamics/__init__.py` & `CDynamics-2.0.3/CDynamics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import sympy as sp
 import matplotlib.pyplot as plt
 from matplotlib.patches import ConnectionPatch
 
 class Julia:
     def __init__(self,expr):
-        z = sp.symbols('z')
+        self.z = sp.symbols('z')
         self.expr = expr
-        self.eval = sp.lambdify(z,expr)
-        self.fixed_points = [complex(float(sp.re(i)),float(sp.im(i))) for i in sp.solve(expr-z,z)]
-        self.critical_points = [complex(float(sp.re(i)),float(sp.im(i))) for i in sp.solve(expr.diff(),z)]
+        self.eval = sp.lambdify(self.z,expr)
+        self.fixed_points = [complex(float(sp.re(i)),float(sp.im(i))) for i in sp.solve(expr-self.z,self.z)]
+        self.critical_points = [complex(float(sp.re(i)),float(sp.im(i))) for i in sp.solve(expr.diff(),self.z)]
 
     def grid(a,b,c,d,resx,resy):
         xvals = np.linspace(a,b,resx)
         yvals = np.linspace(c,d,resy)
         points = []
         for i in yvals:
             for j in xvals:
@@ -45,19 +45,19 @@
         if filled:
             ol = []
             cfp = []
             for i in points:
                 o = self.orbit(i,depth,bail_out)
                 ol.append(len(o))
                 can = find_nearest(self.fixed_points,o[-1])
-                if (self.expr.limit(z,sp.oo)!=sp.oo) or (self.expr.limit(z,sp.oo)==sp.oo and np.abs(can-o[-1])<1):
+                if (self.expr.limit(self.z,sp.oo)!=sp.oo) or (self.expr.limit(self.z,sp.oo)==sp.oo and np.abs(can-o[-1])<1):
                     cfp.append(can)
                 else:
                     cfp.append(np.inf)
-            if self.expr.limit(z,sp.oo)==sp.oo:
+            if self.expr.limit(self.z,sp.oo)==sp.oo:
                 self.fixed_points.insert(0, np.inf)
             colors = [ (int(cols[self.fixed_points.index(cfp[i])][0]+(ol[i]*glow*0.299)),
                         int(cols[self.fixed_points.index(cfp[i])][1]+(ol[i]*glow*0.587)),
                         int(cols[self.fixed_points.index(cfp[i])][2]+(ol[i]*glow*0.114) )) for i in range(len(points)) ]
             colors = np.asarray(colors).reshape(resy,resx,-1)
             ydim,xdim = colors.shape[:2]
             plt.imshow(colors,aspect=(d-c)/(b-a))
```

### Comparing `CDynamics-2.0.2/setup.py` & `CDynamics-2.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 '''
 setup(
    name="CDynamics",
-   version="2.0.2",
+   version="2.0.3",
    packages=find_packages(),
-   install_requires=['numpy','matplotlib'],
+   install_requires=['numpy','matplotlib','sympy'],
 )
 '''
 
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 DESCRIPTION = 'Plot Julia Sets Of Complex Valued Functions'
 LONG_DESCRIPTION = 'A package that allows users to visualize julia sets of complex-valued holormorhphic self-maps defined on the Riemann sphere.'
 
 setup(
     name="CDynamics",
     version=VERSION,
     author="Kanak Dhotre",
     author_email="dhotrekanak@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['numpy','matplotlib'],
+    install_requires=['numpy','matplotlib','sympy'],
     keywords=['python', 'complex dynamics', 'julia set', 'filled julia sets'],
 )
```

