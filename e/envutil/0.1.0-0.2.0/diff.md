# Comparing `tmp/envutil-0.1.0.tar.gz` & `tmp/envutil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envutil-0.1.0.tar", max compression
+gzip compressed data, was "envutil-0.2.0.tar", max compression
```

## Comparing `envutil-0.1.0.tar` & `envutil-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-03 17:17:31.415430 envutil-0.1.0/README.md
--rw-r--r--   0        0        0     1781 2023-06-03 17:20:17.539577 envutil-0.1.0/envutil/__init__.py
--rw-r--r--   0        0        0      346 2023-06-03 17:19:29.801804 envutil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 envutil-0.1.0/setup.py
--rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 envutil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-03 17:17:31.415430 envutil-0.2.0/README.md
+-rw-r--r--   0        0        0     1826 2023-06-03 17:27:15.960244 envutil-0.2.0/envutil/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-03 17:27:22.798729 envutil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 envutil-0.2.0/setup.py
+-rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 envutil-0.2.0/PKG-INFO
```

### Comparing `envutil-0.1.0/envutil/__init__.py` & `envutil-0.2.0/envutil/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from functools import wraps
 from os import environ
 
 from dotenv import load_dotenv
 
 __ENV_LOADED: bool = False
 
 
 def depends_on_env(func):
+    @wraps(func)
     def wrapper(*args, **kwargs):
         load_env()
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `envutil-0.1.0/setup.py` & `envutil-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'envutil',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
     'author': 'Berke Arslan',
     'author_email': 'berke@kwilabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

