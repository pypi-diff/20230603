# Comparing `tmp/pylsp-mypy-0.6.6.tar.gz` & `tmp/pylsp-mypy-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsp-mypy-0.6.6.tar", last modified: Sun Feb 26 17:05:12 2023, max compression
+gzip compressed data, was "pylsp-mypy-0.6.7.tar", last modified: Sat Jun  3 13:59:18 2023, max compression
```

## Comparing `pylsp-mypy-0.6.6.tar` & `pylsp-mypy-0.6.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 17:05:12.803830 pylsp-mypy-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-26 17:05:12.803830 pylsp-mypy-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 17:05:12.803830 pylsp-mypy-0.6.6/pylsp_mypy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/pylsp_mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/pylsp_mypy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/pylsp_mypy/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 17:05:12.803830 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-26 17:05:12.000000 pylsp-mypy-0.6.6/pylsp_mypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-26 17:05:12.807830 pylsp-mypy-0.6.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 17:05:12.803830 pylsp-mypy-0.6.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-02-26 17:05:04.000000 pylsp-mypy-0.6.6/test/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:59:18.378334 pylsp-mypy-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-03 13:59:18.378334 pylsp-mypy-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:59:18.374334 pylsp-mypy-0.6.7/pylsp_mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/pylsp_mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/pylsp_mypy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/pylsp_mypy/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:59:18.378334 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 13:59:18.000000 pylsp-mypy-0.6.7/pylsp_mypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-03 13:59:18.378334 pylsp-mypy-0.6.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:59:18.378334 pylsp-mypy-0.6.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-06-03 13:59:08.000000 pylsp-mypy-0.6.7/test/test_plugin.py
```

### Comparing `pylsp-mypy-0.6.6/LICENSE` & `pylsp-mypy-0.6.7/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 Copyright (c) 2017 Tom van Ommeren
-Copyright (c) 2022 Richard Kellnberger
+Copyright (c) 2023 Richard Kellnberger
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylsp-mypy-0.6.6/PKG-INFO` & `pylsp-mypy-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pylsp-mypy
-Version: 0.6.6
+Version: 0.6.7
 Summary: Mypy linter for the Python LSP Server
 Home-page: https://github.com/python-lsp/pylsp-mypy
 Author: Richard Kellnberger, Tom van Ommeren
 License: 'MIT'
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 Mypy plugin for PYLSP
 ======================
```

### Comparing `pylsp-mypy-0.6.6/README.rst` & `pylsp-mypy-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `pylsp-mypy-0.6.6/pylsp_mypy/plugin.py` & `pylsp-mypy-0.6.7/pylsp_mypy/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,20 @@
     import tomli as tomllib
 
 from mypy import api as mypy_api
 from pylsp import hookimpl
 from pylsp.config.config import Config
 from pylsp.workspace import Document, Workspace
 
-line_pattern: str = r"((?:^[a-z]:)?[^:]+):(?:(\d+):)?(?:(\d+):)? (\w+): (.*)"
+line_pattern = re.compile(
+    (
+        r"^(?P<file>.+):(?P<start_line>\d+):(?P<start_col>\d*):(?P<end_line>\d*):(?P<end_col>\d*): "
+        r"(?P<severity>\w+): (?P<message>.+?)(?: +\[(?P<code>.+)\])?$"
+    )
+)
 
 log = logging.getLogger(__name__)
 
 # A mapping from workspace path to config file path
 mypyConfigFileMap: Dict[str, Optional[str]] = {}
 
 settingsCache: Dict[str, Dict[str, Any]] = {}
@@ -73,49 +78,46 @@
 
     Returns
     -------
     Optional[Dict[str, Any]]
         The dict with the lint data.
 
     """
-    result = re.match(line_pattern, line)
-    if result:
-        file_path, linenoStr, offsetStr, severity, msg = result.groups()
-
-        if file_path != "<string>":  # live mode
-            # results from other files can be included, but we cannot return
-            # them.
-            if document and document.path and not document.path.endswith(file_path):
-                log.warning("discarding result for %s against %s", file_path, document.path)
-                return None
-
-        lineno = int(linenoStr or 1) - 1  # 0-based line number
-        offset = int(offsetStr or 1) - 1  # 0-based offset
-        errno = 2
-        if severity == "error":
-            errno = 1
-        diag: Dict[str, Any] = {
-            "source": "mypy",
-            "range": {
-                "start": {"line": lineno, "character": offset},
-                # There may be a better solution, but mypy does not provide end
-                "end": {"line": lineno, "character": offset + 1},
-            },
-            "message": msg,
-            "severity": errno,
-        }
-        if document:
-            # although mypy does not provide the end of the affected range, we
-            # can make a good guess by highlighting the word that Mypy flagged
-            word = document.word_at_position(diag["range"]["start"])
-            if word:
-                diag["range"]["end"]["character"] = diag["range"]["start"]["character"] + len(word)
-
-        return diag
-    return None
+    result = line_pattern.match(line)
+    if not result:
+        return None
+
+    file_path = result["file"]
+    if file_path != "<string>":  # live mode
+        # results from other files can be included, but we cannot return
+        # them.
+        if document and document.path and not document.path.endswith(file_path):
+            log.warning("discarding result for %s against %s", file_path, document.path)
+            return None
+
+    lineno = int(result["start_line"]) - 1  # 0-based line number
+    offset = int(result["start_col"]) - 1  # 0-based offset
+    end_lineno = int(result["end_line"]) - 1
+    end_offset = int(result["end_col"])  # end is exclusive
+
+    severity = result["severity"]
+    if severity not in ("error", "note"):
+        log.warning(f"invalid error severity '{severity}'")
+    errno = 1 if severity == "error" else 3
+
+    return {
+        "source": "mypy",
+        "range": {
+            "start": {"line": lineno, "character": offset},
+            "end": {"line": end_lineno, "character": end_offset},
+        },
+        "message": result["message"],
+        "severity": errno,
+        "code": result["code"],
+    }
 
 
 def apply_overrides(args: List[str], overrides: List[Any]) -> List[str]:
     """Replace or combine default command-line options with overrides."""
     overrides_iterator = iter(overrides)
     if True not in overrides_iterator:
         return overrides
@@ -225,22 +227,22 @@
         # https://github.com/python/mypy/issues/9309
         log.warning("live_mode is not supported with dmypy, disabling")
         live_mode = False
 
     if dmypy:
         dmypy_status_file = settings.get("dmypy_status_file", ".dmypy.json")
 
-    args = ["--show-column-numbers"]
+    args = ["--show-error-end", "--no-error-summary"]
 
     global tmpFile
     if live_mode and not is_saved:
         if tmpFile:
-            tmpFile = open(tmpFile.name, "w")
+            tmpFile = open(tmpFile.name, "w", encoding="utf-8")
         else:
-            tmpFile = tempfile.NamedTemporaryFile("w", delete=False)
+            tmpFile = tempfile.NamedTemporaryFile("w", delete=False, encoding="utf-8")
         log.info("live_mode tmpFile = %s", tmpFile.name)
         tmpFile.write(document.source)
         tmpFile.close()
         args.extend(["--shadow-file", document.path, tmpFile.name])
     elif not is_saved and document.path in last_diagnostics:
         # On-launch the document isn't marked as saved, so fall through and run
         # the diagnostics anyway even if the file contents may be out of date.
```

### Comparing `pylsp-mypy-0.6.6/pylsp_mypy.egg-info/PKG-INFO` & `pylsp-mypy-0.6.7/pylsp_mypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pylsp-mypy
-Version: 0.6.6
+Version: 0.6.7
 Summary: Mypy linter for the Python LSP Server
 Home-page: https://github.com/python-lsp/pylsp-mypy
 Author: Richard Kellnberger, Tom van Ommeren
 License: 'MIT'
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 Mypy plugin for PYLSP
 ======================
```

### Comparing `pylsp-mypy-0.6.6/setup.cfg` & `pylsp-mypy-0.6.7/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 	Intended Audience :: Developers
 	Topic :: Software Development
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >= 3.7
 packages = find:
 install_requires = 
 	python-lsp-server >=1.7.0
-	mypy
+	mypy >= 0.981
 	tomli >= 1.1.0 ; python_version < "3.11"
 
 [flake8]
 max-complexity = 20
 max-line-length = 100
 
 [options.entry_points]
```

### Comparing `pylsp-mypy-0.6.6/test/test_plugin.py` & `pylsp-mypy-0.6.7/test/test_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import os
 import subprocess
+import sys
 from pathlib import Path
 from typing import Dict
 from unittest.mock import Mock
 
 import pytest
 from pylsp import _utils, uris
 from pylsp.config.config import Config
@@ -12,19 +13,20 @@
 
 from pylsp_mypy import plugin
 
 # TODO using these file as a document is a bad idea as tests can break by adding new tests
 DOC_URI = f"file:/{Path(__file__)}"
 DOC_TYPE_ERR = """{}.append(3)
 """
-TYPE_ERR_MSG = '"Dict[<nothing>, <nothing>]" has no attribute "append"  [attr-defined]'
+TYPE_ERR_MSG = '"Dict[<nothing>, <nothing>]" has no attribute "append"'
 
-TEST_LINE = 'test_plugin.py:279:8: error: "Request" has no attribute "id"'
-TEST_LINE_WITHOUT_COL = "test_plugin.py:279: " 'error: "Request" has no attribute "id"'
-TEST_LINE_WITHOUT_LINE = "test_plugin.py: " 'error: "Request" has no attribute "id"'
+TEST_LINE = 'test_plugin.py:279:8:279:16: error: "Request" has no attribute "id"  [attr-defined]'
+TEST_LINE_NOTE = (
+    'test_plugin.py:124:1:129:77: note: Use "-> None" if function does not return a value'
+)
 
 windows_flag: Dict[str, int] = (
     {"creationflags": subprocess.CREATE_NO_WINDOW} if os.name == "nt" else {}  # type: ignore
 )
 
 
 @pytest.fixture
@@ -61,57 +63,48 @@
     plugin.pylsp_settings(workspace._config)
     diags = plugin.pylsp_lint(workspace._config, workspace, doc, is_saved=False)
 
     assert len(diags) == 1
     diag = diags[0]
     assert diag["message"] == TYPE_ERR_MSG
     assert diag["range"]["start"] == {"line": 0, "character": 0}
-    assert diag["range"]["end"] == {"line": 0, "character": 1}
+    # Running mypy in 3.7 produces wrong error ends this can be removed when 3.7 reaches EOL
+    if sys.version_info < (3, 8):
+        assert diag["range"]["end"] == {"line": 0, "character": 1}
+    else:
+        assert diag["range"]["end"] == {"line": 0, "character": 9}
+    assert diag["severity"] == 1
+    assert diag["code"] == "attr-defined"
 
 
 def test_parse_full_line(workspace):
     diag = plugin.parse_line(TEST_LINE)  # TODO parse a document here
     assert diag["message"] == '"Request" has no attribute "id"'
     assert diag["range"]["start"] == {"line": 278, "character": 7}
-    assert diag["range"]["end"] == {"line": 278, "character": 8}
-
+    assert diag["range"]["end"] == {"line": 278, "character": 16}
+    assert diag["severity"] == 1
+    assert diag["code"] == "attr-defined"
 
-def test_parse_line_without_col(workspace):
-    doc = Document(DOC_URI, workspace)
-    diag = plugin.parse_line(TEST_LINE_WITHOUT_COL, doc)
-    assert diag["message"] == '"Request" has no attribute "id"'
-    assert diag["range"]["start"] == {"line": 278, "character": 0}
-    assert diag["range"]["end"] == {"line": 278, "character": 1}
 
-
-def test_parse_line_without_line(workspace):
-    doc = Document(DOC_URI, workspace)
-    diag = plugin.parse_line(TEST_LINE_WITHOUT_LINE, doc)
-    assert diag["message"] == '"Request" has no attribute "id"'
-    assert diag["range"]["start"] == {"line": 0, "character": 0}
-    assert diag["range"]["end"] == {"line": 0, "character": 6}
-
-
-@pytest.mark.parametrize("word,bounds", [("", (7, 8)), ("my_var", (7, 13))])
-def test_parse_line_with_context(monkeypatch, word, bounds, workspace):
-    doc = Document(DOC_URI, workspace)
-    monkeypatch.setattr(Document, "word_at_position", lambda *args: word)
-    diag = plugin.parse_line(TEST_LINE, doc)
-    assert diag["message"] == '"Request" has no attribute "id"'
-    assert diag["range"]["start"] == {"line": 278, "character": bounds[0]}
-    assert diag["range"]["end"] == {"line": 278, "character": bounds[1]}
+def test_parse_note_line(workspace):
+    diag = plugin.parse_line(TEST_LINE_NOTE)
+    assert diag["message"] == 'Use "-> None" if function does not return a value'
+    assert diag["range"]["start"] == {"line": 123, "character": 0}
+    assert diag["range"]["end"] == {"line": 128, "character": 77}
+    assert diag["severity"] == 3
+    assert diag["code"] is None
 
 
 def test_multiple_workspaces(tmpdir, last_diagnostics_monkeypatch):
     DOC_SOURCE = """
 def foo():
     return
     unreachable = 1
 """
-    DOC_ERR_MSG = "Statement is unreachable  [unreachable]"
+    DOC_ERR_MSG = "Statement is unreachable"
 
     # Initialize two workspace folders.
     folder1 = tmpdir.mkdir("folder1")
     folder2 = tmpdir.mkdir("folder2")
 
     # Create configuration file for workspace folder 1.
     mypy_config = folder1.join("mypy.ini")
@@ -128,14 +121,15 @@
 
     # Test document in workspace 1 (uses mypy.ini configuration).
     doc1 = Document(DOC_URI, ws1, DOC_SOURCE)
     diags = plugin.pylsp_lint(ws1._config, ws1, doc1, is_saved=False)
     assert len(diags) == 1
     diag = diags[0]
     assert diag["message"] == DOC_ERR_MSG
+    assert diag["code"] == "unreachable"
 
     # Test document in workspace 2 (without mypy.ini configuration)
     doc2 = Document(DOC_URI, ws2, DOC_SOURCE)
     diags = plugin.pylsp_lint(ws2._config, ws2, doc2, is_saved=False)
     assert len(diags) == 0
 
 
@@ -222,15 +216,16 @@
         "dmypy",
         "--status-file",
         ".dmypy.json",
         "run",
         "--",
         "--python-executable",
         "/tmp/fake",
-        "--show-column-numbers",
+        "--show-error-end",
+        "--no-error-summary",
         document.path,
     ]
     m.assert_called_with(expected, capture_output=True, **windows_flag, encoding="utf-8")
 
 
 def test_dmypy_status_file(tmpdir, last_diagnostics_monkeypatch, workspace):
     statusFile = tmpdir / ".custom_dmypy_status_file.json"
@@ -266,15 +261,15 @@
 
 def test_config_sub_paths(tmpdir, last_diagnostics_monkeypatch):
     DOC_SOURCE = """
 def foo():
     return
     unreachable = 1
 """
-    DOC_ERR_MSG = "Statement is unreachable  [unreachable]"
+    DOC_ERR_MSG = "Statement is unreachable"
 
     config_sub_paths = [".config"]
 
     # Create configuration file for workspace.
     plugin_config = tmpdir.join("pyproject.toml")
     plugin_config.write(f"[tool.pylsp-mypy]\nenabled = true\nconfig_sub_paths = {config_sub_paths}")
     config_dir = tmpdir.mkdir(".config")
@@ -292,23 +287,24 @@
 
     # Test document to make sure it uses .config/mypy.ini configuration.
     doc = Document(DOC_URI, ws, DOC_SOURCE)
     diags = plugin.pylsp_lint(ws._config, ws, doc, is_saved=False)
     assert len(diags) == 1
     diag = diags[0]
     assert diag["message"] == DOC_ERR_MSG
+    assert diag["code"] == "unreachable"
 
 
 def test_config_sub_paths_config_changed(tmpdir, last_diagnostics_monkeypatch):
     DOC_SOURCE = """
 def foo():
     return
     unreachable = 1
 """
-    DOC_ERR_MSG = "Statement is unreachable  [unreachable]"
+    DOC_ERR_MSG = "Statement is unreachable"
 
     # Create configuration file for workspace.
     config_dir = tmpdir.mkdir(".config")
     mypy_config = config_dir.join("mypy.ini")
     mypy_config.write("[mypy]\nwarn_unreachable = True\ncheck_untyped_defs = True")
 
     config_sub_paths = [".config"]
@@ -323,7 +319,8 @@
 
     # Test document to make sure it uses .config/mypy.ini configuration.
     doc = Document(DOC_URI, ws, DOC_SOURCE)
     diags = plugin.pylsp_lint(ws._config, ws, doc, is_saved=False)
     assert len(diags) == 1
     diag = diags[0]
     assert diag["message"] == DOC_ERR_MSG
+    assert diag["code"] == "unreachable"
```

