# Comparing `tmp/custom_numbers-1.1.0.tar.gz` & `tmp/custom_numbers-1.1.1.tar.gz`

## Comparing `custom_numbers-1.1.0.tar` & `custom_numbers-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.bumpversion.cfg
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/i2.sh
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/inst.sh
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/mm.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/pytest.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/requirements.txt
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/setup_environment.sh
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/t.sh
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/uninst.sh
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/__init__.py
--rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/custom_numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/src/custom_numbers/py.typed
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_customnumber.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_customnumeralsystem.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/tests/test_geariterator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/LICENSE
--rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 custom_numbers-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.bumpversion.cfg
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/i2.sh
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/inst.sh
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/mm.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/pytest.ini
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/requirements.txt
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/setup_environment.sh
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/t.sh
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/uninst.sh
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/__init__.py
+-rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/custom_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/src/custom_numbers/py.typed
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_customnumber.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_customnumeralsystem.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/tests/test_geariterator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/LICENSE
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 custom_numbers-1.1.1/PKG-INFO
```

### Comparing `custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `custom_numbers-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/src/custom_numbers/custom_numbers.py` & `custom_numbers-1.1.1/src/custom_numbers/custom_numbers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://github.com/StrayFeral/custom_numbers
 """
 
 import re
 import math
 from typing import List, Generator
 
-__version__: str = "1.1.0"
+__version__: str = "1.1.1"
 __author__: str = r"Evgueni Antonov (Evgueni.Antonov@gmail.com)"
 
 
 
 class CustomNumeralSystem:
     r"""Definition of custom numeral systems with basic consistency validation.
```

### Comparing `custom_numbers-1.1.0/tests/test_customnumber.py` & `custom_numbers-1.1.1/tests/test_customnumber.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/tests/test_customnumeralsystem.py` & `custom_numbers-1.1.1/tests/test_customnumeralsystem.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/tests/test_geariterator.py` & `custom_numbers-1.1.1/tests/test_geariterator.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/.gitignore` & `custom_numbers-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/LICENSE` & `custom_numbers-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.0/README.md` & `custom_numbers-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# custom_numbers 1.1.0
+# custom_numbers 1.1.1
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
```

### Comparing `custom_numbers-1.1.0/pyproject.toml` & `custom_numbers-1.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "custom_numbers"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "Evgueni Antonov", email = "Evgueni.Antonov@gmail.com" },
 ]
 description = "Swiss-army knife for numbers of custom numeral systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 license = { file = "LICENSE" }
 keywords = ["number", "numbers", "numeral", "counter", "mathematics", "math"]
```

### Comparing `custom_numbers-1.1.0/PKG-INFO` & `custom_numbers-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_numbers
-Version: 1.1.0
+Version: 1.1.1
 Summary: Swiss-army knife for numbers of custom numeral systems.
 Project-URL: Homepage, https://github.com/StrayFeral/custom_numbers
 Project-URL: Bug Tracker, https://github.com/StrayFeral/custom_numbers/issues
 Author-email: Evgueni Antonov <Evgueni.Antonov@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Evgueni Antonov
@@ -24,23 +24,23 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Keywords: counter,math,mathematics,number,numbers,numeral
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# custom_numbers 1.1.0
+# custom_numbers 1.1.1
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
```

