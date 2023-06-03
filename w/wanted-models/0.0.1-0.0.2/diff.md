# Comparing `tmp/wanted-models-0.0.1.tar.gz` & `tmp/wanted-models-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wanted-models-0.0.1.tar", last modified: Sat Jun  3 07:10:23 2023, max compression
+gzip compressed data, was "dist\wanted-models-0.0.2.tar", last modified: Sat Jun  3 07:17:38 2023, max compression
```

## Comparing `wanted-models-0.0.1.tar` & `wanted-models-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:10:23.718734 wanted-models-0.0.1/
--rw-rw-rw-   0        0        0      193 2023-06-03 07:10:23.718734 wanted-models-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-03 07:10:23.718734 wanted-models-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-06-03 07:09:55.000000 wanted-models-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:10:23.694345 wanted-models-0.0.1/wanted_models/
--rw-rw-rw-   0        0        0      125 2023-06-03 07:09:34.000000 wanted-models-0.0.1/wanted_models/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-03 07:08:14.000000 wanted-models-0.0.1/wanted_models/document.py
--rw-rw-rw-   0        0        0      108 2023-06-03 07:08:23.000000 wanted-models-0.0.1/wanted_models/photo.py
--rw-rw-rw-   0        0        0     1239 2023-06-03 07:09:34.000000 wanted-models-0.0.1/wanted_models/record.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:10:23.716696 wanted-models-0.0.1/wanted_models.egg-info/
--rw-rw-rw-   0        0        0      193 2023-06-03 07:10:23.000000 wanted-models-0.0.1/wanted_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-03 07:10:23.000000 wanted-models-0.0.1/wanted_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:10:23.000000 wanted-models-0.0.1/wanted_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 07:10:23.000000 wanted-models-0.0.1/wanted_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-03 07:10:23.000000 wanted-models-0.0.1/wanted_models.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 07:17:38.093103 wanted-models-0.0.2/
+-rw-rw-rw-   0        0        0      193 2023-06-03 07:17:38.092118 wanted-models-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-03 07:17:38.093103 wanted-models-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      341 2023-06-03 07:17:33.000000 wanted-models-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:17:38.079278 wanted-models-0.0.2/wanted_models/
+-rw-rw-rw-   0        0        0      125 2023-06-03 07:09:34.000000 wanted-models-0.0.2/wanted_models/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-06-03 07:17:23.000000 wanted-models-0.0.2/wanted_models/base_model.py
+-rw-rw-rw-   0        0        0      333 2023-06-03 07:17:23.000000 wanted-models-0.0.2/wanted_models/document.py
+-rw-rw-rw-   0        0        0      124 2023-06-03 07:17:23.000000 wanted-models-0.0.2/wanted_models/photo.py
+-rw-rw-rw-   0        0        0     1253 2023-06-03 07:17:23.000000 wanted-models-0.0.2/wanted_models/record.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:17:38.091136 wanted-models-0.0.2/wanted_models.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-06-03 07:17:38.000000 wanted-models-0.0.2/wanted_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-06-03 07:17:38.000000 wanted-models-0.0.2/wanted_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 07:17:38.000000 wanted-models-0.0.2/wanted_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 07:17:38.000000 wanted-models-0.0.2/wanted_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-03 07:17:38.000000 wanted-models-0.0.2/wanted_models.egg-info/top_level.txt
```

### Comparing `wanted-models-0.0.1/wanted_models/record.py` & `wanted-models-0.0.2/wanted_models/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from datetime import datetime
 from typing import List, Optional
 
-from pydantic import BaseModel
-
+from wanted_models.base_model import BaseModel
 from wanted_models.document import Document
 from wanted_models.photo import Photo
 
 
 class Record(BaseModel):
     platform_id: str
     url: Optional[str]
```

