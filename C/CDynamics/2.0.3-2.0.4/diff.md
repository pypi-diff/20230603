# Comparing `tmp/CDynamics-2.0.3.tar.gz` & `tmp/CDynamics-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDynamics-2.0.3.tar", last modified: Sat Jun  3 05:38:20 2023, max compression
+gzip compressed data, was "CDynamics-2.0.4.tar", last modified: Sat Jun  3 09:13:59 2023, max compression
```

## Comparing `CDynamics-2.0.3.tar` & `CDynamics-2.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/CDynamics/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     4258 2023-06-03 05:32:24.000000 CDynamics-2.0.3/CDynamics/__init__.py
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 05:38:20.313935 CDynamics-2.0.3/CDynamics.egg-info/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 05:38:19.000000 CDynamics-2.0.3/CDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      194 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2023-06-03 05:38:19.000000 CDynamics-2.0.3/CDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       23 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/requires.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       10 2023-06-03 05:38:20.000000 CDynamics-2.0.3/CDynamics.egg-info/top_level.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 05:38:20.313935 CDynamics-2.0.3/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2023-06-03 05:38:20.313935 CDynamics-2.0.3/setup.cfg
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      760 2023-06-03 05:35:31.000000 CDynamics-2.0.3/setup.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 09:13:59.149720 CDynamics-2.0.4/
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 09:13:59.149720 CDynamics-2.0.4/CDynamics/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     4346 2023-06-03 09:13:34.000000 CDynamics-2.0.4/CDynamics/__init__.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2023-06-03 09:13:59.149720 CDynamics-2.0.4/CDynamics.egg-info/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 09:13:58.000000 CDynamics-2.0.4/CDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      194 2023-06-03 09:13:59.000000 CDynamics-2.0.4/CDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2023-06-03 09:13:58.000000 CDynamics-2.0.4/CDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       23 2023-06-03 09:13:58.000000 CDynamics-2.0.4/CDynamics.egg-info/requires.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       10 2023-06-03 09:13:58.000000 CDynamics-2.0.4/CDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      387 2023-06-03 09:13:59.149720 CDynamics-2.0.4/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2023-06-03 09:13:59.149720 CDynamics-2.0.4/setup.cfg
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      760 2023-06-03 09:13:46.000000 CDynamics-2.0.4/setup.py
```

### Comparing `CDynamics-2.0.3/CDynamics/__init__.py` & `CDynamics-2.0.4/CDynamics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,22 @@
             for j in xvals:
                 points.append(complex(j,i))
         return(points)
     
     def orbit(self,seed,depth,bail_out):
         o = [seed]
         for i in range(depth):
-            z = self.eval(o[-1])
-            if abs(z)<bail_out:
-                o.append(z)
-            else:
-                break
+            try:
+                z = self.eval(o[-1])
+                if abs(z)<bail_out:
+                    o.append(z)
+                else:
+                    break
+            except Exception:
+                pass
         return(o)
     
     def plot(self,a=-1,b=1,c=-1,d=1,resx=300,resy=300,depth=25,bail_out=1000,filled=True,glow=0,cmap='binary',
              scale=1,grid=True,critical_orbit_depth=0,fixed_points=True,
              cols=[(61, 64, 91),(244, 241, 222), (224, 122, 95),(129, 178, 154),(242, 204, 143)]):
         def plot_orbit(orb):
             orb_mod = [[(orb[i].real+b)*(resx/(b-a)),(orb[i].imag+d)*(resy/(d-c))] for i in range(len(orb))]
```

### Comparing `CDynamics-2.0.3/setup.py` & `CDynamics-2.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 '''
 setup(
    name="CDynamics",
-   version="2.0.3",
+   version="2.0.4",
    packages=find_packages(),
    install_requires=['numpy','matplotlib','sympy'],
 )
 '''
 
-VERSION = '2.0.3'
+VERSION = '2.0.4'
 DESCRIPTION = 'Plot Julia Sets Of Complex Valued Functions'
 LONG_DESCRIPTION = 'A package that allows users to visualize julia sets of complex-valued holormorhphic self-maps defined on the Riemann sphere.'
 
 setup(
     name="CDynamics",
     version=VERSION,
     author="Kanak Dhotre",
```

