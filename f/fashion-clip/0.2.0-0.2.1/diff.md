# Comparing `tmp/fashion-clip-0.2.0.tar.gz` & `tmp/fashion-clip-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fashion-clip-0.2.0.tar", last modified: Fri Jun  2 22:40:32 2023, max compression
+gzip compressed data, was "fashion-clip-0.2.1.tar", last modified: Fri Jun  2 22:53:08 2023, max compression
```

## Comparing `fashion-clip-0.2.0.tar` & `fashion-clip-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:40:32.011661 fashion-clip-0.2.0/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-04-04 01:09:03.000000 fashion-clip-0.2.0/LICENSE
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       58 2023-06-02 22:32:42.000000 fashion-clip-0.2.0/MANIFEST.in
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    10505 2023-06-02 22:40:32.011661 fashion-clip-0.2.0/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     9820 2023-06-02 22:26:04.000000 fashion-clip-0.2.0/README.md
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:40:32.011661 fashion-clip-0.2.0/fashion_clip/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-03-03 05:22:25.000000 fashion-clip-0.2.0/fashion_clip/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     2608 2023-03-03 05:22:25.000000 fashion-clip-0.2.0/fashion_clip/attention_map.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    14208 2023-06-02 22:32:42.000000 fashion-clip-0.2.0/fashion_clip/fashion_clip.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     3579 2023-03-03 05:22:25.000000 fashion-clip-0.2.0/fashion_clip/s3_client.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     6047 2023-03-03 05:22:25.000000 fashion-clip-0.2.0/fashion_clip/utils.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:40:32.011661 fashion-clip-0.2.0/fashion_clip.egg-info/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    10505 2023-06-02 22:40:31.000000 fashion-clip-0.2.0/fashion_clip.egg-info/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      411 2023-06-02 22:40:31.000000 fashion-clip-0.2.0/fashion_clip.egg-info/SOURCES.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-06-02 22:40:31.000000 fashion-clip-0.2.0/fashion_clip.egg-info/dependency_links.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-04-06 20:01:33.000000 fashion-clip-0.2.0/fashion_clip.egg-info/not-zip-safe
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      180 2023-06-02 22:40:31.000000 fashion-clip-0.2.0/fashion_clip.egg-info/requires.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       13 2023-06-02 22:40:31.000000 fashion-clip-0.2.0/fashion_clip.egg-info/top_level.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      179 2023-06-02 22:32:42.000000 fashion-clip-0.2.0/requirements.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      179 2023-06-02 22:40:32.011661 fashion-clip-0.2.0/setup.cfg
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1076 2023-06-02 22:36:15.000000 fashion-clip-0.2.0/setup.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:53:08.235684 fashion-clip-0.2.1/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-04-04 01:09:03.000000 fashion-clip-0.2.1/LICENSE
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       58 2023-06-02 22:32:42.000000 fashion-clip-0.2.1/MANIFEST.in
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    10561 2023-06-02 22:53:08.235684 fashion-clip-0.2.1/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     9820 2023-06-02 22:26:04.000000 fashion-clip-0.2.1/README.md
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:53:08.235684 fashion-clip-0.2.1/fashion_clip/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-03-03 05:22:25.000000 fashion-clip-0.2.1/fashion_clip/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2608 2023-03-03 05:22:25.000000 fashion-clip-0.2.1/fashion_clip/attention_map.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    14208 2023-06-02 22:32:42.000000 fashion-clip-0.2.1/fashion_clip/fashion_clip.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     3579 2023-03-03 05:22:25.000000 fashion-clip-0.2.1/fashion_clip/s3_client.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     6047 2023-03-03 05:22:25.000000 fashion-clip-0.2.1/fashion_clip/utils.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-06-02 22:53:08.235684 fashion-clip-0.2.1/fashion_clip.egg-info/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    10561 2023-06-02 22:53:08.000000 fashion-clip-0.2.1/fashion_clip.egg-info/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      411 2023-06-02 22:53:08.000000 fashion-clip-0.2.1/fashion_clip.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-06-02 22:53:08.000000 fashion-clip-0.2.1/fashion_clip.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-04-06 20:01:33.000000 fashion-clip-0.2.1/fashion_clip.egg-info/not-zip-safe
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      191 2023-06-02 22:53:08.000000 fashion-clip-0.2.1/fashion_clip.egg-info/requires.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       13 2023-06-02 22:53:08.000000 fashion-clip-0.2.1/fashion_clip.egg-info/top_level.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      190 2023-06-02 22:52:15.000000 fashion-clip-0.2.1/requirements.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      179 2023-06-02 22:53:08.239684 fashion-clip-0.2.1/setup.cfg
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1076 2023-06-02 22:53:07.000000 fashion-clip-0.2.1/setup.py
```

### Comparing `fashion-clip-0.2.0/LICENSE` & `fashion-clip-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/PKG-INFO` & `fashion-clip-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: fashion-clip
-Version: 0.2.0
+Version: 0.2.1
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: Jacopo Tagliabue, Patrick John Chia, Federico Bianchi
 Author-email: jtagliabue@coveo.com, pchia@coveo.com, f.bianchi@unibocconi.it
 License: MIT license
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -218,7 +221,9 @@
                        image_source_path='path/to/images', 
                        image_source_type='local')
 fclip = FashionCLIP('fasihon-clip', ff_dataset)
 ```
 
 For further details on how to use the package, refer to the accompanying notebook!
 
+
+
```

### Comparing `fashion-clip-0.2.0/README.md` & `fashion-clip-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/fashion_clip/attention_map.py` & `fashion-clip-0.2.1/fashion_clip/attention_map.py`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/fashion_clip/fashion_clip.py` & `fashion-clip-0.2.1/fashion_clip/fashion_clip.py`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/fashion_clip/s3_client.py` & `fashion-clip-0.2.1/fashion_clip/s3_client.py`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/fashion_clip/utils.py` & `fashion-clip-0.2.1/fashion_clip/utils.py`

 * *Files identical despite different names*

### Comparing `fashion-clip-0.2.0/fashion_clip.egg-info/PKG-INFO` & `fashion-clip-0.2.1/fashion_clip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: fashion-clip
-Version: 0.2.0
+Version: 0.2.1
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: Jacopo Tagliabue, Patrick John Chia, Federico Bianchi
 Author-email: jtagliabue@coveo.com, pchia@coveo.com, f.bianchi@unibocconi.it
 License: MIT license
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -218,7 +221,9 @@
                        image_source_path='path/to/images', 
                        image_source_type='local')
 fclip = FashionCLIP('fasihon-clip', ff_dataset)
 ```
 
 For further details on how to use the package, refer to the accompanying notebook!
 
+
+
```

### Comparing `fashion-clip-0.2.0/setup.py` & `fashion-clip-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='fashion-clip',
-    version='0.2.0',
+    version='0.2.1',
     description='',
     python_requires='>=3.5',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
```

