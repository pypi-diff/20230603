# Comparing `tmp/FLAI_CAUSAL-1.0.8.tar.gz` & `tmp/FLAI_CAUSAL-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.8.tar", last modified: Sat Jun  3 15:51:23 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.0.9.tar", last modified: Sat Jun  3 17:57:07 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.8.tar` & `FLAI_CAUSAL-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/FLAI/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/__init__.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9661 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/causal_graph.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/FLAI/data.py
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6455 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-03 15:51:23.000000 FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/LICENSE
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6455 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     6139 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/README.md
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-03 15:51:23.126744 FLAI_CAUSAL-1.0.8/setup.cfg
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-03 15:50:49.000000 FLAI_CAUSAL-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.962318 FLAI_CAUSAL-1.0.9/FLAI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/causal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.962318 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.8/FLAI_CAUSAL.egg-info/PKG-INFO` & `FLAI_CAUSAL-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
-Name: FLAI-CAUSAL
-Version: 1.0.8
+Name: FLAI_CAUSAL
+Version: 1.0.9
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
+Project-URL: Documentation, https://scikit-learn.org/stable/documentation.html
+Project-URL: Source Code, https://github.com/rugonzs/FLAI
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
@@ -17,15 +19,15 @@
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-[Overview](Documents/fair_algorithm.svg)
+![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -59,26 +61,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-[Original Graph](Documents/original_graph.svg)
+![Original Graph](https://github.com/rugonzs/FLAI/blob/main/Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-[Mitigated Graph.](Documents/mitigated_graph.svg)
+![Mitigated Graph.](https://github.com/rugonzs/FLAI/blob/main/Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -133,15 +135,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-[Correlation in original and Fair Data.](Documents/corr.svg)
+![Correlation in original and Fair Data.](https://github.com/rugonzs/FLAI/blob/main/Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -186,10 +188,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-[shap values.](Documents/shap.svg)
+![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.8/LICENSE` & `FLAI_CAUSAL-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.8/PKG-INFO` & `FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
-Name: FLAI_CAUSAL
-Version: 1.0.8
+Name: FLAI-CAUSAL
+Version: 1.0.9
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
+Project-URL: Documentation, https://scikit-learn.org/stable/documentation.html
+Project-URL: Source Code, https://github.com/rugonzs/FLAI
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
@@ -17,15 +19,15 @@
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-[Overview](Documents/fair_algorithm.svg)
+![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -59,26 +61,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-[Original Graph](Documents/original_graph.svg)
+![Original Graph](https://github.com/rugonzs/FLAI/blob/main/Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-[Mitigated Graph.](Documents/mitigated_graph.svg)
+![Mitigated Graph.](https://github.com/rugonzs/FLAI/blob/main/Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -133,15 +135,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-[Correlation in original and Fair Data.](Documents/corr.svg)
+![Correlation in original and Fair Data.](https://github.com/rugonzs/FLAI/blob/main/Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -186,10 +188,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-[shap values.](Documents/shap.svg)
+![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.8/README.md` & `FLAI_CAUSAL-1.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
 ## Overview
 
-[Overview](Documents/fair_algorithm.svg)
+![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
 
 2. **Bias Mitigation:** Fairness is pursued in two significant areas - **In-Training** and **Pre-Training**.
 
@@ -48,26 +48,26 @@
 import pandas as pd
 
 df = pd.read_pickle('../Data/adult.pickle')
 flai_dataset = data.Data(df, transform=True)
 flai_graph = causal_graph.CausalGraph(flai_dataset, target = 'label')
 flai_graph.plot(directed = True)
 ```
-[Original Graph](Documents/original_graph.svg)
+![Original Graph](https://github.com/rugonzs/FLAI/blob/main/Documents/original_graph.svg)
 
 
 ### Causal Mitigation
 
 #### Relations Mitigation
 
 ```python
 
 flai_graph.mitigate_edge_relation(sensible_feature=['sex','age'])
 ```
-[Mitigated Graph.](Documents/mitigated_graph.svg)
+![Mitigated Graph.](https://github.com/rugonzs/FLAI/blob/main/Documents/mitigated_graph.svg)
 
 #### Table Probabilities Mitigation
 
 ```python
 
 flai_graph.mitigate_calculation_cpd(sensible_feature = ['age','sex'])
 
@@ -122,15 +122,15 @@
 
 
 ### Fair Data
 
 ```python
 fair_data = flai_graph.generate_dataset(n_samples = 1000, methodtype = 'bayes')
 ```
-[Correlation in original and Fair Data.](Documents/corr.svg)
+![Correlation in original and Fair Data.](https://github.com/rugonzs/FLAI/blob/main/Documents/corr.svg)
 
 #### Train Algorithm With Fair Data.
 
 ```python
 from xgboost import XGBClassifier
 from sklearn.model_selection import train_test_split
 
@@ -175,10 +175,10 @@
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-[shap values.](Documents/shap.svg)
+![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap.svg)
 
 ## Citation
```

### Comparing `FLAI_CAUSAL-1.0.8/setup.py` & `FLAI_CAUSAL-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.8' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.0.9' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
-
+PROJECT_URLS = {
+    "Documentation": "https://scikit-learn.org/stable/documentation.html",
+    "Source Code": 'https://github.com/rugonzs/FLAI',
+}
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
       'bnlearn==0.7.8','networkx==2.8.8','matplotlib==3.6.2','pgmpy==0.1.20','numpy==1.23.4', 'pandas==1.5.1','scikit-learn==1.0.2','scipy==1.9.3','statsmodels==0.13.5'
       ]
 
 setup(
@@ -25,12 +28,13 @@
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
+    project_urls=PROJECT_URLS,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
     include_package_data=True
 )
```

