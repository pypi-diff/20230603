# Comparing `tmp/firegs-0.3.tar.gz` & `tmp/firegs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firegs-0.3.tar", last modified: Sat Jun  3 16:20:23 2023, max compression
+gzip compressed data, was "firegs-0.4.tar", last modified: Sat Jun  3 16:34:58 2023, max compression
```

## Comparing `firegs-0.3.tar` & `firegs-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.288804 firegs-0.3/
--rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.3/LICENSE
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:20:23.288631 firegs-0.3/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.3/README.md
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.287197 firegs-0.3/firegs/
--rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.3/firegs/__init__.py
--rw-r--r--   0 ask        (501) staff       (20)     5642 2023-06-03 15:57:54.000000 firegs-0.3/firegs/script.py
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:20:23.288378 firegs-0.3/firegs.egg-info/
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      244 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/SOURCES.txt
--rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/dependency_links.txt
--rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/entry_points.txt
--rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/requires.txt
--rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:20:23.000000 firegs-0.3/firegs.egg-info/top_level.txt
--rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:20:23.288851 firegs-0.3/setup.cfg
--rw-r--r--   0 ask        (501) staff       (20)      834 2023-06-03 16:19:11.000000 firegs-0.3/setup.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:34:58.757136 firegs-0.4/
+-rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.4/LICENSE
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:34:58.756991 firegs-0.4/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.4/README.md
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:34:58.755833 firegs-0.4/firegs/
+-rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.4/firegs/__init__.py
+-rw-r--r--   0 ask        (501) staff       (20)     5715 2023-06-03 16:34:28.000000 firegs-0.4/firegs/script.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 16:34:58.756805 firegs-0.4/firegs.egg-info/
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      244 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/SOURCES.txt
+-rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/dependency_links.txt
+-rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/entry_points.txt
+-rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/requires.txt
+-rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 16:34:58.000000 firegs-0.4/firegs.egg-info/top_level.txt
+-rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 16:34:58.757179 firegs-0.4/setup.cfg
+-rw-r--r--   0 ask        (501) staff       (20)      834 2023-06-03 16:34:36.000000 firegs-0.4/setup.py
```

### Comparing `firegs-0.3/LICENSE` & `firegs-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `firegs-0.3/PKG-INFO` & `firegs-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.3
+Version: 0.4
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.3/README.md` & `firegs-0.4/README.md`

 * *Files identical despite different names*

### Comparing `firegs-0.3/firegs/script.py` & `firegs-0.4/firegs/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 parser = argparse.ArgumentParser(description='Manage Firebase Android Apps')
 parser.add_argument('-p', '--project', help='Project ID for the Firebase project')
 parser.add_argument('-c', '--create', help='Create an app with the provided Application ID or package name')
 parser.add_argument('-d', '--display', help='Display name for the app')
 parser.add_argument('-l', '--list', help='List all apps in the project', action='store_true')
 args = parser.parse_args()
 
+if len(sys.argv) == 1:
+    print("Hello, welcome to firegs")
+    exit()
+
 if args.project:
     PROJECT_ID = args.project
 
 PROJECT_ID = validate_project_id(PROJECT_ID)
 SERVICE_ACCOUNT_FILE = validate_service_account_file(SERVICE_ACCOUNT_FILE)
 
 # Save the project id to the configuration file for future use
```

### Comparing `firegs-0.3/firegs.egg-info/PKG-INFO` & `firegs-0.4/firegs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.3
+Version: 0.4
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.3/setup.py` & `firegs-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="firegs",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     install_requires=[
         'requests',
         'google-auth',
         'google-auth-httplib2',
         'google-auth-oauthlib',
         'google-api-python-client',
```

