# Comparing `tmp/lldb_dfsan-0.1.tar.gz` & `tmp/lldb_dfsan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lldb_dfsan-0.1.tar", last modified: Sat Jun  3 07:33:33 2023, max compression
+gzip compressed data, was "lldb_dfsan-0.1.1.tar", last modified: Sat Jun  3 08:13:20 2023, max compression
```

## Comparing `lldb_dfsan-0.1.tar` & `lldb_dfsan-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 07:33:33.465682 lldb_dfsan-0.1/
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)    11358 2023-04-19 18:16:26.000000 lldb_dfsan-0.1/LICENSE
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)     1410 2023-06-03 07:33:33.465682 lldb_dfsan-0.1/PKG-INFO
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)      825 2023-03-25 14:37:09.000000 lldb_dfsan-0.1/README.md
-drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 07:33:33.465682 lldb_dfsan-0.1/lldb_dfsan.egg-info/
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)     1410 2023-06-03 07:33:33.000000 lldb_dfsan-0.1/lldb_dfsan.egg-info/PKG-INFO
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)      196 2023-06-03 07:33:33.000000 lldb_dfsan-0.1/lldb_dfsan.egg-info/SOURCES.txt
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)        1 2023-06-03 07:33:33.000000 lldb_dfsan-0.1/lldb_dfsan.egg-info/dependency_links.txt
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)       11 2023-06-03 07:33:33.000000 lldb_dfsan-0.1/lldb_dfsan.egg-info/top_level.txt
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)     7659 2023-06-03 07:17:22.000000 lldb_dfsan-0.1/lldb_dfsan.py
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)      651 2023-06-03 07:31:10.000000 lldb_dfsan-0.1/pyproject.toml
--rw-r--r--   0 teemperor  (1000) teemperor  (1000)       38 2023-06-03 07:33:33.465682 lldb_dfsan-0.1/setup.cfg
-drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 07:33:33.465682 lldb_dfsan-0.1/tests/
--rwxr-xr-x   0 teemperor  (1000) teemperor  (1000)     2591 2023-04-27 10:44:36.000000 lldb_dfsan-0.1/tests/test.py
+drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 08:13:20.424783 lldb_dfsan-0.1.1/
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)    11358 2023-04-19 18:16:26.000000 lldb_dfsan-0.1.1/LICENSE
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)     1327 2023-06-03 08:13:20.424783 lldb_dfsan-0.1.1/PKG-INFO
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)      740 2023-06-03 07:38:55.000000 lldb_dfsan-0.1.1/README.md
+drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 08:13:20.424783 lldb_dfsan-0.1.1/lldb_dfsan.egg-info/
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)     1327 2023-06-03 08:13:20.000000 lldb_dfsan-0.1.1/lldb_dfsan.egg-info/PKG-INFO
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)      196 2023-06-03 08:13:20.000000 lldb_dfsan-0.1.1/lldb_dfsan.egg-info/SOURCES.txt
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)        1 2023-06-03 08:13:20.000000 lldb_dfsan-0.1.1/lldb_dfsan.egg-info/dependency_links.txt
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)       11 2023-06-03 08:13:20.000000 lldb_dfsan-0.1.1/lldb_dfsan.egg-info/top_level.txt
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)     7675 2023-06-03 07:46:25.000000 lldb_dfsan-0.1.1/lldb_dfsan.py
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)      654 2023-06-03 08:12:54.000000 lldb_dfsan-0.1.1/pyproject.toml
+-rw-r--r--   0 teemperor  (1000) teemperor  (1000)       38 2023-06-03 08:13:20.424783 lldb_dfsan-0.1.1/setup.cfg
+drwxr-xr-x   0 teemperor  (1000) teemperor  (1000)        0 2023-06-03 08:13:20.424783 lldb_dfsan-0.1.1/tests/
+-rwxr-xr-x   0 teemperor  (1000) teemperor  (1000)     2591 2023-04-27 10:44:36.000000 lldb_dfsan-0.1.1/tests/test.py
```

### Comparing `lldb_dfsan-0.1/LICENSE` & `lldb_dfsan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lldb_dfsan-0.1/PKG-INFO` & `lldb_dfsan-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lldb_dfsan
-Version: 0.1
+Version: 0.1.1
 Summary: LLDB plugin for debugging DFSan'd binaries.
 Author-email: Raphael Isemann <teemperor@gmail.com>
 Project-URL: Homepage, https://github.com/vusec/lldb-dfsan
 Project-URL: Bug Tracker, https://github.com/vusec/lldb-dfsan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -18,17 +18,15 @@
 
 `lldb-dfsan` is an LLDB plugin that allows inspecting the DFSan labels of
 variables, structures and memory in the target process.
 
 ## Installation
 
 ```bash
-wget "https://raw.githubusercontent.com/vusec/lldb-dfsan/main/lldb_dfsan.py" ;
-sudo mv lldb_dfsan.py (lldb -P) ;
-echo "command script import lldb_dfsan" >> .lldbinit
+pip install lldb-dfsan && echo "command script import lldb_dfsan" >> ~/.lldbinit
 ```
 
 ## How to use
 
 This plugin provides the `label VAR` command which prints all labels of the
 references local variable `VAR`. For example:
```

### Comparing `lldb_dfsan-0.1/README.md` & `lldb_dfsan-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 `lldb-dfsan` is an LLDB plugin that allows inspecting the DFSan labels of
 variables, structures and memory in the target process.
 
 ## Installation
 
 ```bash
-wget "https://raw.githubusercontent.com/vusec/lldb-dfsan/main/lldb_dfsan.py" ;
-sudo mv lldb_dfsan.py (lldb -P) ;
-echo "command script import lldb_dfsan" >> .lldbinit
+pip install lldb-dfsan && echo "command script import lldb_dfsan" >> ~/.lldbinit
 ```
 
 ## How to use
 
 This plugin provides the `label VAR` command which prints all labels of the
 references local variable `VAR`. For example:
```

### Comparing `lldb_dfsan-0.1/lldb_dfsan.egg-info/PKG-INFO` & `lldb_dfsan-0.1.1/lldb_dfsan.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lldb-dfsan
-Version: 0.1
+Version: 0.1.1
 Summary: LLDB plugin for debugging DFSan'd binaries.
 Author-email: Raphael Isemann <teemperor@gmail.com>
 Project-URL: Homepage, https://github.com/vusec/lldb-dfsan
 Project-URL: Bug Tracker, https://github.com/vusec/lldb-dfsan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -18,17 +18,15 @@
 
 `lldb-dfsan` is an LLDB plugin that allows inspecting the DFSan labels of
 variables, structures and memory in the target process.
 
 ## Installation
 
 ```bash
-wget "https://raw.githubusercontent.com/vusec/lldb-dfsan/main/lldb_dfsan.py" ;
-sudo mv lldb_dfsan.py (lldb -P) ;
-echo "command script import lldb_dfsan" >> .lldbinit
+pip install lldb-dfsan && echo "command script import lldb_dfsan" >> ~/.lldbinit
 ```
 
 ## How to use
 
 This plugin provides the `label VAR` command which prints all labels of the
 references local variable `VAR`. For example:
```

### Comparing `lldb_dfsan-0.1/lldb_dfsan.py` & `lldb_dfsan-0.1.1/lldb_dfsan.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,12 +247,12 @@
                 old_taint_storage = taint_storage.copy()
                 output = LabelOutput(frame=frame,
                                      only_tainted=options.only_tainted,
                                      follow_pointers=options.follow_pointers,
                                      indentation=options.indentation,
                                      diff=options.diff)
                 print_label(output, frame, var)
-                result.Print(output.get_final_output())
+                result.Print(output.get_final_output().rstrip() + "\n")
 
 
 def __lldb_init_module(debugger, dict):
     debugger.HandleCommand("command script add -f %s.label label" % __name__)
```

### Comparing `lldb_dfsan-0.1/pyproject.toml` & `lldb_dfsan-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lldb_dfsan"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Raphael Isemann", email="teemperor@gmail.com" },
 ]
 description = "LLDB plugin for debugging DFSan'd binaries."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,8 +16,8 @@
 
 [project.urls]
 "Homepage" = "https://github.com/vusec/lldb-dfsan"
 "Bug Tracker" = "https://github.com/vusec/lldb-dfsan/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `lldb_dfsan-0.1/tests/test.py` & `lldb_dfsan-0.1.1/tests/test.py`

 * *Files identical despite different names*

