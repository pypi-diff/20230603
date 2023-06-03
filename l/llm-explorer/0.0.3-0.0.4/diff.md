# Comparing `tmp/llm_explorer-0.0.3.tar.gz` & `tmp/llm_explorer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.3.tar", last modified: Sat Jun  3 04:21:33 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.4.tar", last modified: Sat Jun  3 16:56:06 2023, max compression
```

## Comparing `llm_explorer-0.0.3.tar` & `llm_explorer-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/llm/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.041965 llm_explorer-0.0.3/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 04:21:33.000000 llm_explorer-0.0.3/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:21:33.045965 llm_explorer-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 04:21:23.000000 llm_explorer-0.0.3/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/DockerFile
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.074532 llm_explorer-0.0.4/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/setup.py
```

### Comparing `llm_explorer-0.0.3/.gitignore` & `llm_explorer-0.0.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *$py.class
 
 .streamlit/secrets.toml
 
 # C extensions
 *.so
 
-*.DS_Store
+.DS_Store
 .__pycache__
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
```

### Comparing `llm_explorer-0.0.3/LICENSE` & `llm_explorer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/Makefile` & `llm_explorer-0.0.4/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 SHELL=/bin/bash
 devops_state = main
 working_dir = `pwd`
 datadog_api_key = ""
 
+install: install_python_dependencies
 
 package_build:
 	python -m build
 
 package_list:
 	unzip -l dist/*.whl  
 
 set_env:
-	source tse/orchestrator/astro/$(devops_state).env
-
-init:
-	@echo "init" && source ./environments/tse_dev_env/bin/activate \
-	&& pip install -r requirements.txt
-
+	source /astro/$(devops_state).env
 
 setup_docker:
 	sudo apt-get install ca-certificates curl gnupg lsb-release make \
 	&& curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg \
 	&& echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null \
 	&& sudo apt-get update \
 	&& sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose \
@@ -57,24 +53,18 @@
 	curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.14.0/kind-linux-amd64 \
 	&& chmod +x ./kind \
 	&& sudo mv ./kind /usr/local/bin/kind
 
 setup_miniconda:
 	curl -Lo ./miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
 	&& chmod +x ./miniconda.sh \
-	&& ./miniconda.sh -b -p ./environments/tse-env \
-	&& source ./environments/tse-env/bin/activate \
-	&& conda install -c conda-forge jupyterlab
 
-miniconda_update:
-	curl -Lo ./miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
-	&& chmod +x ./miniconda.sh \
-	&& ./miniconda.sh -u -b -p ./environments/tse-env \
-	&& source ./environments/tse-env/bin/activate \
-	&& conda install -c conda-forge jupyterlab 
+miniconda_create_llm_explorer:
+	conda create  --yes -n llm_explorer python=3.10 \
+	&& conda init bash
 
 miniconda_create_adb_connect:
 	conda create --name adb_connect python=3.8 \
 	&& conda activate adb_connect
 
 miniconda_configure_adb_connect:
 	pip uninstall pyspark \
@@ -94,20 +84,20 @@
 	curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" \
 	&& sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
 
 setup_airflow:
 	curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.3.3/docker-compose.yaml'
 
 airflow_start:
-	cd tse/orchestrator/airflow \
+	cd airflow \
 	&& sudo docker-compose up airflow-init -d \
 	&& sudo docker-compose up -d
 
 airflow_kill:
-	cd tse/orchestrator/airflow \
+	cd /airflow \
 	&& sudo docker compose down --volumes --rmi all   
 
 docker_exec_root:
 	docker exec -u root -it airflow-airflow-scheduler-1 bash
 
 setup_helm:
 	curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 \
```

### Comparing `llm_explorer-0.0.3/PKG-INFO` & `llm_explorer-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-Metadata-Version: 2.1
-Name: llm_explorer
-Version: 0.0.3
-Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
-Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
-Author: Carlos D. Escobar-Valbuena
-Author-email: carlosdavidescobar@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Occlusion LLM Explorer
 
+[![CodeQL](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql) [![python-ci](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml) [![python-cd](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml) [![PyPI version](https://badge.fury.io/py/llm-explorer.svg)](https://badge.fury.io/py/llm-explorer)
+
+
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
 
 ## Setup
 **Important** This package requires **Open AI & HuggingFace API key**
 
 ### Pypi
 ```shell
-pip install llm-explorer
+python -m pip install llm-explorer
+```
+
+```shell
+touch main.py
 ```
 
+```python
+from llm_explorer import main
+
+if __name__ == "__main__":
+    main()
+```
+
+```shell
+python -m streamlit run main.py
+```
+
+Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
+
 
 ### Build from source
 Create a virtual environment
 
 ```shell
 conda create -n occlusion python=3.10
 conda activate occlusion
@@ -114,8 +120,8 @@
 Action Input: "SELECT WELL_CODE, SUM(PROD_GAS_VOLUME_MCF) AS total_gas_volume_mcf FROM padalloc GROUP BY WELL_CODE ORDER BY total_gas_volume_mcf DESC LIMIT 10"
 Observation: [('1222344             ', Decimal('8429191.6172')), ('1212560             ', Decimal('8211108.4867')), ('1222345             ', Decimal('8163411.9976')), ('1212503             ', Decimal('6621501.8683')), ('1222335             ', Decimal('4773668.6216')), ('1222340             ', Decimal('4276560.8228')), ('1222338             ', Decimal('4153258.1434')), ('1222367             ', Decimal('4018012.2406')), ('1220189             ', Decimal('3965394.4453')), ('1222352             ', Decimal('3786076.4127'))]
 Thought: I now know the top 10 producing wells.
 
 Final Answer: The top 10 producing wells are 1222344, 1212560, 1222345, 1212503, 1222335, 1222340, 1222338, 1222367, 1220189, and 1222352.
 
 > Finished chain.
-```
+```
```

### Comparing `llm_explorer-0.0.3/SECURITY.md` & `llm_explorer-0.0.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/__init__.py` & `llm_explorer-0.0.4/llm_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.4/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.4/llm_explorer/chains/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     )
     return question_generator, doc_chain
 
 
 class ExplorerConversationChain:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        self.llm = st.session_state.llm
+        self.llm = set_llm()
         self.embeddings = OpenAIEmbeddings(
             openai_api_key=st.secrets.connections.openai.api_key
         )
 
     def get_qa_retrieval_chain(self, vectorstore):
         return RetrievalQA.from_chain_type(
             llm=self.llm,
```

### Comparing `llm_explorer-0.0.3/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.4/llm_explorer/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.4/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.4/llm_explorer/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.4/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/llm/__init__.py` & `llm_explorer-0.0.4/llm_explorer/llm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import streamlit as st
 from langchain.llms import OpenAI
 
 
 def set_llm(**kwargs):
-    st.session_state.llm = OpenAI(
+    llm = OpenAI(
         temperature=kwargs.get("temperature", 0),
         openai_api_key=st.secrets.connections.openai.api_key,
         model_name="gpt-3.5-turbo",
         max_tokens=kwargs.get("max_tokens", -1),  # Max number of tokens to generate
         # top_p=kwargs.get(
         #     "top_p", 1
         # ),  # Total probability mass of tokens to consider at each step
@@ -18,7 +18,10 @@
         #     "presence_penalty", 0
         # ),  # Penalizes repeated tokens.
         # n=kwargs.get("n", 1),  # How many completions to generate for each prompt.
         # best_of=kwargs.get(
         #     "best_of", 1
         # ),  # Generates best_of completions server-side and returns the "best".
     )
+    if "llm" not in st.session_state:
+        st.session_state["llm"] = llm
+    return llm
```

### Comparing `llm_explorer-0.0.3/llm_explorer/templates/agents.py` & `llm_explorer-0.0.4/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/templates/chains.py` & `llm_explorer-0.0.4/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.4/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/templates/ui.py` & `llm_explorer-0.0.4/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.4/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer/ui/lang.py` & `llm_explorer-0.0.4/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.4/llm_explorer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-.DS_Store
 .gitcommit
 .gitignore
+CHANGELOG.md
+CODE_OF_CONDUCT.md
+CONTRIBUTING.rst
+DockerFile
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 SECURITY.md
+app.py
 main.py
 package.json
 pip.conf
 pyproject.toml
 requirements.txt
+setup.cfg
 setup.py
-test.py
-./llm_explorer/__init__.py
-./llm_explorer/agents/__init__.py
-./llm_explorer/auth/__init__.py
-./llm_explorer/chains/__init__.py
-./llm_explorer/chat/__init__.py
-./llm_explorer/databases/__init__.py
-./llm_explorer/databases/adbddl.py
-./llm_explorer/indexes/__init__.py
-./llm_explorer/indexes/vectorstore.py
-./llm_explorer/interfaces/__init__.py
-./llm_explorer/interfaces/frontend.py
-./llm_explorer/llm/__init__.py
-./llm_explorer/templates/__init__.py
-./llm_explorer/templates/agents.py
-./llm_explorer/templates/chains.py
-./llm_explorer/templates/prompt.py
-./llm_explorer/templates/ui.py
-./llm_explorer/ui/__init__.py
-./llm_explorer/ui/lang.py
-./pages/__init__.py
-./pages/pandas_agent.py
+llm_explorer/__init__.py
 llm_explorer.egg-info/PKG-INFO
 llm_explorer.egg-info/SOURCES.txt
 llm_explorer.egg-info/dependency_links.txt
+llm_explorer.egg-info/entry_points.txt
+llm_explorer.egg-info/not-zip-safe
 llm_explorer.egg-info/requires.txt
-llm_explorer.egg-info/top_level.txt
+llm_explorer.egg-info/top_level.txt
+llm_explorer/agents/__init__.py
+llm_explorer/auth/__init__.py
+llm_explorer/chains/__init__.py
+llm_explorer/chat/__init__.py
+llm_explorer/databases/__init__.py
+llm_explorer/databases/adbddl.py
+llm_explorer/indexes/__init__.py
+llm_explorer/indexes/vectorstore.py
+llm_explorer/interfaces/__init__.py
+llm_explorer/interfaces/frontend.py
+llm_explorer/llm/__init__.py
+llm_explorer/templates/__init__.py
+llm_explorer/templates/agents.py
+llm_explorer/templates/chains.py
+llm_explorer/templates/prompt.py
+llm_explorer/templates/ui.py
+llm_explorer/ui/__init__.py
+llm_explorer/ui/lang.py
+pages/__init__.py
+pages/pandas_agent.py
```

### Comparing `llm_explorer-0.0.3/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.4/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/requirements.txt` & `llm_explorer-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.3/setup.py` & `llm_explorer-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,43 +23,56 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.3"
+    version = "0.0.4"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
-    package_name = package_name + f"_{package_env}"
+    package_name += f"_{package_env}"
 
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 print(package_name, version)
 setup(
     name=package_name,
     version=version,
     author="Carlos D. Escobar-Valbuena",
     author_email="carlosdavidescobar@gmail.com",
     description="A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
+    packages=find_packages(where="."),
+    include_package_data=True,
+    setup_requires=["setuptools", "wheel"],
+    tests_require=["pytest"],
+    python_requires=">=3.10",
+    nstall_requires=required,
+    test_suite="tests",
+    zip_safe=False,
     url="https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    package_dir={"": "."},
-    packages=find_packages(where="."),
-    python_requires=">=3.6",
-    include_package_data=True,
     install_requires=required,
     package_data={
         "": ["*.json"],
     },
+    entry_points={
+        "console_scripts": [
+            "llm_explorer=llm_explorer:main",
+        ],
+    },
 )
```

