# Comparing `tmp/strategais-0.2.7.tar.gz` & `tmp/strategais-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.7.tar", last modified: Fri Jun  2 15:04:17 2023, max compression
+gzip compressed data, was "strategais-0.2.8.tar", last modified: Fri Jun  2 22:53:05 2023, max compression
```

## Comparing `strategais-0.2.7.tar` & `strategais-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.015421 strategais-0.2.7/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.7/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 15:04:17.015274 strategais-0.2.7/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-02 14:50:13.000000 strategais-0.2.7/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-02 15:04:17.015464 strategais-0.2.7/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1459 2023-06-02 15:03:49.000000 strategais-0.2.7/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.013474 strategais-0.2.7/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-02 14:50:13.000000 strategais-0.2.7/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     4749 2023-06-02 15:03:41.000000 strategais-0.2.7/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.7/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.7/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.014738 strategais-0.2.7/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-02 14:50:13.000000 strategais-0.2.7/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.014586 strategais-0.2.7/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 22:53:05.051500 strategais-0.2.8/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.8/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1325 2023-06-02 22:53:05.051349 strategais-0.2.8/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-02 14:50:13.000000 strategais-0.2.8/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-02 22:53:05.051540 strategais-0.2.8/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1498 2023-06-02 22:48:16.000000 strategais-0.2.8/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 22:53:05.049741 strategais-0.2.8/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-02 14:50:13.000000 strategais-0.2.8/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4749 2023-06-02 15:03:41.000000 strategais-0.2.8/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.8/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.8/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 22:53:05.050913 strategais-0.2.8/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-02 14:50:13.000000 strategais-0.2.8/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 22:53:05.050768 strategais-0.2.8/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1325 2023-06-02 22:53:05.000000 strategais-0.2.8/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-02 22:53:05.000000 strategais-0.2.8/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-02 22:53:05.000000 strategais-0.2.8/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      486 2023-06-02 22:53:05.000000 strategais-0.2.8/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-02 22:53:05.000000 strategais-0.2.8/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.7/LICENSE` & `strategais-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.7/PKG-INFO` & `strategais-0.2.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
+Provides-Extra: ext
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
 
 ```pip install strategais```
```

### Comparing `strategais-0.2.7/README.md` & `strategais-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.2.7/setup.py` & `strategais-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.7', 
+    version='0.2.8', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html', 'static/*.js', 'static/*.css' , 'models/*.sav']},
     install_requires=[
         'fastapi',
@@ -23,24 +23,21 @@
         'requests',
         'scikit-learn',
         'scipy',
         'SQLAlchemy',
         'pydantic',
         'aiofiles',
         'psycopg2-binary',
-        'watchdog[watchmedo]',
         'email-validator',
-        'boto3',
         'jinja2',
         'python-multipart',
         'httpx',
         'sse-starlette',
         'langchain',
         'python-dotenv',
-        'openai',
         'huggingface_hub',
         'chromadb',
         'redis',
         'sentence_transformers',
         'unstructured',
         'pydantic',
         'datasets', 
@@ -50,9 +47,12 @@
         'pytorch-lightning',
         'torch',
         'accelerate',
         'torchaudio',
         'cryptography==38.0.4',
         'xformers==0.0.12'
     ],
+    extras_require={
+        'ext': ['openai', 'boto3', 'email-validator', 'watchdog[watchmedo]'],
+    }
 )
```

### Comparing `strategais-0.2.7/strategais/__main__.py` & `strategais-0.2.8/strategais/__main__.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.7/strategais/save_tools.py` & `strategais-0.2.8/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.7/strategais/templates/index.html` & `strategais-0.2.8/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.7/strategais.egg-info/PKG-INFO` & `strategais-0.2.8/strategais.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
+Provides-Extra: ext
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
 
 ```pip install strategais```
```

