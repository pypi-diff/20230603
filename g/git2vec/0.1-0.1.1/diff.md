# Comparing `tmp/git2vec-0.1.tar.gz` & `tmp/git2vec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.tar", last modified: Sat Jun  3 01:26:21 2023, max compression
+gzip compressed data, was "git2vec-0.1.1.tar", last modified: Sat Jun  3 01:37:19 2023, max compression
```

## Comparing `git2vec-0.1.tar` & `git2vec-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.677036 git2vec-0.1/
--rw-rw-rw-   0        0        0      607 2023-06-03 01:26:21.676029 git2vec-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-06-03 00:41:21.000000 git2vec-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.663748 git2vec-0.1/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-03 01:26:04.000000 git2vec-0.1/git2vec/__init__.py
--rw-rw-rw-   0        0        0     4594 2023-06-03 00:41:21.000000 git2vec-0.1/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-03 00:41:21.000000 git2vec-0.1/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.673762 git2vec-0.1/git2vec.egg-info/
--rw-rw-rw-   0        0        0      607 2023-06-03 01:26:21.000000 git2vec-0.1/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-03 01:26:21.000000 git2vec-0.1/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:26:21.000000 git2vec-0.1/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 01:26:21.000000 git2vec-0.1/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 01:26:21.000000 git2vec-0.1/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 01:26:21.677036 git2vec-0.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-06-03 01:26:19.000000 git2vec-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:37:19.001129 git2vec-0.1.1/
+-rw-rw-rw-   0        0        0     2422 2023-06-03 01:37:19.001129 git2vec-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2023-06-03 01:36:21.000000 git2vec-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 01:37:18.988987 git2vec-0.1.1/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-03 01:26:04.000000 git2vec-0.1.1/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     4594 2023-06-03 00:41:21.000000 git2vec-0.1.1/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-03 00:41:21.000000 git2vec-0.1.1/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:37:18.999133 git2vec-0.1.1/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2422 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 01:37:19.002126 git2vec-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-06-03 01:37:01.000000 git2vec-0.1.1/setup.py
```

### Comparing `git2vec-0.1/git2vec/loader.py` & `git2vec-0.1.1/git2vec/loader.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1/git2vec/vectordb.py` & `git2vec-0.1.1/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1/setup.py` & `git2vec-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1',
+    version='0.1.1',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
@@ -19,9 +19,11 @@
         'Intended Audience :: Developers',  
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-    ],
+	],
+	long_description=open("README.md", encoding="utf-8").read(),
+    long_description_content_type='text/markdown'
 )
```

