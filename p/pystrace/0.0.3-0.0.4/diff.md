# Comparing `tmp/pystrace-0.0.3.tar.gz` & `tmp/pystrace-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystrace-0.0.3.tar", last modified: Fri Feb 10 21:26:44 2023, max compression
+gzip compressed data, was "pystrace-0.0.4.tar", last modified: Sat Jun  3 13:01:14 2023, max compression
```

## Comparing `pystrace-0.0.3.tar` & `pystrace-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 21:26:44.162416 pystrace-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-02-10 21:26:39.000000 pystrace-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-02-10 21:26:39.000000 pystrace-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-02-10 21:26:44.162416 pystrace-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-02-10 21:26:39.000000 pystrace-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 21:26:44.162416 pystrace-0.0.3/pystrace/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18474 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/config.json
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4569 2023-02-10 21:26:39.000000 pystrace-0.0.3/pystrace/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 21:26:44.162416 pystrace-0.0.3/pystrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-10 21:26:44.000000 pystrace-0.0.3/pystrace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-10 21:26:39.000000 pystrace-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-02-10 21:26:44.162416 pystrace-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-02-10 21:26:39.000000 pystrace-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 13:01:14.996279 pystrace-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-03 13:01:06.000000 pystrace-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-03 13:01:06.000000 pystrace-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-03 13:01:14.996279 pystrace-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-06-03 13:01:06.000000 pystrace-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 13:01:14.992279 pystrace-0.0.4/pystrace/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18474 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/config.json
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-06-03 13:01:06.000000 pystrace-0.0.4/pystrace/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 13:01:14.996279 pystrace-0.0.4/pystrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-03 13:01:14.000000 pystrace-0.0.4/pystrace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-03 13:01:06.000000 pystrace-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-03 13:01:14.996279 pystrace-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-03 13:01:06.000000 pystrace-0.0.4/setup.py
```

### Comparing `pystrace-0.0.3/LICENSE` & `pystrace-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/PKG-INFO` & `pystrace-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystrace
-Version: 0.0.3
+Version: 0.0.4
 Summary: Report files opened while executing a command
 Home-page: https://github.com/joaompinto/pystrace
 Author: João Pinto
 Author-email: joao.pinto@vshn.ch
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pystrace-0.0.3/README.md` & `pystrace-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/pystrace/__main__.py` & `pystrace-0.0.4/pystrace/__main__.py`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/pystrace/_version.py` & `pystrace-0.0.4/pystrace/_version.py`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/pystrace/cli.py` & `pystrace-0.0.4/pystrace/cli.py`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/pystrace/config.json` & `pystrace-0.0.4/pystrace/config.json`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/pystrace/tracer.py` & `pystrace-0.0.4/pystrace/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         while True:
             with open(self.fifo_filename, 'r') as fifo:
                 data = fifo.read()
                 while data:
                     # When there is an error during strace, it will not open the fifo
                     # which means we only get  single FIFO item with the rc
-                    if data.isnumeric():
+                    if data.lstrip("-").isnumeric():
                         rc = int(data)
                         return rc
                     for line in data.splitlines():
                         syscall_data = self.parse_regex_ok.findall(line)
                         if syscall_data:
                             pid, syscall, arguments, result = syscall_data[0]
                             syscall_dict = {
```

### Comparing `pystrace-0.0.3/pystrace.egg-info/PKG-INFO` & `pystrace-0.0.4/pystrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystrace
-Version: 0.0.3
+Version: 0.0.4
 Summary: Report files opened while executing a command
 Home-page: https://github.com/joaompinto/pystrace
 Author: João Pinto
 Author-email: joao.pinto@vshn.ch
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pystrace-0.0.3/setup.cfg` & `pystrace-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pystrace-0.0.3/setup.py` & `pystrace-0.0.4/setup.py`

 * *Files identical despite different names*

