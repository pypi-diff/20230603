# Comparing `tmp/facere_sensum-0.0.3.tar.gz` & `tmp/facere_sensum-0.0.4.tar.gz`

## Comparing `facere_sensum-0.0.3.tar` & `facere_sensum-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/log.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/requirements.txt
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.github/workflows/lints.yaml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/src/facere_sensum/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/src/facere_sensum/facere_sensum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/ref.csv
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/LICENSE
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/log.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/.github/workflows/lints.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/src/facere_sensum/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/src/facere_sensum/facere_sensum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/test/ref.csv
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/test/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 facere_sensum-0.0.4/PKG-INFO
```

### Comparing `facere_sensum-0.0.3/.github/workflows/lints.yaml` & `facere_sensum-0.0.4/.github/workflows/lints.yaml`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.3/src/facere_sensum/facere_sensum.py` & `facere_sensum-0.0.4/src/facere_sensum/facere_sensum.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 
 from argparse import ArgumentParser
 import datetime
 import numpy as np
 import pandas as pd
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 def score_manual(metric):
     '''
     Get metric score as a direct user input.
     'metric' is the metric text description.
     '''
     while True:
```

### Comparing `facere_sensum-0.0.3/test/test.py` & `facere_sensum-0.0.4/test/test.py`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.3/.gitignore` & `facere_sensum-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.3/LICENSE` & `facere_sensum-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.3/README.md` & `facere_sensum-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.3/pyproject.toml` & `facere_sensum-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "facere-sensum"
 dynamic = [
     "version",
     "dependencies"
@@ -26,9 +26,9 @@
 
 [project.scripts]
 facere-sensum = "facere_sensum.facere_sensum:main"
 
 [tool.hatch.version]
 path = "src/facere_sensum/facere_sensum.py"
 
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements.txt"]
```

### Comparing `facere_sensum-0.0.3/PKG-INFO` & `facere_sensum-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: facere-sensum
-Version: 0.0.3
+Version: 0.0.4
 Summary: facere-sensum: make sense of the turmoil
 Project-URL: Homepage, https://github.com/lunarserge/facere-sensum
 Project-URL: Bug Tracker, https://github.com/lunarserge/facere-sensum/issues
 Author: Serge Lunev
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pandas>=2.0.1
 Description-Content-Type: text/markdown
 
 # facere-sensum: make sense of the turmoil
 
 Too often in life we deal with many things and also often with more than we can realistically accomplish. `facere-sensum` helps its users to be in control by:
 * Having the user assign relative priorities for things in scope and define their corresponding success metrics.
 * Calculating a meaningful single score across all specified metrics that can be used as a pivot indicator of overall performance.
```

