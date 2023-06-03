# Comparing `tmp/custom_numbers-1.1.1.tar.gz` & `tmp/custom_numbers-1.1.2.tar.gz`

## Comparing `custom_numbers-1.1.1.tar` & `custom_numbers-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.bumpversion.cfg
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/i2.sh
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/inst.sh
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/mm.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/pytest.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/requirements.txt
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/setup_environment.sh
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/t.sh
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/uninst.sh
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/__init__.py
--rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/custom_numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/py.typed
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_customnumber.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_customnumeralsystem.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_geariterator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/LICENSE
--rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.bumpversion.cfg
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/i2.sh
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/inst.sh
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/mm.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/pytest.ini
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/requirements.txt
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/setup_environment.sh
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/t.sh
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/uninst.sh
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/__init__.py
+-rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/custom_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/py.typed
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_customnumber.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_customnumeralsystem.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_geariterator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/LICENSE
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/PKG-INFO
```

### Comparing `custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/src/custom_numbers/custom_numbers.py` & `custom_numbers-1.1.2/src/custom_numbers/custom_numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://github.com/StrayFeral/custom_numbers
 """
 
 import re
 import math
 from typing import List, Generator
 
-__version__: str = "1.1.1"
+__version__: str = "1.1.2"
 __author__: str = r"Evgueni Antonov (Evgueni.Antonov@gmail.com)"
 
 
 
 class CustomNumeralSystem:
     r"""Definition of custom numeral systems with basic consistency validation.
```

### Comparing `custom_numbers-1.1.1/tests/test_customnumber.py` & `custom_numbers-1.1.2/tests/test_customnumber.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/tests/test_customnumeralsystem.py` & `custom_numbers-1.1.2/tests/test_customnumeralsystem.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/tests/test_geariterator.py` & `custom_numbers-1.1.2/tests/test_geariterator.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/.gitignore` & `custom_numbers-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/LICENSE` & `custom_numbers-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.1/README.md` & `custom_numbers-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# custom_numbers 1.1.1
+# custom_numbers 1.1.2
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -309,14 +309,7 @@
 
 ```
 combinations -> int
     Returns the number of possible combinations (iterations).
 ```
 
 > The class implements the Python context management protocol.
-
-### class GearIterator
-
-The GearIterator in a generator form.
-    
-I wrote this class as part of an exercise. Not sure if anyone would need it,
-but would leave it here.
```

### Comparing `custom_numbers-1.1.1/pyproject.toml` & `custom_numbers-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "custom_numbers"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
     { name = "Evgueni Antonov", email = "Evgueni.Antonov@gmail.com" },
 ]
 description = "Swiss-army knife for numbers of custom numeral systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `custom_numbers-1.1.1/PKG-INFO` & `custom_numbers-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_numbers
-Version: 1.1.1
+Version: 1.1.2
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
 
-# custom_numbers 1.1.1
+# custom_numbers 1.1.2
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -347,14 +347,7 @@
 
 ```
 combinations -> int
     Returns the number of possible combinations (iterations).
 ```
 
 > The class implements the Python context management protocol.
-
-### class GearIterator
-
-The GearIterator in a generator form.
-    
-I wrote this class as part of an exercise. Not sure if anyone would need it,
-but would leave it here.
```

