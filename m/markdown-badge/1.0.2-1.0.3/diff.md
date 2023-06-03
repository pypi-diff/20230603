# Comparing `tmp/markdown-badge-1.0.2.tar.gz` & `tmp/markdown-badge-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-badge-1.0.2.tar", last modified: Fri Jun  2 23:53:20 2023, max compression
+gzip compressed data, was "markdown-badge-1.0.3.tar", last modified: Sat Jun  3 00:00:08 2023, max compression
```

## Comparing `markdown-badge-1.0.2.tar` & `markdown-badge-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-02 23:53:20.456813 markdown-badge-1.0.2/
--rw-r--r--   0 afletcher   (502) staff       (20)     1072 2023-05-20 04:03:15.000000 markdown-badge-1.0.2/LICENSE
--rw-r--r--   0 afletcher   (502) staff       (20)     2361 2023-06-02 23:53:20.456301 markdown-badge-1.0.2/PKG-INFO
--rw-r--r--   0 afletcher   (502) staff       (20)     1731 2023-05-20 04:06:02.000000 markdown-badge-1.0.2/README.md
-drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-02 23:53:20.454988 markdown-badge-1.0.2/markdown_badge.egg-info/
--rw-r--r--   0 afletcher   (502) staff       (20)     2361 2023-06-02 23:53:20.000000 markdown-badge-1.0.2/markdown_badge.egg-info/PKG-INFO
--rw-r--r--   0 afletcher   (502) staff       (20)      259 2023-06-02 23:53:20.000000 markdown-badge-1.0.2/markdown_badge.egg-info/SOURCES.txt
--rw-r--r--   0 afletcher   (502) staff       (20)        1 2023-06-02 23:53:20.000000 markdown-badge-1.0.2/markdown_badge.egg-info/dependency_links.txt
--rw-r--r--   0 afletcher   (502) staff       (20)       23 2023-06-02 23:53:20.000000 markdown-badge-1.0.2/markdown_badge.egg-info/requires.txt
--rw-r--r--   0 afletcher   (502) staff       (20)       15 2023-06-02 23:53:20.000000 markdown-badge-1.0.2/markdown_badge.egg-info/top_level.txt
--rw-r--r--   0 afletcher   (502) staff       (20)       38 2023-06-02 23:53:20.457014 markdown-badge-1.0.2/setup.cfg
--rw-r--r--   0 afletcher   (502) staff       (20)      973 2023-06-02 23:53:06.000000 markdown-badge-1.0.2/setup.py
-drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-02 23:53:20.455872 markdown-badge-1.0.2/tests/
--rw-r--r--   0 afletcher   (502) staff       (20)     1967 2023-05-20 04:09:31.000000 markdown-badge-1.0.2/tests/test_badge.py
--rw-r--r--   0 afletcher   (502) staff       (20)      548 2023-05-20 04:11:08.000000 markdown-badge-1.0.2/tests/test_extension.py
+drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-03 00:00:08.817237 markdown-badge-1.0.3/
+-rw-r--r--   0 afletcher   (502) staff       (20)     1072 2023-05-20 04:03:15.000000 markdown-badge-1.0.3/LICENSE
+-rw-r--r--   0 afletcher   (502) staff       (20)     2361 2023-06-03 00:00:08.816901 markdown-badge-1.0.3/PKG-INFO
+-rw-r--r--   0 afletcher   (502) staff       (20)     1731 2023-05-20 04:06:02.000000 markdown-badge-1.0.3/README.md
+drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-03 00:00:08.815546 markdown-badge-1.0.3/markdown_badge.egg-info/
+-rw-r--r--   0 afletcher   (502) staff       (20)     2361 2023-06-03 00:00:08.000000 markdown-badge-1.0.3/markdown_badge.egg-info/PKG-INFO
+-rw-r--r--   0 afletcher   (502) staff       (20)      259 2023-06-03 00:00:08.000000 markdown-badge-1.0.3/markdown_badge.egg-info/SOURCES.txt
+-rw-r--r--   0 afletcher   (502) staff       (20)        1 2023-06-03 00:00:08.000000 markdown-badge-1.0.3/markdown_badge.egg-info/dependency_links.txt
+-rw-r--r--   0 afletcher   (502) staff       (20)       14 2023-06-03 00:00:08.000000 markdown-badge-1.0.3/markdown_badge.egg-info/requires.txt
+-rw-r--r--   0 afletcher   (502) staff       (20)       15 2023-06-03 00:00:08.000000 markdown-badge-1.0.3/markdown_badge.egg-info/top_level.txt
+-rw-r--r--   0 afletcher   (502) staff       (20)       38 2023-06-03 00:00:08.817313 markdown-badge-1.0.3/setup.cfg
+-rw-r--r--   0 afletcher   (502) staff       (20)      961 2023-06-02 23:59:46.000000 markdown-badge-1.0.3/setup.py
+drwxr-xr-x   0 afletcher   (502) staff       (20)        0 2023-06-03 00:00:08.816426 markdown-badge-1.0.3/tests/
+-rw-r--r--   0 afletcher   (502) staff       (20)     1967 2023-05-20 04:09:31.000000 markdown-badge-1.0.3/tests/test_badge.py
+-rw-r--r--   0 afletcher   (502) staff       (20)      548 2023-05-20 04:11:08.000000 markdown-badge-1.0.3/tests/test_extension.py
```

### Comparing `markdown-badge-1.0.2/LICENSE` & `markdown-badge-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-badge-1.0.2/PKG-INFO` & `markdown-badge-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-badge
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extension for python-markdown that adds markdown syntax for badges.
 Home-page: https://github.com/BitwiseAndrea/python-markdown.git
 Author: Andrea Fletcher
 Author-email: bitwiseandrea@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `markdown-badge-1.0.2/README.md` & `markdown-badge-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `markdown-badge-1.0.2/markdown_badge.egg-info/PKG-INFO` & `markdown-badge-1.0.3/markdown_badge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-badge
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extension for python-markdown that adds markdown syntax for badges.
 Home-page: https://github.com/BitwiseAndrea/python-markdown.git
 Author: Andrea Fletcher
 Author-email: bitwiseandrea@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `markdown-badge-1.0.2/setup.py` & `markdown-badge-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="markdown-badge",
-    version="1.0.2",
+    version="1.0.3",
     description='Extension for python-markdown that adds markdown syntax for badges.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/BitwiseAndrea/python-markdown.git',
     author='Andrea Fletcher',
     author_email='bitwiseandrea@gmail.com',
     license='MIT',
@@ -22,9 +22,9 @@
         "Programming Language :: Python :: 3",
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Topic :: Text Processing :: Markup',
         'Topic :: Text Processing :: Markup :: HTML',
     ],
     py_modules=["markdown-badge"],  
-    install_requires=["markdown>=3.0", "unittest"],
+    install_requires=["markdown>=3.0"],
 )
```

### Comparing `markdown-badge-1.0.2/tests/test_badge.py` & `markdown-badge-1.0.3/tests/test_badge.py`

 * *Files identical despite different names*

### Comparing `markdown-badge-1.0.2/tests/test_extension.py` & `markdown-badge-1.0.3/tests/test_extension.py`

 * *Files identical despite different names*

