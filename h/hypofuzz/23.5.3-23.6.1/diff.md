# Comparing `tmp/hypofuzz-23.5.3.tar.gz` & `tmp/hypofuzz-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-23.5.3.tar", last modified: Mon May 22 21:36:05 2023, max compression
+gzip compressed data, was "hypofuzz-23.6.1.tar", last modified: Sat Jun  3 19:00:44 2023, max compression
```

## Comparing `hypofuzz-23.5.3.tar` & `hypofuzz-23.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.910917 hypofuzz-23.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_coverage_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_fuzz_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.003682 hypofuzz-23.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.011682 hypofuzz-23.6.1/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.011682 hypofuzz-23.6.1/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_version.py
```

### Comparing `hypofuzz-23.5.3/LICENSE` & `hypofuzz-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/PKG-INFO` & `hypofuzz-23.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.3
+Version: 23.6.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.3/README.md` & `hypofuzz-23.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/setup.py` & `hypofuzz-23.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,19 @@
         "Documentation": "https://hypofuzz.com/docs/",
         "Changelog": "https://hypofuzz.com/docs/changelog.html",
     },
     license="AGPL-3.0",
     description="Adaptive fuzzing for property-based tests",
     zip_safe=False,
     install_requires=[
+        "black >= 23.3.0",
         "coverage >= 5.2.1",
         "dash >= 2.0.0",
-        "hypothesis[cli] >= 6.75.2",
+        "hypothesis[cli] >= 6.75.7",
+        "libcst >= 1.0.0",
         "pandas >= 1.0.0",
         "psutil >= 3.0.0",
         "pytest >= 6.0.1",
         "requests >= 2.24.0",
     ],
     extras_require={
         "pytrace": [
```

### Comparing `hypofuzz-23.5.3/src/hypofuzz/corpus.py` & `hypofuzz-23.6.1/src/hypofuzz/corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/src/hypofuzz/cov.py` & `hypofuzz-23.6.1/src/hypofuzz/cov.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/src/hypofuzz/dashboard.py` & `hypofuzz-23.6.1/src/hypofuzz/dashboard.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """Live web dashboard for a fuzzing run."""
+import atexit
 import datetime
 import os
+import signal
 from typing import List, Tuple
 
 import black
 import dash
 import flask
 import plotly.express as px
 import plotly.graph_objects as go
 from dash import dcc, html
 from dash.dependencies import Input, Output
+from hypothesis.configuration import storage_directory
+
+from .patching import make_and_save_patches
 
 DATA_TO_PLOT = [{"nodeid": "", "elapsed_time": 0, "ninputs": 0, "branches": 0}]
 LAST_UPDATE: dict = {}
 
+PYTEST_ARGS = None
+
 headings = ["nodeid", "elapsed time", "ninputs", "since new cov", "branches", "note"]
 app = flask.Flask(__name__, static_folder=os.path.abspath("pycrunch-recordings"))
 
 try:
     import flask_cors
     from pycrunch_trace.oop.safe_filename import SafeFilename
 except ImportError:
@@ -93,14 +100,20 @@
     # Main page
     if pathname == "/" or pathname is None:
         return html.Div(
             children=[
                 html.Div("Total branch coverage for each test."),
                 dcc.Graph(id="live-update-graph"),
                 html.Button("Toggle log-xaxis", id="xaxis-state", n_clicks=0),
+                html.Div(
+                    dcc.Link(
+                        "See patches with covering and/or failing examples",
+                        href="/patches/",
+                    )
+                ),
                 html.Div(html.Table(id="summary-table-rows")),
                 html.Div("Estimated number of inputs to discover new coverage or bugs"),
                 html.Div(html.Table(id="estimators-table-rows")),
             ]
         )
 
     # Target-specific subpages
@@ -260,17 +273,76 @@
     return contents
 
 
 @app.route("/pycrunch-recordings/<path:name>")  # type: ignore
 def download_file(name: str) -> flask.Response:
     return flask.send_from_directory(
         directory="pycrunch-recordings",
-        filename=name,
+        path=name,
+        mimetype="application/octet-stream",
+    )
+
+
+@app.route("/patches/<path:name>")  # type: ignore
+def download_patch(name: str) -> flask.Response:
+    return flask.send_from_directory(
+        directory=os.path.relpath(storage_directory("patches"), app.root_path),
+        path=name,
         mimetype="application/octet-stream",
     )
 
 
+@app.route("/patches/")  # type: ignore
+def patch_summary() -> flask.Response:
+    patches = make_and_save_patches(PYTEST_ARGS, LAST_UPDATE)
+    if not patches:
+        return """<html>
+    <head><title>HypoFuzz patches</title><meta charset="utf-8"/></head>
+    <body style="font-family: Sans-Serif">
+        Waiting for examples, please refresh the page in minute or so.
+    </body></html>"""
+    show = "fail"
+    if show not in patches:
+        show = "cov"
+    patch_path = patches[show]
+    describe = {"fail": "failing", "cov": "covering", "all": "covering and failing"}
+    links = "\n".join(
+        f'<li><a href="/patches/{patches[k].name}">patch with {v} examples</a></li>'
+        for k, v in describe.items()
+        if k in patches
+    )
+    return f"""<html>
+    <head>
+        <title>HypoFuzz patches</title>
+        <meta charset="utf-8" />
+        <link rel="stylesheet" type="text/css" href="/assets/prism.css" />
+        <script src="/assets/prism.js"></script>
+    </head>
+    <body style="font-family: Sans-Serif">
+        <h2>Download links</h2>
+        <ul>{links}</ul>
+        <h2>Latest {describe[show]} patch</h2>
+        <pre class="language-diff-python diff-highlight"><code>{patch_path.read_text()}</code></pre>
+    </body>
+    </html>"""
+
+
 def start_dashboard_process(
-    port: int, *, host: str = "localhost", debug: bool = False
+    port: int, *, pytest_args: list, host: str = "localhost", debug: bool = False
 ) -> None:
+    global PYTEST_ARGS
+    PYTEST_ARGS = pytest_args
+
+    # Ensure that we dump whatever patches are ready before shutting down
+    def signal_handler(signum, frame):  # type: ignore
+        make_and_save_patches(pytest_args, LAST_UPDATE)
+        if old_handler in (signal.SIG_DFL, None):
+            return old_handler
+        elif old_handler is not signal.SIG_IGN:
+            return old_handler(signum, frame)
+        raise NotImplementedError("Unreachable")
+
+    old_handler = signal.signal(signal.SIGTERM, signal_handler)
+    atexit.register(make_and_save_patches, pytest_args, LAST_UPDATE)
+
     print(f"\n\tNow serving dashboard at  http://{host}:{port}/\n")  # noqa
     app.run(host=host, port=port, debug=debug)
```

### Comparing `hypofuzz-23.5.3/src/hypofuzz/debugger.py` & `hypofuzz-23.6.1/src/hypofuzz/debugger.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/src/hypofuzz/entrypoint.py` & `hypofuzz-23.6.1/src/hypofuzz/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,18 @@
 
     testnames = "\n    ".join(t.nodeid for t in tests)
     print(f"using up to {numprocesses} processes to fuzz:\n    {testnames}\n")  # noqa
 
     if dashboard:
         from .dashboard import start_dashboard_process
 
-        Process(target=start_dashboard_process, kwargs={"port": port}).start()
+        Process(
+            target=start_dashboard_process,
+            kwargs={"port": port, "pytest_args": pytest_args},
+        ).start()
 
     processes = []
     for i in range(numprocesses):
         nodes = {t.nodeid for t in (tests if unsafe else tests[i::numprocesses])}
         p = Process(
             target=_fuzz_several,
             kwargs={"pytest_args": pytest_args, "nodeids": nodes, "port": port},
```

### Comparing `hypofuzz-23.5.3/src/hypofuzz/hy.py` & `hypofuzz-23.6.1/src/hypofuzz/hy.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         nodeid: Optional[str] = None,
         database_key: bytes,
         hypothesis_database: ExampleDatabase,
     ) -> None:
         """Construct a FuzzProcess from specific arguments."""
         # The actual fuzzer implementation
         self.random = Random(random_seed)
-        self.__test_fn = test_fn
+        self._test_fn = test_fn
         self.__stuff = stuff
         self.nodeid = nodeid or test_fn.__qualname__
 
         # The seed pool is responsible for managing all seed state, including saving
         # novel seeds to the database.  This includes tracking how often each branch
         # has been hit, minimal covering examples, and so on.
         self.pool = Pool(hypothesis_database, database_key)
@@ -276,28 +276,28 @@
                         (), self.__stuff.given_kwargs
                     )
                     assert not a, "strategies all moved to kwargs by now"
                     kwargs.update(kw)
 
                     printer = RepresentationPrinter(context=context)
                     printer.repr_call(
-                        self.__test_fn.__name__,
+                        self._test_fn.__name__,
                         args,
                         kwargs,
                         force_split=True,
                         arg_slices=argslices,
                         leading_comment=(
                             "# " + context.data.slice_comments[(0, 0)]
                             if (0, 0) in context.data.slice_comments
                             else None
                         ),
                     )
                     data.extra_information.call_repr = printer.getvalue()
 
-                    self.__test_fn(*args, **kwargs)
+                    self._test_fn(*args, **kwargs)
         except StopTest:
             data.status = Status.OVERRUN
         except UnsatisfiedAssumption:
             data.status = Status.INVALID
         except failure_exceptions_to_catch() as e:
             data.status = Status.INTERESTING
             tb = get_trimmed_traceback()
```

### Comparing `hypofuzz-23.5.3/src/hypofuzz/interface.py` & `hypofuzz-23.6.1/src/hypofuzz/interface.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.6.1/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.3
+Version: 23.6.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.3/src/hypofuzz.egg-info/SOURCES.txt` & `hypofuzz-23.6.1/src/hypofuzz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/hypofuzz/corpus.py
 src/hypofuzz/cov.py
 src/hypofuzz/dashboard.py
 src/hypofuzz/debugger.py
 src/hypofuzz/entrypoint.py
 src/hypofuzz/hy.py
 src/hypofuzz/interface.py
+src/hypofuzz/patching.py
 src/hypofuzz/py.typed
 src/hypofuzz.egg-info/PKG-INFO
 src/hypofuzz.egg-info/SOURCES.txt
 src/hypofuzz.egg-info/dependency_links.txt
 src/hypofuzz.egg-info/entry_points.txt
 src/hypofuzz.egg-info/not-zip-safe
 src/hypofuzz.egg-info/requires.txt
```

### Comparing `hypofuzz-23.5.3/tests/test_corpus.py` & `hypofuzz-23.6.1/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/tests/test_fuzz_process.py` & `hypofuzz-23.6.1/tests/test_fuzz_process.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.3/tests/test_version.py` & `hypofuzz-23.6.1/tests/test_version.py`

 * *Files identical despite different names*

