# Comparing `tmp/motionsenseapp-0.0.1.tar.gz` & `tmp/motionsenseapp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionsenseapp-0.0.1.tar", last modified: Sat Jun  3 17:13:22 2023, max compression
+gzip compressed data, was "motionsenseapp-0.0.2.tar", last modified: Sat Jun  3 17:29:37 2023, max compression
```

## Comparing `motionsenseapp-0.0.1.tar` & `motionsenseapp-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 17:13:22.723657 motionsenseapp-0.0.1/
--rw-rw-rw-   0        0        0      384 2023-06-03 17:13:22.722659 motionsenseapp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-03 15:06:30.000000 motionsenseapp-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 17:13:22.711695 motionsenseapp-0.0.1/app/
--rw-rw-rw-   0        0        0        0 2023-06-03 15:07:39.000000 motionsenseapp-0.0.1/app/__init__.py
--rw-rw-rw-   0        0        0    34936 2023-06-03 15:11:01.000000 motionsenseapp-0.0.1/app/app.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:13:22.720666 motionsenseapp-0.0.1/motionsenseapp.egg-info/
--rw-rw-rw-   0        0        0      384 2023-06-03 17:13:22.000000 motionsenseapp-0.0.1/motionsenseapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-06-03 17:13:22.000000 motionsenseapp-0.0.1/motionsenseapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 17:13:22.000000 motionsenseapp-0.0.1/motionsenseapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-03 17:13:22.000000 motionsenseapp-0.0.1/motionsenseapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 17:13:22.724651 motionsenseapp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-03 16:50:00.000000 motionsenseapp-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:29:37.249253 motionsenseapp-0.0.2/
+-rw-rw-rw-   0        0        0      384 2023-06-03 17:29:37.248257 motionsenseapp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-03 15:06:30.000000 motionsenseapp-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 17:29:37.226328 motionsenseapp-0.0.2/app/
+-rw-rw-rw-   0        0        0        0 2023-06-03 15:07:39.000000 motionsenseapp-0.0.2/app/__init__.py
+-rw-rw-rw-   0        0        0    34936 2023-06-03 15:11:01.000000 motionsenseapp-0.0.2/app/app.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:29:37.246263 motionsenseapp-0.0.2/motionsenseapp.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-06-03 17:29:37.000000 motionsenseapp-0.0.2/motionsenseapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-03 17:29:37.000000 motionsenseapp-0.0.2/motionsenseapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 17:29:37.000000 motionsenseapp-0.0.2/motionsenseapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-03 17:29:37.000000 motionsenseapp-0.0.2/motionsenseapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-03 17:29:37.000000 motionsenseapp-0.0.2/motionsenseapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 17:29:37.250250 motionsenseapp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-06-03 17:29:18.000000 motionsenseapp-0.0.2/setup.py
```

### Comparing `motionsenseapp-0.0.1/app/app.py` & `motionsenseapp-0.0.2/app/app.py`

 * *Files identical despite different names*

### Comparing `motionsenseapp-0.0.1/setup.py` & `motionsenseapp-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import setuptools
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="motionsenseapp",
-    version="0.0.1",
+    version="0.0.2",
     author="Cole Hagen",
     author_email="hagencolej@gmail.com",
     description="Motion Sense",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    install_requires=[            # I get to this in a second
+          'mediapipe',
+          'opencv-python-headless',
+          'plotly',
+          'pandas',
+          'numpy'
+      ],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

