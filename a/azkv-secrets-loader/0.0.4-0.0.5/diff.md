# Comparing `tmp/azkv-secrets-loader-0.0.4.tar.gz` & `tmp/azkv-secrets-loader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azkv-secrets-loader-0.0.4.tar", last modified: Sat Jun  3 10:05:21 2023, max compression
+gzip compressed data, was "azkv-secrets-loader-0.0.5.tar", last modified: Sat Jun  3 11:30:23 2023, max compression
```

## Comparing `azkv-secrets-loader-0.0.4.tar` & `azkv-secrets-loader-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/secrets_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/secrets_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/secrets_loader/secrets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:30:23.887551 azkv-secrets-loader-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 11:30:23.887551 azkv-secrets-loader-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 11:30:14.000000 azkv-secrets-loader-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:30:23.883551 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 11:30:23.000000 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-03 11:30:23.000000 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:30:23.000000 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 11:30:23.000000 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 11:30:23.000000 azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:30:23.887551 azkv-secrets-loader-0.0.5/secrets_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-03 11:30:14.000000 azkv-secrets-loader-0.0.5/secrets_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-03 11:30:14.000000 azkv-secrets-loader-0.0.5/secrets_loader/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 11:30:23.887551 azkv-secrets-loader-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-03 11:30:14.000000 azkv-secrets-loader-0.0.5/setup.py
```

### Comparing `azkv-secrets-loader-0.0.4/PKG-INFO` & `azkv-secrets-loader-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/PKG-INFO` & `azkv-secrets-loader-0.0.5/azkv_secrets_loader.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.4/secrets_loader/secrets_loader.py` & `azkv-secrets-loader-0.0.5/secrets_loader/secrets_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 def load_secret(secret_name):
     underscore_name = secret_name.replace("-", "_")
     ev = os.getenv(underscore_name)
     if ev:
         return ev
     
-    credential = DefaultAzureCredential()
+    if os.getenv("TENANT_ID"):
+        credential = DefaultAzureCredential(additionally_allowed_tenants=os.getenv("TENANT_ID"))
+    else:
+        credential = DefaultAzureCredential()
+
     key_vault_uri = os.getenv("KEY_VAULT_URI")
     if not key_vault_uri:
         raise Exception("Enviromental Variable KEY_VAULT_URI missing.")
     
     client = SecretClient(vault_url=key_vault_uri, credential=credential)
 
     dashed_name = secret_name.replace("_", "-")
```

### Comparing `azkv-secrets-loader-0.0.4/setup.py` & `azkv-secrets-loader-0.0.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 LONG_DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 
 # Setting up
 setup(
     name="azkv-secrets-loader",
     version=VERSION,
```

