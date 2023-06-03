# Comparing `tmp/metodosanalisenumerica-0.0.1.tar.gz` & `tmp/metodosanalisenumerica-0.1.0.tar.gz`

## Comparing `metodosanalisenumerica-0.0.1.tar` & `metodosanalisenumerica-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/src/RaizesFuncoes/__init__.py
--rw-r--r--   0        0        0    18399 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/src/RaizesFuncoes/metodos_iterativos.py
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/src/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/LICENSE
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/src/RaizesFuncoes/__init__.py
+-rw-r--r--   0        0        0    18399 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/src/RaizesFuncoes/metodos_iterativos.py
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/src/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/LICENSE
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 metodosanalisenumerica-0.1.0/PKG-INFO
```

### Comparing `metodosanalisenumerica-0.0.1/src/RaizesFuncoes/metodos_iterativos.py` & `metodosanalisenumerica-0.1.0/src/RaizesFuncoes/metodos_iterativos.py`

 * *Files identical despite different names*

### Comparing `metodosanalisenumerica-0.0.1/src/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb` & `metodosanalisenumerica-0.1.0/src/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `metodosanalisenumerica-0.0.1/LICENSE` & `metodosanalisenumerica-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metodosanalisenumerica-0.0.1/README.md` & `metodosanalisenumerica-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Métodos Numéricos Elementares
 
 Implementação dos métodos elementares de análise numérica em python.
 ## Ferramentas disponíveis:
 
-v0.0.1:
+v0.1.0:
+Aproximação de raízes de funções de uma variável:
 - Biseção
 - Posição falsa
 - Ponto fixo
 - Newton Raphson
 - Secante
 
 # Referência:
```

### Comparing `metodosanalisenumerica-0.0.1/pyproject.toml` & `metodosanalisenumerica-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MetodosAnaliseNumerica"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Gabriel Martins", email="gabe.hm.ml@gmail.com" },
 ]
 description = "Conjunto de ferramentas para implementação de métodos elementares de análise numérica"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `metodosanalisenumerica-0.0.1/PKG-INFO` & `metodosanalisenumerica-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetodosAnaliseNumerica
-Version: 0.0.1
+Version: 0.1.0
 Summary: Conjunto de ferramentas para implementação de métodos elementares de análise numérica
 Project-URL: Homepage, https://github.com/GHM-ML/Metodos-Numericos
 Project-URL: Bug Tracker, https://github.com/GHM-ML/Metodos-Numericos/issues
 Author-email: Gabriel Martins <gabe.hm.ml@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,16 @@
 Description-Content-Type: text/markdown
 
 # Métodos Numéricos Elementares
 
 Implementação dos métodos elementares de análise numérica em python.
 ## Ferramentas disponíveis:
 
-v0.0.1:
+v0.1.0:
+Aproximação de raízes de funções de uma variável:
 - Biseção
 - Posição falsa
 - Ponto fixo
 - Newton Raphson
 - Secante
 
 # Referência:
```

