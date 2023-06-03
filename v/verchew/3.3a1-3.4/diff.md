# Comparing `tmp/verchew-3.3a1.tar.gz` & `tmp/verchew-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verchew-3.3a1.tar", max compression
+gzip compressed data, was "verchew-3.4.tar", max compression
```

## Comparing `verchew-3.3a1.tar` & `verchew-3.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1088 2018-03-29 20:56:27.000000 verchew-3.3a1/LICENSE.md
--rw-r--r--   0        0        0     3080 2022-03-10 17:37:44.089349 verchew-3.3a1/README.md
--rw-r--r--   0        0        0     1996 2022-04-17 22:54:17.984456 verchew-3.3a1/pyproject.toml
--rw-r--r--   0        0        0       60 2016-10-17 21:38:01.000000 verchew-3.3a1/verchew/__init__.py
--rw-r--r--   0        0        0      124 2020-11-25 23:10:46.000000 verchew-3.3a1/verchew/__main__.py
--rwxr-xr-x   0        0        0    10255 2022-04-17 22:54:17.984786 verchew-3.3a1/verchew/script.py
--rw-r--r--   0        0        0       34 2016-10-12 14:39:17.000000 verchew-3.3a1/verchew/tests/__init__.py
--rw-r--r--   0        0        0      291 2020-11-25 23:10:52.000000 verchew-3.3a1/verchew/tests/conftest.py
--rw-r--r--   0        0        0     6175 2022-04-17 22:54:17.985099 verchew-3.3a1/verchew/tests/test_script.py
--rw-r--r--   0        0        0      147 2022-04-17 22:54:42.338278 verchew-3.3a1/verchew/wrapper.sh
--rw-r--r--   0        0        0     3873 2022-04-17 22:59:17.906517 verchew-3.3a1/setup.py
--rw-r--r--   0        0        0     4461 2022-04-17 22:59:17.906829 verchew-3.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-10-23 17:28:02.191465 verchew-3.4/LICENSE.md
+-rw-r--r--   0        0        0     3064 2023-06-03 20:17:02.276081 verchew-3.4/README.md
+-rw-r--r--   0        0        0     2038 2023-06-03 20:21:25.127676 verchew-3.4/pyproject.toml
+-rw-r--r--   0        0        0       60 2020-10-23 17:28:02.195541 verchew-3.4/verchew/__init__.py
+-rw-r--r--   0        0        0      124 2020-10-23 17:28:02.195675 verchew-3.4/verchew/__main__.py
+-rwxr-xr-x   0        0        0    10571 2023-06-03 21:34:08.124188 verchew-3.4/verchew/script.py
+-rw-r--r--   0        0        0       34 2020-10-23 17:28:02.195975 verchew-3.4/verchew/tests/__init__.py
+-rw-r--r--   0        0        0      291 2020-10-23 17:28:02.196080 verchew-3.4/verchew/tests/conftest.py
+-rw-r--r--   0        0        0     6288 2023-06-03 21:34:26.121376 verchew-3.4/verchew/tests/test_script.py
+-rwxr-xr-x   0        0        0      393 2022-09-12 19:07:47.825706 verchew-3.4/verchew/wrapper.sh
+-rw-r--r--   0        0        0     4796 1970-01-01 00:00:00.000000 verchew-3.4/PKG-INFO
```

### Comparing `verchew-3.3a1/LICENSE.md` & `verchew-3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `verchew-3.3a1/README.md` & `verchew-3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Overview
 
 > ...chews through your system dependencies, spitting out incompatible versions.
 
 When onboarding new team members, ensuring their computer has everything needed to work on the project can be painful. Verchew is a command-line program and embeddable Python script to check the versions of your project's system dependencies. Its only external dependency is any Python interpreter, which should already be installed on macOS and most Linux-based operating systems.
 
-[![Unix Build Status](https://img.shields.io/travis/jacebrowning/verchew/main.svg?label=unix)](https://travis-ci.org/jacebrowning/verchew)
-[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/verchew/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/verchew)
+[![Travis CI](https://img.shields.io/travis/com/jacebrowning/verchew/main.svg?label=unix)](https://travis-ci.com/jacebrowning/verchew)
+[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/verchew/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/verchew)
 [![Coverage Status](https://img.shields.io/coveralls/jacebrowning/verchew/main.svg)](https://coveralls.io/r/jacebrowning/verchew)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/verchew.svg)](https://scrutinizer-ci.com/g/jacebrowning/verchew/?branch=main)
 [![PyPI License](https://img.shields.io/pypi/l/verchew.svg)](https://pypi.org/project/verchew)
 [![PyPI Version](https://img.shields.io/pypi/v/verchew.svg)](https://pypi.python.org/pypi/verchew)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/verchew.svg?color=orange)](https://pypistats.org/packages/verchew)
 
 # Setup
```

### Comparing `verchew-3.3a1/pyproject.toml` & `verchew-3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "verchew"
-version = "3.3a1"  # also update verchew/script.py
+version = "3.4"  # also update verchew/script.py
 description = "System dependency version checker."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -28,14 +28,15 @@
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Testing",
     "Topic :: System :: Installation/Setup",
     "Topic :: Utilities",
 ]
 
@@ -59,15 +60,15 @@
 pytest-cov = "*"
 pytest-describe = "^1.0"
 pytest-expecter = "*"
 pytest-random = "*"
 scripttest = "*"
 
 # Reports
-coveragespace = "^3.1.1"
+coveragespace = "^4.2"
 
 # Documentation
 mkdocs = "~1.2.3"
 pygments = "~2.7.4"
 
 # Tooling
 pyinstaller = "*"
```

### Comparing `verchew-3.3a1/verchew/script.py` & `verchew-3.4/verchew/script.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 if PY2:
     import ConfigParser as configparser
     from urllib import urlretrieve
 else:
     import configparser
     from urllib.request import urlretrieve
 
-__version__ = '3.3a1'
+__version__ = '3.4'
 
 SCRIPT_URL = (
     "https://raw.githubusercontent.com/jacebrowning/verchew/main/verchew/script.py"
 )
 WRAPPER_URL = (
     "https://raw.githubusercontent.com/jacebrowning/verchew/main/verchew/wrapper.sh"
 )
@@ -291,31 +291,45 @@
         args = [program] + argument.split()
     else:
         args = [program]
 
     show("$ {0}".format(" ".join(args)))
     output = call(args)
     lines = output.splitlines()
-    show(lines[0] if lines else "<nothing>")
+
+    if lines:
+        for line in lines:
+            if any(char.isdigit() for char in line):
+                show(line)
+                break
+        else:
+            show(lines[0])
+    else:
+        show("<nothing>")
 
     return output
 
 
 def match_version(pattern, output):
-    if "not found" in output.split('\n')[0]:
+    lines = output.splitlines()
+    if "not found" in lines[0]:
         return False
 
     regex = pattern.replace('.', r'\.') + r'(\b|/)'
 
-    log.debug("Matching %s: %s", regex, output)
-    match = re.match(regex, output)
-    if match is None:
-        match = re.match(r'.*[^\d.]' + regex, output)
+    for line in lines:
+        log.debug("Matching %s: %s", regex, line)
+        match = re.match(regex, line)
+        if match is None:
+            log.debug("Matching %s: %s", regex, line)
+            match = re.match(r'.*[^\d.]' + regex, line)
+        if match:
+            return True
 
-    return bool(match)
+    return False
 
 
 def call(args):
     try:
         process = Popen(args, stdout=PIPE, stderr=STDOUT)
     except OSError:
         log.debug("Command not found: %s", args[0])
```

### Comparing `verchew-3.3a1/verchew/tests/test_script.py` & `verchew-3.4/verchew/tests/test_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,17 @@
             match_version(".pyenv", "Users/foobar/.pyenv/versions/2.7.14/bin/python")
         ) == True
 
     def when_mismatch_with_missing_program():
         expect(match_version("", "program not found")) == False
         expect(match_version("", "v1.2.3\nother not found")) == True
 
+    def when_match_with_multiple_lines():
+        expect(match_version("1.2", "Foobar\nVersion 1.2.3")) == True
+
 
 def describe_format():
     def default():
         expect(_('~')) == "~"
 
     @pytest.mark.parametrize(
         "is_tty,supports_utf8,supports_ansi,formatted",
```

### Comparing `verchew-3.3a1/PKG-INFO` & `verchew-3.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: verchew
-Version: 3.3a1
+Version: 3.4
 Summary: System dependency version checker.
 Home-page: https://pypi.org/project/verchew
 License: MIT
 Keywords: dependencies,configuration management,continuous integration
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
@@ -33,16 +40,16 @@
 
 # Overview
 
 > ...chews through your system dependencies, spitting out incompatible versions.
 
 When onboarding new team members, ensuring their computer has everything needed to work on the project can be painful. Verchew is a command-line program and embeddable Python script to check the versions of your project's system dependencies. Its only external dependency is any Python interpreter, which should already be installed on macOS and most Linux-based operating systems.
 
-[![Unix Build Status](https://img.shields.io/travis/jacebrowning/verchew/main.svg?label=unix)](https://travis-ci.org/jacebrowning/verchew)
-[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/verchew/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/verchew)
+[![Travis CI](https://img.shields.io/travis/com/jacebrowning/verchew/main.svg?label=unix)](https://travis-ci.com/jacebrowning/verchew)
+[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/verchew/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/verchew)
 [![Coverage Status](https://img.shields.io/coveralls/jacebrowning/verchew/main.svg)](https://coveralls.io/r/jacebrowning/verchew)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/verchew.svg)](https://scrutinizer-ci.com/g/jacebrowning/verchew/?branch=main)
 [![PyPI License](https://img.shields.io/pypi/l/verchew.svg)](https://pypi.org/project/verchew)
 [![PyPI Version](https://img.shields.io/pypi/v/verchew.svg)](https://pypi.python.org/pypi/verchew)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/verchew.svg?color=orange)](https://pypistats.org/packages/verchew)
 
 # Setup
```

