# Comparing `tmp/vscode_task_runner-0.1.5.tar.gz` & `tmp/vscode_task_runner-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vscode_task_runner-0.1.5.tar", max compression
+gzip compressed data, was "vscode_task_runner-0.1.6.tar", max compression
```

## Comparing `vscode_task_runner-0.1.5.tar` & `vscode_task_runner-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/LICENSE
--rw-r--r--   0        0        0     7679 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/README.md
--rw-r--r--   0        0        0     1331 2023-05-31 23:04:21.629002 vscode_task_runner-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/__init__.py
--rw-r--r--   0        0        0       39 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/__main__.py
--rw-r--r--   0        0        0     2780 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/console.py
--rw-r--r--   0        0        0     1557 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/constants.py
--rw-r--r--   0        0        0     1199 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/executor.py
--rw-r--r--   0        0        0     3981 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/helpers.py
--rw-r--r--   0        0        0     1842 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/json_parser.py
--rw-r--r--   0        0        0     1489 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/models.py
--rw-r--r--   0        0        0     9315 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/task.py
--rw-r--r--   0        0        0     7523 2023-05-31 23:04:21.633002 vscode_task_runner-0.1.5/vtr/terminal_task_system.py
--rw-r--r--   0        0        0     8749 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 00:08:29.810838 vscode_task_runner-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7650 2023-06-03 00:08:29.810838 vscode_task_runner-0.1.6/README.md
+-rw-r--r--   0        0        0     1331 2023-06-03 00:08:29.814838 vscode_task_runner-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 00:08:29.814838 vscode_task_runner-0.1.6/vtr/__init__.py
+-rw-r--r--   0        0        0       39 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/__main__.py
+-rw-r--r--   0        0        0     2488 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/console.py
+-rw-r--r--   0        0        0     1557 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/constants.py
+-rw-r--r--   0        0        0     1199 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/executor.py
+-rw-r--r--   0        0        0     3981 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/helpers.py
+-rw-r--r--   0        0        0     1842 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/json_parser.py
+-rw-r--r--   0        0        0     1489 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/models.py
+-rw-r--r--   0        0        0     9315 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/task.py
+-rw-r--r--   0        0        0     7523 2023-06-03 00:08:29.818838 vscode_task_runner-0.1.6/vtr/terminal_task_system.py
+-rw-r--r--   0        0        0     8720 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.6/PKG-INFO
```

### Comparing `vscode_task_runner-0.1.5/LICENSE` & `vscode_task_runner-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/README.md` & `vscode_task_runner-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ```
 
 Additionally, for convenience, extra arguments can be tacked on to a task.
 For example, you can add extra settings or overrides when running in CI/CD.
 Continuing the example above:
 
 ```bash
-$ vtr pre-commit --extra-args="--color=always" --extra-args="--show-diff-on-failure"
+$ vtr pre-commit --color=always --show-diff-on-failure
 [1/1] Executing task "pre-commit": C:\Program Files\WindowsApps\Microsoft.PowerShell_7.3.4.0_x64__8wekyb3d8bbwe\pwsh.exe -Command poetry run pre-commit run --all-files --color=always --show-diff-on-failure
 check json...............................................................Passed
 check toml...............................................................Passed
 check yaml...............................................................Passed
 check for case conflicts.................................................Passed
 trim trailing whitespace.................................................Passed
 check for merge conflicts................................................Passed
@@ -135,15 +135,15 @@
 ```
 
 You can also use it as a [pre-commit](https://pre-commit.com) hook if desired:
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
-    rev: v0.1.3
+    rev: v0.1.6
     hooks:
       - id: vtr
         # Optionally override the hook name here
         # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
@@ -196,8 +196,8 @@
 
 - If a task is of type `"shell"`, and a specific shell is not defined, the parent
   shell will be used
 - Only schema version 2.0.0 is supported
 - If no `cwd` is specified, the current working directory is used for the task instead
 - Does not support any extensions that add extra options/functionality
 - Does not load any VS Code settings
-- `--extra-args` option
+- Extra arguments option
```

### Comparing `vscode_task_runner-0.1.5/pyproject.toml` & `vscode_task_runner-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "vscode-task-runner"
-    version = "0.1.5"
+    version = "0.1.6"
     description = "Task runner for VS Code tasks.json"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/vscode-task-runner"
     repository = "https://github.com/NathanVaughn/vscode-task-runner.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
```

### Comparing `vscode_task_runner-0.1.5/vtr/console.py` & `vscode_task_runner-0.1.6/vtr/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import itertools
 import os
 from typing import Dict
 
 import vtr.executor
 import vtr.json_parser
 from vtr.task import Task
 
@@ -23,59 +22,52 @@
     except FileNotFoundError:
         all_tasks = {}
         task_label_help_text += (
             " Invoke this command inside a directory with a"
             + f" {os.path.join('.vscode', 'tasks.json')} file to see and run tasks."
         )
 
-    parser = argparse.ArgumentParser(description="VS Code Task Runner")
-    parser.add_argument(
-        "task_labels",
-        nargs="+",
-        choices=all_tasks.keys(),
-        help=task_label_help_text,
-    )
-    parser.add_argument(
-        "--extra-args",
-        nargs="*",
-        action="append",
-        default=[],
-        help="When running a single task, extra args to append to that task."
+    parser = argparse.ArgumentParser(
+        description="VS Code Task Runner",
+        epilog="When running a single task, extra args can be appended only to that task."
         + " If a single task is requested, but has dependent tasks, only the top-level"
         + " task will be given the extra arguments."
         + ' If the task is a "process" type, then this will be added to "args".'
         + ' If the task is a "shell" type with only a "command" then this will'
         + " be tacked on to the end and joined by spaces."
         + ' If the task is a "shell" type with '
         + ' a "command" and "args", then this will be appended to "args".',
     )
-    args = parser.parse_args()
+    parser.add_argument(
+        "task_labels",
+        nargs="+",
+        choices=all_tasks.keys(),
+        help=task_label_help_text,
+    )
 
-    # the append action makes it come in as a list, but it's the only way
-    # to allow multiple --extra-args= flags work
-    args.extra_args = list(itertools.chain.from_iterable(args.extra_args))
+    args, extra_args = parser.parse_known_args()
 
-    if len(args.task_labels) > 1 and args.extra_args:
+    if len(args.task_labels) > 1 and extra_args:
         parser.error("Extra arguments can only be used with a single task.")
 
     # filter to tasks explicitly asked for
     top_level_tasks = [all_tasks[t] for t in args.task_labels]
 
     # get all tasks, following dependencies
     tasks_to_execute = []
     for task in top_level_tasks:
         tasks_to_execute.extend(vtr.executor.collect_task(task))
 
     # start executing
     for i, task in enumerate(tasks_to_execute):
-        extra_args = []
+        i_extra_args = []
         # top-level task will always be the last one
         if i + 1 == len(tasks_to_execute):
-            extra_args = args.extra_args
+            i_extra_args = extra_args
 
         vtr.executor.execute_task(
-            task, index=i + 1, total=len(tasks_to_execute), extra_args=extra_args
+            task, index=i + 1, total=len(tasks_to_execute), extra_args=i_extra_args
         )
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `vscode_task_runner-0.1.5/vtr/constants.py` & `vscode_task_runner-0.1.6/vtr/constants.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/executor.py` & `vscode_task_runner-0.1.6/vtr/executor.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/helpers.py` & `vscode_task_runner-0.1.6/vtr/helpers.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/json_parser.py` & `vscode_task_runner-0.1.6/vtr/json_parser.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/models.py` & `vscode_task_runner-0.1.6/vtr/models.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/task.py` & `vscode_task_runner-0.1.6/vtr/task.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/vtr/terminal_task_system.py` & `vscode_task_runner-0.1.6/vtr/terminal_task_system.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.5/PKG-INFO` & `vscode_task_runner-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vscode-task-runner
-Version: 0.1.5
+Version: 0.1.6
 Summary: Task runner for VS Code tasks.json
 Home-page: https://github.com/NathanVaughn/vscode-task-runner
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -97,15 +97,15 @@
 ```
 
 Additionally, for convenience, extra arguments can be tacked on to a task.
 For example, you can add extra settings or overrides when running in CI/CD.
 Continuing the example above:
 
 ```bash
-$ vtr pre-commit --extra-args="--color=always" --extra-args="--show-diff-on-failure"
+$ vtr pre-commit --color=always --show-diff-on-failure
 [1/1] Executing task "pre-commit": C:\Program Files\WindowsApps\Microsoft.PowerShell_7.3.4.0_x64__8wekyb3d8bbwe\pwsh.exe -Command poetry run pre-commit run --all-files --color=always --show-diff-on-failure
 check json...............................................................Passed
 check toml...............................................................Passed
 check yaml...............................................................Passed
 check for case conflicts.................................................Passed
 trim trailing whitespace.................................................Passed
 check for merge conflicts................................................Passed
@@ -160,15 +160,15 @@
 ```
 
 You can also use it as a [pre-commit](https://pre-commit.com) hook if desired:
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
-    rev: v0.1.3
+    rev: v0.1.6
     hooks:
       - id: vtr
         # Optionally override the hook name here
         # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
@@ -221,9 +221,9 @@
 
 - If a task is of type `"shell"`, and a specific shell is not defined, the parent
   shell will be used
 - Only schema version 2.0.0 is supported
 - If no `cwd` is specified, the current working directory is used for the task instead
 - Does not support any extensions that add extra options/functionality
 - Does not load any VS Code settings
-- `--extra-args` option
+- Extra arguments option
```

