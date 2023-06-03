# Comparing `tmp/nuudel_best_time_finder-0.1.0.tar.gz` & `tmp/nuudel_best_time_finder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuudel_best_time_finder-0.1.0.tar", max compression
+gzip compressed data, was "nuudel_best_time_finder-0.2.0.tar", max compression
```

## Comparing `nuudel_best_time_finder-0.1.0.tar` & `nuudel_best_time_finder-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-05-09 13:39:14.429705 nuudel_best_time_finder-0.1.0/LICENSE
--rw-r--r--   0        0        0     1551 2023-05-09 13:41:43.062125 nuudel_best_time_finder-0.1.0/README.md
--rw-r--r--   0        0        0     1183 2023-05-09 13:40:58.194039 nuudel_best_time_finder-0.1.0/nuudel_best_time_finder/__init__.py
--rw-r--r--   0        0        0      418 2023-05-09 13:39:14.437705 nuudel_best_time_finder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 nuudel_best_time_finder-0.1.0/setup.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 nuudel_best_time_finder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 13:39:14.429705 nuudel_best_time_finder-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1706 2023-05-31 11:48:53.619413 nuudel_best_time_finder-0.2.0/README.md
+-rw-r--r--   0        0        0     1768 2023-06-03 13:40:40.979413 nuudel_best_time_finder-0.2.0/nuudel_best_time_finder/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-03 13:45:25.276890 nuudel_best_time_finder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 nuudel_best_time_finder-0.2.0/PKG-INFO
```

### Comparing `nuudel_best_time_finder-0.1.0/LICENSE` & `nuudel_best_time_finder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuudel_best_time_finder-0.1.0/README.md` & `nuudel_best_time_finder-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,20 +27,27 @@
 pip install nuudel-best-time-finder
 
 ```
 
 ## How to use
 
 Say we have a nuudel poll at: <https://nuudel.digitalcourage.de/nuudel-poll-id> and want
-to find two dates that cover the most amount of people simply run:
+to find two dates that cover the most amount of people simply run the following in your
+console:
+
+```console
+nuudel-find-best-times {nuudel-poll-id} 2 --results-file results.csv
+```
+
+or alternatively as part of a script:
 
 ```python
 from nuudel_best_time_finder import find_best_times
 
-find_best_times(poll = "{nuudel-poll-id}", n =2, results_file = "results.csv")
+find_best_times(poll = "{nuudel-poll-id}", n = 2, results_file = "results.csv")
 ```
 
 The results are then written to a file called `results.csv` with three columns:
 
 * Time combinations
 * Number of people covered by the combination
 * Percent coverage out of all participants
```

### Comparing `nuudel_best_time_finder-0.1.0/setup.py` & `nuudel_best_time_finder-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nuudel-best-time-finder
+Version: 0.2.0
+Summary: 
+License: MIT
+Author: Philip Hackstock
+Author-email: p.hackstock@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
+
+# Nuudel best time finder
+
+In a poll like this:
+
+|         | 2023-06-05 | 2023-06-07 | 2023-06-08 | 2023-06-12 | ... |
+|---------|------------|------------|------------|------------|-----|
+| Alice   | Yes        | No         | No         | Yes        | ... |
+| Bob     | No         | No         | No         | Yes        | ... |
+| Carl    | Yes        | Yes        | No         | No         | ... |
+| Dave    | Yes        | No         | No         | Yes        | ... |
+| Eve     | No         | No         | No         | Yes        | ... |
+| Francis | No         | No         | No         | No         | ... |
+| ...     | ...        | ...        | ...        | ...        | ... |
+
+a common task is to find the set of two or more days that cover as many people as
+possible.
+
+This tool works with the poll service nuudel (<https://nuudel.digitalcourage.de/>),
+reads the data directly from a given poll and finds the best combinations for any number
+of times.
+
+## Install
+
+Install using pip:
+
+```console
+pip install nuudel-best-time-finder
+
+```
+
+## How to use
+
+Say we have a nuudel poll at: <https://nuudel.digitalcourage.de/nuudel-poll-id> and want
+to find two dates that cover the most amount of people simply run the following in your
+console:
+
+```console
+nuudel-find-best-times {nuudel-poll-id} 2 --results-file results.csv
+```
+
+or alternatively as part of a script:
+
+```python
+from nuudel_best_time_finder import find_best_times
+
+find_best_times(poll = "{nuudel-poll-id}", n = 2, results_file = "results.csv")
+```
+
+The results are then written to a file called `results.csv` with three columns:
+
+* Time combinations
+* Number of people covered by the combination
+* Percent coverage out of all participants
 
-packages = \
-['nuudel_best_time_finder']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pandas>=2.0.1,<3.0.0', 'requests>=2.30.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nuudel-best-time-finder',
-    'version': '0.1.0',
-    'description': '',
-    'long_description': '# Nuudel best time finder\n\nIn a poll like this:\n\n|         | 2023-06-05 | 2023-06-07 | 2023-06-08 | 2023-06-12 | ... |\n|---------|------------|------------|------------|------------|-----|\n| Alice   | Yes        | No         | No         | Yes        | ... |\n| Bob     | No         | No         | No         | Yes        | ... |\n| Carl    | Yes        | Yes        | No         | No         | ... |\n| Dave    | Yes        | No         | No         | Yes        | ... |\n| Eve     | No         | No         | No         | Yes        | ... |\n| Francis | No         | No         | No         | No         | ... |\n| ...     | ...        | ...        | ...        | ...        | ... |\n\na common task is to find the set of two or more days that cover as many people as\npossible.\n\nThis tool works with the poll service nuudel (<https://nuudel.digitalcourage.de/>),\nreads the data directly from a given poll and finds the best combinations for any number\nof times.\n\n## Install\n\nInstall using pip:\n\n```console\npip install nuudel-best-time-finder\n\n```\n\n## How to use\n\nSay we have a nuudel poll at: <https://nuudel.digitalcourage.de/nuudel-poll-id> and want\nto find two dates that cover the most amount of people simply run:\n\n```python\nfrom nuudel_best_time_finder import find_best_times\n\nfind_best_times(poll = "{nuudel-poll-id}", n =2, results_file = "results.csv")\n```\n\nThe results are then written to a file called `results.csv` with three columns:\n\n* Time combinations\n* Number of people covered by the combination\n* Percent coverage out of all participants\n',
-    'author': 'Philip Hackstock',
-    'author_email': '20710924+phackstock@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

