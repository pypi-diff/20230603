# Comparing `tmp/betweens-0.3.0.tar.gz` & `tmp/betweens-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.3.0.tar", last modified: Mon May  8 10:57:31 2023, max compression
+gzip compressed data, was "betweens-1.1.1.tar", last modified: Sat Jun  3 03:33:00 2023, max compression
```

## Comparing `betweens-0.3.0.tar` & `betweens-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.081975 betweens-0.3.0/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-05-08 10:57:31.081975 betweens-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-08 10:56:31.000000 betweens-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.066354 betweens-0.3.0/betweens/
--rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-0.3.0/betweens/__init__.py
--rw-rw-rw-   0        0        0     3905 2023-05-08 10:52:21.000000 betweens-0.3.0/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.3.0/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.081975 betweens-0.3.0/betweens.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      455 2023-05-08 10:53:43.000000 betweens-0.3.0/new.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 10:57:31.081975 betweens-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-05-08 10:52:35.000000 betweens-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:33:00.661989 betweens-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1777 2023-06-03 03:33:00.661989 betweens-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-08 10:56:31.000000 betweens-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 03:33:00.646352 betweens-1.1.1/betweens/
+-rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-1.1.1/betweens/__init__.py
+-rw-rw-rw-   0        0        0     3905 2023-05-08 10:52:21.000000 betweens-1.1.1/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-1.1.1/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:33:00.661989 betweens-1.1.1/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1777 2023-06-03 03:33:00.000000 betweens-1.1.1/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-03 03:33:00.000000 betweens-1.1.1/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:33:00.000000 betweens-1.1.1/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 03:33:00.000000 betweens-1.1.1/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      543 2023-06-03 03:26:43.000000 betweens-1.1.1/new.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:33:00.661989 betweens-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2023-06-03 03:31:57.000000 betweens-1.1.1/setup.py
```

### Comparing `betweens-0.3.0/LICENSE` & `betweens-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.3.0/PKG-INFO` & `betweens-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.3.0
+Version: 1.1.1
+Summary: 0.0.1:
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Common Public License
+Classifier: License :: OSI Approved :: W3C License
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Environment :: Console :: Curses
+Classifier: Environment :: X11 Applications
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Betweens
 
 This is a package named betweens.
 There are 3 between mode.
```

### Comparing `betweens-0.3.0/betweens/betweens.py` & `betweens-1.1.1/betweens/betweens.py`

 * *Files identical despite different names*

### Comparing `betweens-0.3.0/betweens.egg-info/PKG-INFO` & `betweens-1.1.1/betweens.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.3.0
+Version: 1.1.1
+Summary: 0.0.1:
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Common Public License
+Classifier: License :: OSI Approved :: W3C License
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Environment :: Console :: Curses
+Classifier: Environment :: X11 Applications
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Betweens
 
 This is a package named betweens.
 There are 3 between mode.
```

### Comparing `betweens-0.3.0/setup.py` & `betweens-1.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,33 +2,46 @@
 # import betweens.python_ver_check
 # 
 # betweens.python_ver_check.check()
 # 以上为失败的操作
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 long_description = None
+description = None
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
+with open(path.join(this_directory, 'new.txt'), encoding='utf-8') as f:
+    description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='0.3.0', # 版本
+      version='1.1.1', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
+          'License :: OSI Approved :: Common Public License',
+          'License :: OSI Approved :: W3C License',
+          'License :: OSI Approved :: Academic Free License (AFL)',
+          'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
+          'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
           'Operating System :: MacOS :: MacOS X',
+          'Operating System :: Microsoft :: Windows :: Windows 8.1',
           'Operating System :: Microsoft :: Windows :: Windows 10',
           'Operating System :: Microsoft :: Windows :: Windows 11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11'
+          'Programming Language :: Python :: 3.11',
+          'Environment :: Console',
+          'Environment :: Console :: Curses',
+          'Environment :: X11 Applications'
       ],
+      description = description,
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='yuanbaoge', # 作者
       author_email='yuanbaoge@outlook.com', # 作者邮箱
       keywords='pimm source manager')
```

