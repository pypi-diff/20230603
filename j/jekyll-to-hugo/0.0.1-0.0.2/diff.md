# Comparing `tmp/jekyll_to_hugo-0.0.1.tar.gz` & `tmp/jekyll_to_hugo-0.0.2.tar.gz`

## Comparing `jekyll_to_hugo-0.0.1.tar` & `jekyll_to_hugo-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.DS_Store
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/Dockerfile
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/config.yaml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/main.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/requirements.txt
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/setup.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/config.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/converter/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/converter/converter.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/io/reader.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/tests/utils.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/LICENSE
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/readme.md
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.DS_Store
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/Dockerfile
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/config.yaml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/main.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/config.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/converter.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/reader.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/utils.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/readme.md
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.1/.DS_Store` & `jekyll_to_hugo-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/config.yaml` & `jekyll_to_hugo-0.0.2/config.yaml`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/main.py` & `jekyll_to_hugo-0.0.2/main.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/config.py` & `jekyll_to_hugo-0.0.2/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/utils.py` & `jekyll_to_hugo-0.0.2/app/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/converter/converter.py` & `jekyll_to_hugo-0.0.2/app/converter/converter.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.2/app/converter/regex_heuristics.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.2/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/io/reader.py` & `jekyll_to_hugo-0.0.2/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/io/writer.py` & `jekyll_to_hugo-0.0.2/app/io/writer.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/tests/utils.py` & `jekyll_to_hugo-0.0.2/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.2/app/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.2/app/tests/converter/wordpress_markdown_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/.gitignore` & `jekyll_to_hugo-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/LICENSE` & `jekyll_to_hugo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/readme.md` & `jekyll_to_hugo-0.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.1/PKG-INFO` & `jekyll_to_hugo-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Provides-Extra: dev
+Requires-Dist: autoflake; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: pdoc; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Jekyll to Hugo Converter
 
 Jekyll to Hugo Converter is a simple tool to convert Jekyll posts to Hugo posts.
 
 I've used this tool to convert [my blog](https://blog.nuculabs.dev) from WorPress to Jekyll to Hugo.
```

