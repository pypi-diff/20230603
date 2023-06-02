# Comparing `tmp/lixiang90sblog-0.0.3.tar.gz` & `tmp/lixiang90sblog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixiang90sblog-0.0.3.tar", last modified: Fri Jun  2 23:15:32 2023, max compression
+gzip compressed data, was "lixiang90sblog-0.1.0.tar", last modified: Fri Jun  2 23:24:08 2023, max compression
```

## Comparing `lixiang90sblog-0.0.3.tar` & `lixiang90sblog-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:32.712334 lixiang90sblog-0.0.3/
--rw-rw-rw-   0        0        0      719 2023-06-02 23:15:32.712334 lixiang90sblog-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-02 13:58:19.000000 lixiang90sblog-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:32.681025 lixiang90sblog-0.0.3/lixiang90sblog/
--rw-rw-rw-   0        0        0      468 2023-06-02 20:03:42.000000 lixiang90sblog-0.0.3/lixiang90sblog/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:32.712334 lixiang90sblog-0.0.3/lixiang90sblog/blog/
--rw-rw-rw-   0        0        0       45 2023-06-02 09:38:30.000000 lixiang90sblog-0.0.3/lixiang90sblog/blog/0.txt
--rw-rw-rw-   0        0        0     1056 2023-06-02 13:08:11.000000 lixiang90sblog-0.0.3/lixiang90sblog/blog/1.txt
--rw-rw-rw-   0        0        0     7509 2023-06-02 23:11:03.000000 lixiang90sblog-0.0.3/lixiang90sblog/blog/2.txt
--rw-rw-rw-   0        0        0      390 2023-06-02 13:05:47.000000 lixiang90sblog-0.0.3/lixiang90sblog/blog/metadata.json
--rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.0.3/lixiang90sblog/blog.py
--rw-rw-rw-   0        0        0      990 2023-06-02 21:15:03.000000 lixiang90sblog-0.0.3/lixiang90sblog/client.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:32.681025 lixiang90sblog-0.0.3/lixiang90sblog.egg-info/
--rw-rw-rw-   0        0        0      719 2023-06-02 23:15:32.000000 lixiang90sblog-0.0.3/lixiang90sblog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-02 23:15:32.000000 lixiang90sblog-0.0.3/lixiang90sblog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 23:15:32.000000 lixiang90sblog-0.0.3/lixiang90sblog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 23:15:32.000000 lixiang90sblog-0.0.3/lixiang90sblog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 23:15:32.712334 lixiang90sblog-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-06-02 23:14:39.000000 lixiang90sblog-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/
+-rw-rw-rw-   0        0        0      810 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-02 23:22:16.000000 lixiang90sblog-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog/
+-rw-rw-rw-   0        0        0      468 2023-06-02 20:03:42.000000 lixiang90sblog-0.1.0/lixiang90sblog/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog/blog/
+-rw-rw-rw-   0        0        0       45 2023-06-02 09:38:30.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/0.txt
+-rw-rw-rw-   0        0        0     1056 2023-06-02 13:08:11.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/1.txt
+-rw-rw-rw-   0        0        0     7509 2023-06-02 23:11:03.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/2.txt
+-rw-rw-rw-   0        0        0      390 2023-06-02 13:05:47.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog/metadata.json
+-rw-rw-rw-   0        0        0     2064 2023-06-02 12:36:13.000000 lixiang90sblog-0.1.0/lixiang90sblog/blog.py
+-rw-rw-rw-   0        0        0      990 2023-06-02 21:15:03.000000 lixiang90sblog-0.1.0/lixiang90sblog/client.py
+drwxrwxrwx   0        0        0        0 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 23:24:08.000000 lixiang90sblog-0.1.0/lixiang90sblog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 23:24:08.424511 lixiang90sblog-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-06-02 23:23:00.000000 lixiang90sblog-0.1.0/setup.py
```

### Comparing `lixiang90sblog-0.0.3/PKG-INFO` & `lixiang90sblog-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.0.3
+Version: 0.1.0
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # lixiang90sblog
 
 lixiang90的个人博客
 
 ## list_articles()
@@ -26,7 +26,11 @@
 ## print_article(title)
 
 输入标题title，在控制台上打印文章
 
 ## print_article_by_id(id)
 
 输入文章序号id，在控制台上打印文章
+
+## client()
+
+一个简单的命令行界面，可以用于选择和阅读博客文章
```

### Comparing `lixiang90sblog-0.0.3/lixiang90sblog/blog/1.txt` & `lixiang90sblog-0.1.0/lixiang90sblog/blog/1.txt`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.0.3/lixiang90sblog/blog/2.txt` & `lixiang90sblog-0.1.0/lixiang90sblog/blog/2.txt`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.0.3/lixiang90sblog/blog.py` & `lixiang90sblog-0.1.0/lixiang90sblog/blog.py`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.0.3/lixiang90sblog/client.py` & `lixiang90sblog-0.1.0/lixiang90sblog/client.py`

 * *Files identical despite different names*

### Comparing `lixiang90sblog-0.0.3/lixiang90sblog.egg-info/PKG-INFO` & `lixiang90sblog-0.1.0/lixiang90sblog.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lixiang90sblog
-Version: 0.0.3
+Version: 0.1.0
 Summary: Lixiang90's personal blog
 Home-page: https://github.com/lixiang90/lixiang90sblog.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # lixiang90sblog
 
 lixiang90的个人博客
 
 ## list_articles()
@@ -26,7 +26,11 @@
 ## print_article(title)
 
 输入标题title，在控制台上打印文章
 
 ## print_article_by_id(id)
 
 输入文章序号id，在控制台上打印文章
+
+## client()
+
+一个简单的命令行界面，可以用于选择和阅读博客文章
```

### Comparing `lixiang90sblog-0.0.3/setup.py` & `lixiang90sblog-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lixiang90sblog",  # Replace with your own username
-    version="0.0.3",
+    version="0.1.0",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="Lixiang90's personal blog",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/lixiang90sblog.git",
     packages=setuptools.find_packages(),
     package_dir={'lixiang90sblog':'lixiang90sblog'},
     package_data={'lixiang90sblog':['blog/*.txt','blog/*.md','blog/metadata.json']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

