# Comparing `tmp/motion_python-0.1.52.tar.gz` & `tmp/motion_python-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.52.tar", max compression
+gzip compressed data, was "motion_python-0.1.53.tar", max compression
```

## Comparing `motion_python-0.1.52.tar` & `motion_python-0.1.53.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-02 16:01:25.780389 motion_python-0.1.52/README.md
--rw-r--r--   0        0        0      202 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/component.py
--rw-r--r--   0        0        0    14131 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/execute.py
--rw-r--r--   0        0        0     5182 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/fit_task.py
--rw-r--r--   0        0        0     9364 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/utils.py
--rw-r--r--   0        0        0     1555 2023-06-02 16:01:43.648863 motion_python-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-02 23:34:06.476208 motion_python-0.1.53/README.md
+-rw-r--r--   0        0        0      202 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/component.py
+-rw-r--r--   0        0        0    14780 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/execute.py
+-rw-r--r--   0        0        0     5182 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/fit_task.py
+-rw-r--r--   0        0        0    10503 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-02 23:34:06.480208 motion_python-0.1.53/motion/utils.py
+-rw-r--r--   0        0        0     1555 2023-06-02 23:34:31.620453 motion_python-0.1.53/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.53/PKG-INFO
```

### Comparing `motion_python-0.1.52/README.md` & `motion_python-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/cli.py` & `motion_python-0.1.53/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/component.py` & `motion_python-0.1.53/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/execute.py` & `motion_python-0.1.53/motion/execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import threading
 from typing import Any, Callable, Dict, List, Optional
 from uuid import uuid4
 
 import cloudpickle
 import psutil
 import redis
+from redis.lock import Lock
 
 from motion.fit_task import FitTask
 from motion.route import Route
 from motion.utils import (
     CustomDict,
     FitEvent,
     FitEventGroup,
@@ -212,25 +213,46 @@
 
         # Join fit processes
         for process in processes_to_wait_for:
             process.join()
 
         self.monitor_thread.join()
 
-    def update(self, new_state: Dict[str, Any]) -> None:
-        if new_state:
+    def _updateState(self, new_state: Dict[str, Any]) -> None:
+        if not new_state:
+            return
+
+        if not isinstance(new_state, dict):
+            raise TypeError("State should be a dict.")
+
+        # Acquire a lock
+        lock_timeout = 5  # Lock timeout in seconds
+        lock = Lock(self._redis_con, self._instance_name, lock_timeout)
+
+        acquired_lock = lock.acquire(blocking=True)
+        if acquired_lock:
             self._state.update(new_state)
+
+            # Get latest state
+            self._state = self._loadState()
+            self._state.update(new_state)
+
             # Save state to redis
             saveState(
                 self._state,
                 self._redis_con,
                 self._instance_name,
                 self._save_state_func,
             )
 
+            self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
+
+            # Release lock
+            lock.release()
+
     def empty_batch(self) -> Dict[str, List[Any]]:
         return {
             "fit_events": [],
             "values": [],
             "infer_results": [],
         }
```

### Comparing `motion_python-0.1.52/motion/fit_task.py` & `motion_python-0.1.53/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/instance.py` & `motion_python-0.1.53/motion/instance.py`

 * *Files 13% similar despite different names*

```diff
@@ -125,34 +125,69 @@
 
         c_instance = C()
         c_instance.get_version() # Returns 1 (first version)
         ```
         """
         return self._executor.version  # type: ignore
 
+    def update_state(self, state_update: Dict[str, Any]) -> None:
+        """Writes the state update to the component instance's state.
+        If a fit op is currently running, the state update will be
+        applied after the fit op is finished. Warning: this could
+        take a while if your fit op takes a long time!
+
+        Usage:
+        ```python
+        from motion import Component
+
+        C = Component("MyComponent")
+
+        @C.init_state
+        def setUp():
+            return {"value": 0}
+
+        # Define infer and fit operations
+        ...
+
+        if __name__ == "__main__":
+            c_instance = C()
+            c_instance.read_state("value") # Returns 0
+            c_instance.update_state({"value": 1, "value2": 2})
+            c_instance.read_state("value") # Returns 1
+            c_instance.read_state("value2") # Returns 2
+        ```
+
+        Args:
+            state_update (Dict[str, Any]): Dictionary of key-value pairs
+                to update the state with.
+        """
+        self._executor._updateState(state_update)
+
     def read_state(self, key: str) -> Any:
-        """Gets the current value for the key in the component's state.
+        """Gets the current value for the key in the component instance's state.
 
         Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
         # Define infer and fit operations
+        ...
 
-        c_instance = C()
-        c_instance.read_state("value") # Returns 0
-        c_instance.run(...)
-        c_instance.read_state("value") # This will return the current value of
-        # "value" in the state
+        if __name__ == "__main__":
+            c_instance = C()
+            c_instance.read_state("value") # Returns 0
+            c_instance.run(...)
+            c_instance.read_state("value") # This will return the current value
+            # of "value" in the state
         ```
 
         Args:
             key (str): Key in the state to get the value for.
 
         Returns:
             Any: Current value for the key.
```

### Comparing `motion_python-0.1.52/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.53/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/route.py` & `motion_python-0.1.53/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/motion/utils.py` & `motion_python-0.1.53/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.52/pyproject.toml` & `motion_python-0.1.53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.52"
+version = "0.1.53"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.52/PKG-INFO` & `motion_python-0.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.52
+Version: 0.1.53
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

