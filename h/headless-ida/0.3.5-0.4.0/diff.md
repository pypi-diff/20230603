# Comparing `tmp/headless-ida-0.3.5.tar.gz` & `tmp/headless-ida-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headless-ida-0.3.5.tar", last modified: Sat May 20 06:01:18 2023, max compression
+gzip compressed data, was "headless-ida-0.4.0.tar", last modified: Sat Jun  3 04:12:03 2023, max compression
```

## Comparing `headless-ida-0.3.5.tar` & `headless-ida-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 06:01:08.000000 headless-ida-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-20 06:01:18.669571 headless-ida-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-20 06:01:08.000000 headless-ida-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/headless_ida/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/ida_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/ida_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/headless_ida.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-20 06:01:10.000000 headless-ida-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:01:18.669571 headless-ida-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 04:11:53.000000 headless-ida-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:12:03.869734 headless-ida-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-03 04:11:53.000000 headless-ida-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/headless_ida/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/ida_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/ida_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 04:11:53.000000 headless-ida-0.4.0/headless_ida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:12:03.869734 headless-ida-0.4.0/headless_ida.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 04:12:03.000000 headless-ida-0.4.0/headless_ida.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-03 04:11:56.000000 headless-ida-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:12:03.869734 headless-ida-0.4.0/setup.cfg
```

### Comparing `headless-ida-0.3.5/LICENSE` & `headless-ida-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.5/PKG-INFO` & `headless-ida-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.3.5
+Version: 0.4.0
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -127,7 +127,12 @@
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
 - [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
 - [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
+
+# Known Issues
+### `from XXX import *`
+ - Using `from XXX import *` syntax with certain ida modules (like idaapi, ida_ua, etc.) is currently unsupported due to SWIG and RPyC compatibility issues. We recommend importing specific items with `from XXX import YYY, ZZZ`, or importing the entire module using `import XXX`.
+ - The issue arises because SWIG, employed for creating Python bindings for C/C++ code, generates intermediary objects (SwigVarlink) that RPyC, our remote procedure call mechanism, cannot serialize or transmit correctly.
```

### Comparing `headless-ida-0.3.5/README.md` & `headless-ida-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -92,7 +92,12 @@
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
 - [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
 - [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
+
+# Known Issues
+### `from XXX import *`
+ - Using `from XXX import *` syntax with certain ida modules (like idaapi, ida_ua, etc.) is currently unsupported due to SWIG and RPyC compatibility issues. We recommend importing specific items with `from XXX import YYY, ZZZ`, or importing the entire module using `import XXX`.
+ - The issue arises because SWIG, employed for creating Python bindings for C/C++ code, generates intermediary objects (SwigVarlink) that RPyC, our remote procedure call mechanism, cannot serialize or transmit correctly.
```

### Comparing `headless-ida-0.3.5/headless_ida/cli.py` & `headless-ida-0.4.0/headless_ida/cli.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.5/headless_ida/client.py` & `headless-ida-0.4.0/headless_ida/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,15 +39,18 @@
             port = s.getsockname()[1]
         tempidb = tempfile.NamedTemporaryFile(suffix=".idb")
         p = subprocess.Popen(
             f'{idat_path} -o{tempidb.name} -A -S"{server_path} {port}" -P+ {binary_path}', shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         while True:
             if p.poll() is not None:
                 raise Exception(
-                    f"IDA failed to start: return code {p.poll()}\n{p.stderr.read().decode()}")
+                    f"IDA failed to start: return code {p.poll()}\n"
+                    f"=============== STDOUT ===============\n{p.stdout.read().decode()}"
+                    f"=============== STDERR ===============\n{p.stderr.read().decode()}"
+                )
             try:
                 self.conn = rpyc.connect("localhost", port)
             except:
                 continue
             break
 
         if override_import:
```

### Comparing `headless-ida-0.3.5/headless_ida/ida_headers.py` & `headless-ida-0.4.0/headless_ida/ida_headers.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.5/headless_ida/ida_script.py` & `headless-ida-0.4.0/headless_ida/ida_script.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.5/headless_ida/server.py` & `headless-ida-0.4.0/headless_ida/server.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.5/headless_ida.egg-info/PKG-INFO` & `headless-ida-0.4.0/headless_ida.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.3.5
+Version: 0.4.0
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -127,7 +127,12 @@
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
 - [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
 - [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
+
+# Known Issues
+### `from XXX import *`
+ - Using `from XXX import *` syntax with certain ida modules (like idaapi, ida_ua, etc.) is currently unsupported due to SWIG and RPyC compatibility issues. We recommend importing specific items with `from XXX import YYY, ZZZ`, or importing the entire module using `import XXX`.
+ - The issue arises because SWIG, employed for creating Python bindings for C/C++ code, generates intermediary objects (SwigVarlink) that RPyC, our remote procedure call mechanism, cannot serialize or transmit correctly.
```

### Comparing `headless-ida-0.3.5/pyproject.toml` & `headless-ida-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "headless-ida"
-version = "0.3.5"
+version = "0.4.0"
 dependencies = [
     "rpyc",
 ]
 readme = "README.md"
 description = "Headless IDA"
 authors = [
     {name = "Han Dai", email = "pypi@han.do"},
```

