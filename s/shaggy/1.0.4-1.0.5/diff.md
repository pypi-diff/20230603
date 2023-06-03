# Comparing `tmp/shaggy-1.0.4.tar.gz` & `tmp/shaggy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaggy-1.0.4.tar", last modified: Sat Jun  3 06:32:40 2023, max compression
+gzip compressed data, was "shaggy-1.0.5.tar", last modified: Sat Jun  3 06:34:40 2023, max compression
```

## Comparing `shaggy-1.0.4.tar` & `shaggy-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:32:40.714180 shaggy-1.0.4/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-01 10:20:38.000000 shaggy-1.0.4/.gitignore
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1071 2023-05-31 17:40:10.000000 shaggy-1.0.4/LICENSE
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:32:40.714180 shaggy-1.0.4/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.4/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       54 2023-06-03 06:31:03.000000 shaggy-1.0.4/publish.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-05-31 18:26:53.000000 shaggy-1.0.4/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:32:40.714180 shaggy-1.0.4/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2023-06-03 06:32:08.000000 shaggy-1.0.4/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:32:40.710180 shaggy-1.0.4/shaggy/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.4/shaggy/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4190 2023-06-03 06:14:32.000000 shaggy-1.0.4/shaggy/hunt.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.4/shaggy/output.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4088 2023-06-03 06:14:32.000000 shaggy-1.0.4/shaggy/sources.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:32:40.714180 shaggy-1.0.4/shaggy.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      316 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:32:40.000000 shaggy-1.0.4/shaggy.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.548852 shaggy-1.0.5/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-01 10:20:38.000000 shaggy-1.0.5/.gitignore
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1071 2023-05-31 17:40:10.000000 shaggy-1.0.5/LICENSE
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:34:40.548852 shaggy-1.0.5/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.5/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       54 2023-06-03 06:31:03.000000 shaggy-1.0.5/publish.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-05-31 18:26:53.000000 shaggy-1.0.5/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:34:40.548852 shaggy-1.0.5/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2023-06-03 06:34:05.000000 shaggy-1.0.5/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.544852 shaggy-1.0.5/shaggy/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4185 2023-06-03 06:34:14.000000 shaggy-1.0.5/shaggy/hunt.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/output.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4088 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/sources.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.544852 shaggy-1.0.5/shaggy.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      316 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/top_level.txt
```

### Comparing `shaggy-1.0.4/.gitignore` & `shaggy-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.4/LICENSE` & `shaggy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.4/PKG-INFO` & `shaggy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
 Description: # Shaggy
```

### Comparing `shaggy-1.0.4/README.md` & `shaggy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.4/setup.py` & `shaggy-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='shaggy',
-    version='1.0.4',
+    version='1.0.5',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mauro Baladés',
     author_email='mauro.balades@tutanota.com',
     description='Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.',
     url='https://github.com/mauro-balades/shaggy',
     packages=["shaggy"],
```

### Comparing `shaggy-1.0.4/shaggy/__init__.py` & `shaggy-1.0.5/shaggy/__init__.py`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.4/shaggy/hunt.py` & `shaggy-1.0.5/shaggy/hunt.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import requests
 
 headers = {
     "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.12; rv:55.0) Gecko/20100101 Firefox/55.0",
 }
 
 
-def hunt(names: list[str]):
+def hunt(names: list):
     # Create an empty list to store the found social media accounts
     found = []
 
     # Add data to the found sources if it does not exist
     def add_to_name(data):
         
         # A flag indicating that the source has already been found
```

### Comparing `shaggy-1.0.4/shaggy/sources.py` & `shaggy-1.0.5/shaggy/sources.py`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.4/shaggy.egg-info/PKG-INFO` & `shaggy-1.0.5/shaggy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
 Description: # Shaggy
```

