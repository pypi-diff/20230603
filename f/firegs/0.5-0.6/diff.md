# Comparing `tmp/firegs-0.5.tar.gz` & `tmp/firegs-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firegs-0.5.tar", last modified: Sat Jun  3 16:46:11 2023, max compression
+gzip compressed data, was "firegs-0.6.tar", last modified: Sat Jun  3 16:53:42 2023, max compression
```

## Comparing `firegs-0.5.tar` & `firegs-0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:46:11.378316 firegs-0.5/
--rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.5/LICENSE
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:46:11.378144 firegs-0.5/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.5/README.md
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:46:11.376837 firegs-0.5/firegs/
--rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.5/firegs/__init__.py
--rw-r--r--   0 ask        (501) staff       (20)     5893 2023-06-03 16:44:51.000000 firegs-0.5/firegs/script.py
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:46:11.377915 firegs-0.5/firegs.egg-info/
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      244 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/SOURCES.txt
--rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/dependency_links.txt
--rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/entry_points.txt
--rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/requires.txt
--rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:46:11.000000 firegs-0.5/firegs.egg-info/top_level.txt
--rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:46:11.378367 firegs-0.5/setup.cfg
--rw-r--r--   0 ask        (501) staff       (20)      872 2023-06-03 16:44:26.000000 firegs-0.5/setup.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.659941 firegs-0.6/
+-rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.6/LICENSE
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:53:42.659803 firegs-0.6/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.6/README.md
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.658868 firegs-0.6/firegs/
+-rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.6/firegs/__init__.py
+-rw-r--r--   0 ask        (501) staff       (20)     5921 2023-06-03 16:53:08.000000 firegs-0.6/firegs/script.py
+-rw-r--r--   0 ask        (501) staff       (20)       19 2023-06-03 16:53:36.000000 firegs-0.6/firegs/version.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:53:42.659612 firegs-0.6/firegs.egg-info/
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      262 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/SOURCES.txt
+-rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/dependency_links.txt
+-rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/entry_points.txt
+-rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/requires.txt
+-rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:53:42.000000 firegs-0.6/firegs.egg-info/top_level.txt
+-rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:53:42.659982 firegs-0.6/setup.cfg
+-rw-r--r--   0 ask        (501) staff       (20)      879 2023-06-03 16:53:08.000000 firegs-0.6/setup.py
```

### Comparing `firegs-0.5/LICENSE` & `firegs-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `firegs-0.5/PKG-INFO` & `firegs-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.5
+Version: 0.6
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.5/README.md` & `firegs-0.6/README.md`

 * *Files identical despite different names*

### Comparing `firegs-0.5/firegs/script.py` & `firegs-0.6/firegs/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import json
 import configparser
 from google.oauth2 import service_account
 from google.auth.transport.requests import AuthorizedSession
 import argparse
 import webbrowser
 import sys
-from version import __version__
+from firegs.version import __version__
 
 # Firebase project ID
 PROJECT_ID = None
 
 # Path to the service account key file
 SERVICE_ACCOUNT_FILE = None
 
 # Determine the location of the configuration file
 config_file = os.path.expanduser('~/.firegs_config')
 
 # Create a ConfigParser object
 config = configparser.ConfigParser()
 
+
 def validate_project_id(project_id):
     if project_id is None:
         project_id = input("Please enter your Firebase Project ID: ")
         if not project_id:
             print("Invalid Project ID. Exiting.")
             exit(1)
     return project_id
@@ -34,14 +35,15 @@
     if service_account_file is None:
         service_account_file = input("Please enter the path to your Service Account file: ")
         if not os.path.isfile(service_account_file):
             print("Invalid file path. Exiting.")
             exit(1)
     return service_account_file
 
+
 # Check if the configuration file exists
 if os.path.exists(config_file):
     # If it exists, read it
     config.read(config_file)
 
     # Get the service account file path
     SERVICE_ACCOUNT_FILE = config.get('DEFAULT', 'service_account_file')
@@ -61,18 +63,18 @@
 
 # Parse command line arguments
 parser = argparse.ArgumentParser(description='Manage Firebase Android Apps')
 parser.add_argument('-p', '--project', help='Project ID for the Firebase project')
 parser.add_argument('-c', '--create', help='Create an app with the provided Application ID or package name')
 parser.add_argument('-d', '--display', help='Display name for the app')
 parser.add_argument('-l', '--list', help='List all apps in the project', action='store_true')
-parser.add_argument('-v', '--version', action='version', version=f'firegs {__version__}', help='Display the version of the program')
+parser.add_argument('-v', '--version', action='version', version=f'firegs {__version__}',
+                    help='Display the version of the program')
 args = parser.parse_args()
 
-
 if len(sys.argv) == 1:
     print("Hello, welcome to firegs!")
     exit()
 
 if args.project:
     PROJECT_ID = args.project
```

### Comparing `firegs-0.5/firegs.egg-info/PKG-INFO` & `firegs-0.6/firegs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.5
+Version: 0.6
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.5/setup.py` & `firegs-0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-from version import __version__
+from firegs.version import __version__
 
 setup(
     name="firegs",
     version=__version__,
     packages=find_packages(),
     install_requires=[
         'requests',
```

