# Comparing `tmp/PoePT-0.2.0.tar.gz` & `tmp/PoePT-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoePT-0.2.0.tar", last modified: Sat Jun  3 16:32:19 2023, max compression
+gzip compressed data, was "PoePT-0.2.1.tar", last modified: Sat Jun  3 16:48:17 2023, max compression
```

## Comparing `PoePT-0.2.0.tar` & `PoePT-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 16:32:19.335244 PoePT-0.2.0/
--rw-rw-rw-   0        0        0     4896 2023-06-03 16:32:19.334245 PoePT-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 16:32:19.327059 PoePT-0.2.0/PoePT.egg-info/
--rw-rw-rw-   0        0        0     4896 2023-06-03 16:32:18.000000 PoePT-0.2.0/PoePT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-03 16:32:19.000000 PoePT-0.2.0/PoePT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 16:32:18.000000 PoePT-0.2.0/PoePT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 16:32:18.000000 PoePT-0.2.0/PoePT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 16:32:18.000000 PoePT-0.2.0/PoePT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4240 2023-06-03 15:48:41.000000 PoePT-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 16:32:19.332078 PoePT-0.2.0/poept/
--rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.0/poept/__init__.py
--rw-rw-rw-   0        0        0     6235 2023-06-01 22:13:50.000000 PoePT-0.2.0/poept/poept.py
--rw-rw-rw-   0        0        0       42 2023-06-03 16:32:19.335244 PoePT-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-06-03 15:50:35.000000 PoePT-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.256677 PoePT-0.2.1/
+-rw-rw-rw-   0        0        0     4898 2023-06-03 16:48:17.256677 PoePT-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.252676 PoePT-0.2.1/PoePT.egg-info/
+-rw-rw-rw-   0        0        0     4898 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4240 2023-06-03 15:48:41.000000 PoePT-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.254677 PoePT-0.2.1/poept/
+-rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.1/poept/__init__.py
+-rw-rw-rw-   0        0        0     6234 2023-06-03 16:42:19.000000 PoePT-0.2.1/poept/poept.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 16:48:17.256677 PoePT-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      962 2023-06-03 16:43:40.000000 PoePT-0.2.1/setup.py
```

### Comparing `PoePT-0.2.0/PKG-INFO` & `PoePT-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PoePT
-Version: 0.2.0
-Summary: Python package for interacting with the Quora POE chatbot
+Version: 0.2.1
+Summary: Python package for interacting with the Quora`s POE chatbot
 Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0
 Author-email: mamaexus@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: PoePT Version: 0.2.0 Summary: Python package for
-interacting with the Quora POE chatbot Home-page: https://github.com/saikyo0/
+Metadata-Version: 2.1 Name: PoePT Version: 0.2.1 Summary: Python package for
+interacting with the Quora`s POE chatbot Home-page: https://github.com/saikyo0/
 PoePT Author: Saikyo0 Author-email: mamaexus@gmail.com Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
 Content-Type: text/markdown # PoePT PoePT is a Selenium Python package that
```

### Comparing `PoePT-0.2.0/PoePT.egg-info/PKG-INFO` & `PoePT-0.2.1/PoePT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PoePT
-Version: 0.2.0
-Summary: Python package for interacting with the Quora POE chatbot
+Version: 0.2.1
+Summary: Python package for interacting with the Quora`s POE chatbot
 Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0
 Author-email: mamaexus@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: PoePT Version: 0.2.0 Summary: Python package for
-interacting with the Quora POE chatbot Home-page: https://github.com/saikyo0/
+Metadata-Version: 2.1 Name: PoePT Version: 0.2.1 Summary: Python package for
+interacting with the Quora`s POE chatbot Home-page: https://github.com/saikyo0/
 PoePT Author: Saikyo0 Author-email: mamaexus@gmail.com Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
 Content-Type: text/markdown # PoePT PoePT is a Selenium Python package that
```

### Comparing `PoePT-0.2.0/README.md` & `PoePT-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PoePT-0.2.0/poept/poept.py` & `PoePT-0.2.1/poept/poept.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from webdriver_manager.chrome import ChromeDriverManager
 import speech_recognition as sr
 
 class PoePT:
     def __init__(self):
         chrome_options = Options()
         chrome_options.add_argument("--log-level=3")
-        #chrome_options.add_argument("--headless")
+        chrome_options.add_argument("--headless")
         chrome_options.add_argument("--disable-infobars")
         chrome_options.add_argument("--disable-extensions")
         chrome_options.add_argument("--disable-notifications")
         chrome_options.add_argument("--disable-popup-blocking")
         chrome_options.add_argument("--disable-logging")
         chrome_service = webdriver.chrome.service.Service(ChromeDriverManager().install())
         self.driver = webdriver.Chrome(service=chrome_service, options=chrome_options)
```

### Comparing `PoePT-0.2.0/setup.py` & `PoePT-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 with open('readme.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='PoePT',
-    version='0.2.0',
-    description='Python package for interacting with the Quora POE chatbot',
+    version='0.2.1',
+    description='Python package for interacting with the Quora`s POE chatbot',
     author='Saikyo0',
     author_email='mamaexus@gmail.com',
     url='https://github.com/saikyo0/PoePT',
     packages=['poept'],
     install_requires=[
         'selenium',
         'webdriver_manager',
```

