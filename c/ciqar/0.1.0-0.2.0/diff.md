# Comparing `tmp/ciqar-0.1.0.tar.gz` & `tmp/ciqar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciqar-0.1.0.tar", last modified: Sun Apr 23 09:19:30 2023, max compression
+gzip compressed data, was "ciqar-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ciqar-0.1.0.tar` & `ciqar-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,49 @@
--rw-r--r--   0        0        0       99 2023-04-06 15:48:56.585664 ciqar-0.1.0/.gitignore
--rw-r--r--   0        0        0      386 2023-04-23 09:06:14.425336 ciqar-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    34020 2023-03-21 20:11:54.896059 ciqar-0.1.0/LICENSE
--rw-r--r--   0        0        0     2731 2023-04-23 09:14:04.133862 ciqar-0.1.0/README.md
--rw-r--r--   0        0        0      323 2023-04-14 17:36:34.484571 ciqar-0.1.0/mypy.ini
--rw-r--r--   0        0        0     1599 2023-04-08 09:36:12.519369 ciqar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-01 11:47:09.294889 ciqar-0.1.0/requirements.txt
--rw-r--r--   0        0        0      245 2023-04-23 09:01:35.471673 ciqar-0.1.0/src/ciqar/__init__.py
--rw-r--r--   0        0        0     5217 2023-04-22 07:11:40.841358 ciqar-0.1.0/src/ciqar/application.py
--rw-r--r--   0        0        0     5026 2023-04-17 15:16:50.357702 ciqar-0.1.0/src/ciqar/input/linter/mypy_logfile.py
--rw-r--r--   0        0        0     1028 2023-04-01 16:50:27.244987 ciqar-0.1.0/src/ciqar/input/linter/pyright_json.py
--rw-r--r--   0        0        0     2009 2023-04-12 16:41:37.894246 ciqar-0.1.0/src/ciqar/input/linter/result_parser.py
--rw-r--r--   0        0        0     5870 2023-04-22 07:09:06.268724 ciqar-0.1.0/src/ciqar/input/sourcefiles.py
--rw-r--r--   0        0        0     5155 2023-04-22 07:13:21.657771 ciqar-0.1.0/src/ciqar/input/violations.py
--rw-r--r--   0        0        0     4725 2023-04-20 15:48:04.819651 ciqar-0.1.0/src/ciqar/report/generator.py
--rw-r--r--   0        0        0     2426 2023-04-08 09:37:00.127329 ciqar-0.1.0/src/ciqar/report/jinja_wrapper.py
--rw-r--r--   0        0        0     2019 2023-04-06 16:00:50.539870 ciqar-0.1.0/src/ciqar/report/pages/all_source_files_list.py
--rw-r--r--   0        0        0     2895 2023-04-06 16:01:40.815510 ciqar-0.1.0/src/ciqar/report/pages/files_per_rule_list.py
--rw-r--r--   0        0        0     1527 2023-04-05 17:45:29.437405 ciqar-0.1.0/src/ciqar/report/pages/rule_list.py
--rw-r--r--   0        0        0     4291 2023-04-05 17:44:43.917059 ciqar-0.1.0/src/ciqar/report/pages/single_file_base.py
--rw-r--r--   0        0        0     2532 2023-04-06 15:56:11.629865 ciqar-0.1.0/src/ciqar/report/pages/source_file.py
--rw-r--r--   0        0        0     2393 2023-04-05 17:54:02.548517 ciqar-0.1.0/src/ciqar/report/pages/summary.py
--rw-r--r--   0        0        0     5021 2023-04-05 17:18:46.801715 ciqar-0.1.0/src/ciqar/templates/api.py
--rw-r--r--   0        0        0     1559 2023-04-06 16:01:31.107580 ciqar-0.1.0/src/ciqar/templates/default-mypy/all_source_files_list.html.in
--rw-r--r--   0        0        0     1397 2023-04-05 17:12:30.207934 ciqar-0.1.0/src/ciqar/templates/default-mypy/files_per_rule_list.html.in
--rw-r--r--   0        0        0     1342 2023-04-05 16:46:17.596887 ciqar-0.1.0/src/ciqar/templates/default-mypy/rule_list.html.in
--rw-r--r--   0        0        0     1164 2023-04-05 16:46:49.748255 ciqar-0.1.0/src/ciqar/templates/default-mypy/source_file.html.in
--rw-r--r--   0        0        0     1790 2023-03-27 15:39:13.692170 ciqar-0.1.0/src/ciqar/templates/default-mypy/style.css
--rw-r--r--   0        0        0     2075 2023-04-05 17:55:14.964573 ciqar-0.1.0/src/ciqar/templates/default-mypy/summary.html.in
--rw-r--r--   0        0        0      215 2023-04-01 11:47:09.294889 ciqar-0.1.0/src/main.py
--rw-r--r--   0        0        0      724 2023-04-07 08:28:48.649546 ciqar-0.1.0/tasks.py
--rw-r--r--   0        0        0     8780 2023-04-17 15:20:35.945883 ciqar-0.1.0/test/ciqar/input/linter/test_mypy_logfile.py
--rw-r--r--   0        0        0     4196 2023-04-08 10:35:52.307764 ciqar-0.1.0/test/ciqar/input/linter/test_pyright_json.py
--rw-r--r--   0        0        0     8854 2023-04-22 07:07:22.920300 ciqar-0.1.0/test/ciqar/input/test_sourcefiles.py
--rw-r--r--   0        0        0     3008 2023-04-08 09:37:15.634990 ciqar-0.1.0/test/ciqar/report/test_jinja_wrapper.py
--rw-r--r--   0        0        0      568 2023-04-08 10:45:37.462580 ciqar-0.1.0/test/ciqar/templates/test_api.py
--rw-r--r--   0        0        0      541 2023-04-11 05:09:51.877327 ciqar-0.1.0/test/ciqar/test___init__.py
--rw-r--r--   0        0        0     3375 2023-04-14 17:33:50.826592 ciqar-0.1.0/test/ciqar/test_application.py
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 ciqar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-04-23 17:02:45.328418 ciqar-0.2.0/.gitignore
+-rw-r--r--   0        0        0      781 2023-06-03 16:41:51.690342 ciqar-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34020 2023-04-23 17:02:45.328418 ciqar-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3754 2023-05-28 12:09:29.012295 ciqar-0.2.0/README.md
+-rw-r--r--   0        0        0      464 2023-05-25 16:06:22.626616 ciqar-0.2.0/mypy.ini
+-rw-r--r--   0        0        0    21165 2023-06-03 16:45:47.400022 ciqar-0.2.0/pylint.rc
+-rw-r--r--   0        0        0     1769 2023-05-28 12:02:20.423772 ciqar-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2011 2023-06-03 16:27:22.024489 ciqar-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0      245 2023-06-03 16:41:51.690342 ciqar-0.2.0/src/ciqar/__init__.py
+-rw-r--r--   0        0        0     7720 2023-06-03 16:40:29.015120 ciqar-0.2.0/src/ciqar/application.py
+-rw-r--r--   0        0        0     1841 2023-06-01 15:56:28.920290 ciqar-0.2.0/src/ciqar/input/__init__.py
+-rw-r--r--   0        0        0     5218 2023-06-01 15:55:53.788402 ciqar-0.2.0/src/ciqar/input/linter/mypy_logfile.py
+-rw-r--r--   0        0        0     1158 2023-06-01 15:56:03.524371 ciqar-0.2.0/src/ciqar/input/linter/pyright_json.py
+-rw-r--r--   0        0        0     1559 2023-06-01 15:56:14.820335 ciqar-0.2.0/src/ciqar/input/linter/result_parser.py
+-rw-r--r--   0        0        0     4870 2023-05-14 15:20:04.251398 ciqar-0.2.0/src/ciqar/input/sourcefiles.py
+-rw-r--r--   0        0        0     3497 2023-05-31 16:16:39.074993 ciqar-0.2.0/src/ciqar/input/violations.py
+-rw-r--r--   0        0        0     1313 2023-06-01 15:08:37.441143 ciqar-0.2.0/src/ciqar/report/datagen/__init__.py
+-rw-r--r--   0        0        0     6170 2023-06-01 15:19:38.085267 ciqar-0.2.0/src/ciqar/report/datagen/_base.py
+-rw-r--r--   0        0        0     2636 2023-06-01 15:12:37.569014 ciqar-0.2.0/src/ciqar/report/datagen/listings.py
+-rw-r--r--   0        0        0     3945 2023-06-01 15:12:26.529642 ciqar-0.2.0/src/ciqar/report/datagen/rules.py
+-rw-r--r--   0        0        0     1494 2023-06-01 15:12:37.545016 ciqar-0.2.0/src/ciqar/report/datagen/sources.py
+-rw-r--r--   0        0        0     2336 2023-06-01 15:12:37.589013 ciqar-0.2.0/src/ciqar/report/datagen/summary.py
+-rw-r--r--   0        0        0     2589 2023-06-01 15:12:37.573014 ciqar-0.2.0/src/ciqar/report/datagen/violations.py
+-rw-r--r--   0        0        0     6565 2023-05-28 17:32:53.409855 ciqar-0.2.0/src/ciqar/report/generator.py
+-rw-r--r--   0        0        0     2944 2023-04-27 16:05:09.624006 ciqar-0.2.0/src/ciqar/report/jinja_wrapper.py
+-rw-r--r--   0        0        0     9075 2023-05-24 14:48:49.058025 ciqar-0.2.0/src/ciqar/templates/api.py
+-rw-r--r--   0        0        0      659 2023-05-20 16:56:35.351615 ciqar-0.2.0/src/ciqar/templates/html_detailed/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-13 16:33:10.750074 ciqar-0.2.0/src/ciqar/templates/html_detailed/index.html.in
+-rw-r--r--   0        0        0     1154 2023-05-13 16:33:08.142094 ciqar-0.2.0/src/ciqar/templates/html_detailed/listing.html.in
+-rw-r--r--   0        0        0     1387 2023-05-13 16:32:58.674170 ciqar-0.2.0/src/ciqar/templates/html_detailed/rule_details.html.in
+-rw-r--r--   0        0        0     1332 2023-05-13 16:32:34.758360 ciqar-0.2.0/src/ciqar/templates/html_detailed/rule_list.html.in
+-rw-r--r--   0        0        0     1549 2023-05-13 16:32:51.610226 ciqar-0.2.0/src/ciqar/templates/html_detailed/source_list.html.in
+-rw-r--r--   0        0        0     1790 2023-04-23 17:02:45.340418 ciqar-0.2.0/src/ciqar/templates/html_detailed/style.css
+-rw-r--r--   0        0        0      341 2023-05-24 14:21:55.082206 ciqar-0.2.0/src/ciqar/templates/html_singlepage/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-24 14:44:39.671157 ciqar-0.2.0/src/ciqar/templates/html_singlepage/index.html.in
+-rw-r--r--   0        0        0      215 2023-04-23 17:02:45.344418 ciqar-0.2.0/src/main.py
+-rw-r--r--   0        0        0     2276 2023-06-03 16:24:45.512701 ciqar-0.2.0/tasks.py
+-rw-r--r--   0        0        0     8994 2023-05-14 16:58:59.618340 ciqar-0.2.0/test/ciqar/input/linter/test_mypy_logfile.py
+-rw-r--r--   0        0        0     4426 2023-05-26 07:01:26.865495 ciqar-0.2.0/test/ciqar/input/linter/test_pyright_json.py
+-rw-r--r--   0        0        0     9198 2023-05-24 15:09:58.478804 ciqar-0.2.0/test/ciqar/input/test_sourcefiles.py
+-rw-r--r--   0        0        0     4895 2023-06-03 05:39:52.346760 ciqar-0.2.0/test/ciqar/input/test_violations.py
+-rw-r--r--   0        0        0    25836 2023-05-24 14:49:28.046546 ciqar-0.2.0/test/ciqar/report/test_datagen.py
+-rw-r--r--   0        0        0     6679 2023-05-28 12:15:46.521689 ciqar-0.2.0/test/ciqar/report/test_generator.py
+-rw-r--r--   0        0        0     3635 2023-05-25 16:06:41.258108 ciqar-0.2.0/test/ciqar/report/test_jinja_wrapper.py
+-rw-r--r--   0        0        0      598 2023-05-23 15:36:30.501858 ciqar-0.2.0/test/ciqar/templates/test_api.py
+-rw-r--r--   0        0        0      765 2023-05-24 14:59:38.476318 ciqar-0.2.0/test/ciqar/templates/test_template_metadata.py
+-rw-r--r--   0        0        0      576 2023-05-22 16:30:09.643680 ciqar-0.2.0/test/ciqar/test___init__.py
+-rw-r--r--   0        0        0     5186 2023-05-22 16:59:52.140802 ciqar-0.2.0/test/ciqar/test_application.py
+-rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 ciqar-0.2.0/PKG-INFO
```

### Comparing `ciqar-0.1.0/LICENSE` & `ciqar-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ciqar-0.1.0/README.md` & `ciqar-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # Ciqar
 
 Ciqar is a tool for creating useful and (at least somewhat) pretty HTML reports from different code
 quality analyzers output in case the analyzers do not provide sufficient report or you want a uniform
 style. The report is generated from a Jinja template so that it can be customized. At the moment, MyPy
-and Pyright are supported as analyzers and there is only one default report template.
+and Pyright are supported as analyzers.
 
 The name is made up from how we pronounced the earliest project name `cqr` (which is the abbreviation
-for *code quality reports*) as a word. Do not confuse it with `Cigar` ;)
+for *code quality reports*) as a word. Do not confuse it with `Cigar` 😉
+
+Have a look at two HTML reports for Ciqar version 0.1.0 (some violations were added purposely 😉):
+ - MyPy: https://aardjon.codeberg.page/ciqar/reports/mypy/
+ - Pyright: https://aardjon.codeberg.page/ciqar/reports/pyright/
+
+[![Build status](https://ci.appveyor.com/api/projects/status/11bkqbw0exo6y76s?svg=true)](https://ci.appveyor.com/project/Aardjon/ciqar)
 
 
 ## Installation
 
 Ciqar releases are available on PyPI, so you can easily install it via `pip`:
 ```
 pip install ciqar
@@ -48,24 +54,39 @@
 
 ```
 ciqar --source /path/to/src/dir --exclude /path/to/src/dir/examples --exclude /path/to/src/dir/snippet.py --analyzer-result [...] --output [...]
 ```
 
 The `--output` option simply defines the directory to write the report into. Any existing files will be overwritten.
 
+The optional `--template` parameter defines the report template to use, allowing to generate different
+kinds of reports. The template name must be specified by its name:
+```
+ciqar -r mypy:mypy.log -s src -o output -t html_detailed
+```
+
+At the moment the following report templates are available:
+
+| Template name   | Description                                                                    |
+|-----------------|--------------------------------------------------------------------------------|
+| html_detailed   | Detailed HTML report including file lists, rule list and source code listings. |
+| html_singlepage | More compact, single-page HTML report listing all violations.                  |
+
+
 ### Examples (run from the repository root)
 
 Create MyPy report for Ciqar:
 ```
 mypy --config-file mypy.ini src test | tee mypy.log
 ciqar -r mypy:mypy.log -s src -s test -o report-mypy
 ```
 
 Create Pyright report for Ciqar:
 ```
 pyright --outputjson src test > pyright.json
 ciqar -r pyright:pyright.json -s src -s test -o report-pyright
 ```
 
+
 ## Some hints
 
 For MyPy reports, it is necessary to set `hide_error_codes = False` in the config (which is default).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ciqar-0.1.0/pyproject.toml` & `ciqar-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -21,22 +21,24 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Software Development :: Quality Assurance",
 ]
 requires-python = ">=3.7"
 dynamic = ["version", "description"]
 dependencies = [
-    "attrs",
-    "Jinja2",
-    "typing_extensions",
+    "Jinja2<4.0",
+    "typing_extensions<5.0",
 ]
 
 [project.optional-dependencies]
 devtools = [
     "invoke",
+    "flit<4",
+    "pip-tools",
+    "pylint",
     "pytest",
     "pytest-cov",
     "pyfakefs",
     "mypy",
     "pyright",
 ]
 
@@ -46,17 +48,24 @@
 
 [project.scripts]
 ciqar = "ciqar:main"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 testpaths=["test"]
-addopts = "--import-mode=importlib --cov src --cov-report=html"
+addopts = "--import-mode=importlib --cov src --cov-report=html --junitxml=junit-pytest.xml"
 
 [tool.coverage.report]
 include_namespace_packages = "true"
+exclude_lines = [
+    '^ +assert_never\(.*?\)$',
+]
+omit = [
+    'src/main.py',
+]
 
 [tool.pyright]
 include = ["src", "test"]
 exclude = ["**/__pycache__"]
+extraPaths = ["src"]
 reportMissingImports = true
 reportMissingTypeStubs = false
```

### Comparing `ciqar-0.1.0/src/ciqar/input/linter/mypy_logfile.py` & `ciqar-0.2.0/src/ciqar/input/linter/mypy_logfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Definition of the MypyLogfileParser class.
 """
 
 from __future__ import annotations
 import re
+from typing import Iterator
 from typing_extensions import override
 
-from ciqar.input.linter.result_parser import LinterResultParser, Violation
+from ciqar.input import Violation
+from ciqar.input.linter.result_parser import GlobalWarning, LinterResultParser, ParsedMessageType
 
 
 class MypyLogfileParser(LinterResultParser):
     """
     Parser implementation for extracting violations from a MyPy logfile.
     """
 
     @property
     @override
     def analyzer_name(self) -> str:
         return "MyPy"
 
     @override
-    def parse(self):
+    def parse(self) -> Iterator[ParsedMessageType]:
         current_violation = None
 
         with self._result_file.open("rt") as fh:
             for log_line in fh:
                 log_line = log_line.strip()
 
                 # Ignore empty lines
@@ -34,15 +36,15 @@
                 # Is it a global message?
                 global_message = self.__parse_global_message(log_line)
                 if global_message:
                     # No need to merge into any previous message, so yield it now
                     if current_violation:
                         yield current_violation
                         current_violation = None
-                    self.global_messages.append(global_message)
+                    yield GlobalWarning(message_text=global_message)
                     continue
 
                 # Is it a regular violation message?
                 violation = self.__parse_violation(log_line)
                 if violation is not None:
                     if (
                         current_violation
@@ -54,15 +56,16 @@
                         # Merge into previous violation
                         current_violation.message_text = "{0}\n{1}: {2}".format(
                             current_violation.message_text,
                             violation.message_type,
                             violation.message_text
                         )
                     elif(
-                        "defined here" in violation.message_text
+                        current_violation
+                        and "defined here" in violation.message_text
                         and violation.message_type == "note"
                         and violation.message_id == "unknown"
                     ):
                         # Merge into previous violation
                         current_violation.message_text = "{0}\n{1}".format(
                             current_violation.message_text,
                             log_line
@@ -76,15 +79,15 @@
                 # else: Parse error, ignore this line
 
             # Yield the last violation, if any
             if current_violation:
                 yield current_violation
                 current_violation = None
 
-    def __parse_violation(self, line):
+    def __parse_violation(self, line: str) -> Violation | None:
         parts = re.fullmatch(
             r"(?P<filepath>.+?)"
             r":(?P<lineno>\d+)"
             r":(?:\d+:)?\s(?P<severity>\w+)"
             r":\s(?P<message>.+)"
             r"\s+\[(?P<rule>[a-z\-]+)\]$",
             line,
```

### Comparing `ciqar-0.1.0/src/ciqar/input/linter/pyright_json.py` & `ciqar-0.2.0/src/ciqar/input/linter/pyright_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 Definition of the PyrightJsonParser class.
 """
 
 from __future__ import annotations
 import json
 from pathlib import Path
+from typing import Iterator
 from typing_extensions import override
 
-from ciqar.input.linter.result_parser import LinterResultParser, Violation
+from ciqar.input import Violation
+from ciqar.input.linter.result_parser import LinterResultParser, ParsedMessageType
 
 
 class PyrightJsonParser(LinterResultParser):
     """
     Parser implementation for extracting violations from a Pyright JSON result file.
     """
 
     @property
     @override
     def analyzer_name(self) -> str:
         return "Pyright"
 
     @override
-    def parse(self):
+    def parse(self) -> Iterator[ParsedMessageType]:
         json_data = json.load(self._result_file.open("rt"))
         for violation_data in json_data.get("generalDiagnostics", []):
             violation = Violation(
                 filename=Path(violation_data["file"]),
-                linenumber=violation_data["range"]["start"]["line"],
+                linenumber=violation_data["range"]["start"]["line"] + 1,  # Pyright is zero-based
                 message_type=violation_data["severity"],
                 message_text=violation_data["message"],
                 message_id=violation_data.get("rule", "unknownRule"),
             )
             yield violation
```

### Comparing `ciqar-0.1.0/src/ciqar/input/linter/result_parser.py` & `ciqar-0.2.0/src/ciqar/input/linter/result_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,51 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-import attrs
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Iterator, Optional, Union
 
+from ciqar.input import Violation
 
-@attrs.define
-class Violation:
-    """
-    Represents a single violation from the linter result. This is the data type provided
-    by LinterResultParser implementation.
-    """
 
-    filename: Path = attrs.field()
+@dataclass
+class GlobalWarning:
     """
-    Full path to the source file this violation was reported in.
+    Represents a linter message that is not tied to a certain source location (e.g. general warnings or errors).
     """
 
-    linenumber: int = attrs.field()
-    """
-    Line number this violation was reported for.
-    """
+    message_text: str
+    """ The message text. """
 
-    message_type = attrs.field()  # TODO: Rename to "message_severity" and use an enum
-    message_text = attrs.field()  # TODO: Refactor to a list of string (multiline messages)
-    message_id = attrs.field()  # TODO: Rename to "rule" and use an enum
+
+ParsedMessageType = Union[Violation, GlobalWarning]
+""" A parsed message that is provided by the parser. """
 
 
 class LinterResultParser(ABC):
     """
     Base class for all result parser implementations.
     Represents a parser providing all reported violations one by one.
     """
 
     def __init__(self, result_file: Path, result_base_path: Optional[Path]=None):
         """
         :param result_file: Linter result file to read violation information from.
         :param result_base_path: The absolute path any relative paths in the linter result file are
                                  relative to.
         """
+
         self._result_file = result_file
         self._result_base_path = result_base_path if result_base_path else self._result_file.parent.resolve()
-        self.global_messages: list[str] = []
-        """
-        List of linter messages that are not tied to a certain source location (e.g. general warnings or
-        errors).
-        """
 
     @property
     @abstractmethod
     def analyzer_name(self) -> str:
         """
-        Name of the code analyzer that created the result result file processed by this parser.
+        Name of the code analyzer that created the result file processed by this parser.
         """
 
     @abstractmethod
-    def parse(self) -> Iterable[Violation]:
+    def parse(self) -> Iterator[ParsedMessageType]:
         """
-        Parses the result data into violation data and returns them one by one.
+        Parses the result data into single messages and returns them one by one.
         """
```

### Comparing `ciqar-0.1.0/src/ciqar/input/sourcefiles.py` & `ciqar-0.2.0/src/ciqar/input/sourcefiles.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,12 @@
 from __future__ import annotations
 from itertools import chain, tee
 from pathlib import Path
-from typing import Iterable, Optional
 
-
-class SourceFile:
-
-    def __init__(self, absolute_path: Path, project_base_path: Path):
-        """
-        :raises: The provided file does not exit
-        """
-        if not absolute_path.exists():
-            raise FileNotFoundError("File not found: {}".format(absolute_path))
-
-        self.absolute_path = absolute_path
-        self.project_relative_path = absolute_path.relative_to(project_base_path)
-        self._line_count: Optional[int] = None
-
-    @property
-    def line_count(self) -> int:
-        """
-        Returns the number of non-empty lines in this file.
-        Line containing only whitespace are considered "empty".
-        """
-        if self._line_count is None:
-            self._line_count = sum(1 for line in self.absolute_path.open("rt").readlines() if line.strip())
-        return self._line_count
-
-    @property
-    def content(self) -> Iterable[str]:
-        with self.absolute_path.open("rt") as fh:
-            for line in fh:
-                yield line.rstrip()
+from ciqar.input import SourceFile
 
 
 class SourceFileCollector:
     """
     Collects all source files that have been analyzed and must therefore be respected for the report.
 
     The collection is done on demand when the data is accessed for the first time.
```

### Comparing `ciqar-0.1.0/src/ciqar/report/jinja_wrapper.py` & `ciqar-0.2.0/src/ciqar/report/jinja_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from jinja2 import Environment, PackageLoader, select_autoescape
 from jinja2.exceptions import TemplateNotFound, TemplateError
 from pathlib import Path
+from typing import cast
 
 
 class JinjaWrapper:
     """
     Represents the Jinja2 library.
     All Jinja2 dependent code is wrapped in this class, to decouple the dependency from
     the application and make mocking as well as future updates easier.
@@ -13,44 +14,53 @@
 
     def __init__(self, template_package_name: str):
         self._jinja_environment = Environment(
             loader=PackageLoader(package_name="ciqar.templates", package_path=template_package_name),
             autoescape=select_autoescape(enabled_extensions=("html", "in"), default_for_string=True,)
         )
  
-    def render_template(self, template_filename: str, **report_data) -> str:
+    def render_template(self, template_filename: str, **report_data: object) -> str:
         try:
             template = self._jinja_environment.get_template(template_filename)
         except TemplateNotFound:
+            # Casting is safe because we explicitly provide PackageLoader to the Jinja
+            # environment during __init()__.
             raise FileNotFoundError("Requested template '{0}' not found in package '{1}'.".format(
-                template_filename, self._jinja_environment.loader.package_path
+                template_filename, cast(PackageLoader, self._jinja_environment.loader).package_path
             ))
 
         try:
             return template.render(**report_data)
         except TemplateError as e:
             # Wrap Jinja2 exception types
             raise TemplateRenderError(str(e))
 
-    def get_static_file(self, template_filename) -> Path:
+    def get_static_file(self, template_filename: str) -> Path:
         """
         Returns the absolute path of the requested template file.
         This is useful for files that simply need to be copied (without any Jinja processing).
 
         :param template_filename: Name of a file within the current template.
         :returns: Absolute path of the requested file.
         :raises FileNotFoundError: The requested file does not exist in the template.
         """
 
+        # Create the "not found" error message in case it is needed later. Casting is safe because we
+        # explicitly provided PackageLoader to the Jinja environment during __init()__.
+        error_message = "Requested static file '{0}' not found in package '{1}'.".format(
+            template_filename, cast(PackageLoader, self._jinja_environment.loader).package_path
+        )
         try:
             template = self._jinja_environment.get_template(template_filename)
         except TemplateNotFound:
-            raise FileNotFoundError("Requested static file '{0}' not found in package '{1}'.".format(
-                template_filename, self._jinja_environment.loader.package_path
-            ))
+            raise FileNotFoundError(error_message)
+
+        if not template.filename:
+            raise FileNotFoundError(error_message)
+
         return Path(template.filename)
 
 
 class TemplateRenderError(Exception):
     """
     Raised on error rendering an existing template. This usually wraps a Jinja2 exception and contains the
     original error message.
```

### Comparing `ciqar-0.1.0/src/ciqar/report/pages/all_source_files_list.py` & `ciqar-0.2.0/src/ciqar/report/datagen/listings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,68 @@
+"""
+Definition of the ListingsRenderInfoGenerator class.
+"""
+
 from __future__ import annotations
-from pathlib import Path
-from typing_extensions import override  # @UnresolvedImport
+from copy import copy
+from typing import Sequence
+from typing_extensions import override
 
-from ciqar.report.pages.single_file_base import SingleFileGenerator
-from ciqar.templates.api import ReportFile, FileListRow
+from ciqar.input import SourceFile, Violation
+from ciqar.report.datagen import FileRenderInformation, RenderInformationGeneratorConfig
+from ciqar.report.datagen._base import RenderInformationGenerator
+from ciqar.templates.api import SourceLine
 
 
-class AllSourceFilesListGenerator(SingleFileGenerator):
+class ListingsRenderInfoGenerator(RenderInformationGenerator):
     """
-    Template Method implementation for generating the source file list.
-    It also summarizes some results for each file (e.g. violation count).
+    Generator that produces render information for source file listing pages.
+    Each iteration returns data for one source file.
     """
 
-    @override
-    def _get_template_filename(self) -> str:
-        return "all_source_files_list.html.in"
+    def __init__(self, generator_config: RenderInformationGeneratorConfig):
+        super().__init__(generator_config=generator_config)
+        self.__source_file_iter = iter(self._source_files)
 
     @override
-    def _get_output_filepath(self, report_base_path: Path) -> Path:
-        return report_base_path.joinpath("all_source_files_list.html")
-
-    @override
-    def _create_template_data(self) -> ReportFile:
-        source_files_data = []
-        for source_file in self._source_file_collector.get_all_source_files():
-            line_count = self._linter_results.get_line_count(source_file.absolute_path)
-            violation_count = self._linter_results.get_violation_count(source_file.absolute_path)
-            rating = 2
-            if violation_count == 0:
-                rating = 0
-            elif violation_count < 10:
-                rating = 1
-            source_files_data.append(FileListRow(
-                display_filename=str(source_file.project_relative_path),
-                report_filename=str(Path("sources").joinpath(
-                    self._create_corresponding_report_output_file_path(source_file.project_relative_path)
-                )),
-                line_count=source_file.line_count,
-                bad_line_count=line_count,
-                violation_count=violation_count,
-                rating=rating,
+    def __next__(self) -> FileRenderInformation:
+        source_file = next(self.__source_file_iter)
+        report_file = copy(self._report_file_prototype)
+        absolute_output_filepath = self._report_base_path.joinpath(
+            "sources",
+            self._create_corresponding_report_output_file_path(source_file.project_relative_path)
+        )
+        report_file.path_to_report_root = self._get_relative_url_to_report_root(absolute_output_filepath)
+        report_file.context_name = str(source_file.project_relative_path)
+        report_file.source_content_data = self.__create_source_content_data(
+            source_file,
+            self._violations
+        )
+
+        return FileRenderInformation(
+            input_template_name=self._input_template_name,
+            output_file_path=absolute_output_filepath,
+            template_data=report_file
+        )
+
+
+    def __create_source_content_data(
+            self,
+            source_file: SourceFile,
+            violations: Sequence[Violation]
+    ) -> list[SourceLine]:
+        file_violations = [v for v in violations if v.filename == source_file.absolute_path]
+        source_lines = []
+        for idx, code in enumerate(source_file.content):
+            lineno = idx + 1
+
+            current_line_violations = [v for v in file_violations if v.linenumber == lineno]
+            source_lines.append(SourceLine(
+                lineno=lineno,
+                content=code.rstrip("\n").rstrip("\r"),
+                rating="good" if not current_line_violations else "bad",
+                messages = [
+                    "{}: {}".format(violation.message_type, violation.message_text)
+                    for violation in current_line_violations
+                ]
             ))
-
-        files_page = ReportFile(
-            report_title=self._report_name,
-            path_to_report_root=self._get_relative_url_to_report_root(),
-            ciqar_tag=self._application_tag,
-            file_list_data=source_files_data
-        ) 
-        return files_page
+        return source_lines
```

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/all_source_files_list.html.in` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/source_list.html.in`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <title>{{data.report_title}}</title>
 </head>
 <body>
 <h1>{{data.report_title}}</h1>
 <table class="navigation">
 <tr class="navigation">
 <td class="navigation"><a href="index.html">Report Summary</a></td>
-<td class="navigation"><a href="all_source_files_list.html">Show by files</a></td>
+<td class="navigation"><a href="source_list.html">Show by files</a></td>
 <td class="navigation"><a href="rule_list.html">Show by rules</a></td>
 </tr>
 </table>
 
 <table class="summary">
 <caption>Summary by File</caption>
 <thead><tr class="summary">
```

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/files_per_rule_list.html.in` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/rule_details.html.in`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <title>{{data.report_title}}</title>
 </head>
 <body>
 <h1>{{data.report_title}}</h1>
 <table class="navigation">
 <tr class="navigation">
 <td class="navigation"><a href="{{data.path_to_report_root}}index.html">Report Summary</a></td>
-<td class="navigation"><a href="{{data.path_to_report_root}}all_source_files_list.html">Show by files</a></td>
+<td class="navigation"><a href="{{data.path_to_report_root}}source_list.html">Show by files</a></td>
 <td class="navigation"><a href="{{data.path_to_report_root}}rule_list.html">Show by rules</a></td>
 </tr>
 </table>
 
 <table class="summary">
 <caption>Files causing violations against rule {{data.context_name}}</caption>
 <thead><tr class="summary">
```

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/rule_list.html.in` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/rule_list.html.in`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <title>{{data.report_title}}</title>
 </head>
 <body>
 <h1>{{data.report_title}}</h1>
 <table class="navigation">
 <tr class="navigation">
 <td class="navigation"><a href="index.html">Report Summary</a></td>
-<td class="navigation"><a href="all_source_files_list.html">Show by files</a></td>
+<td class="navigation"><a href="source_list.html">Show by files</a></td>
 <td class="navigation"><a href="rule_list.html">Show by rules</a></td>
 </tr>
 </table>
 
 <table class="summary">
 <caption>Summary by Linter Rules</caption>
 <thead><tr class="summary">
```

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/source_file.html.in` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/listing.html.in`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <title>{{data.report_title}}</title>
 </head>
 <body>
 <h1>{{data.report_title}}</h1>
 <table class="navigation">
 <tr class="navigation">
 <td class="navigation"><a href="{{data.path_to_report_root}}index.html">Report Summary</a></td>
-<td class="navigation"><a href="{{data.path_to_report_root}}all_source_files_list.html">Show by files</a></td>
+<td class="navigation"><a href="{{data.path_to_report_root}}source_list.html">Show by files</a></td>
 <td class="navigation"><a href="{{data.path_to_report_root}}rule_list.html">Show by rules</a></td>
 </tr>
 </table>
 
 <table class="summary">
 <caption>File Listing for {{data.context_name}}</caption>
 <tbody>
```

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/style.css` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/style.css`

 * *Files identical despite different names*

### Comparing `ciqar-0.1.0/src/ciqar/templates/default-mypy/summary.html.in` & `ciqar-0.2.0/src/ciqar/templates/html_detailed/index.html.in`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <title>{{data.report_title}}</title>
 </head>
 <body>
 <h1>{{data.report_title}}</h1>
 <table class="navigation">
 <tr class="navigation">
 <td class="navigation"><a href="index.html">Report Summary</a></td>
-<td class="navigation"><a href="all_source_files_list.html">Show by files</a></td>
+<td class="navigation"><a href="source_list.html">Show by files</a></td>
 <td class="navigation"><a href="rule_list.html">Show by rules</a></td>
 </tr>
 </table>
 
 <table class="summary50">
 <caption>Report Summary</caption>
 <tr class="summary summary-neutral">
```

### Comparing `ciqar-0.1.0/test/ciqar/input/linter/test_mypy_logfile.py` & `ciqar-0.2.0/test/ciqar/input/linter/test_mypy_logfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 """
 
 from __future__ import annotations
 from pathlib import Path
 from pyfakefs.fake_filesystem import FakeFilesystem
 import pytest
 
+from ciqar.input import Violation
 from ciqar.input.linter.mypy_logfile import MypyLogfileParser
-from ciqar.input.linter.result_parser import Violation
+from ciqar.input.linter.result_parser import GlobalWarning
 
 
 class TestMypyLogfileParser():
     """
     Unit tests for the MypyLogfileParser class.
     """
 
@@ -174,20 +175,22 @@
             fs: FakeFilesystem
     ) -> None:
         MYPY_LOGFILE = Path("/tmp/mypy.log")
 
         fs.create_file(MYPY_LOGFILE, contents=logfile_content.strip())
         parser = MypyLogfileParser(result_file=MYPY_LOGFILE, result_base_path=Path("/out"))
 
-        violations = list(parser.parse())
+        messages = list(parser.parse())
+        violations = [m for m in messages if isinstance(m, Violation)]
+        global_messages = [m for m in messages if isinstance(m, GlobalWarning)]
         assert len(expected_violations) == len(violations)
         for expected, parsed in zip(expected_violations, violations):
             assert str(expected.filename) == str(parsed.filename)
             assert expected.linenumber == parsed.linenumber
             assert expected.message_type == parsed.message_type
             assert expected.message_text == parsed.message_text
             assert expected.message_id == parsed.message_id
-        assert expected_global_messages == parser.global_messages
+        assert expected_global_messages == [m.message_text for m in global_messages]
 
-    def test_analyzer_name(self):
+    def test_analyzer_name(self) -> None:
         parser = MypyLogfileParser(result_file=Path("/tmp/result.log"))
         assert parser.analyzer_name == "MyPy"
```

### Comparing `ciqar-0.1.0/test/ciqar/input/linter/test_pyright_json.py` & `ciqar-0.2.0/test/ciqar/input/linter/test_pyright_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 """
 
 from __future__ import annotations
 from pathlib import Path
 from pyfakefs.fake_filesystem import FakeFilesystem
 import pytest
 
+from ciqar.input import Violation
 from ciqar.input.linter.pyright_json import PyrightJsonParser
-from ciqar.input.linter.result_parser import Violation
+from ciqar.input.linter.result_parser import GlobalWarning
 
 
 class TestPyrightJsonParser:
     """
     Unit tests for the PyrightJsonParser class.
     """
 
@@ -69,19 +70,19 @@
             },
             "rule": "reportGeneralTypeIssues"
         }
     ]
 }
             """,
             [
-                Violation(filename=Path("/path/to/file1.py"), linenumber=68,
+                Violation(filename=Path("/path/to/file1.py"), linenumber=69,
                     message_type="error", message_id="reportGeneralTypeIssues",
                     message_text="No parameter named \"message_type\"",
                 ),
-                Violation(filename=Path("/path/to/file2.py"), linenumber=26,
+                Violation(filename=Path("/path/to/file2.py"), linenumber=27,
                     message_type="error", message_id="reportGeneralTypeIssues",
                     message_text="Dataclass field without type annotation will cause runtime exception",
                 ),
             ]
         ),
 
         (  # Violation without the 'rule' field
@@ -104,32 +105,35 @@
                 }
             }
         }
     ]
 }
             """,
             [
-                Violation(filename=Path("/path/to/file.py"), linenumber=7,
+                Violation(filename=Path("/path/to/file.py"), linenumber=8,
                     message_type="error", message_id="unknownRule",
                     message_text="No parameter named \"message_id\"",
                 )
             ]
         ),
     ])
     def test_parse(self, jsonfile_content:str, expected_violations: list[Violation], fs: FakeFilesystem) -> None:
         PYRIGHT_JSON_FILE = Path("/tmp/pyright.json")
 
         fs.create_file(PYRIGHT_JSON_FILE, contents=jsonfile_content.strip())
         parser = PyrightJsonParser(result_file=PYRIGHT_JSON_FILE, result_base_path=Path("/out"))
 
-        violations = list(parser.parse())
+        messages = list(parser.parse())
+        violations = [m for m in messages if isinstance(m, Violation)]
+        global_messages = [m for m in messages if isinstance(m, GlobalWarning)]
         assert len(expected_violations) == len(violations)
         for expected, parsed in zip(expected_violations, violations):
             assert str(expected.filename) == str(parsed.filename)
             assert expected.linenumber == parsed.linenumber
             assert expected.message_type ==parsed.message_type
             assert expected.message_text == parsed.message_text
             assert expected.message_id == parsed.message_id
+        assert not global_messages
 
-    def test_analyzer_name(self):
+    def test_analyzer_name(self) -> None:
         parser = PyrightJsonParser(result_file=Path("/tmp/result.json"))
         assert parser.analyzer_name == "Pyright"
```

### Comparing `ciqar-0.1.0/test/ciqar/input/test_sourcefiles.py` & `ciqar-0.2.0/test/ciqar/input/test_sourcefiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """
 Unit tests for the ciqar.input.sourcefiles module.
 """
 
 from __future__ import annotations
-from contextlib import nullcontext, AbstractContextManager
+from contextlib import AbstractContextManager, nullcontext 
 from pathlib import Path
 from pyfakefs.fake_filesystem import FakeFilesystem
 import pytest
 
-from ciqar.input.sourcefiles import SourceFile, SourceFileCollector
+from ciqar.input import SourceFile
+from ciqar.input.sourcefiles import SourceFileCollector
 from unittest.mock import MagicMock, Mock
 
 
 class TestSourceFile:
     """
     Unit tests for the SourceFile class.
     """
 
     @pytest.mark.parametrize("file_exists, init_context", [
         (True, nullcontext()),
         (False, pytest.raises(FileNotFoundError)),
     ])
-    def test_init(self, file_exists, init_context, fs):
+    def test_init(
+            self,
+            file_exists: bool,
+            init_context: AbstractContextManager[None],
+            fs: FakeFilesystem
+    ) -> None:
         """
         Ensures the initialisation behaviour of SourceFile objects.
         """
         absolute_file_path = Path("/tmp/file.txt")
 
         if file_exists:
             fs.create_file(absolute_file_path)
@@ -37,27 +43,37 @@
 
     @pytest.mark.parametrize("file_content, expected_line_count", [
         ([], 0),  # Empty file
         (["\n"], 0),  # Empty line
         (["single line"], 1),
         (["first line", "", "third line"], 2),
     ])
-    def test_line_count(self, file_content, expected_line_count, fs):
+    def test_line_count(
+            self,
+            file_content: list[str],
+            expected_line_count: int,
+            fs: FakeFilesystem
+    ) -> None:
         absolute_file_path = Path("/tmp/sourcefile.py")
         fs.create_file(file_path=absolute_file_path, contents="\n".join(file_content))
 
         source_file = SourceFile(absolute_file_path, Path("/tmp"))
         assert source_file.line_count == expected_line_count
 
     @pytest.mark.parametrize("file_content, expected_file_content", [
         ([], []),  # Empty file
         (["Hello", "World"], ["Hello", "World"]),
         (["   indented string   \r"], ["   indented string"]),  # Strip trailing whitespaces
     ])
-    def test_content(self, file_content, expected_file_content, fs):
+    def test_content(
+            self,
+            file_content: list[str],
+            expected_file_content: list[str],
+            fs: FakeFilesystem
+    ) -> None:
         file_path = Path("/tmp/sourcefile.py")
         fs.create_file(file_path=file_path, contents="\n".join(file_content))
 
         source_file = SourceFile(file_path, Path("/tmp"))
         file_content = []
         for line in source_file.content:
             file_content.append(line)
@@ -102,15 +118,15 @@
             pytest.raises(ValueError),
             ""
         )
     ])
     def test_find_common_base_path(
             self,
             search_paths: list[str],
-            init_context: AbstractContextManager,
+            init_context: AbstractContextManager[None],
             expected_base_path: str
     ) -> None:
         """
         Tests the search for finding the largest common ancestor (base path) from the provided list of paths.
         (done during object initialization).
         """
         with init_context:
@@ -217,15 +233,15 @@
         ("/tmp/source.py", nullcontext()),  # Normal case of existing file
         ("/tmp/missingfile.py", pytest.raises(FileNotFoundError)),  # File does not exist
         ("/src/main.py", pytest.raises(FileNotFoundError)),  # File exists, but is not in the search path
     ])
     def test_get_source_file(
             self,
             request_filepath: str,
-            raise_context: AbstractContextManager,
+            raise_context: AbstractContextManager[None],
             fs: FakeFilesystem
     ) -> None:
         """
         Tests correct behaviour of the `get_source_file()` method.
         For this test, the only existings source files are '/tmp/source.py' and '/src/main.py', the collector
         search path is '/tmp'.
         """
```

### Comparing `ciqar-0.1.0/test/ciqar/report/test_jinja_wrapper.py` & `ciqar-0.2.0/test/ciqar/report/test_jinja_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from pathlib import Path
 import pytest
 
 from ciqar.report.jinja_wrapper import JinjaWrapper, TemplateRenderError
 
 
 @pytest.mark.parametrize("template_name, raise_context", [
-    ("default-mypy", nullcontext()),  # Existing template
-    ("does-not-exist", pytest.raises(ValueError)),  # Non-existing template
+    ("html_detailed", nullcontext()),  # Existing template
+    ("does_not_exist", pytest.raises(ValueError)),  # Non-existing template
 ])
-def test_init(template_name: str, raise_context: AbstractContextManager) -> None:
+def test_init(template_name: str, raise_context: AbstractContextManager[None]) -> None:
     with raise_context:
         JinjaWrapper(template_package_name=template_name)
     assert True
 
 
-def test_render_template_filenotfound():
+def test_render_template_filenotfound() -> None:
     """
     Tests correct behaviour (exception) if the requested template is not available.
     """
-    wrapper = JinjaWrapper(template_package_name="default-mypy")
+    wrapper = JinjaWrapper(template_package_name="html_detailed")
 
     with pytest.raises(FileNotFoundError):
         wrapper.render_template(template_filename="doesntexist.html.in")
 
 @pytest.mark.parametrize("render_side_effect, render_return_value, raise_context", [
     (  # Normal case, everything goes well
         None,
@@ -44,38 +44,52 @@
        None,
        pytest.raises(TemplateRenderError)
     ),
 ])
 def test_render_template(
         render_side_effect: Exception | None,
         render_return_value: str,
-        raise_context: AbstractContextManager
+        raise_context: AbstractContextManager[None]
 ) -> None:
     """
     Tests the correct behaviour of "render_template" (except for the "template does not exist" case, see
     `test_render_template_filenotfound()` for that one).
     """
     mocked_template = Mock(spec=Template)
     mocked_template.render.side_effect = render_side_effect
     mocked_template.render.return_value = render_return_value
 
-    wrapper = JinjaWrapper(template_package_name="default-mypy")
+    wrapper = JinjaWrapper(template_package_name="html_detailed")
     wrapper._jinja_environment = Mock(spec=Environment)
     wrapper._jinja_environment.get_template.return_value = mocked_template
 
     with raise_context:
         rendered_file_content = wrapper.render_template(template_filename="example_file_list.html.in")
         assert render_return_value == rendered_file_content
 
 
 @pytest.mark.parametrize("file_name, raise_context", [
-    ("summary.html.in", nullcontext()),  # File exists
+    ("index.html.in", nullcontext()),  # File exists
     ("notfound.css", pytest.raises(FileNotFoundError)),  # File does not exist
 ])
-def test_get_static_file(file_name: str, raise_context: AbstractContextManager) -> None:
+def test_get_static_file(file_name: str, raise_context: AbstractContextManager[None]) -> None:
     src_dir = Path(__file__).parent.parent.parent.parent.joinpath("src")
-    template_path = src_dir.joinpath("ciqar", "templates", "default-mypy")
-    wrapper = JinjaWrapper(template_package_name="default-mypy")
+    template_path = src_dir.joinpath("ciqar", "templates", "html_detailed")
+    wrapper = JinjaWrapper(template_package_name="html_detailed")
 
     with raise_context:
         static_file_path = wrapper.get_static_file(template_filename=file_name)
         assert template_path.joinpath(file_name) == static_file_path
+
+def test_get_static_file_defunct_template() -> None:
+    """
+    Tests the correct behaviour in case the requested template file could be loaded but doesn't have a
+    file system path (e.g. some kind of in-memory template?)
+    """
+
+    wrapper = JinjaWrapper(template_package_name="html_detailed")
+    mocked_template = Mock(spec=Template)
+    mocked_template.filename = None
+    wrapper._jinja_environment.get_template = Mock(return_value=mocked_template)  # type: ignore[method-assign]
+
+    with pytest.raises(FileNotFoundError):
+        wrapper.get_static_file(template_filename="style.css")
```

### Comparing `ciqar-0.1.0/test/ciqar/test___init__.py` & `ciqar-0.2.0/test/ciqar/test___init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Unit tests for the `ciqar.__init__` module
 """
 
+from __future__ import annotations
 from unittest.mock import Mock, patch
 
 from ciqar import main
 from ciqar.application import CiqarApplication
 
 
 @patch("ciqar.application.CiqarApplication")
```

### Comparing `ciqar-0.1.0/test/ciqar/test_application.py` & `ciqar-0.2.0/test/ciqar/test_application.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 """
 Unit tests for the `ciqar.application` module.
 """
 
-from argparse import ArgumentTypeError
+from __future__ import annotations
+from argparse import ArgumentParser, ArgumentTypeError
 from functools import partial
 from pathlib import Path
 import pytest
-from typing import Type
-from unittest.mock import Mock, patch
+import sys
+from unittest.mock import MagicMock, Mock, patch
 
 from ciqar.application import CiqarApplication
 from ciqar.input.linter.mypy_logfile import MypyLogfileParser
 from ciqar.input.linter.pyright_json import PyrightJsonParser
+from ciqar.input.linter.result_parser import LinterResultParser
 from ciqar.report.generator import ReportGenerator
 
 
 # TODO: It'd be cool to have a test for the command line interface, i.e. allowed options and
 # their syntax, to get a warning when the CLI changes. But I don't have a good idea of how to
 # do this, yet.
 
 
+def _create_argparse_mock(mocked_argparser_cls: Mock) -> None:
+    argument_parser_mock = Mock(spec=ArgumentParser)
+    argument_parser_mock.parse_args = MagicMock()
+    argument_parser_mock.parse_args.return_value.template_metadata = ("default", {})
+    mocked_argparser_cls.return_value = argument_parser_mock
+
+
 @patch("ciqar.application.ArgumentParser")
-def test_app_description(_: Mock) -> None:
+def test_app_description(argument_parser_cls_mock: Mock) -> None:
     """
-    SImple tests for the application name and version properties.
+    Simple tests for the application name and version properties.
     """
+
+    _create_argparse_mock(argument_parser_cls_mock)
+
     application = CiqarApplication()
     assert application.application_name == "Ciqar"
 
     version_strings = application.application_version.split(".")
     assert len(version_strings) == 3
     major, minor, bug = version_strings
     assert major.isdigit()
@@ -38,26 +50,29 @@
 
 @pytest.mark.parametrize("result_url, expected_factory_class, expected_result_path", [
     ("mypy:/path/to/file.log", MypyLogfileParser, Path("/path/to/file.log")),
     ("pyright:/path/to/file.json", PyrightJsonParser, Path("/path/to/file.json")),
 ])
 def test__parse_analyzer_result_url__normal_usecase(
         result_url: str,
-        expected_factory_class: Type,
+        expected_factory_class: type[LinterResultParser],
         expected_result_path: Path
 ) -> None:
     """
     Tests parsing of analyzer result URLs (as provided on command line).
     """
     parser_factory = CiqarApplication._parse_analyzer_result_url(analyzer_result_url=result_url)
     expected_factory = partial(expected_factory_class, expected_result_path)
 
-    # Returning a "partial" object is not a requirement to test, but the following three checks rely on it.
-    # So we want a warning if this ever chanegs, because then we need to adapt this testc ase as well.
-    assert isinstance(parser_factory, partial), "The test requries the factory to be a 'partial' object" 
+    # Returning a "partial" object is not a requirement to test, but the following three checks rely
+    # on it. So we want a warning if this ever chanegs, because then we need to adapt this test case
+    # as well.
+    assert \
+        isinstance(parser_factory, partial), \
+        "The test requries the factory to be a 'partial' object"
     assert parser_factory.func == expected_factory.func
     assert parser_factory.args == expected_factory.args
     assert parser_factory.keywords == expected_factory.keywords
 
 
 @pytest.mark.parametrize("invalid_result_url", [
     "unknown:/some/file.bin",  # Unknown analyzer
@@ -68,21 +83,53 @@
     """
     Tests the behaviour when the provided result URL is invalid.
     """
     with pytest.raises(ArgumentTypeError):
         CiqarApplication._parse_analyzer_result_url(analyzer_result_url=invalid_result_url)
 
 
+def test__load_template_files_specification() -> None:
+    """
+    Tests loading of template metadata by a name (as provided on command line).
+    """
+
+    # Test case 1: Load a valid, existing template (the default one)
+    template_name, template_files_spec = CiqarApplication._load_template_files_specification(
+        template_name="html_detailed"
+    )
+    assert template_name == "html_detailed"
+    assert len(template_files_spec["static_files"]) > 0
+    assert len(template_files_spec["render_files"]) > 0
+
+    # Test case 2: Requested template does not exist
+    with pytest.raises(ArgumentTypeError):
+        CiqarApplication._load_template_files_specification(template_name="does_not_exist")
+
+    # Test case 3: Requested template exists as module, but doesn't provide the necessary metadata
+    # Pretend the metadata module has been imported alreday, and set it to something not providing
+    # the desired metadata
+    sys.modules["ciqar.templates.invalid_template"] = sys
+    with pytest.raises(ArgumentTypeError):
+        CiqarApplication._load_template_files_specification(template_name="invalid_template")
+    del sys.modules["ciqar.templates.invalid_template"]
+
+
 @patch("ciqar.application.ArgumentParser")
 @patch("ciqar.application.ReportGenerator")
 @patch("ciqar.application.SourceFileCollector")
-def test_run(_argument_parser_cls_mock: Mock, generator_cls_mock: Mock, _source_collector_cls_mock: Mock) -> None:
+def test_run(
+        _source_collector_cls_mock: Mock,
+        generator_cls_mock: Mock,
+        argument_parser_cls_mock: Mock,
+) -> None:
     """
     Simple test case for the run() method. Makes sure the ReportGenerator is run).
     """
+
+    _create_argparse_mock(argument_parser_cls_mock)
     generator_mock = Mock(spec=ReportGenerator)
     generator_cls_mock.return_value = generator_mock
 
     app = CiqarApplication()
     app.run()
 
     assert generator_mock.generate_report.call_count == 1
```

### Comparing `ciqar-0.1.0/PKG-INFO` & `ciqar-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciqar
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ciqar is a tool for creating reports from different code quality analyzers output.
 Keywords: linter,report,code analysis,code quality
 Author: Thomas Wesenigk <thw-oss@fomori.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -14,36 +14,44 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: attrs
-Requires-Dist: Jinja2
-Requires-Dist: typing_extensions
+Requires-Dist: Jinja2<4.0
+Requires-Dist: typing_extensions<5.0
 Requires-Dist: invoke ; extra == "devtools"
+Requires-Dist: flit<4 ; extra == "devtools"
+Requires-Dist: pip-tools ; extra == "devtools"
+Requires-Dist: pylint ; extra == "devtools"
 Requires-Dist: pytest ; extra == "devtools"
 Requires-Dist: pytest-cov ; extra == "devtools"
 Requires-Dist: pyfakefs ; extra == "devtools"
 Requires-Dist: mypy ; extra == "devtools"
 Requires-Dist: pyright ; extra == "devtools"
 Project-URL: Home, https://codeberg.org/Aardjon/ciqar/
 Project-URL: Source, https://codeberg.org/Aardjon/ciqar.git
 Provides-Extra: devtools
 
 # Ciqar
 
 Ciqar is a tool for creating useful and (at least somewhat) pretty HTML reports from different code
 quality analyzers output in case the analyzers do not provide sufficient report or you want a uniform
 style. The report is generated from a Jinja template so that it can be customized. At the moment, MyPy
-and Pyright are supported as analyzers and there is only one default report template.
+and Pyright are supported as analyzers.
 
 The name is made up from how we pronounced the earliest project name `cqr` (which is the abbreviation
-for *code quality reports*) as a word. Do not confuse it with `Cigar` ;)
+for *code quality reports*) as a word. Do not confuse it with `Cigar` 😉
+
+Have a look at two HTML reports for Ciqar version 0.1.0 (some violations were added purposely 😉):
+ - MyPy: https://aardjon.codeberg.page/ciqar/reports/mypy/
+ - Pyright: https://aardjon.codeberg.page/ciqar/reports/pyright/
+
+[![Build status](https://ci.appveyor.com/api/projects/status/11bkqbw0exo6y76s?svg=true)](https://ci.appveyor.com/project/Aardjon/ciqar)
 
 
 ## Installation
 
 Ciqar releases are available on PyPI, so you can easily install it via `pip`:
 ```
 pip install ciqar
@@ -81,25 +89,40 @@
 
 ```
 ciqar --source /path/to/src/dir --exclude /path/to/src/dir/examples --exclude /path/to/src/dir/snippet.py --analyzer-result [...] --output [...]
 ```
 
 The `--output` option simply defines the directory to write the report into. Any existing files will be overwritten.
 
+The optional `--template` parameter defines the report template to use, allowing to generate different
+kinds of reports. The template name must be specified by its name:
+```
+ciqar -r mypy:mypy.log -s src -o output -t html_detailed
+```
+
+At the moment the following report templates are available:
+
+| Template name   | Description                                                                    |
+|-----------------|--------------------------------------------------------------------------------|
+| html_detailed   | Detailed HTML report including file lists, rule list and source code listings. |
+| html_singlepage | More compact, single-page HTML report listing all violations.                  |
+
+
 ### Examples (run from the repository root)
 
 Create MyPy report for Ciqar:
 ```
 mypy --config-file mypy.ini src test | tee mypy.log
 ciqar -r mypy:mypy.log -s src -s test -o report-mypy
 ```
 
 Create Pyright report for Ciqar:
 ```
 pyright --outputjson src test > pyright.json
 ciqar -r pyright:pyright.json -s src -s test -o report-pyright
 ```
 
+
 ## Some hints
 
 For MyPy reports, it is necessary to set `hide_error_codes = False` in the config (which is default).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

