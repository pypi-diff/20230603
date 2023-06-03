# Comparing `tmp/jekyll_to_hugo-0.0.2.tar.gz` & `tmp/jekyll_to_hugo-0.0.3.tar.gz`

## Comparing `jekyll_to_hugo-0.0.2.tar` & `jekyll_to_hugo-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.DS_Store
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/Dockerfile
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/config.yaml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/main.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/config.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/converter.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/reader.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/utils.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/readme.md
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.DS_Store
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/Dockerfile
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/config.yaml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/main.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/config.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/converter.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/reader.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/readme.md
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.3/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.2/.DS_Store` & `jekyll_to_hugo-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/config.yaml` & `jekyll_to_hugo-0.0.3/config.yaml`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/main.py` & `jekyll_to_hugo-0.0.3/main.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/config.py` & `jekyll_to_hugo-0.0.3/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/utils.py` & `jekyll_to_hugo-0.0.3/app/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/converter/converter.py` & `jekyll_to_hugo-0.0.3/app/converter/converter.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.3/app/converter/regex_heuristics.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.3/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/io/reader.py` & `jekyll_to_hugo-0.0.3/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/app/io/writer.py` & `jekyll_to_hugo-0.0.3/app/io/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import Callable
 
 from app import utils
 
 
 class IoWriter(metaclass=ABCMeta):
     """
     Abstract class for writing posts.
```

### Comparing `jekyll_to_hugo-0.0.2/app/tests/utils.py` & `jekyll_to_hugo-0.0.3/app/tests/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from app.config import ConverterOptions, Configurator
+from app.config import Configurator, ConverterOptions
 
 
 def make_fake_configurator(converter: str, converter_options: ConverterOptions):
     class FakeConfigurator(Configurator):
         logging_level: str = "INFO"
         source_path: str = ""
         output_path: str = ""
```

### Comparing `jekyll_to_hugo-0.0.2/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.3/app/tests/utils_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import pytest
 
-from app.utils import (
-    guard_against_none,
-    guard_against_none_or_empty_str,
-    key_error_silence,
-)
+from app.utils import (guard_against_none, guard_against_none_or_empty_str,
+                       key_error_silence)
 
 
 def test_key_error_silence():
     # Test that the context manager silences the exception
     with key_error_silence():
         raise KeyError
     # Test that the context manager does not silence other exceptions
```

### Comparing `jekyll_to_hugo-0.0.2/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.3/app/tests/converter/wordpress_markdown_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/.gitignore` & `jekyll_to_hugo-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/LICENSE` & `jekyll_to_hugo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.2/pyproject.toml` & `jekyll_to_hugo-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jekyll-to-hugo"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Denis Nutiu", email="nuculabs@outlook.com" },
 ]
 description = "Python library for converting jekyll md files to Hugo."
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jekyll_to_hugo-0.0.2/PKG-INFO` & `jekyll_to_hugo-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,40 +25,51 @@
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Jekyll to Hugo Converter
 
 Jekyll to Hugo Converter is a simple tool to convert Jekyll posts to Hugo posts.
 
-I've used this tool to convert [my blog](https://blog.nuculabs.dev) from WorPress to Jekyll to Hugo.
+I've used this tool to convert [my blog](https://blog.nuculabs.dev) from WordPress to Jekyll and finally to Hugo.
+
+The tool has the following features:
+- Batch conversion.
+- Post header fields drop/ignore.
+- Links rewrite. (Search and Replace)
+- Author name rewrite.
+
+It was written in a way that is easy to extend, while I wrote it for my own personal use, I hope you'll find some use for it as well.
 
 Note: This tool is not perfect, it will not convert everything. If you find a bug, please open a PR.
 
 ## Table of Contents
 
 * [Usage](#usage)
   * [PiPy](#pipy)
   * [Python From Source](#python-from-source)
   * [Docker](#docker)
 * [Configuration](#configuration)
+  * [Example Configuration](#example-configuration)
 * [License](#license)
 
 ## Usage
 
-### PiPy
+### PiPy or Pipx
 
 If you have Python installed, you can use the following commands:
 
 ```bash
 pip install jekyll-to-hugo
 jekyll-to-hugo
 ```
 
 You will need to create a `config.yaml` file in the current directory. See example [here](./config.yaml).
 
+_`pipx` is a tool to install Python CLI tools in isolated environments_
+
 ### Python From Source
 
 If you have Python installed, you can use the following commands:
 
 ```bash
 pip install -r requirements.txt
 python3 jekyll-to-hugo.py <jekyll_post_path> <hugo_post_path>
@@ -85,13 +96,41 @@
 ```
 
 ## Configuration
 
 The configuration file is a YAML file. See example [here](./config.yaml).
 The configuration file path can be configured with the `CONFIG_PATH` environment variable.
 
+### Example Configuration
+
+```yaml
+logging_level: "INFO"
+source_path: "/Users/dnutiu/PycharmProjects/jekyll-to-hugo/my_test_data/_posts"
+output_path: "/Users/dnutiu/NucuLabsProjects/NucuLabsDevBlog/content/posts"
+converter: "wordpress_markdown_converter"
+converter_options:
+  enable_regex_heuristics: true
+  author_rewrite: "Denis Nuțiu"
+  links_rewrite:
+    - source: "http://localhost/"
+      target: "/"
+    - source: "https://nuculabs.wordpress.com/"
+      target: "https://nuculabs.dev/posts/"
+    - source: "https://twitter.com/metonymyqt"
+      target: "https://twitter.com/nuculabs"
+  header_fields_drop:
+    - restapi_import_id
+    - original_post_id
+    - timeline_notification
+    - wordads_ufa
+    - spay_email
+    - amp_status
+    - advanced_seo_description
+    - publicize_twitter_user
+```
+
 ## License
 
 This project is licensed under the GPL-3.0 license - see the [LICENSE](LICENSE) file for details.
 
 ---
 Made with ❤️ by [NucuLabs.dev](https://blog.nuculabs.dev)
```

