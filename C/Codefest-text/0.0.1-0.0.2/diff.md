# Comparing `tmp/Codefest_text-0.0.1.tar.gz` & `tmp/Codefest_text-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Codefest_text-0.0.1.tar", last modified: Sat Jun  3 08:49:57 2023, max compression
+gzip compressed data, was "Codefest_text-0.0.2.tar", last modified: Sat Jun  3 09:22:54 2023, max compression
```

## Comparing `Codefest_text-0.0.1.tar` & `Codefest_text-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 08:49:57.224512 Codefest_text-0.0.1/
-drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 08:49:57.224512 Codefest_text-0.0.1/Codefest_text/
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       64 2023-06-03 08:40:18.000000 Codefest_text-0.0.1/Codefest_text/__init__.py
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)     4004 2023-06-03 08:37:33.000000 Codefest_text-0.0.1/Codefest_text/functions.py
-drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 08:49:57.224512 Codefest_text-0.0.1/Codefest_text.egg-info/
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      179 2023-06-03 08:49:57.000000 Codefest_text-0.0.1/Codefest_text.egg-info/PKG-INFO
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      255 2023-06-03 08:49:57.000000 Codefest_text-0.0.1/Codefest_text.egg-info/SOURCES.txt
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)        1 2023-06-03 08:49:57.000000 Codefest_text-0.0.1/Codefest_text.egg-info/dependency_links.txt
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       56 2023-06-03 08:49:57.000000 Codefest_text-0.0.1/Codefest_text.egg-info/requires.txt
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       14 2023-06-03 08:49:57.000000 Codefest_text-0.0.1/Codefest_text.egg-info/top_level.txt
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      179 2023-06-03 08:49:57.224512 Codefest_text-0.0.1/PKG-INFO
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 06:11:14.000000 Codefest_text-0.0.1/README.md
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       38 2023-06-03 08:49:57.224512 Codefest_text-0.0.1/setup.cfg
--rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)     1319 2023-06-03 08:43:39.000000 Codefest_text-0.0.1/setup.py
+drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 09:22:54.624082 Codefest_text-0.0.2/
+drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 09:22:54.624082 Codefest_text-0.0.2/Codefest_text/
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       64 2023-06-03 08:40:18.000000 Codefest_text-0.0.2/Codefest_text/__init__.py
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)     4004 2023-06-03 08:37:33.000000 Codefest_text-0.0.2/Codefest_text/functions.py
+drwxr-xr-x   0 santiagofr  (1000) santiagofr  (1000)        0 2023-06-03 09:22:54.624082 Codefest_text-0.0.2/Codefest_text.egg-info/
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      196 2023-06-03 09:22:54.000000 Codefest_text-0.0.2/Codefest_text.egg-info/PKG-INFO
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      255 2023-06-03 09:22:54.000000 Codefest_text-0.0.2/Codefest_text.egg-info/SOURCES.txt
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)        1 2023-06-03 09:22:54.000000 Codefest_text-0.0.2/Codefest_text.egg-info/dependency_links.txt
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       56 2023-06-03 09:22:54.000000 Codefest_text-0.0.2/Codefest_text.egg-info/requires.txt
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       14 2023-06-03 09:22:54.000000 Codefest_text-0.0.2/Codefest_text.egg-info/top_level.txt
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)      196 2023-06-03 09:22:54.624082 Codefest_text-0.0.2/PKG-INFO
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       15 2023-06-03 09:20:42.000000 Codefest_text-0.0.2/README.md
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)       38 2023-06-03 09:22:54.624082 Codefest_text-0.0.2/setup.cfg
+-rw-r--r--   0 santiagofr  (1000) santiagofr  (1000)     1319 2023-06-03 09:22:50.000000 Codefest_text-0.0.2/setup.py
```

### Comparing `Codefest_text-0.0.1/Codefest_text/functions.py` & `Codefest_text-0.0.2/Codefest_text/functions.py`

 * *Files identical despite different names*

### Comparing `Codefest_text-0.0.1/setup.py` & `Codefest_text-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.1' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.2' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'Codefest_text' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Geo Army' #Modificar con vuestros datos
 AUTHOR_EMAIL = '' #Modificar con vuestros datos
 URL = '' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para ' #Descripción corta
```

