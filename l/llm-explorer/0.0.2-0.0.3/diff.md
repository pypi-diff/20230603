# Comparing `tmp/llm_explorer-0.0.2.tar.gz` & `tmp/llm_explorer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.2.tar", last modified: Sat Jun  3 03:14:35 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.3.tar", last modified: Sat Jun  3 04:21:33 2023, max compression
```

## Comparing `llm_explorer-0.0.2.tar` & `llm_explorer-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.932850 llm_explorer-0.0.2/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 03:14:35.000000 llm_explorer-0.0.2/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 03:14:35.936850 llm_explorer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 03:14:26.000000 llm_explorer-0.0.2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/test.py
```

### Comparing `llm_explorer-0.0.2/.DS_Store` & `llm_explorer-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/.gitignore` & `llm_explorer-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/LICENSE` & `llm_explorer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/Makefile` & `llm_explorer-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/PKG-INFO` & `llm_explorer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_explorer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+**Important** This package requires **Open AI & HuggingFace API key**
+
 ### Pypi
 ```shell
 pip install llm-explorer
 ```
 
 
 ### Build from source
```

### Comparing `llm_explorer-0.0.2/README.md` & `llm_explorer-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+**Important** This package requires **Open AI & HuggingFace API key**
+
 ### Pypi
 ```shell
 pip install llm-explorer
 ```
 
 
 ### Build from source
```

### Comparing `llm_explorer-0.0.2/SECURITY.md` & `llm_explorer-0.0.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/__init__.py` & `llm_explorer-0.0.3/llm_explorer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     },
 )
 
 from pathlib import Path
 
 from dotenv import find_dotenv, load_dotenv
 
-from .chains import TSEConversationChain
+from .chains import ExplorerConversationChain
 from .chat import chat_loop
 from .interfaces import frontend as it
 from .ui.lang import en, es
 
 
 def auth():
     import streamlit_authenticator as stauth
@@ -69,15 +69,15 @@
         st.error("Username/password is incorrect")
         return False
     elif authentication_status is None:
         st.warning("Please enter your username and password")
 
 
 load_dotenv(find_dotenv())
-tse_chain = TSEConversationChain()
+chain = ExplorerConversationChain()
 
 # --- PATH SETTINGS ---
 current_dir: Path = Path(__file__).parent if "__file__" in locals() else Path.cwd()
 css_file: Path = "llm_explorer/ui/styles/.css"
 assets_dir: Path = current_dir / "assets"
 icons_dir: Path = assets_dir / "icons"
 img_dir: Path = assets_dir / "img"
@@ -119,14 +119,14 @@
 #     st.session_state.total_tokens = []
 
 
 def main() -> None:
     it.display_header()
     it.display_sidebar()
     if auth():
-        chat_loop(tse_chain)
+        chat_loop(chain)
     else:
         st.write("You are not authorized to access this page.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm_explorer-0.0.2/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.3/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.3/llm_explorer/chains/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 import openai
 import pandas as pd
 import streamlit as st
 from langchain.chains import ConversationalRetrievalChain, LLMChain, RetrievalQA
 from langchain.chains.question_answering import load_qa_chain
 from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.llms import OpenAI
 from langchain.prompts.prompt import PromptTemplate
 
+from llm_explorer.llm import set_llm
+
+set_llm()
+
 from llm_explorer.templates.chains import chains_templates
 
 
 def set_chain(llm, **kwargs):
     condense_question_prompt = PromptTemplate.from_template(
         chains_templates()["snowchat_chain_template"]
     )
@@ -29,36 +32,18 @@
             "chain_type", "stuff"
         ),  # Should be one of "stuff","map_reduce", "map_rerank", and "refine".
         prompt=QA_PROMPT,
     )
     return question_generator, doc_chain
 
 
-class TSEConversationChain:
+class ExplorerConversationChain:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        self.llm = OpenAI(
-            temperature=kwargs.get("temperature", 0),
-            openai_api_key=st.secrets.connections.openai.api_key,
-            model_name="gpt-3.5-turbo",
-            max_tokens=kwargs.get("max_tokens", -1),  # Max number of tokens to generate
-            # top_p=kwargs.get(
-            #     "top_p", 1
-            # ),  # Total probability mass of tokens to consider at each step
-            # frequency_penalty=kwargs.get(
-            #     "frequency_penalty", 0
-            # ),  # Penalizes repeated tokens according to frequency
-            # presence_penalty=kwargs.get(
-            #     "presence_penalty", 0
-            # ),  # Penalizes repeated tokens.
-            # n=kwargs.get("n", 1),  # How many completions to generate for each prompt.
-            # best_of=kwargs.get(
-            #     "best_of", 1
-            # ),  # Generates best_of completions server-side and returns the "best".
-        )
+        self.llm = st.session_state.llm
         self.embeddings = OpenAIEmbeddings(
             openai_api_key=st.secrets.connections.openai.api_key
         )
 
     def get_qa_retrieval_chain(self, vectorstore):
         return RetrievalQA.from_chain_type(
             llm=self.llm,
```

### Comparing `llm_explorer-0.0.2/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.3/llm_explorer/chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import streamlit as st
 from langchain.memory import ConversationBufferMemory
 
 from llm_explorer.agents import ExplorerAgent, HFTAgent
 from llm_explorer.chains import extract_code, is_sql_query
 from llm_explorer.databases.adbddl import ADBDDL
 from llm_explorer.indexes.vectorstore import VectorStoreHandler
+from llm_explorer.llm import set_llm
 from llm_explorer.templates.chains import chains_templates
 from llm_explorer.templates.ui import session_state_templates
 from llm_explorer.ui import UI
 
+set_llm()
+
 adb_ddl = ADBDDL()
 agent_database = (
     st.session_state["agent_database"]
     if "agent_database" in st.session_state
     else "default"
 )
 explorer_agent = ExplorerAgent(**{"database": agent_database})
```

### Comparing `llm_explorer-0.0.2/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.3/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.3/llm_explorer/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.3/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/templates/agents.py` & `llm_explorer-0.0.3/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/templates/chains.py` & `llm_explorer-0.0.3/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.3/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/templates/ui.py` & `llm_explorer-0.0.3/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.3/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer/ui/lang.py` & `llm_explorer-0.0.3/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/llm_explorer.egg-info/PKG-INFO` & `llm_explorer-0.0.3/llm_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-explorer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 # Occlusion LLM Explorer
 
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
+**Important** This package requires **Open AI & HuggingFace API key**
+
 ### Pypi
 ```shell
 pip install llm-explorer
 ```
 
 
 ### Build from source
```

### Comparing `llm_explorer-0.0.2/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.3/llm_explorer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ./llm_explorer/chat/__init__.py
 ./llm_explorer/databases/__init__.py
 ./llm_explorer/databases/adbddl.py
 ./llm_explorer/indexes/__init__.py
 ./llm_explorer/indexes/vectorstore.py
 ./llm_explorer/interfaces/__init__.py
 ./llm_explorer/interfaces/frontend.py
+./llm_explorer/llm/__init__.py
 ./llm_explorer/templates/__init__.py
 ./llm_explorer/templates/agents.py
 ./llm_explorer/templates/chains.py
 ./llm_explorer/templates/prompt.py
 ./llm_explorer/templates/ui.py
 ./llm_explorer/ui/__init__.py
 ./llm_explorer/ui/lang.py
```

### Comparing `llm_explorer-0.0.2/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.3/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/requirements.txt` & `llm_explorer-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.2/setup.py` & `llm_explorer-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.2"
+    version = "0.0.3"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name = package_name + f"_{package_env}"
```

