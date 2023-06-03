# Comparing `tmp/turbo_docs-0.8.4.tar.gz` & `tmp/turbo_docs-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.8.4.tar", last modified: Mon May 29 19:37:26 2023, max compression
+gzip compressed data, was "turbo_docs-0.8.5.tar", last modified: Sat Jun  3 19:01:56 2023, max compression
```

## Comparing `turbo_docs-0.8.4.tar` & `turbo_docs-0.8.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.430960 turbo_docs-0.8.4/
--rw-rw-rw-   0        0        0     2314 2023-05-29 19:37:26.428904 turbo_docs-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2023-05-29 19:26:06.000000 turbo_docs-0.8.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 19:37:26.431971 turbo_docs-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-05-29 19:36:49.000000 turbo_docs-0.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.398384 turbo_docs-0.8.4/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.4/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.416868 turbo_docs-0.8.4/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.4/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.4/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0      731 2023-05-29 19:17:05.000000 turbo_docs-0.8.4/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1036 2023-05-29 19:09:40.000000 turbo_docs-0.8.4/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.427866 turbo_docs-0.8.4/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.4/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.4/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2854 2023-05-29 19:36:03.000000 turbo_docs-0.8.4/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.8.4/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.411864 turbo_docs-0.8.4/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2314 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.375188 turbo_docs-0.8.5/
+-rw-rw-rw-   0        0        0     2314 2023-06-03 19:01:56.375188 turbo_docs-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 19:01:56.376176 turbo_docs-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-06-03 18:58:56.000000 turbo_docs-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.352435 turbo_docs-0.8.5/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.5/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.366150 turbo_docs-0.8.5/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.5/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.5/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0      731 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1036 2023-05-29 19:09:40.000000 turbo_docs-0.8.5/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.372170 turbo_docs-0.8.5/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.5/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.5/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2854 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.8.5/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.362300 turbo_docs-0.8.5/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2314 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.8.4/PKG-INFO` & `turbo_docs-0.8.5/turbo_docs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo_docs
-Version: 0.8.4
+Name: turbo-docs
+Version: 0.8.5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-0.8.4/README.md` & `turbo_docs-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/setup.py` & `turbo_docs-0.8.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.8.4",
+	version="0.8.5",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
 		"gitpython",
+    	"toml",
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
 		],
 	},
 	classifiers=[
```

### Comparing `turbo_docs-0.8.4/turbo_docs/commands/docstring.py` & `turbo_docs-0.8.5/turbo_docs/commands/docstring.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs/commands/readme.py` & `turbo_docs-0.8.5/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs/generate.py` & `turbo_docs-0.8.5/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs/utils/cli_options.py` & `turbo_docs-0.8.5/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs/utils/directory.py` & `turbo_docs-0.8.5/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs/utils/openai_api.py` & `turbo_docs-0.8.5/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.4/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.8.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo-docs
-Version: 0.8.4
+Name: turbo_docs
+Version: 0.8.5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

