# Comparing `tmp/naapc-1.7.0.tar.gz` & `tmp/naapc-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naapc-1.7.0.tar", last modified: Wed May 31 11:43:33 2023, max compression
+gzip compressed data, was "naapc-1.7.1.tar", last modified: Sat Jun  3 04:04:41 2023, max compression
```

## Comparing `naapc-1.7.0.tar` & `naapc-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.530043 naapc-1.7.0/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.7.0/LICENSE
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-31 11:43:31.529041 naapc-1.7.0/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.7.0/README.md
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-31 11:41:06.000000 naapc-1.7.0/pyproject.toml
--rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-31 11:43:31.530043 naapc-1.7.0/setup.cfg
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.395327 naapc-1.7.0/src/
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.453014 naapc-1.7.0/src/naapc/
--rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-31 11:41:06.000000 naapc-1.7.0/src/naapc/__init__.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.7.0/src/naapc/nconfig.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6980 2023-05-31 11:40:32.000000 naapc-1.7.0/src/naapc/ndict.py
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.509041 naapc-1.7.0/src/naapc.egg-info/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/requires.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/top_level.txt
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.518042 naapc-1.7.0/test/
--rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.7.0/test/test.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-06-03 04:04:41.170426 naapc-1.7.1/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.7.1/LICENSE
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-06-03 04:04:41.168426 naapc-1.7.1/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.7.1/README.md
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-06-03 04:03:45.000000 naapc-1.7.1/pyproject.toml
+-rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-06-03 04:04:41.170426 naapc-1.7.1/setup.cfg
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-06-03 04:04:41.038958 naapc-1.7.1/src/
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-06-03 04:04:41.094932 naapc-1.7.1/src/naapc/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-06-03 04:03:45.000000 naapc-1.7.1/src/naapc/__init__.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.7.1/src/naapc/nconfig.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6998 2023-06-03 04:01:25.000000 naapc-1.7.1/src/naapc/ndict.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-06-03 04:04:41.147703 naapc-1.7.1/src/naapc.egg-info/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-06-03 04:04:40.000000 naapc-1.7.1/src/naapc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-06-03 04:04:41.000000 naapc-1.7.1/src/naapc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-06-03 04:04:40.000000 naapc-1.7.1/src/naapc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-06-03 04:04:40.000000 naapc-1.7.1/src/naapc.egg-info/requires.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-06-03 04:04:40.000000 naapc-1.7.1/src/naapc.egg-info/top_level.txt
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-06-03 04:04:41.157702 naapc-1.7.1/test/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.7.1/test/test.py
```

### Comparing `naapc-1.7.0/LICENSE` & `naapc-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naapc-1.7.0/PKG-INFO` & `naapc-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.7.0
+Version: 1.7.1
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.7.0/README.md` & `naapc-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `naapc-1.7.0/pyproject.toml` & `naapc-1.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naapc"
-version = "1.7.0"
+version = "1.7.1"
 description = "Nested Automated Argument Parsing Configuration (NAAPC)."
 readme = "README.md"
 authors = [{name = "Bai Huanyu", email = "eiphnix@gmail.com"}]
 license = {file = "LICENSE"}
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,15 +19,15 @@
 dependencies = ["pyyaml"]
 requires-python = "==3.10.*"
 
 [project.urls]
 repository = "https://github.com/eiphy/naapc"
 
 [tool.bumpver]
-current_version = "1.7.0"
+current_version = "1.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `naapc-1.7.0/src/naapc/nconfig.py` & `naapc-1.7.1/src/naapc/nconfig.py`

 * *Files identical despite different names*

### Comparing `naapc-1.7.0/src/naapc/ndict.py` & `naapc-1.7.1/src/naapc/ndict.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         if isinstance(dictionary, ndict):
             self._d = dictionary.raw_dict
         elif isinstance(dictionary, dict):
             self._d = dictionary
         else:
             raise TypeError(f"Unexpected type {type(dictionary)}.")
 
-        assert isinstance(
-            delimiter, str
-        ), f"delimiter must be str, but recieved {type(delimiter)}"
+        assert isinstance(delimiter, str), f"delimiter must be str, but recieved {type(delimiter)}"
         self.delimiter = delimiter
         self._update_flatten()
 
     @classmethod
     def from_flatten_dict(cls, flatten_dict: dict, delimiter=";") -> ndict:
         """Generate nested from flattened dictionary.
         The delimiter must be the same!
@@ -49,16 +47,15 @@
 
     def is_matched(self, query: dict, missing_method: str = "ignore", **kwargs) -> bool:
         """Test if the dictionary is the queried one.
 
         Syntax:
             1. Normal path-value pair: {path: value}.
             2. Query expression: {path: !QUERY [python expression returns boolean results]}. The
-                expression can use d: the dictionary, path: the query path and any other input
-                kwargs.
+                expression can use d: the dictionary, path: the query path and kwargs.
 
         Args:
             query (dict): query dictionary.
             missing_method (str): actions when the path is missing from the dictionary. Support:
             ['ignore', 'false', 'error'].
         Returns:
             (bool): if the dictionary is the queried one.
@@ -72,19 +69,15 @@
                 if missing_method == "ignore":
                     continue
                 elif missing_method == "false":
                     return False
                 elif missing_method == "error":
                     raise KeyError(f"Wrong path: {path}.")
 
-            if (
-                isinstance(v, str)
-                and v.startswith("!QUERY")
-                and not eval(v[6:].strip())
-            ):
+            if isinstance(v, str) and v.startswith("!QUERY") and not eval(v[6:].strip()):
                 return False
             if self[path] != v:
                 return False
         return True
 
     ### internal manipulation ###
     def _update_flatten(self) -> None:
@@ -106,16 +99,18 @@
         self._flatten_dict = flatten
         self._paths = paths
 
     ### getters ###
     def get(self, path, default=None):
         try:
             return self.__getitem__(path)
-        except Exception:
+        except KeyError:
             return default
+        except Exception as e:
+            raise e
 
     def compare_dict(self, other):
         assert isinstance(other, ndict)
         output = {}
         for path, v in self._flatten_dict.items():
             other_v = other.get(path, None)
             if other_v != v:
@@ -135,43 +130,45 @@
     @property
     def flatten_dict(self):
         return deepcopy(self._flatten_dict)
 
     @property
     def flatten_dict_split(self):
         return deepcopy(
-            [
-                ndict.from_flatten_dict({p: v}).raw_dict
-                for p, v in self.flatten_dict.items()
-            ]
+            [ndict.from_flatten_dict({p: v}).raw_dict for p, v in self.flatten_dict.items()]
         )
 
     @property
     def paths(self):
         return deepcopy(self._paths)
 
     @property
     def size(self):
         return len(self._flatten_dict)
 
     ### setters & updators ###
-    def update(self, d, ignore_missing_path=False, ignore_none=True):
+    def update(self, d, ignore_missing_path=False, ignore_none=False):
         if isinstance(d, dict):
             d = ndict(d, delimiter=self.delimiter)._flatten_dict
         elif isinstance(d, ndict):
             d = d._flatten_dict
         else:
             raise TypeError(f"Unexpected type {type(d)}")
 
         for path, v in d.items():
-            if (path not in self.paths and ignore_missing_path) or (
-                ignore_none and v is None
-            ):
-                continue
-            self[path] = v
+            try:
+                if ignore_none and v is None:
+                    continue
+                self[path] = v
+            except KeyError as e:
+                if ignore_missing_path:
+                    continue
+                raise e
+            except Exception as e:
+                raise e
 
     ### iterations ###
     def items(self):
         return self._d.items()
 
     def keys(self):
         return self._d.keys()
```

### Comparing `naapc-1.7.0/src/naapc.egg-info/PKG-INFO` & `naapc-1.7.1/src/naapc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.7.0
+Version: 1.7.1
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.7.0/test/test.py` & `naapc-1.7.1/test/test.py`

 * *Files identical despite different names*

