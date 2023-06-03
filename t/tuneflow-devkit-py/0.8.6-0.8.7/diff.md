# Comparing `tmp/tuneflow-devkit-py-0.8.6.tar.gz` & `tmp/tuneflow-devkit-py-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.6.tar", last modified: Thu Jun  1 00:46:51 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.7.tar", last modified: Sat Jun  3 07:36:16 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.6.tar` & `tuneflow-devkit-py-0.8.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.6/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.6/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-06-01 00:46:10.000000 tuneflow-devkit-py-0.8.6/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7096 2023-06-01 00:19:56.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8805 2023-06-01 00:42:29.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-06-01 00:46:51.000000 tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-01 00:46:51.238661 tuneflow-devkit-py-0.8.6/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4786 2023-06-01 00:41:52.000000 tuneflow-devkit-py-0.8.6/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.6/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-03 07:36:16.856558 tuneflow-devkit-py-0.8.7/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.7/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-03 07:36:16.856558 tuneflow-devkit-py-0.8.7/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.7/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-06-03 07:35:42.000000 tuneflow-devkit-py-0.8.7/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-03 07:36:16.856558 tuneflow-devkit-py-0.8.7/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-03 07:36:16.846558 tuneflow-devkit-py-0.8.7/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-03 07:36:16.846558 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-06-03 07:29:26.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8805 2023-06-01 00:42:29.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-03 07:36:16.856558 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-06-03 07:36:16.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-06-03 07:36:16.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-03 07:36:16.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-06-03 07:36:16.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-06-03 07:36:16.000000 tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-03 07:36:16.856558 tuneflow-devkit-py-0.8.7/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4786 2023-06-01 00:41:52.000000 tuneflow-devkit-py-0.8.7/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.7/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.6/LICENSE` & `tuneflow-devkit-py-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/PKG-INFO` & `tuneflow-devkit-py-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.6
+Version: 0.8.7
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.6/README.md` & `tuneflow-devkit-py-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/pyproject.toml` & `tuneflow-devkit-py-0.8.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.6"
+version = "0.8.7"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'python-socketio >= 5.7.2',
     'uvicorn[standard] >= 0.20.0',
-    'tuneflow-py >= 0.8.1',
+    'tuneflow-py >= 0.8.3',
     'msgpack == 1.0.4',
     'fastapi == 0.92.0',
     'msgpack-asgi == 1.1.0'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tuneflow/tuneflow-devkit-py"
```

### Comparing `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Creates a local debug server for a single plugin.
         '''
 
         if plugin_class is None or bundle_file_path is None:
             raise Exception("plugin_class and bundle_file must be provided")
         validate_plugin(plugin_class=plugin_class)
         self._plugin_class = plugin_class
-        with open(bundle_file_path, 'rb', encoding='utf-8') as bundle_file:
+        with open(bundle_file_path, 'rb') as bundle_file:
             bundle_info = json.load(bundle_file)
             # Validate plugin and bundle.
             plugin_info = find_match_plugin_info(
                 bundle_info=bundle_info, provider_id=plugin_class.provider_id(),
                 plugin_id=plugin_class.plugin_id())
             if plugin_info is None:
                 raise Exception(
```

### Comparing `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.7/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.7/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.6
+Version: 0.8.7
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.6/test/test_runner.py` & `tuneflow-devkit-py-0.8.7/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.6/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.7/test/test_validation_utils.py`

 * *Files identical despite different names*

