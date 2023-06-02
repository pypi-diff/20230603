# Comparing `tmp/wordpress-auth-0.1.0.tar.gz` & `tmp/wordpress-auth-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-auth-0.1.0.tar", last modified: Fri Jun  2 22:02:45 2023, max compression
+gzip compressed data, was "wordpress-auth-0.2.tar", last modified: Fri Jun  2 23:40:09 2023, max compression
```

## Comparing `wordpress-auth-0.1.0.tar` & `wordpress-auth-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 22:02:45.862375 wordpress-auth-0.1.0/
--rw-r--r--   0 demon     (1000) demon     (1000)     6630 2023-06-02 22:02:45.862375 wordpress-auth-0.1.0/PKG-INFO
--rw-r--r--   0 demon     (1000) demon     (1000)     5079 2023-06-02 21:59:39.000000 wordpress-auth-0.1.0/README.md
--rw-r--r--   0 demon     (1000) demon     (1000)       38 2023-06-02 22:02:45.862375 wordpress-auth-0.1.0/setup.cfg
--rw-r--r--   0 demon     (1000) demon     (1000)      644 2023-06-02 21:02:33.000000 wordpress-auth-0.1.0/setup.py
-drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 22:02:45.862375 wordpress-auth-0.1.0/wordpress_auth/
--rw-r--r--   0 demon     (1000) demon     (1000)        0 2023-06-02 21:12:48.000000 wordpress-auth-0.1.0/wordpress_auth/__init__.py
--rw-r--r--   0 demon     (1000) demon     (1000)      801 2023-06-02 20:45:16.000000 wordpress-auth-0.1.0/wordpress_auth/wordpress_auth.py
-drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 22:02:45.862375 wordpress-auth-0.1.0/wordpress_auth.egg-info/
--rw-r--r--   0 demon     (1000) demon     (1000)     6630 2023-06-02 22:02:45.000000 wordpress-auth-0.1.0/wordpress_auth.egg-info/PKG-INFO
--rw-r--r--   0 demon     (1000) demon     (1000)      267 2023-06-02 22:02:45.000000 wordpress-auth-0.1.0/wordpress_auth.egg-info/SOURCES.txt
--rw-r--r--   0 demon     (1000) demon     (1000)        1 2023-06-02 22:02:45.000000 wordpress-auth-0.1.0/wordpress_auth.egg-info/dependency_links.txt
--rw-r--r--   0 demon     (1000) demon     (1000)       19 2023-06-02 22:02:45.000000 wordpress-auth-0.1.0/wordpress_auth.egg-info/requires.txt
--rw-r--r--   0 demon     (1000) demon     (1000)       15 2023-06-02 22:02:45.000000 wordpress-auth-0.1.0/wordpress_auth.egg-info/top_level.txt
+drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 23:40:09.898403 wordpress-auth-0.2/
+-rw-r--r--   0 demon     (1000) demon     (1000)     6628 2023-06-02 23:40:09.898403 wordpress-auth-0.2/PKG-INFO
+-rw-r--r--   0 demon     (1000) demon     (1000)     5079 2023-06-02 21:59:39.000000 wordpress-auth-0.2/README.md
+-rw-r--r--   0 demon     (1000) demon     (1000)       38 2023-06-02 23:40:09.898403 wordpress-auth-0.2/setup.cfg
+-rw-r--r--   0 demon     (1000) demon     (1000)      642 2023-06-02 23:39:40.000000 wordpress-auth-0.2/setup.py
+drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 23:40:09.898403 wordpress-auth-0.2/wordpress_auth/
+-rw-r--r--   0 demon     (1000) demon     (1000)      167 2023-06-02 23:34:30.000000 wordpress-auth-0.2/wordpress_auth/__init__.py
+-rw-r--r--   0 demon     (1000) demon     (1000)      801 2023-06-02 20:45:16.000000 wordpress-auth-0.2/wordpress_auth/wordpress_auth.py
+drwxr-xr-x   0 demon     (1000) demon     (1000)        0 2023-06-02 23:40:09.898403 wordpress-auth-0.2/wordpress_auth.egg-info/
+-rw-r--r--   0 demon     (1000) demon     (1000)     6628 2023-06-02 23:40:09.000000 wordpress-auth-0.2/wordpress_auth.egg-info/PKG-INFO
+-rw-r--r--   0 demon     (1000) demon     (1000)      267 2023-06-02 23:40:09.000000 wordpress-auth-0.2/wordpress_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 demon     (1000) demon     (1000)        1 2023-06-02 23:40:09.000000 wordpress-auth-0.2/wordpress_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 demon     (1000) demon     (1000)       19 2023-06-02 23:40:09.000000 wordpress-auth-0.2/wordpress_auth.egg-info/requires.txt
+-rw-r--r--   0 demon     (1000) demon     (1000)       15 2023-06-02 23:40:09.000000 wordpress-auth-0.2/wordpress_auth.egg-info/top_level.txt
```

### Comparing `wordpress-auth-0.1.0/PKG-INFO` & `wordpress-auth-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-auth
-Version: 0.1.0
+Version: 0.2
 Summary: A Python package that provides WordPress authentication for Streamlit applications.
 Home-page: https://github.com/Keyvanhardani/streamlit-wordpress-authentication
 Author: Keyvan Hardani
 Author-email: hello@keyvan.ai
 License: UNKNOWN
 Description: #   WordPress Authentication for Streamlit
```

### Comparing `wordpress-auth-0.1.0/README.md` & `wordpress-auth-0.2/README.md`

 * *Files identical despite different names*

### Comparing `wordpress-auth-0.1.0/setup.py` & `wordpress-auth-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="wordpress-auth",
-    version="0.1.0",
+    version="0.2",
     author="Keyvan Hardani",
     author_email="hello@keyvan.ai",
     description="A Python package that provides WordPress authentication for Streamlit applications.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Keyvanhardani/streamlit-wordpress-authentication",
     packages=find_packages(),
```

### Comparing `wordpress-auth-0.1.0/wordpress_auth/wordpress_auth.py` & `wordpress-auth-0.2/wordpress_auth/wordpress_auth.py`

 * *Files identical despite different names*

### Comparing `wordpress-auth-0.1.0/wordpress_auth.egg-info/PKG-INFO` & `wordpress-auth-0.2/wordpress_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-auth
-Version: 0.1.0
+Version: 0.2
 Summary: A Python package that provides WordPress authentication for Streamlit applications.
 Home-page: https://github.com/Keyvanhardani/streamlit-wordpress-authentication
 Author: Keyvan Hardani
 Author-email: hello@keyvan.ai
 License: UNKNOWN
 Description: #   WordPress Authentication for Streamlit
```

