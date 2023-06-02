# Comparing `tmp/lixiang90sblog-0.1.0.tar.gz` & `tmp/lixiang90sblog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixiang90sblog-0.1.0.tar", last modified: Fri Jun  2 23:24:08 2023, max compression
+gzip compressed data, was "lixiang90sblog-0.1.1.tar", last modified: Fri Jun  2 23:33:55 2023, max compression
```

## Comparing `lixiang90sblog-0.1.0.tar` & `lixiang90sblog-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/
--rw-rw-rw-   0        0        0      810 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-02 23:22:16.000000 lixiang90sblog-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog/
--rw-rw-rw-   0        0        0      468 2023-06-02 20:03:42.000000 lixiang90sblog-0.1.0/lixiang90sblog/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog/blog/
--rw-rw-rw-   0        0        0       45 2023-06-02 09:38:30.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/0.txt
--rw-rw-rw-   0        0        0     1056 2023-06-02 13:08:11.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/1.txt
--rw-rw-rw-   0        0        0     7509 2023-06-02 23:11:03.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/2.txt
--rw-rw-rw-   0        0        0      390 2023-06-02 13:05:47.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/metadata.json
--rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog.py
--rw-rw-rw-   0        0        0      990 2023-06-02 21:15:03.000000 lixiang90sblog-0.1.0/lixiang90sblog/client.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/
--rw-rw-rw-   0        0        0      810 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-06-02 23:23:00.000000 lixiang90sblog-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/
+-rw-rw-rw-   0        0        0      810 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-02 23:22:16.000000 lixiang90sblog-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/lixiang90sblog/
+-rw-rw-rw-   0        0        0      468 2023-06-02 20:03:42.000000 lixiang90sblog-0.1.1/lixiang90sblog/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/lixiang90sblog/blog/
+-rw-rw-rw-   0        0        0       45 2023-06-02 09:38:30.000000 lixiang90sblog-0.1.1/lixiang90sblog/blog/0.txt
+-rw-rw-rw-   0        0        0     1056 2023-06-02 13:08:11.000000 lixiang90sblog-0.1.1/lixiang90sblog/blog/1.txt
+-rw-rw-rw-   0        0        0     7509 2023-06-02 23:11:03.000000 lixiang90sblog-0.1.1/lixiang90sblog/blog/2.txt
+-rw-rw-rw-   0        0        0      806 2023-06-02 23:30:12.000000 lixiang90sblog-0.1.1/lixiang90sblog/blog/metadata.json
+-rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.1.1/lixiang90sblog/blog.py
+-rw-rw-rw-   0        0        0      990 2023-06-02 21:15:03.000000 lixiang90sblog-0.1.1/lixiang90sblog/client.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/lixiang90sblog.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-06-02 23:33:55.000000 lixiang90sblog-0.1.1/lixiang90sblog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-02 23:33:55.000000 lixiang90sblog-0.1.1/lixiang90sblog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 23:33:55.000000 lixiang90sblog-0.1.1/lixiang90sblog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 23:33:55.000000 lixiang90sblog-0.1.1/lixiang90sblog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 23:33:55.602078 lixiang90sblog-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-06-02 23:33:31.000000 lixiang90sblog-0.1.1/setup.py
```

### Comparing `lixiang90sblog-0.1.0/PKG-INFO` & `lixiang90sblog-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lixiang90sblog-0.1.0/lixiang90sblog/blog/1.txt` & `lixiang90sblog-0.1.1/lixiang90sblog/blog/1.txt`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.1.0/lixiang90sblog/blog/2.txt` & `lixiang90sblog-0.1.1/lixiang90sblog/blog/2.txt`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.1.0/lixiang90sblog/blog.py` & `lixiang90sblog-0.1.1/lixiang90sblog/blog.py`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.1.0/lixiang90sblog/client.py` & `lixiang90sblog-0.1.1/lixiang90sblog/client.py`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.1.0/lixiang90sblog.egg-info/PKG-INFO` & `lixiang90sblog-0.1.1/lixiang90sblog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lixiang90sblog-0.1.0/setup.py` & `lixiang90sblog-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lixiang90sblog",  # Replace with your own username
-    version="0.1.0",
+    version="0.1.1",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="Lixiang90's personal blog",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/lixiang90sblog.git",
     packages=setuptools.find_packages(),
```

