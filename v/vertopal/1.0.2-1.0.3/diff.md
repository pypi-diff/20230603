# Comparing `tmp/vertopal-1.0.2.tar.gz` & `tmp/vertopal-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertopal-1.0.2.tar", last modified: Tue Mar 28 14:30:17 2023, max compression
+gzip compressed data, was "vertopal-1.0.3.tar", last modified: Sat Jun  3 12:48:04 2023, max compression
```

## Comparing `vertopal-1.0.2.tar` & `vertopal-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:17.404350 vertopal-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-28 14:30:01.000000 vertopal-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-28 14:30:17.404350 vertopal-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-28 14:30:01.000000 vertopal-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-28 14:30:01.000000 vertopal-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 14:30:17.404350 vertopal-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-28 14:30:01.000000 vertopal-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:17.404350 vertopal-1.0.2/vertopal/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:17.404350 vertopal-1.0.2/vertopal/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:17.404350 vertopal-1.0.2/vertopal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-28 14:30:01.000000 vertopal-1.0.2/vertopal/vertopal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 14:30:17.404350 vertopal-1.0.2/vertopal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 14:30:17.000000 vertopal-1.0.2/vertopal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:48:04.146772 vertopal-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-03 12:47:54.000000 vertopal-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-03 12:48:04.146772 vertopal-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-03 12:47:54.000000 vertopal-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-03 12:47:54.000000 vertopal-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:48:04.146772 vertopal-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 12:47:54.000000 vertopal-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:48:04.146772 vertopal-1.0.3/vertopal/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:48:04.146772 vertopal-1.0.3/vertopal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:48:04.146772 vertopal-1.0.3/vertopal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-03 12:47:54.000000 vertopal-1.0.3/vertopal/vertopal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:48:04.146772 vertopal-1.0.3/vertopal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 12:48:04.000000 vertopal-1.0.3/vertopal.egg-info/top_level.txt
```

### Comparing `vertopal-1.0.2/LICENSE` & `vertopal-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vertopal-1.0.2/PKG-INFO` & `vertopal-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertopal
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert your files in terminal using Vertopal API
 Home-page: https://github.com/vertopal/vertopal-cli
 Author-email: Vertopal <contact@vertopal.com>
 License: MIT
 Project-URL: Homepage, https://www.vertopal.com
 Project-URL: Funding, https://www.vertopal.com/en/donate
 Project-URL: Source, https://github.com/vertopal/vertopal-cli
@@ -20,31 +20,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vertopal-CLI
 
-**Vertopal-CLI** is a small, yet powerful utility for converting
-digital files to a variety of file formats
-using [Vertopal](https://www.vertopal.com) public API.
+**Vertopal-CLI** is a small yet powerful utility that allows you to convert
+digital files into various formats using the
+[Vertopal public API](https://www.vertopal.com/en/developer/api).
 
 You can use Vertopal-CLI by either *terminal commands* or
-*importing as Python package*.
+*importing as a Python package*.
 
 ## Installing Vertopal-CLI
 
 Vertopal-CLI is available on [PyPI](https://pypi.org/project/vertopal/):
 
 ```bash
 python -m pip install vertopal
 ```
 
 You can also download the most recent version of Vertopal-CLI binaries for
-**MacOS**, **Windows**, and **Linux** from the
+**macOS**, **Windows**, and **Linux** from the
 [releases page](https://github.com/vertopal/vertopal-cli/releases/latest) or
 the [product page](https://www.vertopal.com/en/product/cli).
 
 ### Installer
 
 An automatic installer is available for each different platform. It will run an
 install script that downloads and copy Vertopal-CLI binaries to the correct
@@ -55,17 +55,25 @@
 ```bash
 curl https://run.vertopal.com/cli/macos | bash
 ```
 
 On Windows using PowerShell:
 
 ```bash
-curl.exe https://run.vertopal.com/cli/windows | iex
+(curl https://run.vertopal.com/cli/windows).Content | iex
 ```
 
+If you are getting any **UnauthorizedAccess** error, then start Windows
+PowerShell with the "Run as administrator" option and run
+`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine`.
+Now re-run the above installation command. To change the
+[*Execution Policies*](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies)
+to its default, you can run
+`Set-ExecutionPolicy -ExecutionPolicy Default -Scope LocalMachine`.
+
 Using Linux Terminal:
 
 ```bash
 curl https://run.vertopal.com/cli/linux | bash
 ```
 
 ## Using Vertopal-CLI
```

### Comparing `vertopal-1.0.2/README.md` & `vertopal-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Vertopal-CLI
 
-**Vertopal-CLI** is a small, yet powerful utility for converting
-digital files to a variety of file formats
-using [Vertopal](https://www.vertopal.com) public API.
+**Vertopal-CLI** is a small yet powerful utility that allows you to convert
+digital files into various formats using the
+[Vertopal public API](https://www.vertopal.com/en/developer/api).
 
 You can use Vertopal-CLI by either *terminal commands* or
-*importing as Python package*.
+*importing as a Python package*.
 
 ## Installing Vertopal-CLI
 
 Vertopal-CLI is available on [PyPI](https://pypi.org/project/vertopal/):
 
 ```bash
 python -m pip install vertopal
 ```
 
 You can also download the most recent version of Vertopal-CLI binaries for
-**MacOS**, **Windows**, and **Linux** from the
+**macOS**, **Windows**, and **Linux** from the
 [releases page](https://github.com/vertopal/vertopal-cli/releases/latest) or
 the [product page](https://www.vertopal.com/en/product/cli).
 
 ### Installer
 
 An automatic installer is available for each different platform. It will run an
 install script that downloads and copy Vertopal-CLI binaries to the correct
@@ -31,17 +31,25 @@
 ```bash
 curl https://run.vertopal.com/cli/macos | bash
 ```
 
 On Windows using PowerShell:
 
 ```bash
-curl.exe https://run.vertopal.com/cli/windows | iex
+(curl https://run.vertopal.com/cli/windows).Content | iex
 ```
 
+If you are getting any **UnauthorizedAccess** error, then start Windows
+PowerShell with the "Run as administrator" option and run
+`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine`.
+Now re-run the above installation command. To change the
+[*Execution Policies*](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies)
+to its default, you can run
+`Set-ExecutionPolicy -ExecutionPolicy Default -Scope LocalMachine`.
+
 Using Linux Terminal:
 
 ```bash
 curl https://run.vertopal.com/cli/linux | bash
 ```
 
 ## Using Vertopal-CLI
```

### Comparing `vertopal-1.0.2/pyproject.toml` & `vertopal-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vertopal"
-version = "1.0.2"
+version = "1.0.3"
 
 description = "Convert your files in terminal using Vertopal API"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {text = "MIT"}
 
 keywords = ["convert", "file", "vertopal", "api", "converter"]
```

### Comparing `vertopal-1.0.2/vertopal/api/interface.py` & `vertopal-1.0.3/vertopal/api/interface.py`

 * *Files identical despite different names*

### Comparing `vertopal-1.0.2/vertopal/api/v1.py` & `vertopal-1.0.3/vertopal/api/v1.py`

 * *Files identical despite different names*

### Comparing `vertopal-1.0.2/vertopal/build.py` & `vertopal-1.0.3/vertopal/build.py`

 * *Files identical despite different names*

### Comparing `vertopal-1.0.2/vertopal/utils/config.py` & `vertopal-1.0.3/vertopal/utils/config.py`

 * *Files identical despite different names*

### Comparing `vertopal-1.0.2/vertopal/utils/terminal.py` & `vertopal-1.0.3/vertopal/utils/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Optional, Dict, Callable, Any
 
 from requests import exceptions
 
 import vertopal
-from vertopal.utils.config import Config
 
 
 class Terminal:
     """Provides different methods for handling command-line jobs.
 
     Attributes:
         silent (bool): If set to `True`, don't write to `stdout` or `stderr`.
@@ -71,16 +70,16 @@
             vertopal.API.upload.__name__,
             vertopal.API.convert.__name__,
             vertopal.API.status.__name__,
             vertopal.API.task_response.__name__,
         ],
     }
 
-    app_id: str = Config.read("api", "appid")
-    security_token: str = Config.read("api", "token")
+    app_id: str = ""
+    security_token: str = ""
 
     @classmethod
     def convert(
             cls,
             input_file: str,
             output_format: str,
             input_format: Optional[str] = None
@@ -133,25 +132,24 @@
         cls._info(f"Convert vCredits used: {task_response.vcredits}")
 
         if task_response.convert == "failed":
             cls._error(
                 "Conversion failed. To learn more, visit: "
                 "https://www.vertopal.com/en/help/post/27",
                 "CONVERT_FAILED",
-                end="",
             )
             cls.exit(cls.EX_CONVERT_FAILED)
 
         elif task_response.convert == "successful":
             cls._step("Downloading converted file", "4/4")
             download = cls._download(convert_connector)
             cls._download_file(download.connector, download.filename)
 
         else:
-            cls._error("An unexpected error happened", end="")
+            cls._error("An unexpected error happened")
             cls.exit(cls.EX_OTHER)
 
     @classmethod
     def check_config(cls) -> None:
         """Show a warning on stdout if AppID and/or Token is not configured.
 
         Returns:
@@ -187,42 +185,40 @@
         Returns:
             Dict[str, Any]: JSON response of the API cast to Python dictionary.
         """
 
         try:
             response = func(**kwargs)
         except FileNotFoundError:
-            cls._error("Input file not exists.", end="")
+            cls._error("Input file not exists.")
             cls.exit(cls.EX_INPUT_NOT_FOUND)
         except exceptions.ConnectionError:
             cls._error(
                 f"Cannot reach API endpoint ({vertopal.API.ENDPOINT}). "
                 "Please check your network connection.",
-                end=""
             )
             cls.exit(cls.EX_CONNECTION_ERROR)
         except Exception as error: # pylint: disable=broad-except
-            cls._error(repr(error), end="")
+            cls._error(repr(error))
             cls.exit(cls.EX_OTHER)
         else:
             try:
                 json = response.json()
             except exceptions.InvalidJSONError:
                 cls._error(
                     "Cannot decode HTTP response",
                     "INVALID_JSON",
-                    end="",
                 )
                 cls.exit(cls.EX_INVALID_JSON_RESPONSE)
             except Exception as error: # pylint: disable=broad-except
-                cls._error(repr(error), end="")
+                cls._error(repr(error))
                 cls.exit(cls.EX_OTHER)
             # if http response code is 4xx or 5xx
             if (response.status_code % 1000) // 100 in (4, 5):
-                cls._error(json["message"], json["code"], end="")
+                cls._error(json["message"], json["code"])
                 cls.exit(cls.EX_API_RESPONSE_ERROR)
             else:
                 if json["result"]["warning"]:
                     # Iterate over all warning messages
                     for w_code, w_message in json["result"]["warning"].items():
                         # Check if it's ignored in the current function call
                         if (w_code in cls.ignore_warning and
@@ -230,15 +226,14 @@
                                 cls.IGNORE_ALL in cls.ignore_warning[w_code])):
                             continue
                         cls._warning(w_message, w_code)
                 if json["result"]["error"]:
                     cls._error(
                         json["result"]["error"]["message"],
                         json["result"]["error"]["code"],
-                        end="",
                     )
                     cls.exit(cls.EX_API_RESPONSE_ERROR)
             return json
 
     @classmethod
     def _upload(cls, filename: str, filepath: str) -> str:
         """Run an upload request using Vertopal API.
@@ -293,15 +288,15 @@
                 "mode": vertopal.API.ASYNC,
             },
         )
 
         if json["entity"]["status"] == "running":
             return json["entity"]["id"]
 
-        cls._error("Entity status is not running.", end="")
+        cls._error("Entity status is not running.")
         cls.exit(cls.EX_OTHER)
         return ""
 
     @classmethod
     def _task_status(cls, connector: str) -> SimpleNamespace:
         """Run a task response request using Vertopal API.
 
@@ -440,15 +435,15 @@
 
         Returns:
             None
         """
 
         if cls.silent:
             return
-        line = f"[DONE] Your converted file saved as {str(filename)}"
+        line = f"[DONE] Your converted file saved as {str(filename)}\n"
         sys.stdout.write(line)
 
     @classmethod
     def _step(cls, text: str, step: str) -> None:
         """Write the step of conversion to the `stdout`.
 
         Args:
@@ -628,14 +623,24 @@
         )
         args_convert.add_argument(
             "-d", "--output-dir",
             metavar="<directory>",
             help="directory for saving converted file"
         )
         args_convert.add_argument(
+            "--app",
+            metavar="<app-id>",
+            help="override Application ID in global config file"
+        )
+        args_convert.add_argument(
+            "--token",
+            metavar="<token>",
+            help="override Security Token in global config file"
+        )
+        args_convert.add_argument(
             "--overwrite",
             action="store_true",
             help="overwrite the converted output file if it exists"
         )
         args_convert.add_argument(
             "--silent",
             action="store_true",
```

### Comparing `vertopal-1.0.2/vertopal/vertopal.py` & `vertopal-1.0.3/vertopal/vertopal.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,16 +22,22 @@
     """
 
     # Define & Parse command-line options
     args = Terminal.parse()
 
     if args.command == "convert":
 
-        # Show a warning on stdout if AppID & Security Token is not configured
-        Terminal.check_config()
+        if args.app and args.token:
+            Terminal.app_id = args.app
+            Terminal.security_token = args.token
+        else:
+            Terminal.app_id: str = Config.read("api", "appid")
+            Terminal.security_token: str = Config.read("api", "token")
+            # Show a warning on stdout if client credentials are not configured
+            Terminal.check_config()
 
         if args.silent:
             Terminal.silent = True
         if args.overwrite:
             Terminal.overwrite = True
         if args.output_dir:
             Terminal.output_dir = args.output_dir
```

### Comparing `vertopal-1.0.2/vertopal.egg-info/PKG-INFO` & `vertopal-1.0.3/vertopal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertopal
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert your files in terminal using Vertopal API
 Home-page: https://github.com/vertopal/vertopal-cli
 Author-email: Vertopal <contact@vertopal.com>
 License: MIT
 Project-URL: Homepage, https://www.vertopal.com
 Project-URL: Funding, https://www.vertopal.com/en/donate
 Project-URL: Source, https://github.com/vertopal/vertopal-cli
@@ -20,31 +20,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vertopal-CLI
 
-**Vertopal-CLI** is a small, yet powerful utility for converting
-digital files to a variety of file formats
-using [Vertopal](https://www.vertopal.com) public API.
+**Vertopal-CLI** is a small yet powerful utility that allows you to convert
+digital files into various formats using the
+[Vertopal public API](https://www.vertopal.com/en/developer/api).
 
 You can use Vertopal-CLI by either *terminal commands* or
-*importing as Python package*.
+*importing as a Python package*.
 
 ## Installing Vertopal-CLI
 
 Vertopal-CLI is available on [PyPI](https://pypi.org/project/vertopal/):
 
 ```bash
 python -m pip install vertopal
 ```
 
 You can also download the most recent version of Vertopal-CLI binaries for
-**MacOS**, **Windows**, and **Linux** from the
+**macOS**, **Windows**, and **Linux** from the
 [releases page](https://github.com/vertopal/vertopal-cli/releases/latest) or
 the [product page](https://www.vertopal.com/en/product/cli).
 
 ### Installer
 
 An automatic installer is available for each different platform. It will run an
 install script that downloads and copy Vertopal-CLI binaries to the correct
@@ -55,17 +55,25 @@
 ```bash
 curl https://run.vertopal.com/cli/macos | bash
 ```
 
 On Windows using PowerShell:
 
 ```bash
-curl.exe https://run.vertopal.com/cli/windows | iex
+(curl https://run.vertopal.com/cli/windows).Content | iex
 ```
 
+If you are getting any **UnauthorizedAccess** error, then start Windows
+PowerShell with the "Run as administrator" option and run
+`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine`.
+Now re-run the above installation command. To change the
+[*Execution Policies*](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies)
+to its default, you can run
+`Set-ExecutionPolicy -ExecutionPolicy Default -Scope LocalMachine`.
+
 Using Linux Terminal:
 
 ```bash
 curl https://run.vertopal.com/cli/linux | bash
 ```
 
 ## Using Vertopal-CLI
```

