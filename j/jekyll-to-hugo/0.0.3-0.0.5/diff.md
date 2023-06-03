# Comparing `tmp/jekyll_to_hugo-0.0.3.tar.gz` & `tmp/jekyll_to_hugo-0.0.5.tar.gz`

## Comparing `jekyll_to_hugo-0.0.3.tar` & `jekyll_to_hugo-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.DS_Store
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/Dockerfile
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/config.yaml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/main.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/config.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/converter.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/reader.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/utils.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/readme.md
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.DS_Store
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/Dockerfile
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/config.yaml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/main.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/config.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/converter.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/reader.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/readme.md
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.3/.DS_Store` & `jekyll_to_hugo-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/config.yaml` & `jekyll_to_hugo-0.0.5/config.yaml`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/main.py` & `jekyll_to_hugo-0.0.5/main.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/config.py` & `jekyll_to_hugo-0.0.5/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/utils.py` & `jekyll_to_hugo-0.0.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/converter/converter.py` & `jekyll_to_hugo-0.0.5/app/converter/converter.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.5/app/converter/regex_heuristics.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.5/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/io/reader.py` & `jekyll_to_hugo-0.0.5/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/io/writer.py` & `jekyll_to_hugo-0.0.5/app/io/writer.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/tests/utils.py` & `jekyll_to_hugo-0.0.5/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.5/app/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.5/app/tests/converter/wordpress_markdown_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/.gitignore` & `jekyll_to_hugo-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/LICENSE` & `jekyll_to_hugo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/pyproject.toml` & `jekyll_to_hugo-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jekyll-to-hugo"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="Denis Nutiu", email="nuculabs@outlook.com" },
 ]
 description = "Python library for converting jekyll md files to Hugo."
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,14 +19,20 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
+dependencies = [
+  "beautifulsoup4>=4.12, <5",
+  "PyYAML",
+  "soupsieve>=2.4, <3",
+  "pydantic>=1.10, <2",
+]
 
 [project.scripts]
 jekyll-to-hugo = "main:main"
 
 [project.optional-dependencies]
 dev = ["black", "pdoc", "isort", "autoflake", "pytest"]
```

### Comparing `jekyll_to_hugo-0.0.3/readme.md` & `jekyll_to_hugo-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.3/PKG-INFO` & `jekyll_to_hugo-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.3
+Version: 0.0.5
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Requires-Dist: beautifulsoup4<5,>=4.12
+Requires-Dist: pydantic<2,>=1.10
+Requires-Dist: pyyaml
+Requires-Dist: soupsieve<3,>=2.4
 Provides-Extra: dev
 Requires-Dist: autoflake; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pdoc; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
```

