# Comparing `tmp/autoparaselenium-0.1.9.tar.gz` & `tmp/autoparaselenium-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoparaselenium-0.1.9.tar", last modified: Wed Oct 20 01:03:09 2021, max compression
+gzip compressed data, was "autoparaselenium-0.2.0.tar", last modified: Sat Jun  3 18:15:16 2023, max compression
```

## Comparing `autoparaselenium-0.1.9.tar` & `autoparaselenium-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/autoparaselenium/browsers/
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/browsers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/browsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/browsers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-10-20 01:02:59.000000 autoparaselenium-0.1.9/autoparaselenium/browser_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-10-20 01:03:09.000000 autoparaselenium-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/autoparaselenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browser_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/autoparaselenium/browsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/autoparaselenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_browsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_everything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_pool.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autoparaselenium-0.1.9/README.md` & `autoparaselenium-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.1.9/autoparaselenium/__init__.py` & `autoparaselenium-0.2.0/autoparaselenium/__init__.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.1.9/autoparaselenium/setup_utils.py` & `autoparaselenium-0.2.0/autoparaselenium/setup_utils.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.1.9/autoparaselenium/browsers/firefox.py` & `autoparaselenium-0.2.0/autoparaselenium/browsers/firefox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import atexit
 from contextlib import suppress
 from functools import partial
 from pathlib import Path
 
 from selenium import webdriver
 
 import autoparaselenium.setup_utils as su
 from autoparaselenium.models import Conf, Extension
 
 
 class FirefoxDriver(webdriver.Firefox):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.has_quit = False
+        atexit.register(self.quit)
 
     def quit(self):
         if not self.has_quit:
             self.has_quit = True
             super().quit()
 
     def __del__(self):
@@ -50,28 +52,29 @@
 __platform_drivers = {
     "win": "geckodriver.exe",
     "darwin": "geckodriver",
     "linux": "geckodriver",
 }
 
 
+version = "0.30.0"
 __setup_driver = partial(
     su.setup_driver,
     {
         "win": [
             "https://github.com/mozilla/geckodriver/releases"
-            "/download/v0.28.0/geckodriver-v0.28.0-win64.zip",
+            f"/download/v{version}/geckodriver-v{version}-win64.zip",
             su.unzip,
         ],
         "darwin": [
             "https://github.com/mozilla/geckodriver/releases/"
-            "download/v0.28.0/geckodriver-v0.28.0-macos.tar.gz",
+            f"download/v{version}/geckodriver-v{version}-macos.tar.gz",
             su.untar,
         ],
         "linux": [
             "https://github.com/mozilla/geckodriver/releases"
-            "/download/v0.28.0/geckodriver-v0.28.0-linux64.tar.gz",
+            f"/download/v{version}/geckodriver-v{version}-linux64.tar.gz",
             su.untar,
         ],
     },
     __platform_drivers,
 )
```

### Comparing `autoparaselenium-0.1.9/autoparaselenium/browsers/chrome.py` & `autoparaselenium-0.2.0/autoparaselenium/browsers/chrome.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import atexit
 import os
 import stat
 import subprocess as sb
 import sys
 from contextlib import suppress
 from functools import partial
 from pathlib import Path
+from typing import Optional
 
+import requests
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 
 import autoparaselenium.setup_utils as su
 from autoparaselenium.models import Conf
 
 
@@ -34,14 +37,15 @@
 class ChromeDriver(webdriver.Chrome):
     def __init__(self, *args, **kwargs):
         old_popen = sb.Popen
         sb.Popen = Popen
         super().__init__(*args, **kwargs)
         sb.Popen = old_popen
         self.has_quit = False
+        atexit.register(self.quit)
 
     def quit(self):
         if not self.has_quit:
             self.has_quit = True
             super().quit()
 
     def __del__(self):
@@ -53,20 +57,56 @@
     options = __get_options(conf)
     browser = ChromeDriver(
         executable_path=pwd / __platform_drivers[su.platform], options=options
     )
     return browser
 
 
-def setup_driver(pwd) -> None:
-    __setup_driver(pwd)
-    if (pwd / "chromedriver").exists():
+def setup_driver(pwd: Path) -> None:
+    chrome_version = __get_chrome_version()
+    driver_version = __get_chromedriver_version(pwd)
+    if driver_version is None or driver_version < chrome_version:
+        r = requests.get(
+            "https://chromedriver.storage.googleapis.com"
+            f"/LATEST_RELEASE_{chrome_version}"
+        )
+        version = r.text.strip()
+        if (pwd / "chromedriver").exists():
+            os.remove(pwd / "chromedriver")
+        __setup_driver(version)(pwd)
         os.chmod(pwd / "chromedriver", stat.S_IEXEC)
 
 
+def __get_chromedriver_version(pwd: Path) -> Optional[int]:
+    with suppress(Exception):
+        # version returned will be the major version
+        p = sb.Popen([str(pwd / "chromedriver"), "--version"], stdout=sb.PIPE)
+        atexit.register(p.terminate)
+
+        # output of cmd will be lik
+        # ChromeDriver 108.0.5359.71 (1e0e3868ee06e91ad6...
+        version = p.communicate()[0].decode().split(" ")[1]
+        major, *_ = version.split(".")
+
+        # will raise ValueError if major version isn't a proper number
+        return int(major)
+
+
+def __get_chrome_version() -> int:
+    p = sb.Popen([__platform_binaries[su.platform], "--version"], stdout=sb.PIPE)
+    atexit.register(p.terminate)
+
+    # output of cmd will be lik
+    # Google Chrome 108.0.5359.124
+    major = p.communicate()[0].decode().split(".")[0].split(" ")[-1]
+
+    # will raise ValueError if major version isn't a proper number
+    return int(major)
+
+
 def __get_options(conf: Conf) -> Options:
     options = Options()
     if conf.headless and all(ext.chrome is None for ext in conf.extensions):
         options.add_argument("--no-sandbox")
         options.add_argument("--headless")
 
     for ext in conf.extensions:
@@ -78,17 +118,21 @@
 
 __platform_drivers = {
     "win": "chromedriver.exe",
     "darwin": "chromedriver",
     "linux": "chromedriver",
 }
 
-version = "95.0.4638.17"
+__platform_binaries = {
+    "darwin": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
+    "win": os.path.expanduser(r"~\AppData\Local\Google\Chrome\Application\chrome.exe"),
+    "linux": "/usr/bin/google-chrome",
+}
 
-__setup_driver = partial(
+__setup_driver = lambda version: partial(
     su.setup_driver,
     {
         "win": [
             "https://chromedriver.storage.googleapis.com"
             f"/{version}/"
             "chromedriver_win32.zip",
             su.unzip,
```

### Comparing `autoparaselenium-0.1.9/autoparaselenium/browser_pool.py` & `autoparaselenium-0.2.0/autoparaselenium/browser_pool.py`

 * *Files identical despite different names*

