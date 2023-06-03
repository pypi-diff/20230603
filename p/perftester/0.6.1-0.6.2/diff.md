# Comparing `tmp/perftester-0.6.1.tar.gz` & `tmp/perftester-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perftester-0.6.1.tar", last modified: Thu Jun  1 10:10:51 2023, max compression
+gzip compressed data, was "perftester-0.6.2.tar", last modified: Sat Jun  3 03:59:12 2023, max compression
```

## Comparing `perftester-0.6.1.tar` & `perftester-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.140047 perftester-0.6.1/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 10:10:51.139047 perftester-0.6.1/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-01 10:09:00.000000 perftester-0.6.1/README.md
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.099044 perftester-0.6.1/perftester/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      284 2023-06-01 10:09:00.000000 perftester-0.6.1/perftester/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5119 2022-06-22 16:29:34.000000 perftester-0.6.1/perftester/__main__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    33369 2023-06-01 10:09:15.000000 perftester-0.6.1/perftester/perftester.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1657 2022-09-02 13:30:35.000000 perftester-0.6.1/perftester/tmp.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      820 2022-09-02 07:16:38.000000 perftester-0.6.1/perftester/tmp_working.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    15670 2023-06-01 10:09:00.000000 perftester-0.6.1/perftester/understand.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-01 10:10:51.135045 perftester-0.6.1/perftester.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      364 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/entry_points.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-01 10:10:51.000000 perftester-0.6.1/perftester.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-01 10:10:51.140503 perftester-0.6.1/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      903 2023-06-01 10:09:41.000000 perftester-0.6.1/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.560365 perftester-0.6.2/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1063 2023-06-03 01:55:57.000000 perftester-0.6.2/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-03 03:59:12.559367 perftester-0.6.2/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-03 01:55:57.000000 perftester-0.6.2/README.md
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.517082 perftester-0.6.2/perftester/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      285 2023-06-03 02:47:03.000000 perftester-0.6.2/perftester/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5212 2023-06-03 02:47:03.000000 perftester-0.6.2/perftester/__main__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    33545 2023-06-03 02:47:06.000000 perftester-0.6.2/perftester/perftester.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.556364 perftester-0.6.2/perftester.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      303 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/entry_points.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-03 03:59:12.561678 perftester-0.6.2/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      917 2023-06-03 02:50:31.000000 perftester-0.6.2/setup.py
```

### Comparing `perftester-0.6.1/PKG-INFO` & `perftester-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.1
+Version: 0.6.2
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.1/README.md` & `perftester-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `perftester-0.6.1/perftester/__main__.py` & `perftester-0.6.2/perftester/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,38 @@
 
     for file in files:
         module, module_name = _import_module(file)
         perftester_functions = _find_perftester_functions(module)
         for func in perftester_functions:
             this_test = _perftester(module_name, func)
             if this_test:
-                failed_perftesters.append(f"{str(module_name)}.{func.__name__}")
+                failed_perftesters.append(
+                    f"{str(module_name)}.{func.__name__}"
+                )
             else:
-                passed_perftesters.append(f"{str(module_name)}.{func.__name__}")
+                passed_perftesters.append(
+                    f"{str(module_name)}.{func.__name__}"
+                )
 
     test_results = TestResults(
         passed_tests=passed_perftesters, failed_tests=failed_perftesters
     )
     _log_perftester_results(test_results)
 
 
 def _read_cli_args():
     if len(sys.argv) == 1:
         path = pathlib.Path(os.getcwd())
     else:
         # sys.argv[1] is always a string, so no need to check it
         path = pathlib.Path(sys.argv[1])
     check_if_paths_exist(
-        path, CLIPathError, "Incorrent path provided with perftester CLI command"
+        path,
+        CLIPathError,
+        "Incorrent path provided with perftester CLI command",
     )
     if path.is_dir():
         files = _find_perftester_files(path)
     elif path.is_file:
         files = [
             path,
         ]
```

### Comparing `perftester-0.6.1/perftester/perftester.py` & `perftester-0.6.2/perftester/perftester.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 class Config:
     """Default configuration for testing.
 
     It is a singleton whose instance is created once, during import
     of the perftester module.
     """
+
     config_file = Path("config_perftester.py")
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls, *args, **kwargs)
         return cls._instance
@@ -285,15 +286,17 @@
         """
         memory_results = [
             memory_usage((self.benchmark_function, (), {}))
             for _ in range(self.defaults["memory"]["repeat"])
         ]
         self.memory_benchmark = min(max(r) for r in memory_results)
 
-    def set_defaults(self, which, number=None, repeat=None, Number=None, Repeat=None):
+    def set_defaults(
+        self, which, number=None, repeat=None, Number=None, Repeat=None
+    ):
         """Change the default settings.
 
         Beware! This does not change particular settings for a particular test,
         but the defaults. So this will affect also how the benchmark tests
         will be run.
 
         However, this will not change any settings for functions that were already
@@ -314,15 +317,17 @@
         self._check_args(lambda: 0, which, number, repeat)
 
         if number is not None:
             self.defaults[which]["number"] = number
         if repeat is not None:
             self.defaults[which]["repeat"] = repeat
 
-    def set(self, func, which, number=None, repeat=None, Number=None, Repeat=None):
+    def set(
+        self, func, which, number=None, repeat=None, Number=None, Repeat=None
+    ):
         """Set a particular argument.
 
         Args:
             func (Callable): a callable for which we want to change
                 the setting
             which (str): either "time" or "memory"
             number (int, optional): passed to timeit.repeat as number.
@@ -452,21 +457,22 @@
         lambda: func(*args, **kwargs),
         number=number,
         repeat=Repeat or config.get_setting(func, "time", "repeat"),
     )
     return [r / number for r in repeat_results]
 
 
-def time_test(func,
-              *args,
-              raw_limit=None,
-              relative_limit=None,
-              Number=None,
-              Repeat=None,
-              **kwargs
+def time_test(
+    func,
+    *args,
+    raw_limit=None,
+    relative_limit=None,
+    Number=None,
+    Repeat=None,
+    **kwargs,
 ):
     """Run time performance test for func.
 
     You need to provide either raw_limit or relative_limit, or both.
 
     Note that if the tested function throws an error, so will time_test(),
     which will raise the FunctionError exception.
@@ -545,15 +551,14 @@
     """
     check_if_not(
         raw_limit is None and relative_limit is None,
         LackingLimitsError,
         message="You must provide raw_limit, relative_limit or both",
     )
     _add_func_to_config(func)
-    
 
     results = time_benchmark(
         func, *args, Number=Number, Repeat=Repeat, **kwargs
     )
 
     config.cut_traceback()
     # Test raw_limit
@@ -580,15 +585,20 @@
                 f"minimum time ratio = {rounder.signif(ratio_time, config.digits_for_printing)}"
             ),
         )
     config.full_traceback()
 
 
 def memory_usage_test(
-    func, *args, raw_limit=None, relative_limit=None, Repeat=None, **kwargs,
+    func,
+    *args,
+    raw_limit=None,
+    relative_limit=None,
+    Repeat=None,
+    **kwargs,
 ):
     """Test memory usage of a function.
 
     You can run a test based on a raw limit for the time of executing
     of the function (this is a time per single run); then use raw_limit to
     provide the limit and relative_limit=None. You can use relative_limit to set up
     a limit for a relative test (against a function defined in the config);
@@ -790,15 +800,15 @@
 
     try:
         results = _repeat(func, *args, Number=Number, Repeat=Repeat, **kwargs)
     except Exception as e:
         raise FunctionError(
             f"The tested function raised {type(e).__name__}: {str(e)}"
         )
-    
+
     min_result = min(results)
 
     # Reload built-in benchmarks
     config.reload_time()
 
     return {
         "min": min_result,
@@ -852,58 +862,67 @@
 
 
 MemLog = namedtuple("MemLog", "ID memory")
 
 
 def MEMPRINT():
     """Pretty-print MEMLOGS."""
-    for i, memlog in enumerate(MEMLOGS): # type: ignore
+    for i, memlog in enumerate(MEMLOGS):  # type: ignore
         ID = memlog.ID if memlog.ID else ""
-        print(f"{i: < 4} "
-              f"{round(memlog.memory / 1024/1024, 1): <6} → "
-              f"{ID}")
+        print(
+            f"{i: < 4} "
+            f"{round(memlog.memory / 1024/1024, 1): <6} → "
+            f"{ID}"
+        )
 
 
 def MEMPOINT(ID=None):
     """Global function to measure full memory and log it into MEMLOGS.
-    
+
     The function is available from any module of a session. It logs into
     MEMLOGS, also available from any module.
-    
+
     Memory is collected using pympler.asizeof.asizeof(), and reported in
     bytes. So, the function measures the size of all current gc objects,
     including module, global and stack frame objects, minus the size
     of `MEMLOGS`.
     """
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        MEMLOGS.append(MemLog( # type: ignore
-                ID,
-                (asizeof(all=True) - asizeof(MEMLOGS))) # type: ignore
-            )
-
+        MEMLOGS.append(
+            MemLog(  # type: ignore
+                ID, (asizeof(all=True) - asizeof(MEMLOGS))
+            )  # type: ignore
+        )
 
 
 def MEMTRACE(func, ID_before=None, ID_after=None):
     """Decorator to log memory before and after running a function."""
+
     @wraps(func)
     def inner(*args, **kwargs):
         before = ID_before if ID_before else f"Before {func.__name__}()"
         MEMPOINT(before)
         f = func(*args, **kwargs)
         after = ID_after if ID_after else f"After {func.__name__}()"
         MEMPOINT(after)
         return f
+
     return inner
 
 
 builtins.__dict__["MEMPOINT"] = MEMPOINT
 builtins.__dict__["MEMPRINT"] = MEMPRINT
 builtins.__dict__["MEMTRACE"] = MEMTRACE
 
 MEMPOINT("perftester import")
 
 
 if __name__ == "__main__":
     import doctest
 
-    doctest.testmod()
+    flags = flags = (
+        doctest.ELLIPSIS
+        | doctest.NORMALIZE_WHITESPACE
+        | doctest.IGNORE_EXCEPTION_DETAIL
+    )
+    doctest.testmod(optionflags=flags)
```

### Comparing `perftester-0.6.1/perftester.egg-info/PKG-INFO` & `perftester-0.6.2/perftester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.1
+Version: 0.6.2
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.1/setup.py` & `perftester-0.6.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_requirements = {
     "dev": ["wheel", "black"],
 }
 
 setuptools.setup(
     name="perftester",
-    version="0.6.1",
+    version="0.6.2",
     author="Nyggus",
     author_email="nyggus@gmail.com",
     description="Lightweight performance testing in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyggus/perftester",
     packages=setuptools.find_packages(),
@@ -21,9 +21,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["easycheck", "rounder", "memory_profiler", "pympler"],
     python_requires=">=3.8",
     extras_require=extras_requirements,
-    entry_points={"console_scripts": ["perftester = perftester.__main__:main"]},
+    entry_points={
+        "console_scripts": ["perftester = perftester.__main__:main"]
+    },
 )
```

