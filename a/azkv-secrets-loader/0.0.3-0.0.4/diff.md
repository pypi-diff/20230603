# Comparing `tmp/azkv-secrets-loader-0.0.3.tar.gz` & `tmp/azkv-secrets-loader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azkv-secrets-loader-0.0.3.tar", last modified: Wed May 31 14:18:06 2023, max compression
+gzip compressed data, was "azkv-secrets-loader-0.0.4.tar", last modified: Sat Jun  3 10:05:21 2023, max compression
```

## Comparing `azkv-secrets-loader-0.0.3.tar` & `azkv-secrets-loader-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.995729 azkv-secrets-loader-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/secrets_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/secrets_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/secrets_loader/secrets_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:18:05.995729 azkv-secrets-loader-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 10:05:21.000000 azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/secrets_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/secrets_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/secrets_loader/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 10:05:21.069600 azkv-secrets-loader-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-03 10:05:09.000000 azkv-secrets-loader-0.0.4/setup.py
```

### Comparing `azkv-secrets-loader-0.0.3/PKG-INFO` & `azkv-secrets-loader-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/PKG-INFO` & `azkv-secrets-loader-0.0.4/azkv_secrets_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.3/secrets_loader/secrets_loader.py` & `azkv-secrets-loader-0.0.4/secrets_loader/secrets_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
 from azure.core.exceptions import ResourceNotFoundError
 
 def load_secret(secret_name):
-    dashed_name = secret_name.replace("-", "_")
-    ev = os.getenv(dashed_name)
+    underscore_name = secret_name.replace("-", "_")
+    ev = os.getenv(underscore_name)
     if ev:
         return ev
     
     credential = DefaultAzureCredential()
     key_vault_uri = os.getenv("KEY_VAULT_URI")
     if not key_vault_uri:
         raise Exception("Enviromental Variable KEY_VAULT_URI missing.")
     
     client = SecretClient(vault_url=key_vault_uri, credential=credential)
 
+    dashed_name = secret_name.replace("_", "-")
     try:
-        secret_value = client.get_secret(secret_name).value
+        secret_value = client.get_secret(dashed_name).value
         return secret_value
     except ResourceNotFoundError:
-        raise ValueError(f"Secret '{secret_name}' not found in Azure Key Vault.")
+        raise ValueError(f"Secret '{dashed_name}' not found in Azure Key Vault.")
     except Exception as e:
-        raise RuntimeError(f"Failed to retrieve secret '{secret_name}' from Azure Key Vault: {str(e)}")
+        raise RuntimeError(f"Failed to retrieve secret '{dashed_name}' from Azure Key Vault: {str(e)}")
```

### Comparing `azkv-secrets-loader-0.0.3/setup.py` & `azkv-secrets-loader-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 LONG_DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 
 # Setting up
 setup(
     name="azkv-secrets-loader",
     version=VERSION,
```

