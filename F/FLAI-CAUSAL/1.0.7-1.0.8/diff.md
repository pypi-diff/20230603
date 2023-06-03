# Comparing `tmp/FLAI_CAUSAL-1.0.7.tar.gz` & `tmp/FLAI_CAUSAL-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.7.tar", last modified: Sat Jun  3 15:45:33 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.0.8.tar", last modified: Sat Jun  3 15:51:23 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.7.tar` & `FLAI_CAUSAL-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/FLAI/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/__init__.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9661 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/causal_graph.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/FLAI/data.py
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6746 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-03 15:45:33.000000 FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/LICENSE
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6746 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6430 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/README.md
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-03 15:45:33.103320 FLAI_CAUSAL-1.0.7/setup.cfg
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-03 15:44:36.000000 FLAI_CAUSAL-1.0.7/setup.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/FLAI/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/__init__.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9661 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/causal_graph.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/data.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6455 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/LICENSE
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6455 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6139 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/README.md
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/setup.cfg
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.7/FLAI/causal_graph.py` & `FLAI_CAUSAL-1.0.8/FLAI/causal_graph.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.7/FLAI/data.py` & `FLAI_CAUSAL-1.0.8/FLAI/data.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.7/FLAI_CAUSAL.egg-info/PKG-INFO` & `FLAI_CAUSAL-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
-Name: FLAI-CAUSAL
-Version: 1.0.7
+Name: FLAI_CAUSAL
+Version: 1.0.8
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<meta name="author" content="Rubén González"/>
-<meta name="description" content="mitigate bias and discrimination through the application of causal algorithms."/>
-<meta name="copyright" content="Rubén González 2022"/>
-<meta name="keywords" content="causal, bayes, fairness, bias"/>
+
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
-![Demo](https://www.rubengonzalez.ai/demo)
+[Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-![Overview](Documents/fair_algorithm.svg)
+[Overview](Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -62,26 +59,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-![Original Graph](Documents/original_graph.svg)
+[Original Graph](Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-![Mitigated Graph.](Documents/mitigated_graph.svg)
+[Mitigated Graph.](Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -136,15 +133,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-![Correlation in original and Fair Data.](Documents/corr.svg)
+[Correlation in original and Fair Data.](Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -189,10 +186,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-![shap values.](Documents/shap.svg)
+[shap values.](Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.7/LICENSE` & `FLAI_CAUSAL-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.7/PKG-INFO` & `FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
-Name: FLAI_CAUSAL
-Version: 1.0.7
+Name: FLAI-CAUSAL
+Version: 1.0.8
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<meta name="author" content="Rubén González"/>
-<meta name="description" content="mitigate bias and discrimination through the application of causal algorithms."/>
-<meta name="copyright" content="Rubén González 2022"/>
-<meta name="keywords" content="causal, bayes, fairness, bias"/>
+
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
-![Demo](https://www.rubengonzalez.ai/demo)
+[Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-![Overview](Documents/fair_algorithm.svg)
+[Overview](Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -62,26 +59,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-![Original Graph](Documents/original_graph.svg)
+[Original Graph](Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-![Mitigated Graph.](Documents/mitigated_graph.svg)
+[Mitigated Graph.](Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -136,15 +133,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-![Correlation in original and Fair Data.](Documents/corr.svg)
+[Correlation in original and Fair Data.](Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -189,10 +186,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-![shap values.](Documents/shap.svg)
+[shap values.](Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.7/README.md` & `FLAI_CAUSAL-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-<meta name="author" content="Rubén González"/>
-<meta name="description" content="mitigate bias and discrimination through the application of causal algorithms."/>
-<meta name="copyright" content="Rubén González 2022"/>
-<meta name="keywords" content="causal, bayes, fairness, bias"/>
+
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
-![Demo](https://www.rubengonzalez.ai/demo)
+[Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-![Overview](Documents/fair_algorithm.svg)
+[Overview](Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -51,26 +48,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-![Original Graph](Documents/original_graph.svg)
+[Original Graph](Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-![Mitigated Graph.](Documents/mitigated_graph.svg)
+[Mitigated Graph.](Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -125,15 +122,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-![Correlation in original and Fair Data.](Documents/corr.svg)
+[Correlation in original and Fair Data.](Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -178,10 +175,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-![shap values.](Documents/shap.svg)
+[shap values.](Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.7/setup.py` & `FLAI_CAUSAL-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.7' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.0.8' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
```

