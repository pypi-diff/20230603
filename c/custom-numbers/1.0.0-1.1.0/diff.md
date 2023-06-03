# Comparing `tmp/custom_numbers-1.0.0.tar.gz` & `tmp/custom_numbers-1.1.0.tar.gz`

## Comparing `custom_numbers-1.0.0.tar` & `custom_numbers-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/.bumpversion.cfg
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/i2.sh
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/inst.sh
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/mm.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/pytest.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/requirements.txt
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/setup_environment.sh
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/t.sh
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/uninst.sh
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/src/custom_numbers/__init__.py
--rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/src/custom_numbers/custom_numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/src/custom_numbers/py.typed
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/tests/test_customnumber.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/tests/test_customnumeralsystem.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/tests/test_geariterator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/LICENSE
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10862 2020-02-02 00:00:00.000000 custom_numbers-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.bumpversion.cfg
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/i2.sh
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/inst.sh
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/mm.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/pytest.ini
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/requirements.txt
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/setup_environment.sh
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/t.sh
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/uninst.sh
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/__init__.py
+-rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/custom_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/py.typed
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_customnumber.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_customnumeralsystem.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_geariterator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/PKG-INFO
```

### Comparing `custom_numbers-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/src/custom_numbers/custom_numbers.py` & `custom_numbers-1.1.0/src/custom_numbers/custom_numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://github.com/StrayFeral/custom_numbers
 """
 
 import re
 import math
 from typing import List, Generator
 
-__version__: str = "1.0.0"
+__version__: str = "1.1.0"
 __author__: str = r"Evgueni Antonov (Evgueni.Antonov@gmail.com)"
 
 
 
 class CustomNumeralSystem:
     r"""Definition of custom numeral systems with basic consistency validation.
```

### Comparing `custom_numbers-1.0.0/tests/test_customnumber.py` & `custom_numbers-1.1.0/tests/test_customnumber.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/tests/test_customnumeralsystem.py` & `custom_numbers-1.1.0/tests/test_customnumeralsystem.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/tests/test_geariterator.py` & `custom_numbers-1.1.0/tests/test_geariterator.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/.gitignore` & `custom_numbers-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/LICENSE` & `custom_numbers-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.0.0/README.md` & `custom_numbers-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# custom_numbers 1.0.0
+# custom_numbers 1.1.0
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -42,16 +42,14 @@
 This package contains one module with few classes made to help you declare
 a custom numeral system, made of custom symbols with a custom base. As
 this may sound strange, in reality this is how it looks:
 
 > NOTE: Subsystems are not supported and I do not plan to implement this
 > feature.
 
-> NOTE: This module supports only positive numbers.
-
 > NOTE: This module supports only custom integer numbers. Custom
 > floating point numbers are not supported and will never be.
 
 ### QUICK RECAP ON EXISTING AND WELL-KNOWN NUMERAL SYSTEMS
 
 Let's start with something you already know - a binary number. These
 are made of only **zeroes and ones** and therefore the Base is 2.
```

### Comparing `custom_numbers-1.0.0/pyproject.toml` & `custom_numbers-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "custom_numbers"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name = "Evgueni Antonov", email = "Evgueni.Antonov@gmail.com" },
 ]
 description = "Swiss-army knife for numbers of custom numeral systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `custom_numbers-1.0.0/PKG-INFO` & `custom_numbers-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_numbers
-Version: 1.0.0
+Version: 1.1.0
 Summary: Swiss-army knife for numbers of custom numeral systems.
 Project-URL: Homepage, https://github.com/StrayFeral/custom_numbers
 Project-URL: Bug Tracker, https://github.com/StrayFeral/custom_numbers/issues
 Author-email: Evgueni Antonov <Evgueni.Antonov@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Evgueni Antonov
@@ -32,15 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# custom_numbers 1.0.0
+# custom_numbers 1.1.0
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -80,16 +80,14 @@
 This package contains one module with few classes made to help you declare
 a custom numeral system, made of custom symbols with a custom base. As
 this may sound strange, in reality this is how it looks:
 
 > NOTE: Subsystems are not supported and I do not plan to implement this
 > feature.
 
-> NOTE: This module supports only positive numbers.
-
 > NOTE: This module supports only custom integer numbers. Custom
 > floating point numbers are not supported and will never be.
 
 ### QUICK RECAP ON EXISTING AND WELL-KNOWN NUMERAL SYSTEMS
 
 Let's start with something you already know - a binary number. These
 are made of only **zeroes and ones** and therefore the Base is 2.
```

