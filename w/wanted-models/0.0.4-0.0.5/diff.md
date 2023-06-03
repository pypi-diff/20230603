# Comparing `tmp/wanted-models-0.0.4.tar.gz` & `tmp/wanted-models-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wanted-models-0.0.4.tar", last modified: Sat Jun  3 07:26:00 2023, max compression
+gzip compressed data, was "dist\wanted-models-0.0.5.tar", last modified: Sat Jun  3 09:55:54 2023, max compression
```

## Comparing `wanted-models-0.0.4.tar` & `wanted-models-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:26:00.905296 wanted-models-0.0.4/
--rw-rw-rw-   0        0        0      193 2023-06-03 07:26:00.905296 wanted-models-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-03 07:26:00.905296 wanted-models-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-06-03 07:25:57.000000 wanted-models-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:26:00.887612 wanted-models-0.0.4/wanted_models/
--rw-rw-rw-   0        0        0      138 2023-06-03 07:25:57.000000 wanted-models-0.0.4/wanted_models/__init__.py
--rw-rw-rw-   0        0        0      570 2023-06-03 07:17:23.000000 wanted-models-0.0.4/wanted_models/base_model.py
--rw-rw-rw-   0        0        0      333 2023-06-03 07:17:23.000000 wanted-models-0.0.4/wanted_models/document.py
--rw-rw-rw-   0        0        0      124 2023-06-03 07:17:23.000000 wanted-models-0.0.4/wanted_models/photo.py
--rw-rw-rw-   0        0        0     1259 2023-06-03 07:22:54.000000 wanted-models-0.0.4/wanted_models/wanted_person.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:26:00.904127 wanted-models-0.0.4/wanted_models.egg-info/
--rw-rw-rw-   0        0        0      193 2023-06-03 07:26:00.000000 wanted-models-0.0.4/wanted_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-03 07:26:00.000000 wanted-models-0.0.4/wanted_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:26:00.000000 wanted-models-0.0.4/wanted_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 07:26:00.000000 wanted-models-0.0.4/wanted_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-03 07:26:00.000000 wanted-models-0.0.4/wanted_models.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.800849 wanted-models-0.0.5/
+-rw-rw-rw-   0        0        0      193 2023-06-03 09:55:54.799553 wanted-models-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:55:54.800849 wanted-models-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      341 2023-06-03 09:55:51.000000 wanted-models-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.780319 wanted-models-0.0.5/wanted_models/
+-rw-rw-rw-   0        0        0      138 2023-06-03 07:25:57.000000 wanted-models-0.0.5/wanted_models/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-06-03 07:17:23.000000 wanted-models-0.0.5/wanted_models/base_model.py
+-rw-rw-rw-   0        0        0      292 2023-06-03 09:55:33.000000 wanted-models-0.0.5/wanted_models/document.py
+-rw-rw-rw-   0        0        0      124 2023-06-03 07:17:23.000000 wanted-models-0.0.5/wanted_models/photo.py
+-rw-rw-rw-   0        0        0     1223 2023-06-03 09:55:41.000000 wanted-models-0.0.5/wanted_models/wanted_person.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.798552 wanted-models-0.0.5/wanted_models.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/top_level.txt
```

### Comparing `wanted-models-0.0.4/wanted_models/base_model.py` & `wanted-models-0.0.5/wanted_models/base_model.py`

 * *Files identical despite different names*

### Comparing `wanted-models-0.0.4/wanted_models/wanted_person.py` & `wanted-models-0.0.5/wanted_models/wanted_person.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime
 from typing import List, Optional
 
 from wanted_models.base_model import BaseModel
 from wanted_models.document import Document
 from wanted_models.photo import Photo
 
 
@@ -32,11 +31,11 @@
     languages: Optional[List[str]]
     state_case: Optional[str]
     article: Optional[str]
     prevent_measure: Optional[str]
     resident: Optional[str]
     documents: Optional[Document]
     description: Optional[List[str]]
-    publish_date: Optional[datetime]
+    publish_date: Optional[str]
     photo: Optional[Photo]
     criminal_record: Optional[str]
     remuneration: Optional[str]
```

