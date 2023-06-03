# Comparing `tmp/motion_python-0.1.53.tar.gz` & `tmp/motion_python-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.53.tar", max compression
+gzip compressed data, was "motion_python-0.1.54.tar", max compression
```

## Comparing `motion_python-0.1.53.tar` & `motion_python-0.1.54.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-02 23:34:06.476208 motion_python-0.1.53/README.md
--rw-r--r--   0        0        0      202 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/component.py
--rw-r--r--   0        0        0    14780 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/execute.py
--rw-r--r--   0        0        0     5182 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/fit_task.py
--rw-r--r--   0        0        0    10503 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/utils.py
--rw-r--r--   0        0        0     1555 2023-06-02 23:34:31.620453 motion_python-0.1.53/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.53/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-03 00:01:31.175881 motion_python-0.1.54/README.md
+-rw-r--r--   0        0        0      202 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/component.py
+-rw-r--r--   0        0        0    14780 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/execute.py
+-rw-r--r--   0        0        0     5209 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/fit_task.py
+-rw-r--r--   0        0        0    10437 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/utils.py
+-rw-r--r--   0        0        0     1555 2023-06-03 00:01:55.879995 motion_python-0.1.54/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.54/PKG-INFO
```

### Comparing `motion_python-0.1.53/README.md` & `motion_python-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/cli.py` & `motion_python-0.1.54/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/component.py` & `motion_python-0.1.54/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/execute.py` & `motion_python-0.1.54/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/fit_task.py` & `motion_python-0.1.54/motion/fit_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         # Keep track of batch
         self.batch: List[Any] = []
 
         # Register the stop event
         # self.running = True
         # self.stop_event = stop_event
         self.running = running
+        self.daemon = True
 
     # def handle_signal(self, signum: int, frame: Any) -> None:
     #     logger.info("Received shutdown signal.")
     #     self.running = False
 
     def run(self) -> None:
         redis_con = redis.Redis(
```

### Comparing `motion_python-0.1.53/motion/instance.py` & `motion_python-0.1.54/motion/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,15 @@
     def instance_name(self) -> str:
         """Component name with a random phrase to represent
         the name of this instance."""
         return self._instance_name
 
     def shutdown(self) -> None:
         """Shuts down a Motion component instance, saving state.
-
-        Warning: if you don't shutdown a component instance when you are
-        finished using it, your program may infinitely hang!
+        Automatically called when the instance is garbage collected.
 
         Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
```

### Comparing `motion_python-0.1.53/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.54/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/route.py` & `motion_python-0.1.54/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/motion/utils.py` & `motion_python-0.1.54/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.53/pyproject.toml` & `motion_python-0.1.54/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.53"
+version = "0.1.54"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.53/PKG-INFO` & `motion_python-0.1.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.53
+Version: 0.1.54
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

