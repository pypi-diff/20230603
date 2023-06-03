# Comparing `tmp/pySSRSapi-0.0.1.tar.gz` & `tmp/pySSRSapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.1.tar", last modified: Sat Jun  3 19:20:10 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.2.tar", last modified: Sat Jun  3 20:19:03 2023, max compression
```

## Comparing `pySSRSapi-0.0.1.tar` & `pySSRSapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 19:20:10.673049 pySSRSapi-0.0.1/
--rw-r--r--   0 quaik8     (501) staff       (20)      497 2023-06-03 19:20:10.672693 pySSRSapi-0.0.1/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.1/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 19:20:10.670828 pySSRSapi-0.0.1/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      497 2023-06-03 19:20:10.000000 pySSRSapi-0.0.1/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      213 2023-06-03 19:20:10.000000 pySSRSapi-0.0.1/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 19:20:10.000000 pySSRSapi-0.0.1/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 19:20:10.000000 pySSRSapi-0.0.1/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        4 2023-06-03 19:20:10.000000 pySSRSapi-0.0.1/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 19:20:10.673150 pySSRSapi-0.0.1/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      782 2023-06-03 19:19:55.000000 pySSRSapi-0.0.1/setup.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 19:20:10.672265 pySSRSapi-0.0.1/src/
--rw-r--r--   0 quaik8     (501) staff       (20)     8870 2023-06-03 19:02:32.000000 pySSRSapi-0.0.1/src/SsrsApi.py
--rw-r--r--   0 quaik8     (501) staff       (20)        0 2023-06-03 19:00:59.000000 pySSRSapi-0.0.1/src/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.720236 pySSRSapi-0.0.2/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 20:19:03.719709 pySSRSapi-0.0.2/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.2/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.712626 pySSRSapi-0.0.2/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)     8870 2023-06-03 20:15:20.000000 pySSRSapi-0.0.2/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.718939 pySSRSapi-0.0.2/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 20:19:03.720350 pySSRSapi-0.0.2/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      800 2023-06-03 20:18:30.000000 pySSRSapi-0.0.2/setup.py
```

### Comparing `pySSRSapi-0.0.1/setup.py` & `pySSRSapi-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.1',
+    version='0.0.2',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
-    url='',
+    url='https://pypi.org/project/pySSRSapi/',
     python_requires='>=3.7',
-    packages=find_packages(),
+    packages=['pySSRSapi'],
     install_requires=['requests'],
     license="MIT license",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
```

### Comparing `pySSRSapi-0.0.1/src/SsrsApi.py` & `pySSRSapi-0.0.2/pySSRSapi/__init__.py`

 * *Files identical despite different names*

