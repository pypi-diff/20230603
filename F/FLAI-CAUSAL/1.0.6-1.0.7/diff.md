# Comparing `tmp/FLAI_CAUSAL-1.0.6.tar.gz` & `tmp/FLAI_CAUSAL-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.6.tar", last modified: Fri Jun  2 20:18:52 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.0.7.tar", last modified: Sat Jun  3 15:45:33 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.6.tar` & `FLAI_CAUSAL-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/FLAI/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/__init__.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9020 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/causal_graph.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/data.py
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/LICENSE
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      238 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/README.md
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/setup.cfg
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/setup.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/FLAI/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/__init__.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9661 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/causal_graph.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/data.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6746 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/LICENSE
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6746 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6430 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/README.md
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/setup.cfg
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.6/FLAI/causal_graph.py` & `FLAI_CAUSAL-1.0.7/FLAI/causal_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,14 +40,26 @@
                 self.flai_dataset = flai_dataset
                 self.graph = bn.make_DAG(node_edge, CPD=CPD,verbose= verbose)
 
 
     def independence_test(self, flai_dataset, test='chi_square', prune=True,verbose= 0):
         self.graph = bn.independence_test(self.graph, flai_dataset.data, test, prune,verbose= verbose)
 
+    def inference(self,variables = [],evidence = {}):
+        if len(variables) == 0:
+            raise Exception("Variables should be provided") 
+        if len(evidence) == 0:
+            raise Exception("Evidence should be provided")  
+        return bn.inference.fit(self.graph, variables=variables, evidence=evidence).df          
+    def predict(self, data = None, variables = []):
+        if len(variables) == 0:
+            raise Exception("Variables should be provided") 
+        if data is None:
+            raise Exception("Data should be provided") 
+        return bn.predict(self.graph, data, variables = variables)
     def learn_cpd(self, flai_dataset = None, methodtype= None,verbose = 0):
         if methodtype is None:
             methodtype = 'bayes'
         if flai_dataset is None and self.flai_dataset is None:
             raise Exception("Data should be provided")
         if flai_dataset is None: 
             self.graph = bn.parameter_learning.fit(self.graph,  self.flai_dataset.data,methodtype = methodtype,verbose= verbose)
```

### Comparing `FLAI_CAUSAL-1.0.6/FLAI/data.py` & `FLAI_CAUSAL-1.0.7/FLAI/data.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.6/LICENSE` & `FLAI_CAUSAL-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.6/setup.py` & `FLAI_CAUSAL-1.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.6' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.0.7' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
```

