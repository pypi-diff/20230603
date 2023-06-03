# Comparing `tmp/SLIW-0.0.2.tar.gz` & `tmp/sliw-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SLIW-0.0.2.tar", last modified: Sat Jun  3 17:57:44 2023, max compression
+gzip compressed data, was "sliw-0.0.5.tar", last modified: Sat Jun  3 12:30:46 2023, max compression
```

## Comparing `SLIW-0.0.2.tar` & `sliw-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:44.688614 SLIW-0.0.2/
--rw-rw-rw-   0        0        0      456 2023-06-03 17:57:44.684611 SLIW-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:44.568586 SLIW-0.0.2/SLIN_GN/
--rw-rw-rw-   0        0        0     8085 2023-06-03 17:57:24.000000 SLIW-0.0.2/SLIN_GN/SLIW_GN.py
--rw-rw-rw-   0        0        0       65 2023-06-03 17:57:21.000000 SLIW-0.0.2/SLIN_GN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:44.676612 SLIW-0.0.2/SLIW.egg-info/
--rw-rw-rw-   0        0        0      456 2023-06-03 17:57:44.000000 SLIW-0.0.2/SLIW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-06-03 17:57:44.000000 SLIW-0.0.2/SLIW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 17:57:44.000000 SLIW-0.0.2/SLIW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 17:57:44.000000 SLIW-0.0.2/SLIW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 17:57:44.000000 SLIW-0.0.2/SLIW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 17:57:44.688614 SLIW-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-03 17:57:25.000000 SLIW-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:30:46.274211 sliw-0.0.5/
+-rw-rw-rw-   0        0        0      456 2023-06-03 12:30:46.270209 sliw-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:30:46.274211 sliw-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-03 12:29:48.000000 sliw-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:30:46.162186 sliw-0.0.5/sliw/
+-rw-rw-rw-   0        0        0       54 2023-06-03 12:29:45.000000 sliw-0.0.5/sliw/__init__.py
+-rw-rw-rw-   0        0        0     4546 2023-06-03 12:29:46.000000 sliw-0.0.5/sliw/sliw.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:30:46.266209 sliw-0.0.5/sliw.egg-info/
+-rw-rw-rw-   0        0        0      456 2023-06-03 12:30:45.000000 sliw-0.0.5/sliw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-03 12:30:45.000000 sliw-0.0.5/sliw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:30:45.000000 sliw-0.0.5/sliw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 12:30:45.000000 sliw-0.0.5/sliw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-03 12:30:45.000000 sliw-0.0.5/sliw.egg-info/top_level.txt
```

### Comparing `SLIW-0.0.2/setup.py` & `sliw-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.5'
 DESCRIPTION = 'Command analyzer for pandas new version'
 
 # Setting up
 setup(
-    name="SLIW",
+    name="sliw",
     version=VERSION,
     author="sliw team",
     author_email="giokhvichia69@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/plain",
     packages=find_packages(),
     install_requires=[
```

