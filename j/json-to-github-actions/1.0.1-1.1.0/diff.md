# Comparing `tmp/json-to-github-actions-1.0.1.tar.gz` & `tmp/json-to-github-actions-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-to-github-actions-1.0.1.tar", last modified: Tue May 30 00:50:34 2023, max compression
+gzip compressed data, was "json-to-github-actions-1.1.0.tar", last modified: Sat Jun  3 11:04:34 2023, max compression
```

## Comparing `json-to-github-actions-1.0.1.tar` & `json-to-github-actions-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-30 00:50:34.047896 json-to-github-actions-1.0.1/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-05-30 00:50:34.047764 json-to-github-actions-1.0.1/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1992 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-30 00:50:34.047586 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4188 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/json_to_github_actions.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-30 00:50:34.047932 json-to-github-actions-1.0.1/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:04:34.475592 json-to-github-actions-1.1.0/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-06-03 11:04:34.475478 json-to-github-actions-1.1.0/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1992 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 11:04:34.475290 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4587 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/json_to_github_actions.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 11:04:34.475624 json-to-github-actions-1.1.0/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-06-03 11:04:34.000000 json-to-github-actions-1.1.0/setup.py
```

### Comparing `json-to-github-actions-1.0.1/PKG-INFO` & `json-to-github-actions-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-to-github-actions
-Version: 1.0.1
+Version: 1.1.0
 Description-Content-Type: text/markdown
 
 # JSON 轉 GitHub Actions YAML
 ```
 🐔動機: 全球免費20 VMs運算，有感試用，可以把 python 或 julia 放到 github actions 算 
 💣地雷: 格式轉換會存在很多 bugs, 要先生最終無 bugs .yml 才反推轉換的 .py 此套件程式碼
 🧪實驗: Roy julia套件清物聯網資料已經分散兩台 VMs (每個4GB .zip處理55分鐘)運算成功
```

### Comparing `json-to-github-actions-1.0.1/README.md` & `json-to-github-actions-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `json-to-github-actions-1.0.1/json_to_github_actions.egg-info/PKG-INFO` & `json-to-github-actions-1.1.0/json_to_github_actions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-to-github-actions
-Version: 1.0.1
+Version: 1.1.0
 Description-Content-Type: text/markdown
 
 # JSON 轉 GitHub Actions YAML
 ```
 🐔動機: 全球免費20 VMs運算，有感試用，可以把 python 或 julia 放到 github actions 算 
 💣地雷: 格式轉換會存在很多 bugs, 要先生最終無 bugs .yml 才反推轉換的 .py 此套件程式碼
 🧪實驗: Roy julia套件清物聯網資料已經分散兩台 VMs (每個4GB .zip處理55分鐘)運算成功
```

### Comparing `json-to-github-actions-1.0.1/json_to_github_actions.py` & `json-to-github-actions-1.1.0/json_to_github_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# json_to_github_actions.py
 import argparse
 import os
 
 import yaml
 
 import json
 
@@ -46,26 +45,26 @@
                 "strategy": {
                     "max-parallel": int(json_dict["max_parallel"]),
                     "matrix": {"parameters": json_dict["json_parameters"]}
                 },
                 "steps": [
                     {
                         "name": f"Checkout repository and setup {env['language']} environment",
-                        "uses": "actions/checkout@v2",
+                        "uses": "actions/checkout@v3",
                         "with": {
                             "repository": json_dict["repo_url"].replace("https://github.com/", ""),
                             "ref": "main"
                         }
                     },
                 ]
             }
             if env["language"] == "python":
                 job_details["steps"].append({
                     "name": "SetUp Python",
-                    "uses": "actions/setup-python@v2",
+                    "uses": "actions/setup-python@v4",
                     "with": {
                         "python-version": env["version"]
                     }
                 })
             elif env["language"] == "julia":
                 job_details["steps"].append({
                     "name": "Set up Julia",
@@ -74,34 +73,43 @@
                         "version": env["version"]
                     }
                 })
             job_details["steps"].append({
                 "name": "Run script",
                 "run": f"{install_command} && cd {json_dict['script_dir'].strip('/')} && {language_command} {steps_params_run}"
             })
+            job_details["steps"].append({
+                "name": "Upload artifact",
+                "uses": "actions/upload-artifact@v3",
+                "with": {
+                    "name": f'id_${{{{github.run_id}}}}',
+                    "path": json_dict['output_directory']
+                }
+            })
             jobs[job_name] = job_details
         return jobs
 
     execution_environment_jobs = create_execution_environment_jobs(json_dict["execution_environment"])
-    actions_base_structure["name"] = json_dict['script_name']
+    actions_base_structure["name"] = json_dict['script_name'].split('.')[0] + '.yml'
     actions_base_structure["jobs"].update(execution_environment_jobs)
 
     yaml_data = yaml.dump(actions_base_structure, sort_keys=False)
 
     # ensure the directory of yaml_file exists
     if cli_params is not None:
-        os.makedirs(os.path.dirname(cli_params.yaml_file), exist_ok=True)
+        if os.path.dirname(cli_params.yaml_file) != '':
+            os.makedirs(os.path.dirname(cli_params.yaml_file), exist_ok=True)
 
     return yaml_data
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description="Convert JSON to a GitHub Actions YAML file.")
-    parser.add_argument("--json_file", type=str, help="Path to the input JSON file.")
-    parser.add_argument("--yaml_file", type=str, help="Path to the output YAML file.")
+    parser.add_argument("--json_file", type=str, help="Path to the input JSON file.", required=True)
+    parser.add_argument("--yaml_file", type=str, help="Path to the output YAML file.", required=True)
     return parser.parse_args()
 
 
 def main():
     args = parse_arguments()
 
     with open(args.json_file, "r") as f:
```

### Comparing `json-to-github-actions-1.0.1/setup.py` & `json-to-github-actions-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="json-to-github-actions",
-    version="1.0.1",
+    version="1.1.0",
     packages=find_packages(),
     py_modules=['json_to_github_actions'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'json_to_github_actions = json_to_github_actions:main',
         ],
```

