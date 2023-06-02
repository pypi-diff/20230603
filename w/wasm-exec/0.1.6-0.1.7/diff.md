# Comparing `tmp/wasm_exec-0.1.6.tar.gz` & `tmp/wasm_exec-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm_exec-0.1.6.tar", max compression
+gzip compressed data, was "wasm_exec-0.1.7.tar", max compression
```

## Comparing `wasm_exec-0.1.6.tar` & `wasm_exec-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/LICENSE
--rw-r--r--   0        0        0     3083 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/README.md
--rw-r--r--   0        0        0      818 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3881 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/__init__.py
--rw-r--r--   0        0        0       41 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/exceptions.py
--rw-r--r--   0        0        0      215 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/schema.py
--rw-r--r--   0        0        0 20538911 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm
--rw-r--r--   0        0        0      121 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm.sha256sum
--rw-r--r--   0        0        0     1424 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/wasm_runtime.py
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 wasm_exec-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3083 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/README.md
+-rw-r--r--   0        0        0      818 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4304 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/wasm_exec/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/wasm_exec/exceptions.py
+-rw-r--r--   0        0        0      215 2023-06-02 22:32:49.675346 wasm_exec-0.1.7/wasm_exec/schema.py
+-rw-r--r--   0        0        0 20538911 2023-06-02 22:32:49.803351 wasm_exec-0.1.7/wasm_runtime/python-3.11.3.wasm
+-rw-r--r--   0        0        0      121 2023-06-02 22:32:49.803351 wasm_exec-0.1.7/wasm_runtime/python-3.11.3.wasm.sha256sum
+-rw-r--r--   0        0        0     1424 2023-06-02 22:32:49.803351 wasm_exec-0.1.7/wasm_runtime/wasm_runtime.py
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 wasm_exec-0.1.7/PKG-INFO
```

### Comparing `wasm_exec-0.1.6/LICENSE` & `wasm_exec-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.6/README.md` & `wasm_exec-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.6/pyproject.toml` & `wasm_exec-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wasm-exec"
-version = "0.1.6"
+version = "0.1.7"
 description = "WASM-powered, sandboxed version of `exec()` for running dynamic code."
 authors = ["Justin Flick"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/jflick58/wasm_exec"
 packages = [
     { include = "wasm_exec" },
```

### Comparing `wasm_exec-0.1.6/wasm_exec/__init__.py` & `wasm_exec-0.1.7/wasm_exec/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -70,25 +70,30 @@
 
         self.config = WasiConfig()
         self.config.argv = ("python", "-c", "")
 
         self.use_fuel = use_fuel
         self.fuel = fuel
 
-    def exec(self, code):
+    def exec(self, code: str, globals: dict = {}, locals: dict = {}):
         """
-        Execute code in an isolated Wasm-based Python interpreter
+        Execute arbitrary code in an isolated Wasm-based Python interpreter
 
         :param code: The WebAssembly code to execute.
         :type code: str
+        :param globals: Allowed global scope
+        :type global: dict
+        :param locals: Allowed local scope
+        :type locals: dict
         :return: The result of the code execution.
         :rtype: Result
         :raises WasmExecError: If an error occurs during code execution.
         """
-        self.config.argv = ("python", "-c", dedent(code))
+        exec_code = f'exec("""{dedent(code)}""", {globals}, {locals})'
+        self.config.argv = ("python", "-c", exec_code)
 
         with tempfile.TemporaryDirectory() as chroot:
             out_log = os.path.join(chroot, "out.log")
             err_log = os.path.join(chroot, "err.log")
             self.config.stdout_file = out_log
             self.config.stderr_file = err_log
 
@@ -99,21 +104,26 @@
             store.set_wasi(self.config)
             instance = self.linker.instantiate(store, self.python_module)
 
             start = instance.exports(store)["_start"]
             mem = instance.exports(store)["memory"]
 
             try:
-                start(store)
+                start(store)  # type: ignore
             except Exception:
                 with open(err_log) as f:
                     raise WasmExecError(f.read())
 
             with open(out_log) as f:
                 result = f.read()
 
             if not self.use_fuel:
                 fuel_consumed = None
             else:
                 fuel_consumed = store.fuel_consumed()
 
-            return Result(result, mem.size(store), mem.data_len(store), fuel_consumed)
+            return Result(
+                result,  # type: ignore
+                mem.size(store),  # type: ignore
+                mem.data_len(store),  # type: ignore
+                fuel_consumed,
+            )  # type: ignore
```

### Comparing `wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm` & `wasm_exec-0.1.7/wasm_runtime/python-3.11.3.wasm`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.6/wasm_runtime/wasm_runtime.py` & `wasm_exec-0.1.7/wasm_runtime/wasm_runtime.py`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.6/PKG-INFO` & `wasm_exec-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-exec
-Version: 0.1.6
+Version: 0.1.7
 Summary: WASM-powered, sandboxed version of `exec()` for running dynamic code.
 Home-page: https://www.github.com/jflick58/wasm_exec
 License: MIT
 Author: Justin Flick
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

