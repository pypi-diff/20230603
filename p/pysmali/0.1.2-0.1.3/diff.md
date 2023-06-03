# Comparing `tmp/pysmali-0.1.2.tar.gz` & `tmp/pysmali-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmali-0.1.2.tar", last modified: Wed May 10 07:59:36 2023, max compression
+gzip compressed data, was "pysmali-0.1.3.tar", last modified: Sat Jun  3 19:31:15 2023, max compression
```

## Comparing `pysmali-0.1.2.tar` & `pysmali-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.529793 pysmali-0.1.2/
--rw-rw-rw-   0        0        0    35802 2023-03-15 06:06:42.000000 pysmali-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6104 2023-05-10 07:59:36.530793 pysmali-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5327 2023-05-10 07:42:34.000000 pysmali-0.1.2/README.md
--rw-rw-rw-   0        0        0      948 2023-05-10 07:42:34.000000 pysmali-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-10 07:59:35.750539 pysmali-0.1.2/pysmali.egg-info/
--rw-rw-rw-   0        0        0     6104 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:59:36.538794 pysmali-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.017443 pysmali-0.1.2/smali/
--rw-rw-rw-   0        0        0     1012 2023-03-18 09:43:56.000000 pysmali-0.1.2/smali/__init__.py
--rw-rw-rw-   0        0        0    20973 2023-05-10 07:03:11.000000 pysmali-0.1.2/smali/base.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.262279 pysmali-0.1.2/smali/bridge/
--rw-rw-rw-   0        0        0      909 2023-03-16 06:04:01.000000 pysmali-0.1.2/smali/bridge/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-05-10 06:59:41.000000 pysmali-0.1.2/smali/bridge/errors.py
--rw-rw-rw-   0        0        0    24171 2023-05-10 07:53:40.000000 pysmali-0.1.2/smali/bridge/executor.py
--rw-rw-rw-   0        0        0     3608 2023-05-10 06:58:48.000000 pysmali-0.1.2/smali/bridge/frame.py
--rw-rw-rw-   0        0        0    28077 2023-05-10 07:56:30.000000 pysmali-0.1.2/smali/bridge/lang.py
--rw-rw-rw-   0        0        0     1133 2023-03-22 12:37:08.000000 pysmali-0.1.2/smali/bridge/objects.py
--rw-rw-rw-   0        0        0    18379 2023-05-10 07:58:29.000000 pysmali-0.1.2/smali/bridge/vm.py
--rw-rw-rw-   0        0        0     8936 2023-03-16 06:04:01.000000 pysmali-0.1.2/smali/opcode.py
--rw-rw-rw-   0        0        0    34770 2023-05-10 07:04:22.000000 pysmali-0.1.2/smali/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.367277 pysmali-0.1.2/smali/shell/
--rw-rw-rw-   0        0        0     1356 2023-03-18 17:29:22.000000 pysmali-0.1.2/smali/shell/__init__.py
--rw-rw-rw-   0        0        0      854 2023-03-18 17:25:00.000000 pysmali-0.1.2/smali/shell/__main__.py
--rw-rw-rw-   0        0        0     2274 2023-05-10 06:59:52.000000 pysmali-0.1.2/smali/shell/cli.py
--rw-rw-rw-   0        0        0    10014 2023-05-10 06:57:18.000000 pysmali-0.1.2/smali/shell/model.py
--rw-rw-rw-   0        0        0    16049 2023-05-10 07:04:38.000000 pysmali-0.1.2/smali/visitor.py
--rw-rw-rw-   0        0        0    22486 2023-05-10 07:36:02.000000 pysmali-0.1.2/smali/writer.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.903026 pysmali-0.1.3/
+-rw-rw-rw-   0        0        0    35803 2023-06-03 19:18:10.000000 pysmali-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6068 2023-06-03 19:31:15.905026 pysmali-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5393 2023-06-03 19:28:49.000000 pysmali-0.1.3/README.md
+-rw-rw-rw-   0        0        0      856 2023-06-03 19:22:30.000000 pysmali-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.198167 pysmali-0.1.3/pysmali.egg-info/
+-rw-rw-rw-   0        0        0     6068 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 19:31:15.916027 pysmali-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.465331 pysmali-0.1.3/smali/
+-rw-rw-rw-   0        0        0     1012 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/__init__.py
+-rw-rw-rw-   0        0        0    21638 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/base.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.724027 pysmali-0.1.3/smali/bridge/
+-rw-rw-rw-   0        0        0      909 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/errors.py
+-rw-rw-rw-   0        0        0    24233 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/executor.py
+-rw-rw-rw-   0        0        0     3733 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/frame.py
+-rw-rw-rw-   0        0        0    28077 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/lang.py
+-rw-rw-rw-   0        0        0     1133 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/objects.py
+-rw-rw-rw-   0        0        0    18607 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/vm.py
+-rw-rw-rw-   0        0        0     8936 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/opcode.py
+-rw-rw-rw-   0        0        0    34778 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/reader.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.869033 pysmali-0.1.3/smali/shell/
+-rw-rw-rw-   0        0        0     1356 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/__main__.py
+-rw-rw-rw-   0        0        0     2274 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/cli.py
+-rw-rw-rw-   0        0        0    10014 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/model.py
+-rw-rw-rw-   0        0        0    16049 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/visitor.py
+-rw-rw-rw-   0        0        0    22486 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/writer.py
```

### Comparing `pysmali-0.1.2/LICENSE` & `pysmali-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pysmali-0.1.2/PKG-INFO` & `pysmali-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 Metadata-Version: 2.1
 Name: pysmali
-Version: 0.1.2
+Version: 0.1.3
 Summary: Smali Visitor-API and Smali emulator
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
 Project-URL: API-Docs, https://pysmali.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
-![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
-![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
-![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-[![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
+![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
+![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
+![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
+[![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
-
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
 
 ```bash
 $ cd ./pysmali && pip install .
 # Or with pip
 $ pip install pysmali
 ```
 
 ## Usage
 
-For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
+For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -57,15 +54,15 @@
 
 Some notes:
 
 * ``p0``: This register always stores the root-instance where defined fields and methods will be stored.
 * ``vars``: This command can be used to print all registers together with their values
 * `L<Root>;`: The name of the root-context class
 
-The API [documentation](https://pysmali.readthedocs.io/) provides some usage examples and usage hints.
+The API [documentation](https://matrixeditor.github.io/pysmali/) provides some usage examples and usage hints.
 
 ### Parsing Smali-Files
 
 The simplest way to parse code is to use a `SmaliReader` together with a visitor:
 
 ```python
 from smali import SmaliReader, ClassVisitor
@@ -135,15 +132,15 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.2` you can import Smali files and execute defined methods:
+As of version `0.1.3` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
 with open('example.smali', 'r', encoding='utf-8') as fp:
     source = fp.read()
```

### Comparing `pysmali-0.1.2/README.md` & `pysmali-0.1.3/pysmali.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,52 @@
+Metadata-Version: 2.1
+Name: pysmali
+Version: 0.1.3
+Summary: Smali Visitor-API and Smali emulator
+Author-email: MatrixEditor <not@supported.com>
+Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
+Project-URL: API-Docs, https://pysmali.readthedocs.io/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
-![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
-![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
-![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-[![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
+![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
+![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
+![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
+[![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
-
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
 
 ```bash
 $ cd ./pysmali && pip install .
 # Or with pip
 $ pip install pysmali
 ```
 
 ## Usage
 
-For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
+For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -39,15 +54,15 @@
 
 Some notes:
 
 * ``p0``: This register always stores the root-instance where defined fields and methods will be stored.
 * ``vars``: This command can be used to print all registers together with their values
 * `L<Root>;`: The name of the root-context class
 
-The API [documentation](https://pysmali.readthedocs.io/) provides some usage examples and usage hints.
+The API [documentation](https://matrixeditor.github.io/pysmali/) provides some usage examples and usage hints.
 
 ### Parsing Smali-Files
 
 The simplest way to parse code is to use a `SmaliReader` together with a visitor:
 
 ```python
 from smali import SmaliReader, ClassVisitor
@@ -117,15 +132,15 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.2` you can import Smali files and execute defined methods:
+As of version `0.1.3` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
 with open('example.smali', 'r', encoding='utf-8') as fp:
     source = fp.read()
```

### Comparing `pysmali-0.1.2/pyproject.toml` & `pysmali-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [project]
 name = "pysmali"
-version = "0.1.2"
+version = "0.1.3"
 description="Smali Visitor-API and Smali emulator"
 authors = [
   { name="MatrixEditor", email="not@supported.com" },
 ]
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 [project.scripts]
 ismali = "smali.shell:start_cli"
```

### Comparing `pysmali-0.1.2/pysmali.egg-info/PKG-INFO` & `pysmali-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,36 @@
-Metadata-Version: 2.1
-Name: pysmali
-Version: 0.1.2
-Summary: Smali Visitor-API and Smali emulator
-Author-email: MatrixEditor <not@supported.com>
-Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
-Project-URL: API-Docs, https://pysmali.readthedocs.io/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
-![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
-![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
-![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-[![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
+![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
+![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
+![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
+[![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
-
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
 
 ```bash
 $ cd ./pysmali && pip install .
 # Or with pip
 $ pip install pysmali
 ```
 
 ## Usage
 
-For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
+For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -57,15 +38,15 @@
 
 Some notes:
 
 * ``p0``: This register always stores the root-instance where defined fields and methods will be stored.
 * ``vars``: This command can be used to print all registers together with their values
 * `L<Root>;`: The name of the root-context class
 
-The API [documentation](https://pysmali.readthedocs.io/) provides some usage examples and usage hints.
+The API [documentation](https://matrixeditor.github.io/pysmali/) provides some usage examples and usage hints.
 
 ### Parsing Smali-Files
 
 The simplest way to parse code is to use a `SmaliReader` together with a visitor:
 
 ```python
 from smali import SmaliReader, ClassVisitor
@@ -135,15 +116,15 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.2` you can import Smali files and execute defined methods:
+As of version `0.1.3` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
 with open('example.smali', 'r', encoding='utf-8') as fp:
     source = fp.read()
```

### Comparing `pysmali-0.1.2/pysmali.egg-info/SOURCES.txt` & `pysmali-0.1.3/pysmali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/__init__.py` & `pysmali-0.1.3/smali/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/base.py` & `pysmali-0.1.3/smali/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     >>> flags = AccessType.PUBLIC + AccessType.FINAL
     >>> flags in AccessType.PUBLIC
     True
     >>> flags in AccessType.PRIVATE
     False
     """
 
+    # !! IMPORTANT: Although, all access types from here (https://source.android.com/docs/core/runtime/dex-format#access-flags)
+    # are covered, their values differ as there are multiple access flags with the same value.
+    # REVISIT: Maybe convert this class into a dictionary
     PUBLIC = 0x1
     PRIVATE = 0x2
     PROTECTED = 0x4
     STATIC = 0x8
     FINAL = 0x10
     SYNCHRONIZED = 0x20
     VOLATILE = 0x40
@@ -331,15 +334,15 @@
     CLINIT = "<clinit>"
     """Static block initializer"""
 
     INIT = "<init>"
     """Constructor method"""
 
     def __init__(self, signature: str) -> None:
-        self.__signature = signature
+        self.__signature = signature.strip()
         if isinstance(signature, type):
             self.__signature = f"{signature.__module__}.{signature.__name__}"
 
     @property
     def descriptor(self) -> str:
         """Returns the type descriptor of this type.
 
@@ -360,14 +363,23 @@
 
         name = f"{name.replace('.', '/')}"
         if name[-1] != ";" and name not in "ZCBSIFVJD":
             name = f"L{name};"
         return name
 
     @property
+    def dim(self) -> int:
+        """Returns the amount of array dimensions.
+
+        :return: the amount of array dimensions.
+        :rtype: int
+        """
+        return self.__signature.count("[")
+
+    @property
     def type_name(self) -> str:
         """Returns the type name without 'L' and ';'
 
         :return: the type name
         :rtype: str
         """
         if not SmaliValueProxy.RE_TYPE_VALUE.match(self.__signature):
@@ -392,60 +404,60 @@
         """
         idx = self.__signature.find("(")
         if idx == -1:
             raise TypeError(
                 f"Invalid method signature: could not find name ({self.__signature})"
             )
 
-        # Handle bracket names if not <clinit> or <init>
+
         name = self.__signature[:idx]
+        if "->" in name:
+            name = name[name.find("->") + 2:]
+        # Handle bracket names if not <clinit> or <init>
         if name in (Type.INIT, Type.CLINIT):
             return name
+
         return name.rstrip(">").lstrip("<")
 
     def get_method_params(self) -> list:
         """Returns the method parameter internal names.
 
         :return: the method parameters
         :rtype: list
         """
         start = self.__signature.find("(")
-        end = self.__signature.find(")")
+        end = self.__signature.find(")") + 1
         if start == -1 or end == -1:
             raise TypeError("Invalid method signature")
 
         params = self.__signature[start + 1 : end]
         if not params:
             return []
 
         param_list = []
-        idx = 0
-        is_type = False
-        current = ""
-        while idx < len(params):
-            if params[idx] == "L":
-                is_type = True
-            elif params[idx] == ";":
-                is_type = False
-                current += ";"
-                param_list.append(current)
-                current = ""
-                idx += 1
+        current_param = ""
+        is_type_def = False
+        for char in params:
+            current_param = f"{current_param}{char}"
+
+            if char == "L":
+                is_type_def = True
                 continue
-            elif params[idx] == "[":
-                current += "["
-                idx += 1
+
+            if char == "[" or is_type_def:
                 continue
 
-            if is_type:
-                current += params[idx]
-            else:
-                param_list.append(params[idx])
-            idx += 1
+            if char == ";":
+                is_type_def = False
+
+            param_list.append(current_param)
+            current_param = ""
 
+        if current_param:
+            param_list.append(current_param)
         return param_list
 
     def get_method_return_type(self) -> str:
         """Retrieves the method's return type
 
         :raises TypeError: if there is no valid return type
         :return: the return type's descriptor
@@ -455,14 +467,16 @@
         if end == -1:
             raise TypeError("Invalid method signature")
         return self.__signature[end + 1 :]
 
     def __str__(self) -> str:
         return self.__signature
 
+    def __repr__(self) -> str:
+        return f"<Type sig='{self.__signature}'>"
 
 def smali_value(value: str) -> "SmaliValueProxy":
     """Parses the given string and returns its Smali value representation.
 
     :param value: the value as a string
     :type value: str
     :raises ValueError: if it has no valid Smali type
@@ -516,27 +530,27 @@
 
     >>> string = SmaliValue('"Hello World"')
     'Hello World'
     >>> len(string)
     11
     """
 
-    RE_INT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+")
+    RE_INT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+$")
     """Pattern for ``int`` values."""
 
     RE_BYTE_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+t$")
     """Pattern for ``byte`` values."""
 
     RE_SHORT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+s$")
     """Pattern for ``short`` values."""
 
-    RE_FLOAT_VALUE = re.compile(r"[\-\+]?(0x)?\d+\.\d+f$")
+    RE_FLOAT_VALUE = re.compile(r"[\-\+]?\d+\.\d+f$")
     """Pattern for ``float`` values."""
 
-    RE_DOUBLE_VALUE = re.compile(r"[\-\+]?(0x)?\d+\.\d+")
+    RE_DOUBLE_VALUE = re.compile(r"[\-\+]?\d+\.\d+")
     """Pattern for ``double`` values."""
 
     RE_LONG_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+l$")
     """Pattern for ``long`` values."""
 
     RE_CHAR_VALUE = re.compile(r"^'.*'$")
     """Pattern for ``char`` values."""
@@ -550,21 +564,21 @@
     RE_BOOL_VALUE = re.compile(r"true|false")
     """Pattern for ``boolean`` values."""
 
     RE_HEX_VALUE = re.compile(r"0x[\dabcdefABCDEF]+")
     """Pattern for integer values."""
 
     TYPE_MAP: list = [
-        (RE_SHORT_VALUE, int),
-        (RE_LONG_VALUE, int),
-        (RE_BYTE_VALUE, int),
+        (RE_SHORT_VALUE, lambda x, **kw: int(x[:-1], **kw)),
+        (RE_LONG_VALUE, lambda x, **kw: int(x[:-1], **kw)),
+        (RE_BYTE_VALUE, lambda x, **kw: int(x[:-1], **kw)),
         (RE_INT_VALUE, int),
-        (RE_BOOL_VALUE, lambda x: x == "true"),
-        (RE_FLOAT_VALUE, float),
-        (RE_DOUBLE_VALUE, float),
+        (RE_BOOL_VALUE, lambda x: str(x).lower() == "true"),
+        (RE_FLOAT_VALUE, lambda x: float(x[:-1])),
+        (RE_DOUBLE_VALUE, lambda x: float(x[:-1])),
         (RE_CHAR_VALUE, lambda x: str(x[1:-1])),
         (RE_STRING_VALUE, lambda x: str(x[1:-1])),
         (RE_TYPE_VALUE, Type),
     ]
     """Defines custom handlers for actual value defintions
 
     :meta private:
```

### Comparing `pysmali-0.1.2/smali/bridge/__init__.py` & `pysmali-0.1.3/smali/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/bridge/errors.py` & `pysmali-0.1.3/smali/bridge/errors.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/bridge/executor.py` & `pysmali-0.1.3/smali/bridge/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import struct
 
 from smali import SmaliValue, Type
-from smali.opcode import * # noqa
+from smali.opcode import *  # noqa
 from smali.bridge.frame import Frame
 from smali.bridge.errors import ExecutionError
 from smali.bridge.lang import SmaliObject
 from smali.bridge.objects import Object, Class
 
 cache = {}
 """Sepcial dict tat stores all opcodes with their executors"""
@@ -155,15 +155,17 @@
             # Remove the first argument
             values = values[1:]
 
         if not vm_class:
             vm_class = self.frame.vm.get_class(owner)
 
         target = vm_class.method(method)
-        self.frame.method_return = self.frame.vm.call(target, instance, *values)
+        self.frame.method_return = self.frame.vm.call(
+            target, instance, *values, vm__frame=self.frame
+        )
 
 
 @opcode_executor()
 def throw(self: Executor, register: str):
     self.frame.error = ExecutionError("RuntimeError", self.frame[register])
 
 
@@ -367,20 +369,20 @@
         instance.init()
 
         self.frame[register] = instance
 
 
 @opcode_executor()
 def new_array(self: Executor, dest: str, count_register: str, descriptor: str):
-    cls = Type(descriptor).class_name
+    cls_name = Type(descriptor).class_name
     values = [None] * self.frame[count_register]
-    if cls in "BSIJ":  # number
+    if cls_name in "BSIJ":  # number
         values = [0] * self.frame[count_register]
 
-    elif cls in "FD":  # floating point
+    elif cls_name in "FD":  # floating point
         values = [0.0] * self.frame[count_register]
 
     self.frame[dest] = values
 
 
 @opcode_executor(map_to=[INSTANCE_OF])
 def check_cast(self: Executor, dest: str, descriptor: str):
```

### Comparing `pysmali-0.1.2/smali/bridge/frame.py` & `pysmali-0.1.3/smali/bridge/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
     vm = None
     """VM reference"""
 
     switch_data: dict
     """Stores packed and sparse-switch data"""
 
+    parent: "Frame" = None
+    """Parent execution context (mainly used for backtracking)"""
+
     def __init__(self):
         self.registers = {}
         self.opcodes = []
         self.labels = {}
         self.catch = {}
         self.array_data = {}
         self.switch_data = {}
@@ -95,14 +98,15 @@
     def reset(self) -> None:
         """Resets this frame and removes execution information."""
         self.label = None
         self.error = None
         self.finished = False
         self.pos = 0
         self.return_value = None
+        self.parent = None
         self.registers.clear()
 
     def __getitem__(self, key: str):
         if key not in self.registers:
             raise NoSuchRegisterError(f"Register with name {key} not found!")
 
         return self.registers[key]
```

### Comparing `pysmali-0.1.2/smali/bridge/lang.py` & `pysmali-0.1.3/smali/bridge/lang.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/bridge/objects.py` & `pysmali-0.1.3/smali/bridge/objects.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/bridge/vm.py` & `pysmali-0.1.3/smali/bridge/vm.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         bool: ("Z", "Ljava/lang/Boolean;"),
     }
 
     def __init__(
         self,
         class_loader: ClassLoader = None,
         executors: dict = executor.cache,
-        use_strict: bool = False
+        use_strict: bool = False,
     ) -> None:
         self.classloader = _SmaliClassLoader(self) or class_loader
         self.executors = executors or {}
         self.use_strict = use_strict
 
     def new_class(self, cls: SmaliClass):
         """Defines a new class that can be accessed globally.
@@ -227,14 +227,18 @@
             if not instance:
                 raise ExecutionError(
                     "NullPtrError",
                     f"Expected instance of '{instance.smali_class.name}'",
                 )
             frame.registers["p0"] = instance
 
+        prev_frame = kwargs.pop("vm__frame", None)
+        if prev_frame:
+            frame.parent = prev_frame
+
         # validate method and set parameter values
         self._validate_call(method, frame, args, kwargs)
         while not frame.finished:
             opcode_exec, args = frame.opcodes[frame.pos]
             opcode_exec.args = args
             if self.debug_handler:
                 self.debug_handler.precall(self, method, opcode_exec)
@@ -314,28 +318,28 @@
         return super().visit_enum(name, owner, const, value_type)
 
     def visit_subannotation(
         self, name: str, access_flags: int, signature: str
     ) -> "AnnotationVisitor":
         sub = SmaliAnnotation(self.annotation, signature, access_flags)
         self.annotation[name] = sub
-        return _SourceAnnotationVisitor(sub)
+        return SmaliVMAnnotationReader(sub)
 
 
 class _SourceFieldVisitor(FieldVisitor):
     field: SmaliField
 
     def __init__(self, field: SmaliField) -> None:
         super().__init__()
         self.field = field
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         annotation = SmaliAnnotation(self.field, signature, access_flags)
         self.field.annotations.append(annotation)
-        return _SourceAnnotationVisitor(annotation)
+        return SmaliVMAnnotationReader(annotation)
 
 
 class _SourceMethodVisitor(MethodVisitor):
     method: SmaliMethod
     frame: Frame
 
     def __init__(self, method: SmaliMethod) -> None:
@@ -344,15 +348,15 @@
         self.frame = Frame()
         self.pos = 0
         self._last_label = None
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         annotation = SmaliAnnotation(self.method, signature, access_flags)
         self.method.annotations.append(annotation)
-        return _SourceAnnotationVisitor(annotation)
+        return SmaliVMAnnotationReader(annotation)
 
     def visit_block(self, name: str) -> None:
         self.frame.labels[name] = self.pos
         self.pos += 1
         self._last_label = name
 
     def visit_locals(self, local_count: int) -> None:
@@ -384,23 +388,26 @@
             self.visit_instruction(f"return-{ret_type}", args)
         else:
             self.visit_instruction("return", args)
 
     def visit_instruction(self, ins_name: str, args: list) -> None:
         cache: dict = self.frame.vm.executors
         for _, value in opcode.__dict__.items():
-             # If the value of an attribute is equal to the given instruction
-             # name,
+            # If the value of an attribute is equal to the given instruction
+            # name,
             if value == ins_name:
                 # Check if the instruction name is not in the list of executors
                 # in the current frame's virtual machine
                 if ins_name not in cache and not self.frame.vm.use_strict:
-                    # If not, add a tuple of the "nop" opcode function and the
-                    # instruction arguments to the frame's opcodes list.
-                    func = cache["nop"] if "nop" in cache else executor.nop
+                    if "*" in cache:
+                        func = cache["*"]
+                    else:
+                        # If not, add a tuple of the "nop" opcode function and the
+                        # instruction arguments to the frame's opcodes list.
+                        func = cache["nop"] if "nop" in cache else executor.nop
                     self.frame.opcodes.append((func, args))
                 else:
                     # If yes, add a tuple of the executor function for the instruction
                     # name and the instruction arguments to the frame's opcodes list.
                     self.frame.opcodes.append((self.frame.vm.executors[ins_name], args))
                 self.pos += 1
                 return
@@ -425,44 +432,44 @@
         super().__init__()
         self.vm = vm
         self.smali_class = smali_class
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         annotation = SmaliAnnotation(self.smali_class, signature, access_flags)
         self.smali_class.annotations.append(annotation)
-        return _SourceAnnotationVisitor(annotation)
+        return SmaliVMAnnotationReader(annotation)
 
     def visit_class(self, name: str, access_flags: int) -> None:
         self.smali_class = SmaliClass(None, name, access_flags)
 
     def visit_inner_class(self, name: str, access_flags: int) -> "ClassVisitor":
         inner = SmaliClass(self.smali_class, name, access_flags)
         self.smali_class[name] = inner
-        return _SourceClassVisitor(self.vm, inner)
+        return SmaliVMClassReader(self.vm, inner)
 
     def visit_field(
         self, name: str, access_flags: int, field_type: str, value=None
     ) -> FieldVisitor:
         field = SmaliField(
             self.smali_class,
             f"{name}:{field_type}",
             access_flags,
             name,
             Type(field_type),
             value=SmaliValue(value) if value else None,
         )
         self.smali_class[name] = field
-        return _SourceFieldVisitor(field)
+        return SmaliVMFieldReader(field)
 
     def visit_method(
         self, name: str, access_flags: int, parameters: list, return_type: str
     ) -> MethodVisitor:
         signature = f"{name}({''.join(parameters)}){return_type}"
         method = SmaliMethod(self.vm, self.smali_class, signature, access_flags)
-        visitor = _SourceMethodVisitor(method)
+        visitor = SmaliVMMethodReader(method)
         self.vm.new_frame(method, visitor.frame)
         self.smali_class[name] = method
         return visitor
 
     def visit_implements(self, interface: str) -> None:
         self.smali_class.interfaces.append(interface)
 
@@ -476,15 +483,15 @@
 
     def __init__(self, vm: SmaliVM) -> None:
         self.vm = vm
 
     def define_class(self, source: bytes) -> SmaliClass:
         reader = SmaliReader(validate=True, comments=False)
 
-        visitor = _SourceClassVisitor(self.vm)
+        visitor = SmaliVMClassReader(self.vm)
         reader.visit(source, visitor)
         smali_class = visitor.smali_class
         if not smali_class:
             raise ValueError("Could not parse class!")
 
         self.vm.new_class(smali_class)
         return smali_class
```

### Comparing `pysmali-0.1.2/smali/opcode.py` & `pysmali-0.1.3/smali/opcode.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/reader.py` & `pysmali-0.1.3/smali/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,16 +877,16 @@
         # number -> use SmaliValue(...) instead
         length = self.line.peek()
         values = []
 
         if do_copy:
             self._copy_line()
         self._publish_comment()
-        self._next_line()
         while True:
+            self._next_line()
             value = self.line.peek()
             self._publish_comment()
             if do_copy:
                 self._copy_line()
             if value[0] == "." and value[1:] == Token.END.value:
                 break
             values.append(value)
@@ -925,16 +925,16 @@
         # one line in the SourceCode
         next(self.line)
 
         values = {}
         if do_copy:
             self._copy_line()
         self._publish_comment()
-        self._next_line()
         while True:
+            self._next_line()
             key = self.line.peek()
             self._publish_comment()
             if do_copy:
                 self._copy_line()
             if key[0] == "." and key[1:] == Token.END.value:
                 break
             # Add the block id without leading ':'
```

### Comparing `pysmali-0.1.2/smali/shell/__init__.py` & `pysmali-0.1.3/smali/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/shell/__main__.py` & `pysmali-0.1.3/smali/shell/__main__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/shell/cli.py` & `pysmali-0.1.3/smali/shell/cli.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/shell/model.py` & `pysmali-0.1.3/smali/shell/model.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/visitor.py` & `pysmali-0.1.3/smali/visitor.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.2/smali/writer.py` & `pysmali-0.1.3/smali/writer.py`

 * *Files identical despite different names*

