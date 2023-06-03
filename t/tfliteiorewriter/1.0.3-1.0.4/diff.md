# Comparing `tmp/tfliteiorewriter-1.0.3.tar.gz` & `tmp/tfliteiorewriter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfliteiorewriter-1.0.3.tar", last modified: Sat Jun  3 15:50:00 2023, max compression
+gzip compressed data, was "tfliteiorewriter-1.0.4.tar", last modified: Sat Jun  3 16:55:29 2023, max compression
```

## Comparing `tfliteiorewriter-1.0.3.tar` & `tfliteiorewriter-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/tfliteiorewriter/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-03 15:49:47.000000 tfliteiorewriter-1.0.3/tfliteiorewriter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:50:00.872747 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 15:50:00.000000 tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/tfliteiorewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/tfliteiorewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-06-03 16:55:17.000000 tfliteiorewriter-1.0.4/tfliteiorewriter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:29.286467 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 16:55:29.000000 tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/top_level.txt
```

### Comparing `tfliteiorewriter-1.0.3/.github/workflows/codeql-analysis.yml` & `tfliteiorewriter-1.0.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/.github/workflows/python-publish.yml` & `tfliteiorewriter-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/Dockerfile` & `tfliteiorewriter-1.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/LICENSE` & `tfliteiorewriter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/PKG-INFO` & `tfliteiorewriter-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.3
+Version: 1.0.4
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tfliteiorewriter-1.0.3/README.md` & `tfliteiorewriter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/pyproject.toml` & `tfliteiorewriter-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfliteiorewriter-1.0.3/tfliteiorewriter/main.py` & `tfliteiorewriter-1.0.4/tfliteiorewriter/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,34 +99,78 @@
         output_json_file_path = f'{output_path}/{output_json_file_name}'
         flat_json = None
 
         with open(input_json_file_path, 'r') as f:
             flat_json = json.load(f)
 
         # Checks if signature_defs are recorded in tflite
+        enable_signature_defs = True
         if 'signature_defs' not in flat_json or not flat_json['signature_defs']:
+            print('')
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} ' +
-                f'Processing is aborted because signature_defs is not recorded in tflite.'
+                f'signature_defs is not recorded in tflite.'
             )
-            sys.exit(0)
+            enable_signature_defs = False
 
         flat_subgraphs = flat_json['subgraphs'][0]
         flat_tensors: List[Dict] = flat_subgraphs['tensors']
-        flat_signature_def: Dict = flat_json['signature_defs'][0]
-        flat_signature_def_inputs: List[Dict] = flat_signature_def['inputs']
-        flat_signature_def_inputs_names = [
-            flat_signature_def_input['name'] \
-                for flat_signature_def_input in flat_signature_def_inputs
-        ]
-        flat_signature_def_outputs: List[Dict] = flat_signature_def['outputs']
-        flat_signature_def_outputs_names = [
-            flat_signature_def_output['name'] \
-                for flat_signature_def_output in flat_signature_def_outputs
-        ]
+        flat_signature_def: Dict = {}
+        flat_signature_def_inputs_names = []
+        flat_signature_def_outputs_names = []
+
+        if enable_signature_defs:
+            # Get the output name to be used for the replacement name from signature_defs
+            # if signature_defs is already defined
+            flat_signature_def = flat_json['signature_defs'][0]
+            flat_signature_def_inputs: List[Dict] = flat_signature_def['inputs']
+            flat_signature_def_inputs_names = [
+                flat_signature_def_input['name'] \
+                    for flat_signature_def_input in flat_signature_def_inputs
+            ]
+            flat_signature_def_outputs: List[Dict] = flat_signature_def['outputs']
+            flat_signature_def_outputs_names = [
+                flat_signature_def_output['name'] \
+                    for flat_signature_def_output in flat_signature_def_outputs
+            ]
+        else:
+            # Generate from tensors if signature_defs is undefined
+            flat_json['signature_defs'] = []
+            flat_subgraphs_inputs: List[int] = flat_subgraphs['inputs']
+            flat_subgraphs_outputs: List[int] = flat_subgraphs['outputs']
+            signature_def_inputs = []
+            signature_def_outputs = []
+            # inputs
+            for idx in flat_subgraphs_inputs:
+                for flat_tensor in flat_tensors:
+                    if int(flat_tensor['buffer']) == idx + 1:
+                        signature_def_inputs.append(
+                            {'name': flat_tensor['name'], 'tensor_index': idx}
+                        )
+                        flat_signature_def_inputs_names.append(flat_tensor['name'])
+                        break
+            # outputs
+            for idx in flat_subgraphs_outputs:
+                for flat_tensor in flat_tensors:
+                    if int(flat_tensor['buffer']) == idx + 1:
+                        signature_def_outputs.append(
+                            {'name': flat_tensor['name'], 'tensor_index': idx}
+                        )
+                        flat_signature_def_outputs_names.append(flat_tensor['name'])
+                        break
+
+            signature_def = {
+                "inputs": signature_def_inputs,
+                "outputs": signature_def_outputs,
+                "signature_key": "serving_default",
+                "subgraph_index": 0,
+            }
+            flat_json['signature_defs'].append(signature_def)
+            flat_signature_def_inputs: List[Dict] = signature_def['inputs']
+            flat_signature_def_outputs: List[Dict] = signature_def['outputs']
 
         # If the signature of the input OP and the signature of the output OP overlap,
         # rename the signature of the output OP.
         if not view_mode:
             if not rename_list:
                 # Override OP name by name in signature_defs
                 for flat_signature_def_outputs_name in flat_signature_def_outputs_names:
```

### Comparing `tfliteiorewriter-1.0.3/tfliteiorewriter.egg-info/PKG-INFO` & `tfliteiorewriter-1.0.4/tfliteiorewriter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfliteiorewriter
-Version: 1.0.3
+Version: 1.0.4
 Summary: This tool displays tflite signatures and rewrites the input/output OP name to the name of the signature. There is no need to install TensorFlow or TFLite.
 Author-email: Katsuya Hyodo <rmsdh122@yahoo.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Katsuya Hyodo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

