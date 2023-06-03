# Comparing `tmp/animedata-0.3.8.tar.gz` & `tmp/animedata-0.3.9.tar.gz`

## Comparing `animedata-0.3.8.tar` & `animedata-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/dict_checking.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/lib_interactions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/metadata.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/saving_process.py
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/resources/animedata_source.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/test_dict_checking.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/test_lib_interaction.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 animedata-0.3.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.8/LICENSE
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.8/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 animedata-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 animedata-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/common/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/common/dict_checking.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/common/lib_interactions.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/common/metadata.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/common/saving_process.py
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/resources/animedata_source.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/tests/test_dict_checking.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 animedata-0.3.9/animedata/tests/test_lib_interaction.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 animedata-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.9/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 animedata-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 animedata-0.3.9/PKG-INFO
```

### Comparing `animedata-0.3.8/animedata/common/dict_checking.py` & `animedata-0.3.9/animedata/common/dict_checking.py`

 * *Files identical despite different names*

### Comparing `animedata-0.3.8/animedata/common/lib_interactions.py` & `animedata-0.3.9/animedata/common/lib_interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import urllib.request
 import warnings
 import json
-import importlib.resources
-from animedata.common.metadata import ad_table, dir_path
+from animedata.common.metadata import ad_table
 
 
 def get_ad_lib(branch: str = "main"):
     """Download and replace local AnimeData library from Github.
 
     Args:
         branch (str, optional): select the target branch.
@@ -38,18 +37,17 @@
     Returns:
         dict: dictionnary containg library data
     """
     if ad_source:
         target_file = ad_table["source_file_path"]
     else:
         target_file = ad_table["local_file_path"]
-        with open(target_file, encoding="utf-8") as ad_json:
-            ad_dict = json.load(ad_json)
-            print(ad_dict)
-        return ad_dict
+    with open(target_file, encoding="utf-8") as ad_json:
+        ad_dict = json.load(ad_json)
+    return ad_dict
 
 
 def show_lib_content():
     """Show the version of the library and the animes available."""
     # STATUS : OK
     ad_dict = get_ad_lib_content()
     print("AnimeData library version :",
```

### Comparing `animedata-0.3.8/animedata/common/metadata.py` & `animedata-0.3.9/animedata/common/metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import importlib.metadata
 import os
+import animedata
 
 ad_version = importlib.metadata.version("animedata")
-dir_path = os.path.dirname(__file__)
+dir_path = os.path.dirname(animedata.__file__)
 ad_table = {
     "repository_url":
     "https://raw.githubusercontent.com/swarthur/animedata/",
     "source_file_name" : "animedata_source.json",
     "local_file_name" : "animedata_local.json",
-    "source_file_path": "..\\resources\\animedata_source.json",
-    "local_file_path": "..\\resources\\animedata_local.json",
+    "source_file_path": os.path.join(dir_path, "resources\\animedata_source.json"),
+    "local_file_path": os.path.join(dir_path, "resources\\animedata_local.json"),
     "anime_name": "anime_name",
     "seasons": "seasons",
     "episode_duration": "episode_duration",
     "episode_release_date": "episode_release_date",
     "episode_name": "episode_name"}
```

### Comparing `animedata-0.3.8/animedata/common/saving_process.py` & `animedata-0.3.9/animedata/common/saving_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from animedata.common.metadata import dir_path, ad_table, ad_version
+from animedata.common.metadata import ad_table, ad_version
 from animedata.common.dict_checking import check_dict
 import json
 import warnings
-import os
 
 
 def save_json(anime_dict: dict):
     """Save a dictionnary into a json file.
 
     Args:
         anime_dict (dict): Dictionnary containing anime's data.
```

### Comparing `animedata-0.3.8/animedata/resources/animedata_source.json` & `animedata-0.3.9/animedata/resources/animedata_source.json`

 * *Files identical despite different names*

### Comparing `animedata-0.3.8/animedata/tests/test_lib_interaction.py` & `animedata-0.3.9/animedata/tests/test_lib_interaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import unittest
-import os
 from animedata.common import lib_interactions as adlib
 from animedata.common import saving_process as adsave
 from animedata.common import metadata as admeta
 from animedata.common import dict_checking as adcheck
 
 
 class test_lib_interaction(unittest.TestCase):
     def test_get_ad_lib(self):
         adlib.get_ad_lib()
-        self.assertTrue(os.path.isfile(admeta.ad_table["source_file_path"]),
+        self.assertTrue(admeta.ad_table["source_file_path"],
                         "Source file not found !")
         
     def test_get_ad_lib_content(self):
         adlib.get_ad_lib()
         self.assertTrue(adcheck.check_dict(adlib.get_ad_lib_content(True))[0])
         
     def test_save_json(self):
```

### Comparing `animedata-0.3.8/LICENSE` & `animedata-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `animedata-0.3.8/README.md` & `animedata-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `animedata-0.3.8/pyproject.toml` & `animedata-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 2020 222f 6469 7374 222c 0d0a 2020 222f    "/dist",..  "/
 00000080: 2e67 6974 222c 0d0a 2020 222e 6769 7469  .git",..  ".giti
 00000090: 676e 6f72 6522 0d0a 2020 5d0d 0a69 6e63  gnore"..  ]..inc
 000000a0: 6c75 6465 203d 205b 0d0a 2020 2261 6e69  lude = [..  "ani
 000000b0: 6d65 6461 7461 2f2a 220d 0a5d 0d0a 0d0a  medata/*"..]....
 000000c0: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 000000d0: 3d20 2261 6e69 6d65 6461 7461 220d 0a76  = "animedata"..v
-000000e0: 6572 7369 6f6e 203d 2022 302e 332e 3822  ersion = "0.3.8"
+000000e0: 6572 7369 6f6e 203d 2022 302e 332e 3922  ersion = "0.3.9"
 000000f0: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
 00000100: 7b6e 616d 653d 2273 7761 7274 6875 7222  {name="swarthur"
 00000110: 7d0d 0a5d 0d0a 6465 7363 7269 7074 696f  }..]..descriptio
 00000120: 6e20 3d20 224f 7065 6e2d 736f 7572 6365  n = "Open-source
 00000130: 206c 6962 7261 7279 2063 6f6e 7461 696e   library contain
 00000140: 696e 6720 7061 636b 6167 6520 6162 6f75  ing package abou
 00000150: 7420 616e 696d 6573 2f73 6572 6965 7320  t animes/series
```

### Comparing `animedata-0.3.8/PKG-INFO` & `animedata-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animedata
-Version: 0.3.8
+Version: 0.3.9
 Summary: Open-source library containing package about animes/series and including a built-in utility.
 Project-URL: Github, https://github.com/swarthur/animedata
 Project-URL: Bug, https://github.com/swarthur/animedata/issues
 Author: swarthur
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

