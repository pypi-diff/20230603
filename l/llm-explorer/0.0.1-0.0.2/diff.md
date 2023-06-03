# Comparing `tmp/llm_explorer-0.0.1.tar.gz` & `tmp/llm_explorer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.1.tar", last modified: Sat Jun  3 02:21:47 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.2.tar", last modified: Sat Jun  3 03:14:35 2023, max compression
```

## Comparing `llm_explorer-0.0.1.tar` & `llm_explorer-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.146076 llm_explorer-0.0.1/explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-03 02:21:47.000000 llm_explorer-0.0.1/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-03 02:21:47.000000 llm_explorer-0.0.1/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 02:21:47.000000 llm_explorer-0.0.1/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 02:21:47.000000 llm_explorer-0.0.1/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 02:21:47.000000 llm_explorer-0.0.1/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 02:21:47.150076 llm_explorer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 02:21:37.000000 llm_explorer-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/test.py
```

### Comparing `llm_explorer-0.0.1/.DS_Store` & `llm_explorer-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/.gitignore` & `llm_explorer-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/LICENSE` & `llm_explorer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/Makefile` & `llm_explorer-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/PKG-INFO` & `llm_explorer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_explorer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,21 @@
 
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+### Pypi
+```shell
+pip install llm-explorer
+```
+
 
+### Build from source
 Create a virtual environment
 
 ```shell
 conda create -n occlusion python=3.10
 conda activate occlusion
 ```
```

### Comparing `llm_explorer-0.0.1/README.md` & `llm_explorer-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+### Pypi
+```shell
+pip install llm-explorer
+```
+
 
+### Build from source
 Create a virtual environment
 
 ```shell
 conda create -n occlusion python=3.10
 conda activate occlusion
 ```
```

### Comparing `llm_explorer-0.0.1/SECURITY.md` & `llm_explorer-0.0.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/__init__.py` & `llm_explorer-0.0.2/llm_explorer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 from pathlib import Path
 
 from dotenv import find_dotenv, load_dotenv
 
 from .chains import TSEConversationChain
 from .chat import chat_loop
 from .interfaces import frontend as it
-from .ui.lang import en, es, ru
+from .ui.lang import en, es
 
 
 def auth():
     import streamlit_authenticator as stauth
     import yaml
     from yaml.loader import SafeLoader
 
-    with open("explorer/auth/access.yaml") as file:
+    with open("llm_explorer/auth/access.yaml") as file:
         config = yaml.load(file, Loader=SafeLoader)
 
     authenticator = stauth.Authenticate(
         config["credentials"],
         config["cookie"]["name"],
         config["cookie"]["key"],
         config["cookie"]["expiry_days"],
@@ -73,15 +73,15 @@
 
 
 load_dotenv(find_dotenv())
 tse_chain = TSEConversationChain()
 
 # --- PATH SETTINGS ---
 current_dir: Path = Path(__file__).parent if "__file__" in locals() else Path.cwd()
-css_file: Path = "explorer/ui/styles/.css"
+css_file: Path = "llm_explorer/ui/styles/.css"
 assets_dir: Path = current_dir / "assets"
 icons_dir: Path = assets_dir / "icons"
 img_dir: Path = assets_dir / "img"
 tg_svg: Path = icons_dir / "tg.svg"
 
 
 # --- LOAD CSS ---
```

### Comparing `llm_explorer-0.0.1/explorer/agents/__init__.py` & `llm_explorer-0.0.2/llm_explorer/agents/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     ZeroShotAgent,
     create_pandas_dataframe_agent,
     initialize_agent,
     load_tools,
 )
 from langchain.agents.load_tools import get_all_tool_names
 
-import explorer.interfaces.frontend as it
-from explorer.templates.agents import agents_templates
-from explorer.templates.prompt import prompt_templates
+import llm_explorer.interfaces.frontend as it
+from llm_explorer.templates.agents import agents_templates
+from llm_explorer.templates.prompt import prompt_templates
 
 load_dotenv(find_dotenv())
 
 
 class TSELLMAgent:
     def __init__(self, agent_id: str = "smart_gpt"):
         self.agent_templates = agents_templates()
@@ -72,15 +72,15 @@
             agent_results = self.execute(query=query, df=df)
             st.success("Completed inferece!")
             st.markdown(f"**Explanation:** {agent_results}")
 
 
 def pandas_agent():
     uploaded_file = it.display_widgets(
-        "explorer/indexes/samples/telemetry_sample_forecast.csv"
+        "llm_explorer/indexes/samples/telemetry_sample_forecast.csv"
     )
     sample_df = pd.read_csv(uploaded_file)
     st.write("Sample of loaded table:")
     st.table(sample_df.head(3))
     # Create the Streamlit dropdown
     option = st.selectbox(
         "Sample Prompt",
```

### Comparing `llm_explorer-0.0.1/explorer/chains/__init__.py` & `llm_explorer-0.0.2/llm_explorer/chains/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import streamlit as st
 from langchain.chains import ConversationalRetrievalChain, LLMChain, RetrievalQA
 from langchain.chains.question_answering import load_qa_chain
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.llms import OpenAI
 from langchain.prompts.prompt import PromptTemplate
 
-from explorer.templates.chains import chains_templates
+from llm_explorer.templates.chains import chains_templates
 
 
 def set_chain(llm, **kwargs):
     condense_question_prompt = PromptTemplate.from_template(
         chains_templates()["snowchat_chain_template"]
     )
     QA_PROMPT = PromptTemplate(
```

### Comparing `llm_explorer-0.0.1/explorer/chat/__init__.py` & `llm_explorer-0.0.2/llm_explorer/chat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import contextlib
 
 import streamlit as st
 from langchain.memory import ConversationBufferMemory
 
-from explorer.agents import ExplorerAgent, HFTAgent
-from explorer.chains import extract_code, is_sql_query
-from explorer.databases.adbddl import ADBDDL
-from explorer.indexes.vectorstore import VectorStoreHandler
-from explorer.templates.chains import chains_templates
-from explorer.templates.ui import session_state_templates
-from explorer.ui import UI
+from llm_explorer.agents import ExplorerAgent, HFTAgent
+from llm_explorer.chains import extract_code, is_sql_query
+from llm_explorer.databases.adbddl import ADBDDL
+from llm_explorer.indexes.vectorstore import VectorStoreHandler
+from llm_explorer.templates.chains import chains_templates
+from llm_explorer.templates.ui import session_state_templates
+from llm_explorer.ui import UI
 
 adb_ddl = ADBDDL()
 agent_database = (
     st.session_state["agent_database"]
     if "agent_database" in st.session_state
     else "default"
 )
```

### Comparing `llm_explorer-0.0.1/explorer/databases/adbddl.py` & `llm_explorer-0.0.2/llm_explorer/databases/adbddl.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def __init__(self):
         self.ddl_dict = self.load_ddls()
 
     @staticmethod
     def load_ddls():
         ddl_files = {
-            "telemetry": "explorer/sql/ddl_tse_telemetry.sql",
+            "telemetry": "llm_explorer/sql/ddl_tse_telemetry.sql",
         }
 
         ddl_dict = {}
         for table_name, file_name in ddl_files.items():
             with open(file_name, "r") as f:
                 ddl_dict[table_name] = f.read()
         return ddl_dict
```

### Comparing `llm_explorer-0.0.1/explorer/indexes/vectorstore.py` & `llm_explorer-0.0.2/llm_explorer/indexes/vectorstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,36 +37,36 @@
 
 @st.cache_resource
 def load_faiss_vectorstore():
     return FAISS.load_local("indexes/faiss_index", embeddings)
 
 
 def faiss_metadata_index_loader(
-    metadata_path: str = "explorer/indexes/metadata/schema.md",
+    metadata_path: str = "llm_explorer/indexes/metadata/schema.md",
     page_content_column: str = "y",
 ):
     loader = UnstructuredMarkdownLoader(metadata_path)
     data = loader.load()
     # df = pd.read_csv(data_path)
     text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=20)
     texts = text_splitter.split_documents(data)
 
     # df_loader = DataFrameLoader(df, page_content_column=page_content_column)
     # docs = df_loader.load()
 
     faiss_store = FAISS.from_documents(texts, embeddings)
     # docsearch.add_documents(docs)
-    faiss_store.save_local("explorer/indexes/faiss_index")
+    faiss_store.save_local("llm_explorer/indexes/faiss_index")
 
     # with open("vectors.pkl", "wb") as f:
     #     pickle.dump(docsearch, f)
 
 
 def pandas_df_vectorstore_loader(
-    data_path: str = "explorer/indexes/samples/telemetry_sample_forecast.csv",
+    data_path: str = "llm_explorer/indexes/samples/telemetry_sample_forecast.csv",
     page_content_column: str = "y",
 ):
     df = pd.read_csv(data_path)
     # jdf = df.to_dict(orient='split')
     loader = DataFrameLoader(df, page_content_column=page_content_column)
     docs = loader.load()
```

### Comparing `llm_explorer-0.0.1/explorer/interfaces/frontend.py` & `llm_explorer-0.0.2/llm_explorer/interfaces/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # import pyautogui
 import streamlit as st
 from streamlit.runtime.uploaded_file_manager import UploadedFile
 
-from explorer.databases.adbddl import ADBDDL
-from explorer.indexes.vectorstore import faiss_metadata_index_loader
-from explorer.ui import UI
+from llm_explorer.databases.adbddl import ADBDDL
+from llm_explorer.indexes.vectorstore import faiss_metadata_index_loader
+from llm_explorer.ui import UI
 
 adb_ddl = ADBDDL()
 
 
 def display_header() -> None:
     # st.image("img/logo.jpg")
     st.title("LLM Explorer")
@@ -63,9 +63,9 @@
         # pyautogui.press("tab")
         # pyautogui.press("down")
     elif choice == "Explorer":
         st.write("Explorer")
     elif choice == "Update Vector Store":
         faiss_metadata_index_loader()
         st.write("Run Update Vector Store")
-    elif choice == "explorer/pages/pandas_agent":
+    elif choice == "llm_explorer/pages/pandas_agent":
         st.write("Run pages/pandas_agent")
```

### Comparing `llm_explorer-0.0.1/explorer/templates/agents.py` & `llm_explorer-0.0.2/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/templates/chains.py` & `llm_explorer-0.0.2/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/templates/prompt.py` & `llm_explorer-0.0.2/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/templates/ui.py` & `llm_explorer-0.0.2/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/ui/__init__.py` & `llm_explorer-0.0.2/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/explorer/ui/lang.py` & `llm_explorer-0.0.2/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/llm_explorer.egg-info/PKG-INFO` & `llm_explorer-0.0.2/llm_explorer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-explorer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,21 @@
 
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+### Pypi
+```shell
+pip install llm-explorer
+```
+
 
+### Build from source
 Create a virtual environment
 
 ```shell
 conda create -n occlusion python=3.10
 conda activate occlusion
 ```
```

### Comparing `llm_explorer-0.0.1/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.2/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/requirements.txt` & `llm_explorer-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.1/setup.py` & `llm_explorer-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.1"
+    version = "0.0.2"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name = package_name + f"_{package_env}"
```

