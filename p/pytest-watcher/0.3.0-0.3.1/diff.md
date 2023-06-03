# Comparing `tmp/pytest-watcher-0.3.0.tar.gz` & `tmp/pytest-watcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-watcher-0.3.0.tar", max compression
+gzip compressed data, was "pytest-watcher-0.3.1.tar", max compression
```

## Comparing `pytest-watcher-0.3.0.tar` & `pytest-watcher-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-10-19 14:45:40.729543 pytest-watcher-0.3.0/LICENSE
--rw-r--r--   0        0        0     3318 2023-06-02 23:06:45.106513 pytest-watcher-0.3.0/README.md
--rw-r--r--   0        0        0     1563 2023-06-02 23:17:38.128731 pytest-watcher-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-06-02 23:15:11.891180 pytest-watcher-0.3.0/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2022-10-19 14:45:40.730627 pytest-watcher-0.3.0/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     4655 2023-06-02 23:07:08.404121 pytest-watcher-0.3.0/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     4300 2023-06-02 23:21:11.185308 pytest-watcher-0.3.0/setup.py
--rw-r--r--   0        0        0     4366 2023-06-02 23:21:11.185496 pytest-watcher-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-19 14:45:40.729543 pytest-watcher-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3330 2023-06-03 11:43:02.936615 pytest-watcher-0.3.1/README.md
+-rw-r--r--   0        0        0     1563 2023-06-03 13:13:33.406945 pytest-watcher-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-03 12:47:15.872901 pytest-watcher-0.3.1/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2022-10-19 14:45:40.730627 pytest-watcher-0.3.1/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     5043 2023-06-03 13:11:24.681213 pytest-watcher-0.3.1/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     4312 2023-06-03 13:14:04.349757 pytest-watcher-0.3.1/setup.py
+-rw-r--r--   0        0        0     4378 2023-06-03 13:14:04.349935 pytest-watcher-0.3.1/PKG-INFO
```

### Comparing `pytest-watcher-0.3.0/LICENSE` & `pytest-watcher-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-watcher-0.3.0/README.md` & `pytest-watcher-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ## Motivation
 
 ### Why not general tools (e.g. `watchmedo`, `entr`)?
 
 - Easy to use and remember
 - Works for most python projects out of the box
 - Minimum dependencies (`watchdog` is the only one)
-- Handles post-processing properly (see delay)
+- Handles post-processing properly (see [delay](#delay))
 
 ### What about pytest-watch?
 
 [pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.
 
 ## File events
 
@@ -84,15 +84,15 @@
 
 ```sh
 ptw . --runner tox
 ```
 
 ## Watching different patterns
 
-You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a colon. The default value is "\*.py".
+You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py".
 
 Example:
 
 ```sh
 ptw . --patterns '*.py,pyproject.toml'
 ```
 
@@ -100,15 +100,15 @@
 
 ```sh
 ptw . --ignore-patterns 'settings.py,db.py'
 ```
 
 ## Delay
 
-`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., black plugin in your IDE). This ensures that tests will be run with the latest version of your code.
+`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.
 
 You can control the actual delay value with the `--delay` flag:
 
 `ptw . --delay 0.2`
 
 To disable the delay altogether, you can provide zero as a value:
```

### Comparing `pytest-watcher-0.3.0/pyproject.toml` & `pytest-watcher-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-watcher"
-version = "0.3.0"
+version = "0.3.1"
 description = "Automatically rerun your tests on file modifications"
 authors = ["Olzhas Arystanov <o.arystanov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/olzhasar/pytest-watcher"
 repository = "https://github.com/olzhasar/pytest-watcher"
 keywords = ["pytest", "watch", "watcher"]
```

### Comparing `pytest-watcher-0.3.0/pytest_watcher/watcher.py` & `pytest-watcher-0.3.1/pytest_watcher/watcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from pathlib import Path
 from typing import List, Sequence
 
 from watchdog import events
 from watchdog.observers import Observer
 from watchdog.utils.patterns import match_any_paths
 
+VERSION = "0.3.1"
 DEFAULT_DELAY = 0.2
 
 trigger_lock = threading.Lock()
 trigger = None
 
 
+logging.basicConfig(level=logging.INFO, format="[ptw] %(message)s")
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ParsedArguments:
     path: Path
     now: bool
@@ -74,15 +76,15 @@
             paths.append(event.dest_path)
 
         return match_any_paths(paths, self.patterns, self.ignore_patterns)
 
     def dispatch(self, event: events.FileSystemEvent) -> None:
         if self._is_event_watched(event):
             emit_trigger()
-            logger.debug(f"TRIGGERED event: {event.event_type} src: {event.src_path}")
+            logger.info(f"{event.src_path} {event.event_type}")
         else:
             logger.debug(f"IGNORED event: {event.event_type} src: {event.src_path}")
 
 
 def _invoke_runner(runner: str, args: Sequence[str]) -> None:
     subprocess.run([runner, *args])
 
@@ -91,44 +93,45 @@
     return arg.split(",")
 
 
 def _parse_arguments(args: Sequence[str]) -> ParsedArguments:
     parser = argparse.ArgumentParser(
         prog="pytest_watcher",
         description="""
-            Watch <path> for file changes in Python projects and run pytest
-            if such change is detected.\n
-            Any additional arguments will be passed to pytest directly
+            Watch the <path> for file changes and trigger the test runner (pytest).\n
+            Additional arguments are passed directly to the test runner.
         """,
     )
-    parser.add_argument("path", type=Path, help="path to watch")
-    parser.add_argument("--now", action="store_true", help="Run pytest instantly")
+    parser.add_argument("path", type=Path, help="The path to watch for file changes.")
+    parser.add_argument(
+        "--now", action="store_true", help="Trigger the test run immediately"
+    )
     parser.add_argument(
         "--delay",
         type=float,
         default=DEFAULT_DELAY,
-        help=f"Watcher delay in seconds (default DEFAULT_DELAY)",
+        help=f"The delay (in seconds) before triggering the test run (default: {DEFAULT_DELAY})",
     )
     parser.add_argument(
         "--runner",
         type=str,
         default="pytest",
-        help="Use another executable to run the tests.",
+        help="Specify the executable for running the tests (default: pytest)",
     )
     parser.add_argument(
         "--patterns",
         default=["*.py"],
         type=_parse_patterns,
-        help="Comma-separated Unix shell-style wildcard patterns list (default: '*.py')",
+        help="File patterns to watch, specified as comma-separated Unix-style patterns (default: '*.py')",
     )
     parser.add_argument(
         "--ignore-patterns",
         default=[],
         type=_parse_patterns,
-        help="Comma-separated Unix shell-style wildcard ignore patterns list (default: '')",
+        help="File patterns to ignore, specified as comma-separated Unix-style patterns (default: '')",
     )
 
     namespace, runner_args = parser.parse_known_args(args)
 
     return ParsedArguments(
         path=namespace.path,
         now=namespace.now,
@@ -161,14 +164,18 @@
     )
 
     observer = Observer()
 
     observer.schedule(event_handler, args.path, recursive=True)
     observer.start()
 
+    sys.stdout.write(f"pytest-watcher version {VERSION}\n")
+    sys.stdout.write(f"Runner command: {args.runner} {' '.join(args.runner_args)}\n")
+    sys.stdout.write(f"Waiting for file changes in {args.path.absolute()}\n")
+
     if args.now:
         emit_trigger()
 
     try:
         while True:
             _run_main_loop(
                 runner=args.runner, runner_args=args.runner_args, delay=args.delay
```

### Comparing `pytest-watcher-0.3.0/setup.py` & `pytest-watcher-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['ptw = pytest_watcher:run',
                      'pytest-watcher = pytest_watcher:run']}
 
 setup_kwargs = {
     'name': 'pytest-watcher',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Automatically rerun your tests on file modifications',
-    'long_description': '# A simple watcher for pytest\n\n[![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)\n\n## Overview\n\n**pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.\n\nWorks on Unix (Linux, MacOS, BSD) and Windows.\n\n## Table of Contents\n\n- [Motivation](#motivation)\n- [File Events](#file-events)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Using a different test runner](#using-a-different-test-runner)\n- [Watching different patterns](#watching-different-patterns)\n- [Delay](#delay)\n- [Compatibility](#compatibility)\n- [License](#license)\n\n## Motivation\n\n### Why not general tools (e.g. `watchmedo`, `entr`)?\n\n- Easy to use and remember\n- Works for most python projects out of the box\n- Minimum dependencies (`watchdog` is the only one)\n- Handles post-processing properly (see delay)\n\n### What about pytest-watch?\n\n[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.\n\n## File events\n\nBy default `pytest-watcher` looks for the following events:\n\n- New `*.py` file created\n- Existing `*.py` file modified\n- Existing `*.py` file deleted\n- A `*.py` file moved either from or to the watched path\n\nYou can specify alternative file patterns to watch. See [Watching different patterns](#watching-different-patterns)\n\n## Installation\n\n```sh\npip install pytest-watcher\n```\n\n## Usage\n\nSpecify the path that you want to monitor:\n\n```sh\nptw .\n```\n\nor\n\n```sh\nptw /home/repos/project\n```\n\nAny arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:\n\n```sh\nptw . -x --lf --nf\n```\n\nwill call `pytest` with the following arguments:\n\n```sh\npytest -x --lf --nf\n```\n\n## Using a different test runner\n\nYou can specify an alternative test runner using the `--runner` flag:\n\n```sh\nptw . --runner tox\n```\n\n## Watching different patterns\n\nYou can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a colon. The default value is "\\*.py".\n\nExample:\n\n```sh\nptw . --patterns \'*.py,pyproject.toml\'\n```\n\nYou can also **ignore** certain patterns using the `--ignore-patterns` flag:\n\n```sh\nptw . --ignore-patterns \'settings.py,db.py\'\n```\n\n## Delay\n\n`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., black plugin in your IDE). This ensures that tests will be run with the latest version of your code.\n\nYou can control the actual delay value with the `--delay` flag:\n\n`ptw . --delay 0.2`\n\nTo disable the delay altogether, you can provide zero as a value:\n\n`ptw . --delay 0`\n\n## Compatibility\n\nThe code is tested for Python versions 3.7+\n\n## License\n\nThis project is licensed under the [MIT License](LICENSE).\n',
+    'long_description': '# A simple watcher for pytest\n\n[![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)\n\n## Overview\n\n**pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.\n\nWorks on Unix (Linux, MacOS, BSD) and Windows.\n\n## Table of Contents\n\n- [Motivation](#motivation)\n- [File Events](#file-events)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Using a different test runner](#using-a-different-test-runner)\n- [Watching different patterns](#watching-different-patterns)\n- [Delay](#delay)\n- [Compatibility](#compatibility)\n- [License](#license)\n\n## Motivation\n\n### Why not general tools (e.g. `watchmedo`, `entr`)?\n\n- Easy to use and remember\n- Works for most python projects out of the box\n- Minimum dependencies (`watchdog` is the only one)\n- Handles post-processing properly (see [delay](#delay))\n\n### What about pytest-watch?\n\n[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.\n\n## File events\n\nBy default `pytest-watcher` looks for the following events:\n\n- New `*.py` file created\n- Existing `*.py` file modified\n- Existing `*.py` file deleted\n- A `*.py` file moved either from or to the watched path\n\nYou can specify alternative file patterns to watch. See [Watching different patterns](#watching-different-patterns)\n\n## Installation\n\n```sh\npip install pytest-watcher\n```\n\n## Usage\n\nSpecify the path that you want to monitor:\n\n```sh\nptw .\n```\n\nor\n\n```sh\nptw /home/repos/project\n```\n\nAny arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:\n\n```sh\nptw . -x --lf --nf\n```\n\nwill call `pytest` with the following arguments:\n\n```sh\npytest -x --lf --nf\n```\n\n## Using a different test runner\n\nYou can specify an alternative test runner using the `--runner` flag:\n\n```sh\nptw . --runner tox\n```\n\n## Watching different patterns\n\nYou can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\\*.py".\n\nExample:\n\n```sh\nptw . --patterns \'*.py,pyproject.toml\'\n```\n\nYou can also **ignore** certain patterns using the `--ignore-patterns` flag:\n\n```sh\nptw . --ignore-patterns \'settings.py,db.py\'\n```\n\n## Delay\n\n`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.\n\nYou can control the actual delay value with the `--delay` flag:\n\n`ptw . --delay 0.2`\n\nTo disable the delay altogether, you can provide zero as a value:\n\n`ptw . --delay 0`\n\n## Compatibility\n\nThe code is tested for Python versions 3.7+\n\n## License\n\nThis project is licensed under the [MIT License](LICENSE).\n',
     'author': 'Olzhas Arystanov',
     'author_email': 'o.arystanov@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/olzhasar/pytest-watcher',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pytest-watcher-0.3.0/PKG-INFO` & `pytest-watcher-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-watcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: Automatically rerun your tests on file modifications
 Home-page: https://github.com/olzhasar/pytest-watcher
 License: MIT
 Keywords: pytest,watch,watcher
 Author: Olzhas Arystanov
 Author-email: o.arystanov@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -52,15 +52,15 @@
 ## Motivation
 
 ### Why not general tools (e.g. `watchmedo`, `entr`)?
 
 - Easy to use and remember
 - Works for most python projects out of the box
 - Minimum dependencies (`watchdog` is the only one)
-- Handles post-processing properly (see delay)
+- Handles post-processing properly (see [delay](#delay))
 
 ### What about pytest-watch?
 
 [pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.
 
 ## File events
 
@@ -111,15 +111,15 @@
 
 ```sh
 ptw . --runner tox
 ```
 
 ## Watching different patterns
 
-You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a colon. The default value is "\*.py".
+You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py".
 
 Example:
 
 ```sh
 ptw . --patterns '*.py,pyproject.toml'
 ```
 
@@ -127,15 +127,15 @@
 
 ```sh
 ptw . --ignore-patterns 'settings.py,db.py'
 ```
 
 ## Delay
 
-`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., black plugin in your IDE). This ensures that tests will be run with the latest version of your code.
+`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.
 
 You can control the actual delay value with the `--delay` flag:
 
 `ptw . --delay 0.2`
 
 To disable the delay altogether, you can provide zero as a value:
```

