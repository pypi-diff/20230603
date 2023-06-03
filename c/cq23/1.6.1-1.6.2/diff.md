# Comparing `tmp/cq23-1.6.1.tar.gz` & `tmp/cq23-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.6.1.tar", last modified: Wed May 31 12:48:51 2023, max compression
+gzip compressed data, was "cq23-1.6.2.tar", last modified: Sat Jun  3 10:14:50 2023, max compression
```

## Comparing `cq23-1.6.1.tar` & `cq23-1.6.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 12:48:51.274707 cq23-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-31 12:48:42.000000 cq23-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 12:48:42.000000 cq23-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-31 12:48:51.274707 cq23-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.270707 cq23-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.270707 cq23-1.6.1/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 12:48:42.000000 cq23-1.6.1/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 12:48:42.000000 cq23-1.6.1/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 12:48:42.000000 cq23-1.6.1/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.270707 cq23-1.6.1/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 12:48:42.000000 cq23-1.6.1/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.270707 cq23-1.6.1/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-31 12:48:42.000000 cq23-1.6.1/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 12:48:51.000000 cq23-1.6.1/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 12:48:42.000000 cq23-1.6.1/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 12:48:42.000000 cq23-1.6.1/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-31 12:48:42.000000 cq23-1.6.1/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 12:48:42.000000 cq23-1.6.1/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-31 12:48:42.000000 cq23-1.6.1/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-31 12:48:42.000000 cq23-1.6.1/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:51.274707 cq23-1.6.1/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:48:42.000000 cq23-1.6.1/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 12:48:42.000000 cq23-1.6.1/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-03 10:14:50.440699 cq23-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-03 10:14:42.000000 cq23-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 10:14:42.000000 cq23-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-03 10:14:50.440699 cq23-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.436699 cq23-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-03 10:14:42.000000 cq23-1.6.2/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-03 10:14:42.000000 cq23-1.6.2/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-03 10:14:42.000000 cq23-1.6.2/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 10:14:50.000000 cq23-1.6.2/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-03 10:14:42.000000 cq23-1.6.2/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-03 10:14:42.000000 cq23-1.6.2/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-03 10:14:42.000000 cq23-1.6.2/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:50.440699 cq23-1.6.2/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 10:14:42.000000 cq23-1.6.2/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-03 10:14:42.000000 cq23-1.6.2/src/zip/command.py
```

### Comparing `cq23-1.6.1/PKG-INFO` & `cq23-1.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.6.1
+Version: 1.6.2
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.6.1/setup.cfg` & `cq23-1.6.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.6.1
+version = 1.6.2
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -19,14 +19,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	docker>=6.0.1
 	boto3>=1.26.143
+	colorama>=0.4.6
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	cq23 = main.command:route_command
```

### Comparing `cq23-1.6.1/src/admin/aws.py` & `cq23-1.6.2/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/admin/builder.py` & `cq23-1.6.2/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/admin/worker.py` & `cq23-1.6.2/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/check/command.py` & `cq23-1.6.2/src/check/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import shutil
 import subprocess
 
 import docker
+from colorama import Fore
+from colorama import init as color_init
 
 
 def is_git_installed():
     try:
         subprocess.run(["git", "--version"], capture_output=True, check=True)
         return True
     except (FileNotFoundError, subprocess.CalledProcessError):
@@ -26,21 +28,28 @@
     root_directory = os.path.abspath(os.sep)
     total, used, free = shutil.disk_usage(root_directory)
     free_gb = free // (2**30)  # Convert bytes to GB
     return free_gb >= minimum_space_gb
 
 
 def check(*args):
+    color_init(autoreset=True)
     git_installed = is_git_installed()
     docker_installed = is_docker_installed()
     enough_disk_space = has_enough_disk_space(5)
 
-    boolean_map = {True: "Yes", False: "No"}
+    boolean_map = {True: Fore.GREEN + "Yes", False: Fore.RED + "No"}
 
     print(f"Git installed: {boolean_map[git_installed]}")
-    print(f"Docker installed: {boolean_map[docker_installed]}")
+    print(f"Docker installed and running: {boolean_map[docker_installed]}")
     print(f"Enough disk space: {boolean_map[enough_disk_space]}")
 
     if git_installed and docker_installed and enough_disk_space:
-        print("You are all set!")
+        print(Fore.LIGHTGREEN_EX + "You are all set!")
     else:
-        print("Some requirements are not met. Check above.")
+        print(Fore.YELLOW + "Some requirements are not met.")
+        if not docker_installed:
+            print(
+                Fore.YELLOW
+                + "-> If you have installed Docker Desktop, you need to make sure it's running. Search "
+                "for Docker in your applications and open it. That will start Docker on your computer."
+            )
```

### Comparing `cq23-1.6.1/src/cleanup/command.py` & `cq23-1.6.2/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/cq23.egg-info/PKG-INFO` & `cq23-1.6.2/src/cq23.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.6.1
+Version: 1.6.2
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.6.1/src/cq23.egg-info/SOURCES.txt` & `cq23-1.6.2/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/main/command.py` & `cq23-1.6.2/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/main/utils.py` & `cq23-1.6.2/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/new_client/command.py` & `cq23-1.6.2/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/run_game/command.py` & `cq23-1.6.2/src/run_game/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         src_file = os.path.join(src_dir, filename)
         dst_file = os.path.join(dst_dir, filename)
         # Copy the file to the destination directory
         shutil.copy2(src_file, dst_file)
 
 
 def run_game(*args):
+    docker_tools.ensure_docker_client_exists()
     game_files_dir = ".game_files"
     gcs_folder_name = "gcs"
     gcs_repo = "https://github.com/CALED-Team/game-communication-system.git"
 
     docker_tools.check_dockerfile_exists()
     docker_tools.build_and_tag_image(docker_tools.get_client_image_tag())
```

### Comparing `cq23-1.6.1/src/run_game/docker_tools.py` & `cq23-1.6.2/src/run_game/docker_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 import os
 import shutil
 
 import docker
-from docker.errors import APIError, NotFound
+from docker.errors import APIError, DockerException, NotFound
 
 AWS_REGION = "ap-southeast-2"
 ECR_REGISTRY = "public.ecr.aws/z3i0q5x8"
 GAME_SERVER_ECR_REPO = "cq-game-server"
 
-DOCKER_CLIENT = docker.from_env()
+DOCKER_CLIENT = None
+
+
+def ensure_docker_client_exists():
+    global DOCKER_CLIENT
+    try:
+        DOCKER_CLIENT = docker.from_env()
+    except DockerException:
+        print(
+            "Docker not found! Either not installed or not running. If you have installed Docker Desktop make sure to "
+            'open it first. Search "Docker Desktop" in your applications.'
+        )
+        exit(1)
 
 
 def get_server_image_tag():
     return f"{ECR_REGISTRY}/{GAME_SERVER_ECR_REPO}:latest"
 
 
 def get_client_image_tag():
```

### Comparing `cq23-1.6.1/src/run_game/gcs.py` & `cq23-1.6.2/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.6.1/src/zip/command.py` & `cq23-1.6.2/src/zip/command.py`

 * *Files identical despite different names*

