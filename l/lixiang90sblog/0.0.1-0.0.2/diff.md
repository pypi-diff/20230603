# Comparing `tmp/lixiang90sblog-0.0.1.tar.gz` & `tmp/lixiang90sblog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixiang90sblog-0.0.1.tar", last modified: Fri Jun  2 14:07:30 2023, max compression
+gzip compressed data, was "lixiang90sblog-0.0.2.tar", last modified: Fri Jun  2 14:27:35 2023, max compression
```

## Comparing `lixiang90sblog-0.0.1.tar` & `lixiang90sblog-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:07:30.884915 lixiang90sblog-0.0.1/
--rw-rw-rw-   0        0        0      719 2023-06-02 14:07:30.884915 lixiang90sblog-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-02 13:58:19.000000 lixiang90sblog-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 14:07:30.884915 lixiang90sblog-0.0.1/lixiang90sblog/
--rw-rw-rw-   0        0        0      430 2023-06-02 13:21:17.000000 lixiang90sblog-0.0.1/lixiang90sblog/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.0.1/lixiang90sblog/blog.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:07:30.884915 lixiang90sblog-0.0.1/lixiang90sblog.egg-info/
--rw-rw-rw-   0        0        0      719 2023-06-02 14:07:30.000000 lixiang90sblog-0.0.1/lixiang90sblog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-06-02 14:07:30.000000 lixiang90sblog-0.0.1/lixiang90sblog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:07:30.000000 lixiang90sblog-0.0.1/lixiang90sblog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 14:07:30.000000 lixiang90sblog-0.0.1/lixiang90sblog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 14:07:30.884915 lixiang90sblog-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-06-02 14:07:27.000000 lixiang90sblog-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:27:35.323192 lixiang90sblog-0.0.2/
+-rw-rw-rw-   0        0        0      719 2023-06-02 14:27:35.320192 lixiang90sblog-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-06-02 13:58:19.000000 lixiang90sblog-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 14:27:35.317191 lixiang90sblog-0.0.2/lixiang90sblog/
+-rw-rw-rw-   0        0        0      430 2023-06-02 13:21:17.000000 lixiang90sblog-0.0.2/lixiang90sblog/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:27:35.320192 lixiang90sblog-0.0.2/lixiang90sblog/blog/
+-rw-rw-rw-   0        0        0       45 2023-06-02 09:38:30.000000 lixiang90sblog-0.0.2/lixiang90sblog/blog/0.txt
+-rw-rw-rw-   0        0        0     1056 2023-06-02 13:08:11.000000 lixiang90sblog-0.0.2/lixiang90sblog/blog/1.txt
+-rw-rw-rw-   0        0        0      390 2023-06-02 13:05:47.000000 lixiang90sblog-0.0.2/lixiang90sblog/blog/metadata.json
+-rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.0.2/lixiang90sblog/blog.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:27:35.319192 lixiang90sblog-0.0.2/lixiang90sblog.egg-info/
+-rw-rw-rw-   0        0        0      719 2023-06-02 14:27:35.000000 lixiang90sblog-0.0.2/lixiang90sblog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-02 14:27:35.000000 lixiang90sblog-0.0.2/lixiang90sblog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:27:35.000000 lixiang90sblog-0.0.2/lixiang90sblog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 14:27:35.000000 lixiang90sblog-0.0.2/lixiang90sblog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:27:35.323192 lixiang90sblog-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-06-02 14:27:28.000000 lixiang90sblog-0.0.2/setup.py
```

### Comparing `lixiang90sblog-0.0.1/PKG-INFO` & `lixiang90sblog-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lixiang90sblog-0.0.1/lixiang90sblog/blog.py` & `lixiang90sblog-0.0.2/lixiang90sblog/blog.py`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.0.1/lixiang90sblog.egg-info/PKG-INFO` & `lixiang90sblog-0.0.2/lixiang90sblog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lixiang90sblog-0.0.1/setup.py` & `lixiang90sblog-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lixiang90sblog",  # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="Lixiang90's personal blog",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/lixiang90sblog.git",
     packages=setuptools.find_packages(),
+    package_dir={'lixiang90sblog':'lixiang90sblog'},
+    package_data={'lixiang90sblog':['blog/*.txt','blog/*.md','blog/metadata.json']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

