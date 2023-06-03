# Comparing `tmp/bare_estate-0.2.tar.gz` & `tmp/bare_estate-0.3.tar.gz`

## Comparing `bare_estate-0.2.tar` & `bare_estate-0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bare_estate-0.2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bare_estate-0.2/bare_estate/__init__.py
--rwxr-xr-x   0        0        0     1115 2020-02-02 00:00:00.000000 bare_estate-0.2/bare_estate/cli.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 bare_estate-0.2/bare_estate/commands.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bare_estate-0.2/bare_estate/config.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 bare_estate-0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bare_estate-0.2/LICENSE
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bare_estate-0.2/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bare_estate-0.2/pyproject.toml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 bare_estate-0.2/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bare_estate-0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 bare_estate-0.3/actions.mk
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/cli.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/commands.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/config.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 bare_estate-0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bare_estate-0.3/LICENSE
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bare_estate-0.3/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 bare_estate-0.3/pyproject.toml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 bare_estate-0.3/PKG-INFO
```

### Comparing `bare_estate-0.2/bare_estate/cli.py` & `bare_estate-0.3/bare_estate/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 import sys
 
 try:
     from bare_estate.commands import cli_args, log_err, init, clone, git, NotARepositoryError
 except ImportError:
     from commands import cli_args, log_err, init, clone, git, NotARepositoryError
 
@@ -17,15 +16,15 @@
             status = clone()
         else:
             status = git()
 
     except FileNotFoundError:
         log_err("Error: the repository has not been initialized yet.")
         log_err("You can create a new repository using the command:\n")
-        log_err("bare init")
+        log_err("estate init")
         status = 2
 
     except NotARepositoryError as error:
         message = error.strerror
         log_err(message)
         status = 3
 
@@ -35,11 +34,7 @@
         status = 3
 
     except IndexError:
         log_err("Error: no command was provided to git")
         status = 4
 
     return status
-
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `bare_estate-0.2/bare_estate/commands.py` & `bare_estate-0.3/bare_estate/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import os
 import sys
 import subprocess as sp
 import errno
 import tempfile
 
-try:
-    from bare_estate.config import configs, HOME
-except ImportError:
-    from config import configs, HOME
+from bare_estate.config import configs
 
 
 class NotARepositoryError(NotADirectoryError):
     pass
 
 
 cli_args = sys.argv[1:]
 bare_cmd = ["git",
             f"--git-dir={configs['history_location']}",
-            f"--work-tree={HOME}"]
+            f"--work-tree={configs['base_directory']}"]
 
 
 log_err = lambda message: print(message, file=sys.stderr)
 
 
 def validate_file_type(file_stats):
     file_entry, file_type = file_stats
@@ -77,27 +74,26 @@
 def clone():
     status = 1
     repository = cli_args[1]
 
     with tempfile.TemporaryDirectory() as tmp_dir:
         clone_cmd = ["git",
                      "clone",
-                     "--bare",
                      "--quiet",
                      f"--separate-git-dir={configs['history_location']}",
                      repository,
                      f"{tmp_dir}/dotfiles"]
 
         rsync_cmd = ["rsync",
                      "--recursive",
                      "--verbose",
                      "--exclude",
                      ".git",
                      f"{tmp_dir}/dotfiles/",
-                     f"{HOME}/"]
+                     f"{configs['base_directory']}/"]
 
         config_cmd = [*bare_cmd, "config", "status.showUntrackedFiles", "no"]
 
         status = sp.run(clone_cmd).returncode
         status += sp.run(rsync_cmd).returncode
         status += sp.run(config_cmd).returncode
```

### Comparing `bare_estate-0.2/LICENSE` & `bare_estate-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bare_estate-0.2/README.md` & `bare_estate-0.3/README.md`

 * *Files identical despite different names*

### Comparing `bare_estate-0.2/pyproject.toml` & `bare_estate-0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 [tool.hatch.build]
 exclude = [
     "tests/",
     "Makefile",
     "dev_requirements.txt",
     ".?*",
+    "estate",
 ]
 
 [project]
 name = "bare_estate"
-version = "0.2"
+version = "0.3"
 authors = [
     { name="Lucas L. S. Haine", email="lucaslshaine@gmail.com" },
 ]
 description = "Manage your dotfiles seamlessly with a bare repo"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bare_estate-0.2/PKG-INFO` & `bare_estate-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bare_estate
-Version: 0.2
+Version: 0.3
 Summary: Manage your dotfiles seamlessly with a bare repo
 Project-URL: Homepage, https://github.com/llucasls/bare-estate
 Author-email: "Lucas L. S. Haine" <lucaslshaine@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
```

