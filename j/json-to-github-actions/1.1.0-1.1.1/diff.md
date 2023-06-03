# Comparing `tmp/json-to-github-actions-1.1.0.tar.gz` & `tmp/json-to-github-actions-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-to-github-actions-1.1.0.tar", last modified: Sat Jun  3 11:04:34 2023, max compression
+gzip compressed data, was "json-to-github-actions-1.1.1.tar", last modified: Sat Jun  3 11:12:01 2023, max compression
```

## Comparing `json-to-github-actions-1.1.0.tar` & `json-to-github-actions-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:04:34.475592 json-to-github-actions-1.1.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-06-03 11:04:34.475478 json-to-github-actions-1.1.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1992 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:04:34.475290 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4587 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 11:04:34.475624 json-to-github-actions-1.1.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:12:01.170735 json-to-github-actions-1.1.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3181 2023-06-03 11:12:01.170622 json-to-github-actions-1.1.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3073 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:12:01.170461 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3181 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4587 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/json_to_github_actions.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 11:12:01.170767 json-to-github-actions-1.1.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-06-03 11:12:01.000000 json-to-github-actions-1.1.1/setup.py
```

### Comparing `json-to-github-actions-1.1.0/json_to_github_actions.py` & `json-to-github-actions-1.1.1/json_to_github_actions.py`

 * *Files identical despite different names*

### Comparing `json-to-github-actions-1.1.0/setup.py` & `json-to-github-actions-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="json-to-github-actions",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     py_modules=['json_to_github_actions'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'json_to_github_actions = json_to_github_actions:main',
         ],
```

