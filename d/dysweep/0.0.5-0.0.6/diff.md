# Comparing `tmp/dysweep-0.0.5.tar.gz` & `tmp/dysweep-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.5.tar", last modified: Mon May 22 17:04:15 2023, max compression
+gzip compressed data, was "dysweep-0.0.6.tar", last modified: Fri Jun  2 22:59:03 2023, max compression
```

## Comparing `dysweep-0.0.5.tar` & `dysweep-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:01:33.000000 dysweep-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:04:15.000854 dysweep-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 17:01:33.000000 dysweep-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:04:15.000854 dysweep-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 17:01:33.000000 dysweep-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.373344 dysweep-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 22:56:20.000000 dysweep-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 22:59:03.373344 dysweep-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-02 22:56:20.000000 dysweep-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.369344 dysweep-0.0.6/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.373344 dysweep-0.0.6/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:59:03.373344 dysweep-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-02 22:56:20.000000 dysweep-0.0.6/setup.py
```

### Comparing `dysweep-0.0.5/LICENSE` & `dysweep-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.5/PKG-INFO` & `dysweep-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.5/dysweep/parallel.py` & `dysweep-0.0.6/dysweep/parallel.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .wandbX import sweep, agent, hierarchical_config
 import functools
 from random_word import RandomWords
 import json
 import shutil
 import os
 import traceback
+import inspect
 
 SPLIT = '-'
 
 
 @dataclass
 class ResumableSweepConfig:
     default_root_dir: th.Union[Path, str]
@@ -20,15 +21,14 @@
     base_config: th.Optional[dict] = None
     #
     entity: th.Optional[str] = None
     project: th.Optional[str] = None
     count: th.Optional[int] = None
     resume: bool = False
     run_name: th.Optional[str] = None
-    checkpoint_interval: int = 3600
     sweep_id: th.Optional[th.Union[int, str]] = None
     #
     use_lightning_logger: bool = False
 
 
 def check_non_empty(checkpoint_dir):
     all_subdirs = [d for d in checkpoint_dir.iterdir() if d.is_dir()]
@@ -125,45 +125,75 @@
                         from lightning.pytorch.loggers import WandbLogger
                         logger = WandbLogger(
                             project=conf.project,
                             entity=conf.entity,
                             name=run_name,
                         )
                         experiment_id = logger.experiment.id
-                        sweep_config = hierarchical_config(logger.experiment.config)
+                        sweep_config = hierarchical_config(
+                            logger.experiment.config)
                     else:
                         import wandb
                         wandb.init(
                             project=conf.project,
                             entity=conf.entity,
                             name=run_name,
                         )
                         experiment_id = wandb.run.id
                         sweep_config = hierarchical_config(wandb.config)
 
                     new_dir_name = f"{len(all_subdirs)+1}{SPLIT}{experiment_id}"
 
                     os.makedirs(checkpoint_dir / new_dir_name)
-                    
+
                     # dump a json in checkpoint_dir/run_id containing the sweep config
                     with open(checkpoint_dir / new_dir_name / "sweep_config.json", "w") as f:
-                        json.dump(sweep_config, f)
+                        json.dump(sweep_config, f, indent=4, sort_keys=True)
 
                 new_checkpoint_dir = checkpoint_dir / new_dir_name
             except Exception as e:
                 print(traceback.format_exc())
                 raise e
 
             if conf.use_lightning_logger:
+                # check the function signature matches
+                # the one we expect.
+                # in which there are two arguments with the first one
+                # named config and the second one named checkpoint_dir
+
+                # get the signature of the function
+                sig = inspect.signature(function)
+                # get the parameters of the function
+                params = sig.parameters
+                # check that the function has two parameters
+                if len(params) != 3 or list(params.keys())[0] != "config" or list(params.keys())[1] != "logger" or list(params.keys())[2] != "checkpoint_dir":
+                    raise ValueError(
+                        "the run function should have the exact following parameters in order: (config, logger, checkpoint_dir)")
+
                 ret = function(sweep_config, logger, new_checkpoint_dir)
             else:
+                # check the function signature matches
+                # the one we expect.
+                # in which there are two arguments with the first one
+                # named config and the second one named checkpoint_dir
+
+                # get the signature of the function
+                sig = inspect.signature(function)
+                # get the parameters of the function
+                params = sig.parameters
+                # check that the function has two parameters
+                if len(params) != 2 or list(params.keys())[0] != "config" or list(params.keys())[1] != "checkpoint_dir":
+                    raise ValueError(
+                        "the run function should have the exact following parameters in order: (config, checkpoint_dir)")
                 ret = function(sweep_config, new_checkpoint_dir)
 
             # remove the entire new_checkpoint_dir if the function has finished
             # running.
+            shutil.copyfile(new_checkpoint_dir / "sweep_config.json",
+                            checkpoint_dir / f"{experiment_id}-config.json")
             shutil.rmtree(new_checkpoint_dir)
 
             return ret
         if conf.resume:
             for _ in range(conf.count):
                 if check_non_empty(checkpoint_dir):
                     modified_function()
@@ -171,12 +201,12 @@
                     break
         else:
             agent(conf.sweep_id, function=modified_function,
                   entity=conf.entity, project=conf.project, count=conf.count)
     else:
         try:
             sweep(conf.base_config, conf.sweep_configuration,
-                entity=conf.entity, project=conf.project)
+                  entity=conf.entity, project=conf.project)
         except Exception as e:
             print("Exception at creation of sweep:")
             print(traceback.format_exc())
-            raise e
+            raise e
```

### Comparing `dysweep-0.0.5/dysweep/utils.py` & `dysweep-0.0.6/dysweep/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             if SWEEP_ALIAS in inner_dict and "values" in inner_dict:
                 new_values = []
                 for idx, value in enumerate(inner_dict["values"]):
                     if inner_dict[SWEEP_ALIAS][idx] in value_compression_mapping:
                         raise Exception(
                             f"Value {inner_dict[SWEEP_ALIAS][idx]} is already used in the sweep config"
                         )
-                    value_compression_mapping[inner_dict[SWEEP_ALIAS][idx]] = value
+                    value_compression_mapping[inner_dict[SWEEP_ALIAS]
+                                              [idx]] = value
                     new_values.append(inner_dict[SWEEP_ALIAS][idx])
                 inner_dict["values"] = new_values
                 inner_dict.pop(SWEEP_ALIAS)
             parameter_config[key] = inner_dict
 
     all_keys = list(parameter_config.keys())
     for key in all_keys:
@@ -205,29 +206,34 @@
                   current_path: th.Optional[th.List[str]] = None,
                   root_args: th.Optional[th.Union[th.Dict, th.List]] = None):
     # try and catch an exception and add "line" to the exception and then re-raise it
     if current_path is None:
         current_path = []
     if root_args is None:
         root_args = args
-        
+
+    # print("000000000000000-------000000000000000")
+    # print("args")
+    # pprint(args)
+    # print("sweep_config")
+    # pprint(sweep_config)
+
     try:
         if isinstance(args, list):
             if isinstance(sweep_config, dict):
                 if DY_LIST_OPERATIONS in sweep_config:
                     ops = sweep_config.pop(DY_LIST_OPERATIONS)
-                    
+
                     # Convert operations from dictionary to a list
                     if not isinstance(ops, list):
                         real_ops = [None for _ in range(len(ops.keys()))]
                         for key, val in ops.items():
                             real_ops[int(key[len(IDX_INDICATOR):])] = val
                         ops = real_ops
-                    
-                    
+
                     for op in ops:
                         if len(op.keys()) != 1:
                             raise Exception(
                                 "Any sweep list operation should be a dictionary with a single key")
                         if DY_LIST_INSERT in op:
                             val = None
                             idx = op[DY_LIST_INSERT]
@@ -272,15 +278,15 @@
                             if not isinstance(idx, int):
                                 raise Exception(
                                     f"Expected an integer for {DY_LIST_REMOVE} but got: {idx}")
                             args.pop(idx)
                         else:
                             raise Exception(
                                 f"Unknown sweep list operation: {op}")
-                
+
                     sweep_config[DY_LIST_OPERATIONS] = ops
                 else:
                     for key, val in sweep_config.items():
                         args_key = int(key[len(IDX_INDICATOR):])
                         if isinstance(val, dict) or isinstance(val, list):
 
                             if isinstance(val, dict) and DY_EVAL in val:
@@ -325,62 +331,55 @@
                     elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
                         args[idx] = val
                     else:
                         pat = f"{DY_EVAL}\((.*)\)"
                         func_to_eval = re.search(pat, val).group(1)
                         args[idx] = dy.eval(func_to_eval)(args[idx])
 
-        else:
+        elif isinstance(args, dict):
             all_sweep_group_keys = []
-            if isinstance(args, dict):
-                is_list_pretender = True
+            is_list_pretender = True
+            for key in args.keys():
+                if not key.startswith(IDX_INDICATOR):
+                    is_list_pretender = False
+            if is_list_pretender:
+                true_args = [None for _ in range(len(args.keys()))]
                 for key in args.keys():
-                    if not key.startswith(IDX_INDICATOR):
-                        is_list_pretender = False
-                if is_list_pretender:
-                    true_args = [None for _ in range(len(args.keys()))]
-                    for key in args.keys():
-                        true_args[int(key[len(IDX_INDICATOR):])] = args[key]
-                    return upsert_config(true_args, sweep_config, current_path, root_args)
-                else:
-                    all_upsert = []
-                    if DY_UPSERT in sweep_config:
-                        all_upsert = sweep_config.pop(DY_UPSERT)
-                    for key, val in sweep_config.items():
-                        if key.startswith(SWEEP_GROUP):
-                            all_sweep_group_keys.append(key)
-                            continue
-                        if key not in args:
-                            args[key] = None
-                        if isinstance(val, dict) or isinstance(val, list):
+                    true_args[int(key[len(IDX_INDICATOR):])] = args[key]
+                return upsert_config(true_args, sweep_config, current_path, root_args)
+            else:
+                all_upsert = []
+                if DY_UPSERT in sweep_config:
+                    all_upsert = sweep_config.pop(DY_UPSERT)
+                for key, val in sweep_config.items():
+                    if key.startswith(SWEEP_GROUP):
+                        all_sweep_group_keys.append(key)
+                        continue
+                    if key not in args:
+                        args[key] = None
+                    if isinstance(val, dict) or isinstance(val, list):
 
-                            if isinstance(val, dict) and DY_EVAL in val:
-                                if isinstance(val[DY_EVAL], str):
-                                    args[key] = dy.eval(
-                                        val[DY_EVAL])(root_args)
-                                else:
-                                    args[key] = dy.eval(
-                                        **val[DY_EVAL])(root_args)
-                                continue
+                        if isinstance(val, dict) and DY_EVAL in val:
+                            if isinstance(val[DY_EVAL], str):
+                                args[key] = dy.eval(
+                                    val[DY_EVAL])(root_args)
+                            else:
+                                args[key] = dy.eval(
+                                    **val[DY_EVAL])(root_args)
+                            continue
 
-                            new_args = upsert_config(
-                                args[key] if key in args else None, val, current_path + [str(key)], root_args)
-                            args[key] = new_args
-                        elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
-                            args[key] = val
-                        else:
-                            pat = f"{DY_EVAL}\((.*)\)"
-                            func_to_eval = re.search(pat, val).group(1)
-                            args[key] = dy.eval(func_to_eval)(args[key])
-            elif isinstance(sweep_config, str) and sweep_config.find(DY_EVAL) != -1:
-                pat = f"{DY_EVAL}\((.*)\)"
-                func_to_eval = re.search(pat, sweep_config).group(1)
-                return dy.eval(func_to_eval)(args)
-            else:
-                return sweep_config
+                        new_args = upsert_config(
+                            args[key] if key in args else None, val, current_path + [str(key)], root_args)
+                        args[key] = new_args
+                    elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
+                        args[key] = val
+                    else:
+                        pat = f"{DY_EVAL}\((.*)\)"
+                        func_to_eval = re.search(pat, val).group(1)
+                        args[key] = dy.eval(func_to_eval)(args[key])
             # sort all_sweep_group_keys
             all_sweep_group_keys.sort()
             for key in all_sweep_group_keys:
                 val = sweep_config[key]
                 new_args = upsert_config(
                     args, val, current_path + [f"{key}"], root_args)
                 args = new_args
@@ -390,15 +389,47 @@
                         args, val, current_path + [f"{DY_UPSERT}-{i}"], root_args)
                     args = new_args
             elif isinstance(all_upsert, dict):
                 for key, val in all_upsert.items():
                     new_args = upsert_config(
                         args, val, current_path + [f"{DY_UPSERT}-{key}"], root_args)
                     args = new_args
+        else:
+            if isinstance(sweep_config, str) and sweep_config.find(DY_EVAL) != -1:
+                pat = f"{DY_EVAL}\((.*)\)"
+                func_to_eval = re.search(pat, sweep_config).group(1)
+                sweep_config = dy.eval(func_to_eval)(args)
+
+            if isinstance(sweep_config, dict):
+                if DY_EVAL in sweep_config:
+                    if len(sweep_config.keys()) != 1:
+                        raise Exception(
+                            f"{DY_EVAL} should be the only key in the dict")
+                    args = dy.eval(
+                        **sweep_config[DY_EVAL])(root_args)
+                else:
+                    args = {}
+                    for key, val in sweep_config.items():
+                        args[key] = None
+                        args[key] = upsert_config(
+                            args[key], val, current_path=current_path + [str(key)], root_args=root_args)
+            elif isinstance(sweep_config, list):
+                args = []
+                for val in sweep_config:
+                    args.append(None)
+                    args[-1] = upsert_config(args[-1], val, current_path=current_path + [
+                                             str(len(args) - 1)], root_args=root_args)
+            else:
+                # a primitive type
+                args = sweep_config
+
         if len(current_path) == 0:
+            # print("Final config:")
+            # pprint(args)
+
             # Sanity check if any of the nested dicts contain special keys
             # If they do, then we need to throw an error
             # This is because we don't want to allow the user to specify
             # a sweep config that has a special key in it
             sanity_check_special_keys(args, current_path=current_path)
 
     except Exception as e:
@@ -410,26 +441,28 @@
                        str(current_path),)
             # update e so that it has the sweep_config
             # format sweep_config in a nice string using pprint
 
             e.args += ("Configuration to upsert: " +
                        json.dumps(sweep_config, indent=2),)
         raise e
-
+    # print("After upsert:")
+    # pprint(args)
+    # print("000000000000000-------000000000000000")
     return args
 
 
 def standardize_sweep_config(sweep_config: dict):
     global remaining_bunch
     config_copy = {k: copy.deepcopy(v) if isinstance(
         v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     flat, remaining_bunch = flatten_sweep_config(config_copy['parameters'])
     config_copy['parameters'] = compress_parameter_config(flat)
     global compression_mapping, value_compression_mapping
-    
+
     return config_copy, {'keys': compression_mapping, 'values': value_compression_mapping, 'remaining_bunch': remaining_bunch}
 
 
 def add_where_needed(
     base: th.Union[th.List, th.Dict],
     to_add: th.Union[th.List, th.Dict]
 ) -> th.Union[th.List, th.Dict]:
@@ -468,11 +501,15 @@
         compression_mapping = mapping['keys']
         value_compression_mapping = mapping['values']
         remaining_bunch = mapping['remaining_bunch']
     config_copy = {k: copy.deepcopy(v) if isinstance(
         v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     config_copy = unflatten_sweep_config(
         decompress_parameter_config(config_copy))
-    
+
     ret = add_where_needed(config_copy, remaining_bunch)
 
+    # print("This is what I'm trying to upsert:")
+
+    # pprint(ret)
+
     return ret
```

### Comparing `dysweep-0.0.5/dysweep/wandbX.py` & `dysweep-0.0.6/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.5/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.6/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.5/setup.py` & `dysweep-0.0.6/setup.py`

 * *Files identical despite different names*

