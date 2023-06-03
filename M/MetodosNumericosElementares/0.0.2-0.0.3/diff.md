# Comparing `tmp/metodosnumericoselementares-0.0.2.tar.gz` & `tmp/metodosnumericoselementares-0.0.3.tar.gz`

## Comparing `metodosnumericoselementares-0.0.2.tar` & `metodosnumericoselementares-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/src/AproximacoesRaizes/__init__.py
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/src/AproximacoesRaizes/metodos_iterativos.py
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/src/AproximacoesRaizes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/LICENSE
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/README.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/src/AproximacoesRaizes/__init__.py
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/src/AproximacoesRaizes/metodos_iterativos.py
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/src/AproximacoesRaizes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/LICENSE
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 metodosnumericoselementares-0.0.3/PKG-INFO
```

### Comparing `metodosnumericoselementares-0.0.2/src/AproximacoesRaizes/metodos_iterativos.py` & `metodosnumericoselementares-0.0.3/src/AproximacoesRaizes/metodos_iterativos.py`

 * *Files identical despite different names*

### Comparing `metodosnumericoselementares-0.0.2/src/AproximacoesRaizes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb` & `metodosnumericoselementares-0.0.3/src/AproximacoesRaizes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `metodosnumericoselementares-0.0.2/LICENSE` & `metodosnumericoselementares-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metodosnumericoselementares-0.0.2/README.md` & `metodosnumericoselementares-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metodosnumericoselementares-0.0.2/pyproject.toml` & `metodosnumericoselementares-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MetodosNumericosElementares"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gabriel Martins", email="gabe.hm.ml@gmail.com" },
 ]
 description = "Conjunto de ferramentas para implementação de métodos elementares de análise numérica"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `metodosnumericoselementares-0.0.2/PKG-INFO` & `metodosnumericoselementares-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: MetodosNumericosElementares
-Version: 0.0.2
+Version: 0.0.3
 Summary: Conjunto de ferramentas para implementação de métodos elementares de análise numérica
 Project-URL: Homepage, https://github.com/GHM-ML/MetodosNumericosElementares
 Project-URL: Bug Tracker, https://github.com/GHM-ML/MetodosNumericosElementares/issues
 Author-email: Gabriel Martins <gabe.hm.ml@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Métodos Numéricos Elementares
 
 Implementação dos métodos elementares de análise numérica em python.
 ## Ferramentas disponíveis:
```

