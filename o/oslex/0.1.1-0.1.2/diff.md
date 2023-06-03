# Comparing `tmp/oslex-0.1.1.tar.gz` & `tmp/oslex-0.1.2.tar.gz`

## Comparing `oslex-0.1.1.tar` & `oslex-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 oslex-0.1.1/.editorconfig
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 oslex-0.1.1/oslex.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 oslex-0.1.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oslex-0.1.1/LICENSE
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 oslex-0.1.1/README.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 oslex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 oslex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 oslex-0.1.2/.editorconfig
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 oslex-0.1.2/pyproject.toml2
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 oslex-0.1.2/oslex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oslex-0.1.2/oslex/py.typed
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 oslex-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oslex-0.1.2/LICENSE
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 oslex-0.1.2/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 oslex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 oslex-0.1.2/PKG-INFO
```

### Comparing `oslex-0.1.1/oslex.py` & `oslex-0.1.2/oslex/__init__.py`

 * *Files identical despite different names*

### Comparing `oslex-0.1.1/.gitignore` & `oslex-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oslex-0.1.1/LICENSE` & `oslex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oslex-0.1.1/README.md` & `oslex-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oslex-0.1.1/pyproject.toml` & `oslex-0.1.2/pyproject.toml2`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "oslex"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
 	{ name="Tamás PEREGI", email="petamas@gmail.com" },
 ]
 description = "OS-independent wrapper for shlex and mslex"
 readme = "README.md"
 # mslex is supposed to support >=3.5, but it has an accidental f-string, making it unusable on 3.5
 # see https://github.com/smoofra/mslex/issues/1
@@ -29,7 +29,10 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/petamas/oslex"
 "Bug Tracker" = "https://github.com/petamas/oslex/issues"
+
+[tool.hatch.build.targets.wheel.force-include]
+"py.typed" = "py.typed"
```

### Comparing `oslex-0.1.1/PKG-INFO` & `oslex-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslex
-Version: 0.1.1
+Version: 0.1.2
 Summary: OS-independent wrapper for shlex and mslex
 Project-URL: Homepage, https://github.com/petamas/oslex
 Project-URL: Bug Tracker, https://github.com/petamas/oslex/issues
 Author-email: Tamás PEREGI <petamas@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

