# Comparing `tmp/metanum-0.1.0.tar.gz` & `tmp/metanum-0.1.1.tar.gz`

## Comparing `metanum-0.1.0.tar` & `metanum-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metanum-0.1.0/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metanum-0.1.0/metanum/RaizesFuncoes/__init__.py
--rw-r--r--   0        0        0    18399 2020-02-02 00:00:00.000000 metanum-0.1.0/metanum/RaizesFuncoes/metodos_iterativos.py
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metanum-0.1.0/metanum/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 metanum-0.1.0/LICENSE
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 metanum-0.1.0/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 metanum-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 metanum-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metanum-0.1.1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metanum-0.1.1/metanum/RaizesFuncoes/__init__.py
+-rw-r--r--   0        0        0    18420 2020-02-02 00:00:00.000000 metanum-0.1.1/metanum/RaizesFuncoes/metodos_iterativos.py
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 metanum-0.1.1/metanum/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 metanum-0.1.1/LICENSE
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 metanum-0.1.1/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 metanum-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 metanum-0.1.1/PKG-INFO
```

### Comparing `metanum-0.1.0/metanum/RaizesFuncoes/metodos_iterativos.py` & `metanum-0.1.1/metanum/RaizesFuncoes/metodos_iterativos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-#!/usr/bin/env python
-# coding: utf-8
+import sympy as sp
+from sympy.calculus.util import continuous_domain
 
-# In[ ]:
-
-
-def metodo_bisecao(funcao, inicio_intervalo, fim_intervalo, precisao_tipo = 'e1',
+def metodo_bissecao(funcao, inicio_intervalo, fim_intervalo, precisao_tipo = 'e1',
                         precisao = 1e-9, mostre_iteracoes = True, max_iter = 15):
     
     # a função é recebida no formato string e depois desse 'if' muda para objeto sympy
     # por isso, esse bloco só é executado uma vez
     if type(funcao) == str:
         
         global x
```

### Comparing `metanum-0.1.0/metanum/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb` & `metanum-0.1.1/metanum/RaizesFuncoes/.ipynb_checkpoints/metodos_iterativos.py-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `metanum-0.1.0/LICENSE` & `metanum-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metanum-0.1.0/pyproject.toml` & `metanum-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metanum"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Gabriel Martins", email="gabe.hm.ml@gmail.com" },
 ]
 description = "Conjunto de ferramentas para implementação de métodos elementares de análise numérica"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `metanum-0.1.0/PKG-INFO` & `metanum-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metanum
-Version: 0.1.0
+Version: 0.1.1
 Summary: Conjunto de ferramentas para implementação de métodos elementares de análise numérica
 Project-URL: Homepage, https://github.com/GHM-ML/metanum
 Project-URL: Bug Tracker, https://github.com/GHM-ML/metanum/issues
 Author-email: Gabriel Martins <gabe.hm.ml@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,9 +21,13 @@
 Aproximação de raízes de funções de uma variável pelos métodos:
 - Biseção
 - Posição falsa
 - Ponto fixo
 - Newton-Raphson
 - Secante
 
+
+v0.1.1:
+- correção de erros de digitação
+
 # Referência:
 [Cálculo numérico: Aspectos teóricos e computacionais. 2ª Ed. Livro por: Marcia Ruggiero e Vera Lúcia Lopes](https://www.google.com/search?q=C%C3%A1lculo+Num%C3%A9rico:+Aspectos+Te%C3%B3ricos+e+Computacionais&sxsrf=APwXEdfgqS5mIzsXo3Rk-RsZe0XDspg7lA:1685770539697&source=lnms&sa=X&ved=2ahUKEwik18PRsKb_AhWsjZUCHSdsAf4Q_AUoAHoECAoQAg&biw=1292&bih=668&dpr=1)
```

