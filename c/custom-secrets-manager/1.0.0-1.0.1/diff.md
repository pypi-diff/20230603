# Comparing `tmp/custom_secrets_manager-1.0.0.tar.gz` & `tmp/custom_secrets_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_secrets_manager-1.0.0.tar", last modified: Sat Jun  3 20:40:16 2023, max compression
+gzip compressed data, was "custom_secrets_manager-1.0.1.tar", last modified: Sat Jun  3 21:11:47 2023, max compression
```

## Comparing `custom_secrets_manager-1.0.0.tar` & `custom_secrets_manager-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 20:40:16.256945 custom_secrets_manager-1.0.0/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1694 2023-06-03 20:40:16.254624 custom_secrets_manager-1.0.0/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      941 2023-06-03 19:59:38.000000 custom_secrets_manager-1.0.0/README.md
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 20:40:16.240034 custom_secrets_manager-1.0.0/custom_secrets_manager/
--rw-r--r--   0 vashishtha   (501) staff       (20)       22 2023-06-03 20:00:39.000000 custom_secrets_manager-1.0.0/custom_secrets_manager/__init__.py
--rw-r--r--   0 vashishtha   (501) staff       (20)      460 2023-06-03 19:53:35.000000 custom_secrets_manager-1.0.0/custom_secrets_manager/secrets_loader.py
--rw-r--r--   0 vashishtha   (501) staff       (20)     2422 2023-06-03 19:50:25.000000 custom_secrets_manager-1.0.0/custom_secrets_manager/starter_process.py
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 20:40:16.253873 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1694 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      414 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/SOURCES.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)        1 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/dependency_links.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       87 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/entry_points.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       10 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/requires.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       23 2023-06-03 20:40:16.000000 custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/top_level.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       38 2023-06-03 20:40:16.257094 custom_secrets_manager-1.0.0/setup.cfg
--rw-r--r--   0 vashishtha   (501) staff       (20)     1411 2023-06-03 20:39:12.000000 custom_secrets_manager-1.0.0/setup.py
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.325421 custom_secrets_manager-1.0.1/
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 21:11:47.313691 custom_secrets_manager-1.0.1/PKG-INFO
+-rw-r--r--   0 vashishtha   (501) staff       (20)      943 2023-06-03 21:05:39.000000 custom_secrets_manager-1.0.1/README.md
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.292712 custom_secrets_manager-1.0.1/custom_secrets_manager/
+-rw-r--r--   0 vashishtha   (501) staff       (20)       22 2023-06-03 21:10:29.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/__init__.py
+-rw-r--r--   0 vashishtha   (501) staff       (20)      460 2023-06-03 19:53:35.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/secrets_loader.py
+-rw-r--r--   0 vashishtha   (501) staff       (20)     2422 2023-06-03 19:50:25.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/starter_process.py
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.301356 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/PKG-INFO
+-rw-r--r--   0 vashishtha   (501) staff       (20)      414 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)        1 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       87 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/entry_points.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       10 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/requires.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       23 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/top_level.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       38 2023-06-03 21:11:47.325866 custom_secrets_manager-1.0.1/setup.cfg
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1411 2023-06-03 20:39:12.000000 custom_secrets_manager-1.0.1/setup.py
```

### Comparing `custom_secrets_manager-1.0.0/PKG-INFO` & `custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom_secrets_manager
-Version: 1.0.0
+Name: custom-secrets-manager
+Version: 1.0.1
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,12 +16,12 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 This starter_process script performs the following tasks:
   - Creates a `secrets_registry.log` file as a database for secrets, API keys, or passwords found in the parent directory of the script.
   - Scans the parent directory for suggestive file names like secrets or keys with file extensions **`.yaml`**, **`.json`**, or **`.ini`**. If there is a mention of a key name without a value, it checks the corresponding value in `os.environ` and updates the registry accordingly.
-  - Uses the modified `secrets_loader.py` module to load secrets from the secrets_registry.log file.
-  - Generates meaningful logs in the standard output and saves logs in the load_config_process.log file in the same directory.
+  - Makes available a `secrets_loader.py` module to load secrets from the secrets_registry.log file.
+  - Generates meaningful logs in the standard output and saves logs in the `load_config_process.log` file in the same directory.
   - Checks if a `.gitignore` file exists in the directory and ensures that entries are made for secrets files.
 
 Please note that this script assumes that you have the secrets_loader.py module in the same directory as `starter_process.py`
```

### Comparing `custom_secrets_manager-1.0.0/README.md` & `custom_secrets_manager-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 This starter_process script performs the following tasks:
   - Creates a `secrets_registry.log` file as a database for secrets, API keys, or passwords found in the parent directory of the script.
   - Scans the parent directory for suggestive file names like secrets or keys with file extensions **`.yaml`**, **`.json`**, or **`.ini`**. If there is a mention of a key name without a value, it checks the corresponding value in `os.environ` and updates the registry accordingly.
-  - Uses the modified `secrets_loader.py` module to load secrets from the secrets_registry.log file.
-  - Generates meaningful logs in the standard output and saves logs in the load_config_process.log file in the same directory.
+  - Makes available a `secrets_loader.py` module to load secrets from the secrets_registry.log file.
+  - Generates meaningful logs in the standard output and saves logs in the `load_config_process.log` file in the same directory.
   - Checks if a `.gitignore` file exists in the directory and ensures that entries are made for secrets files.
 
 Please note that this script assumes that you have the secrets_loader.py module in the same directory as `starter_process.py`
```

### Comparing `custom_secrets_manager-1.0.0/custom_secrets_manager/starter_process.py` & `custom_secrets_manager-1.0.1/custom_secrets_manager/starter_process.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.0/custom_secrets_manager.egg-info/PKG-INFO` & `custom_secrets_manager-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom-secrets-manager
-Version: 1.0.0
+Name: custom_secrets_manager
+Version: 1.0.1
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,12 +16,12 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 This starter_process script performs the following tasks:
   - Creates a `secrets_registry.log` file as a database for secrets, API keys, or passwords found in the parent directory of the script.
   - Scans the parent directory for suggestive file names like secrets or keys with file extensions **`.yaml`**, **`.json`**, or **`.ini`**. If there is a mention of a key name without a value, it checks the corresponding value in `os.environ` and updates the registry accordingly.
-  - Uses the modified `secrets_loader.py` module to load secrets from the secrets_registry.log file.
-  - Generates meaningful logs in the standard output and saves logs in the load_config_process.log file in the same directory.
+  - Makes available a `secrets_loader.py` module to load secrets from the secrets_registry.log file.
+  - Generates meaningful logs in the standard output and saves logs in the `load_config_process.log` file in the same directory.
   - Checks if a `.gitignore` file exists in the directory and ensures that entries are made for secrets files.
 
 Please note that this script assumes that you have the secrets_loader.py module in the same directory as `starter_process.py`
```

### Comparing `custom_secrets_manager-1.0.0/setup.py` & `custom_secrets_manager-1.0.1/setup.py`

 * *Files identical despite different names*

