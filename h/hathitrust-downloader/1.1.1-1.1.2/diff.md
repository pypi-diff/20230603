# Comparing `tmp/hathitrust-downloader-1.1.1.tar.gz` & `tmp/hathitrust-downloader-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hathitrust-downloader-1.1.1.tar", last modified: Mon Sep 14 14:51:23 2020, max compression
+gzip compressed data, was "hathitrust-downloader-1.1.2.tar", last modified: Sat Jun  3 10:48:30 2023, max compression
```

## Comparing `hathitrust-downloader-1.1.1.tar` & `hathitrust-downloader-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 14:51:23.431249 hathitrust-downloader-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     4074 2020-09-14 14:51:23.431249 hathitrust-downloader-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2635 2020-09-14 14:51:12.000000 hathitrust-downloader-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 14:51:23.431249 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4074 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      351 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       73 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2020-09-14 14:51:23.000000 hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 14:51:23.431249 hathitrust-downloader-1.1.1/hathitrustdownloader/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-14 14:51:12.000000 hathitrust-downloader-1.1.1/hathitrustdownloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1550 2020-09-14 14:51:12.000000 hathitrust-downloader-1.1.1/hathitrustdownloader/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-14 14:51:23.431249 hathitrust-downloader-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1419 2020-09-14 14:51:12.000000 hathitrust-downloader-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:48:30.830389 hathitrust-downloader-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 10:48:21.000000 hathitrust-downloader-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-03 10:48:30.830389 hathitrust-downloader-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-03 10:48:21.000000 hathitrust-downloader-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:48:30.830389 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-03 10:48:30.000000 hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:48:30.830389 hathitrust-downloader-1.1.2/hathitrustdownloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:48:21.000000 hathitrust-downloader-1.1.2/hathitrustdownloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-03 10:48:21.000000 hathitrust-downloader-1.1.2/hathitrustdownloader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 10:48:30.830389 hathitrust-downloader-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-03 10:48:21.000000 hathitrust-downloader-1.1.2/setup.py
```

### Comparing `hathitrust-downloader-1.1.1/PKG-INFO` & `hathitrust-downloader-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: hathitrust-downloader
-Version: 1.1.1
+Version: 1.1.2
 Summary: Downloads multiple pages from Hathitrust from the CLI.
 Home-page: http://github.com/addono/hathitrust-downloader
 Author: Adriaan Knapen
 Author-email: hi@aknapen.nl
 License: MIT
 Description: # HathiTrust Downloader
-        [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square)](https://pypi.org/project/hathitrust-downloader/)
+        [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square&logo=pypi)][pypi]
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/hathitrust-downloader?logo=pypi&style=flat-square)][pypi]
+        [![GitHub version](https://img.shields.io/github/release/Addono/HathiTrust-downloader.svg?style=flat-square&logo=github)][github-releases]
+        [![GitHub download](https://img.shields.io/github/downloads/Addono/HathiTrust-downloader/total.svg?style=flat-square&logo=github)][github-releases]
+        [![GitHub stars](https://img.shields.io/github/stars/Addono/HathiTrust-downloader?style=flat-square)](https://github.com/Addono/HathiTrust-downloader/stargazers)
+        [![License](https://img.shields.io/github/license/Addono/HathiTrust-downloader.svg?style=flat-square)](LICENSE)
         
         ## Installing
         
         ### Python 3 (OS Agnostic)
         
         Check that you have Python 3 installed and available on your shell. The following command should return something like `Python 3.8.5`.
         
@@ -72,21 +77,24 @@
         
         ## Troubleshooting
         
         ### No Progess / Progress Bar is Stuck
         
         Make sure that you can access books on HathiTrust. Try to open a book in your browser to see if everything is working fine. HathiTrust can require you to connect from an American IP. In addition, they limit the amount of pages you can download to 15 every 5 minutes. When you hit that limit you will need to wait, the tool will automatically wait and resume when the timeout is finished.
         
+        [pypi]: https://pypi.org/project/hathitrust-downloader/
+        [github-releases]: https://github.com/Addono/HathiTrust-downloader/releases/latest
+        
 Keywords: hathitrust download downloader cli
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `hathitrust-downloader-1.1.1/README.md` & `hathitrust-downloader-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # HathiTrust Downloader
-[![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square)](https://pypi.org/project/hathitrust-downloader/)
+[![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square&logo=pypi)][pypi]
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/hathitrust-downloader?logo=pypi&style=flat-square)][pypi]
+[![GitHub version](https://img.shields.io/github/release/Addono/HathiTrust-downloader.svg?style=flat-square&logo=github)][github-releases]
+[![GitHub download](https://img.shields.io/github/downloads/Addono/HathiTrust-downloader/total.svg?style=flat-square&logo=github)][github-releases]
+[![GitHub stars](https://img.shields.io/github/stars/Addono/HathiTrust-downloader?style=flat-square)](https://github.com/Addono/HathiTrust-downloader/stargazers)
+[![License](https://img.shields.io/github/license/Addono/HathiTrust-downloader.svg?style=flat-square)](LICENSE)
 
 ## Installing
 
 ### Python 3 (OS Agnostic)
 
 Check that you have Python 3 installed and available on your shell. The following command should return something like `Python 3.8.5`.
 
@@ -63,7 +68,10 @@
 The ID of the file can be found as part of the URL when opening a book through your browser.
 
 ## Troubleshooting
 
 ### No Progess / Progress Bar is Stuck
 
 Make sure that you can access books on HathiTrust. Try to open a book in your browser to see if everything is working fine. HathiTrust can require you to connect from an American IP. In addition, they limit the amount of pages you can download to 15 every 5 minutes. When you hit that limit you will need to wait, the tool will automatically wait and resume when the timeout is finished.
+
+[pypi]: https://pypi.org/project/hathitrust-downloader/
+[github-releases]: https://github.com/Addono/HathiTrust-downloader/releases/latest
```

### Comparing `hathitrust-downloader-1.1.1/hathitrust_downloader.egg-info/PKG-INFO` & `hathitrust-downloader-1.1.2/hathitrust_downloader.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: hathitrust-downloader
-Version: 1.1.1
+Version: 1.1.2
 Summary: Downloads multiple pages from Hathitrust from the CLI.
 Home-page: http://github.com/addono/hathitrust-downloader
 Author: Adriaan Knapen
 Author-email: hi@aknapen.nl
 License: MIT
 Description: # HathiTrust Downloader
-        [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square)](https://pypi.org/project/hathitrust-downloader/)
+        [![PyPI](https://img.shields.io/pypi/v/hathitrust-downloader?style=flat-square&logo=pypi)][pypi]
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/hathitrust-downloader?logo=pypi&style=flat-square)][pypi]
+        [![GitHub version](https://img.shields.io/github/release/Addono/HathiTrust-downloader.svg?style=flat-square&logo=github)][github-releases]
+        [![GitHub download](https://img.shields.io/github/downloads/Addono/HathiTrust-downloader/total.svg?style=flat-square&logo=github)][github-releases]
+        [![GitHub stars](https://img.shields.io/github/stars/Addono/HathiTrust-downloader?style=flat-square)](https://github.com/Addono/HathiTrust-downloader/stargazers)
+        [![License](https://img.shields.io/github/license/Addono/HathiTrust-downloader.svg?style=flat-square)](LICENSE)
         
         ## Installing
         
         ### Python 3 (OS Agnostic)
         
         Check that you have Python 3 installed and available on your shell. The following command should return something like `Python 3.8.5`.
         
@@ -72,21 +77,24 @@
         
         ## Troubleshooting
         
         ### No Progess / Progress Bar is Stuck
         
         Make sure that you can access books on HathiTrust. Try to open a book in your browser to see if everything is working fine. HathiTrust can require you to connect from an American IP. In addition, they limit the amount of pages you can download to 15 every 5 minutes. When you hit that limit you will need to wait, the tool will automatically wait and resume when the timeout is finished.
         
+        [pypi]: https://pypi.org/project/hathitrust-downloader/
+        [github-releases]: https://github.com/Addono/HathiTrust-downloader/releases/latest
+        
 Keywords: hathitrust download downloader cli
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `hathitrust-downloader-1.1.1/hathitrustdownloader/cli.py` & `hathitrust-downloader-1.1.2/hathitrustdownloader/cli.py`

 * *Files identical despite different names*

### Comparing `hathitrust-downloader-1.1.1/setup.py` & `hathitrust-downloader-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
     ],
     keywords='hathitrust download downloader cli',
     packages=find_packages(),
     install_requires=[
-        'requests==2.24.0',
+        'requests==2.31.0',
         'tqdm==4.48.2',
     ],
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'hathitrust-downloader=hathitrustdownloader.cli:main',
         ],
```

