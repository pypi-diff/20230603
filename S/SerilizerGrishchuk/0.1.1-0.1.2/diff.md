# Comparing `tmp/SerilizerGrishchuk-0.1.1.tar.gz` & `tmp/SerilizerGrishchuk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerilizerGrishchuk-0.1.1.tar", last modified: Sat Jun  3 15:26:53 2023, max compression
+gzip compressed data, was "SerilizerGrishchuk-0.1.2.tar", last modified: Sat Jun  3 15:30:01 2023, max compression
```

## Comparing `SerilizerGrishchuk-0.1.1.tar` & `SerilizerGrishchuk-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:26:53.507724 SerilizerGrishchuk-0.1.1/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      720 2023-06-03 15:26:53.507724 SerilizerGrishchuk-0.1.1/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-05-10 18:19:58.000000 SerilizerGrishchuk-0.1.1/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:26:53.507724 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      407 2023-06-03 14:33:17.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/Creator.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3150 2023-06-03 14:32:46.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/JSONSerializer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3267 2023-06-03 14:33:04.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/XMLSerializator.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      120 2023-06-03 15:18:16.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      554 2023-05-10 18:20:03.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/constans.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    11727 2023-06-03 14:29:41.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/serializer_functions.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:26:53.507724 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      720 2023-06-03 15:26:53.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      437 2023-06-03 15:26:53.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-03 15:26:53.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        6 2023-06-03 15:26:53.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       19 2023-06-03 15:26:53.000000 SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-03 15:26:53.507724 SerilizerGrishchuk-0.1.1/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1240 2023-06-03 15:26:43.000000 SerilizerGrishchuk-0.1.1/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:30:01.969309 SerilizerGrishchuk-0.1.2/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      720 2023-06-03 15:30:01.969309 SerilizerGrishchuk-0.1.2/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-05-10 18:19:58.000000 SerilizerGrishchuk-0.1.2/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:30:01.969309 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      409 2023-06-03 15:29:26.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/Creator.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3151 2023-06-03 15:29:26.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/JSONSerializer.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3268 2023-06-03 15:29:26.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/XMLSerializator.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      120 2023-06-03 15:18:16.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      554 2023-05-10 18:20:03.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/constans.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11728 2023-06-03 15:29:26.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/serializer_functions.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-03 15:30:01.969309 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      720 2023-06-03 15:30:01.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      437 2023-06-03 15:30:01.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-03 15:30:01.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        6 2023-06-03 15:30:01.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       19 2023-06-03 15:30:01.000000 SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-03 15:30:01.969309 SerilizerGrishchuk-0.1.2/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1240 2023-06-03 15:29:53.000000 SerilizerGrishchuk-0.1.2/setup.py
```

### Comparing `SerilizerGrishchuk-0.1.1/PKG-INFO` & `SerilizerGrishchuk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerilizerGrishchuk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Grishchuk Alexandr
 Author-email: grishchuk.2004ag@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/JSONSerializer.py` & `SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/JSONSerializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from serializer_functions import serialize, deserialize
+from .serializer_functions import serialize, deserialize
 import regex
 
 class JsonSerializer:
     INT_P = r"[+-]?\d+"
     FLOAT_P = r"(?:[+-]?\d+(?:\.\d+)?(?:e[+-]?\d+)?)"
     BOOL_P = r"((?:true)|(?:false))\b"
     STR_P = r"\"(?:(?:\\\")|[^\"])*\""
```

### Comparing `SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/XMLSerializator.py` & `SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/XMLSerializator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from serializer_functions import serialize, deserialize
+from .serializer_functions import serialize, deserialize
 import regex
 
 class XMLSerializer:
     
     BASE_TYPES = r"str|int|float|bool|NoneType|list|dict"
     key = "key"
     val = "value"
```

### Comparing `SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/constans.py` & `SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/constans.py`

 * *Files identical despite different names*

### Comparing `SerilizerGrishchuk-0.1.1/SerilizerGrishchuk/serializer_functions.py` & `SerilizerGrishchuk-0.1.2/SerilizerGrishchuk/serializer_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import inspect
 import types
-from constans import CODE, BASE_TYPE, BASE_COLLECTION
+from .constans import CODE, BASE_TYPE, BASE_COLLECTION
 
 
 def serialize(obj):
     ser = dict()
     obj_type = type(obj)
     def get_base_type():
         return re.search(r"\'(\w+)\'", str(obj_type))[1]
```

### Comparing `SerilizerGrishchuk-0.1.1/SerilizerGrishchuk.egg-info/PKG-INFO` & `SerilizerGrishchuk-0.1.2/SerilizerGrishchuk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerilizerGrishchuk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Grishchuk Alexandr
 Author-email: grishchuk.2004ag@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerilizerGrishchuk-0.1.1/setup.py` & `SerilizerGrishchuk-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="SerilizerGrishchuk",
-    version="0.1.1",
+    version="0.1.2",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Grishchuk Alexandr",
     author_email="grishchuk.2004ag@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

